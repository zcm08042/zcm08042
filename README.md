### 飒飒

写本地优先的小工具：待办、番茄钟、视频截帧、AI 聊天。数据留在设备上，不联网、不要账号。

---

### 项目

#### focus-todo · 本地优先待办

记一件事，排一个期，做完勾掉。Electron 桌面端和 Android 用同一套界面。

- 今日 / 全部 / 已完成 / 到期 / 统计五个视图，到期按「已过期 → 今天 → 以后」分组
- 近 7 天完成柱状图、优先级分布
- 启动时若有到期或过期任务，弹一次系统通知
- 优先级高 / 中 / 低，支持搜索即时过滤、深浅色主题
- 本地 JSON 存储，可导出 / 导入备份
- Windows 安装包 + Android APK

#### Focus-Timer · 番茄专注钟

focus-todo 的配套件：一个记任务，一个做专注。

- 专注 / 短休息双模式，时长可调（默认 25 / 5 分钟）
- 开始 / 暂停 / 重置 / 跳过，专注结束自动进休息（可关）
- 今日专注次数与总时长统计
- 原生 HTML / CSS / JS，数据存 localStorage
- Android APK

#### FrameGrabber-Pro · 帧捕获

从视频里精确截出某一帧——当封面、当参考图、当素材，或者逐帧看动画节奏。

- 逐帧浏览 + 进度条导航，帧缓存（LRU）与拖动防抖让操作不卡
- 时间跳转支持秒 / `mm:ss` / `h:mm:ss`
- 保存为 PNG / JPEG / BMP，可设默认保存目录
- 快捷键覆盖逐帧、跳 1 秒、跳 10 秒
- 莫兰迪暗色主题，单 exe 免安装（约 235 MB）

#### ai-chat · 极简聊天客户端

填 Base URL、API Key、模型名就能对话，类似 Chatbox 的极简版。

- OpenAI 兼容接口（`/chat/completions`）
- 内置 OpenAI / DeepSeek / Kimi / 通义预设，也可自定义
- 支持系统提示词，对话历史本地保存
- 密钥只存在设备 localStorage，请求直连你配置的接口
- Android APK

### 共同的地方

- 能本地就不联网，能原生控件就不堆依赖
- 数据属于使用者：可导出、可备份、可带走
- 界面干净、可扫读，少即是多
- 单文件能解决的事，不拆成十个模块

### 技术

原生 HTML / CSS / JavaScript · Electron · Capacitor · Python（tkinter / OpenCV）

---

所有项目以 MIT 许可发布，下载见各仓库 Releases。
