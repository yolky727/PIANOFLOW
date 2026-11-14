# PIANO FLOW 2.2 DuET 接入试用版
全部文件平铺，直接上传到原 GitHub Pages 仓库根目录。旧文件可保留。

## DuET 接入状态
已验证 Wayne42/DuET-demo 公开 /transcribe 接口、上传和任务提交。测试音频的云端任务返回服务器 ValueError，尚未完成端到端真实扒谱验证。因此标记为试用，不保证公共服务可用。可能遇到队列、额度、休眠、跨域或服务变动，不能作为稳定后端的承诺。

先录音或导入，选择有效片段，再点击「上传并用 DuET 扒谱」。此按钮会把所选片段上传至第三方 Hugging Face Space，最长 240 秒。取消不等于删除已上传音频。无需将密钥放进公开仓库；未接入账户登录或付费额度。

结果保留 DuET 原始 MusicXML，并读取 score.mid 进行采样钢琴试听和滚动钢琴流。可下载远端 PDF、MIDI、MusicXML；链接可能过期，及时保存。手工导入时，同时选择 score.musicxml 和 score.mid。若 API 无法工作，可打开原演示运行，再将这两个结果文件导回。

本地 Basic Pitch 模式继续可用，最长 60 秒；不上传音频。对 DuET 乐谱不套用旧版量化、分手或音符表编辑，以免损坏其节奏声部；请用专业制谱软件编辑原始 MusicXML。

音色已改为 smplr Soundfont 的 acoustic_grand_piano 采样，首次需要联网加载第三方采样资源；失败会明确提示并回退合成音色。本项目自行实现钢琴流，没有复制演示完整播放器或承诺音色完全相同。外部采样供应者条件和可用性仍适用。

DuET 源码为 MIT，模型权重 CC BY-NC 4.0。本包不分发其代码或权重，仅调用公共接口，适合此处个人非商业体验。来源：https://huggingface.co/spaces/Wayne42/DuET-demo 及 https://github.com/wei-zeng98/DuET 。

本版完成构建和语法检查、公开接口连接与任务提交检查，服务器识别未成功；未在你的 iPad 实测。原音频不保存在 JSON 中，谱面及事件保存在当前浏览器。
