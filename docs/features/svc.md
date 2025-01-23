### 变声

#### DDSP-SVC

官方仓库：[DDSP-SVC](//github.com/yxlllc/DDSP-SVC)  

个人提供的已训练好的模型：[点我跳转](//github.com/Ikaros-521/DDSP-SVC/releases)  

羽毛佬视频教程：[【AI翻唱/变声/整合包】有张N卡就能跑！媲美So-VITS却不吃配置，全新的DDSP-SVC 3.0训练/推理教程](//www.bilibili.com/video/BV1rs4y1Q7BQ)  

视频教程：[【AI主播-功能篇】新增 DDSP-SVC 接入。变声选项再加一，多种选择总有一个是适合你的（](https://www.bilibili.com/video/BV1s8411m7rX/)  

修改 `flask_api.py` 最后几行中的模型路径，其他配置自行调整，另外需要注意！ `enable_spk_id_cover` 改为 `False` ，即可接入。  

```python
# config和模型得同一目录。 这是我自己训练的DDSP模型，新鲜出炉
checkpoint_path = "exp/combsub-test/model_68000.pt"
# 是否使用预训练的基于声码器的增强器增强输出，但对硬件要求更高。
use_vocoder_based_enhancer = True
# 结合增强器使用，0为正常音域范围（最高G5)内的高音频质量，大于0则可以防止超高音破音
enhancer_adaptive_key = 0
# f0提取器，有parselmouth, dio, harvest, crepe
select_pitch_extractor = 'crepe'
# f0范围限制(Hz)
limit_f0_min = 50
limit_f0_max = 1100
# 音量响应阈值(dB)
threhold = -60
# 默认说话人。
spk_id = 1
# 是否优先使用默认说话人覆盖vst传入的参数，改为False，不要覆盖！！！
enable_spk_id_cover = False
```

#### so-vits-svc

官方仓库：[so-vits-svc](//github.com/svc-develop-team/so-vits-svc)  

个人提供的已训练好的模型：[点我跳转](//github.com/Ikaros-521/so-vits-svc/releases)  

视频教程：[【AI歌姬】so-vits-svc 简单使用讲解 + 伊卡洛斯 模型开源](//www.bilibili.com/video/BV1k24y1F7Us) ， [【AI主播-功能篇】如何接入so-vits-svc？用什么版本？4.1版为什么会报错？运行哪个程序？在哪下载？](https://www.bilibili.com/video/BV1dh4y1j7hM/)  

修改 `flask_api_full_song.py` 最后几行中的模型路径，运行，配置相关信息即可接入。  

```python
if __name__ == '__main__':
    model_name = "logs/44k/ikaros_G_54600.pth" # 你的模型地址
    config_name = "configs/ikaros_v1.json"  # 你的config地址
    svc_model = infer_tool.Svc(model_name, config_name)
    app.run(port=1145, host="0.0.0.0", debug=False, threaded=False)
```  

注意！！！如果你是 `4.1` 版本的整合包，还需要修改 `flask_api_full_song.py` 的38行左右：  
改  

```python
out_audio, out_sr = svc_model.infer(spk, tran, raw_path)
```

为

```python
out_audio, out_sr, n_frames = svc_model.infer(spk, tran, raw_path)
```

