# PIANO FLOW 2.0 GitHub Pages 部署

上传本目录的全部内容到仓库根目录，必须保留 `index.html`、`app.js`、`style.css` 和完整的 `model` 文件夹。模型目录中必须能看到 `model.json` 与 `group1-shard1of1.bin`。不要只上传网页文件，也不要把 ZIP 原样传到仓库。

扒谱使用 Spotify Basic Pitch 模型在浏览器本机推理，音频不上传。提供录音/音频导入、分段识别、五线谱、音符校正、MIDI 与 MusicXML 导出。20 类和弦、12 根音、转位、高亮琴键、试听及键盘练习。

如模型无法加载，先在 GitHub 仓库 Files 页面确认路径为 `model/model.json` 和 `model/group1-shard1of1.bin`，注意大小写。等待 GitHub Pages 部署完成后强制刷新 Safari，旧版本可先关闭标签重新打开。

限制：每次识别 60 秒以内；手动设置 BPM；谱面按八分音符网格整理。混音或踏板混响会降低准确率；需要手动校正。录音麦克风权限需 HTTPS。原始音频不在 JSON 备份中。
