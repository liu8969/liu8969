## Skill 合集

四十来个仓库，都是围绕 **Agent skill / MCP / 工具链** 的。按用途分好组放在下面，省得在仓库列表里翻。

<sub>40 个仓库 = 11 公开 + 30 私有　·　**加粗**是公开仓库　·　带 · 的是私有，你点得开、别人点开是 404</sub>

---

### 🧪 验证与门禁

<sub>改完代码，怎么知道它是对的</sub>

| 仓库 | 说明 |
|---|---|
| [qa-flow](https://github.com/liu8969/qa-flow) · | 分层测试与门禁（qa CLI）。 |
| [sec-review](https://github.com/liu8969/sec-review) · | 用安全标准合集审查代码：一份可查询判据（OWASP / ASVS / CWE / 语言级规则集）， |
| [EasyReviewer](https://github.com/liu8969/EasyReviewer) · | 夜间代码审查产线（本地模型 + sec-review）：nightrev CLI/run/schedule/digest … |
| [skill-eval](https://github.com/liu8969/skill-eval) · | skill 触发率评测；runs/ .work/ 是产物。 |

### 🌐 浏览器与抓取

<sub>把网页变成能读、能断言的东西</sub>

| 仓库 | 说明 |
|---|---|
| [browser-mcp](https://github.com/liu8969/browser-mcp) · | 本机 stdio MCP，跑 <repo>/.venv/bin/python run_server.py；venv 平台绑… |
| [grabber-mcp](https://github.com/liu8969/grabber-mcp) · | MCP 本体是 ubuntu-dev 上的远端 HTTP 端点；references/ 原来只活在 ~/.dsh/skil… |

### 🚚 部署与基础设施

<sub>送上去、连上去、绕过去</sub>

| 仓库 | 说明 |
|---|---|
| [deploy-skill](https://github.com/liu8969/deploy-skill) · | 把本地项目同步到 Hyper-V 里的 Ubuntu VM（ubuntu-dev），构建、启动、等健康， |
| [server-access](https://github.com/liu8969/server-access) · | 内网六台机器的唯一入口；密钥在 /etc/srvctl/keys（root-only，不进 git）。 |
| [mirror-router](https://github.com/liu8969/mirror-router) · | 服务跑在 ubuntu-dev:8899/8443，本机只装 skill（地址与走法）。 |
| [cloudvault](https://github.com/liu8969/cloudvault) · | Go 项目；.gocache/.gomodcache/.gopath 必须排除（194MB → 源码不到 1MB）。 |
| [ssh-maneger](https://github.com/liu8969/ssh-maneger) · | 远程管理ubuntu ai服务器 |
| [ssh-start2.0](https://github.com/liu8969/ssh-start2.0) · | 一个用于管理盘古AI服务器的SSH连接工具，支持vLLM和Dify服务的启动和管理。 |
| [mac-remote-tools](https://github.com/liu8969/mac-remote-tools) · | 从 Mac 一键开 Ubuntu 上的远端 VS Code：Dock 选择器 + codeu/dsh-ubuntu + 自… |
| [remote-agent-iphone](https://github.com/liu8969/remote-agent-iphone) · | 从 iPhone 远程操作/审批本机 Coding Agent 的方案，以及 DSH 侧的 web-boot-guard … |

### 🖥️ 本地模型与算力

<sub>自己那几张卡上的模型，部署、压测、看读数</sub>

| 仓库 | 说明 |
|---|---|
| **[dual-5060ti-qwen38](https://github.com/liu8969/dual-5060ti-qwen38)** | GPU 模型部署项目；它同时出一个 DSH 宿主插件（「接入本地大模型」：发现端口/模型名/ 上下文 → 建 provid… |
| [model-bench](https://github.com/liu8969/model-bench) · | 含 52MB 语料，只在需要压测的机器上装。 |
| [gpu-model-dashboard](https://github.com/liu8969/gpu-model-dashboard) · | 本机 GPU 推理引擎的实时监控面板：抓引擎自己的 Prometheus /metrics，做计数器差分，给出 |
| **[VllmTester](https://github.com/liu8969/VllmTester)** | vLLM Concurrency Testing Tool |
| **[qwen_rtx5060ti_concurrency_bench](https://github.com/liu8969/qwen_rtx5060ti_concurrency_bench)** |  |
| **[Run-vllm-on-nvidia-50-Series](https://github.com/liu8969/Run-vllm-on-nvidia-50-Series)** | Run vllm on nvidia RTX 50 Series in Ubuntu24.04 LST |

### 🧩 DSH 本体

<sub>让 harness 自己更好用的那批组件</sub>

| 仓库 | 说明 |
|---|---|
| [dsh-sync](https://github.com/liu8969/dsh-sync) · | 清单 + 引擎 + 同步插件本体。这三个孤儿 skill 原来只活在 ~/.dsh/skills 里。 插件占两个座：会话… |
| [skill-issues](https://github.com/liu8969/skill-issues) · | skill 反馈通道 + AI 分诊；宿主插件是唯一能绕开工具沙箱写 ~/.dsh 的通道。 |
| [dsh-core-plugins](https://github.com/liu8969/dsh-core-plugins) · | 仓库里还留着 local-models-sync.v1.mjs 作上一代存档，但不再声明为安装项 —— 2026-09-2… |
| [dsh-plan](https://github.com/liu8969/dsh-plan) · | Plan 评审旁的「白话解释 / 复制 Plan」两枚胶囊 + 计划面板开关。 |
| [dsh-reboot](https://github.com/liu8969/dsh-reboot) · | 「设置 → 常规」里的重启按钮 + 重启后验收结论；重启语义两端完全不同 （linux = systemd 把 SIGTE… |
| [hover-gloss](https://github.com/liu8969/hover-gloss) · | 悬浮取词：鼠标停在英文单词上弹中文释义 + 词根/词源 + 美/英发音。 释义本地优先（ECDICT 裁剪词库 5.8 万… |

### 🎬 内容生产

<sub>从代码、网盘、视频里做东西</sub>

| 仓库 | 说明 |
|---|---|
| [code-video](https://github.com/liu8969/code-video) · | 纯代码做视频：Three.js/Canvas 逐帧画 → 无头 Chrome 截图 → FFmpeg 合成 + 代码合成音… |
| [quarkclouddrive](https://github.com/liu8969/quarkclouddrive) · | 夸克网盘官方(Quark Drive)Skill，用于文件上传/下载（支持断点续传）、文件分享与转存、转存分享更新查询、网… |
| [emil-skills](https://github.com/liu8969/emil-skills) · | 标准模式（standard）+ 13 个界面/动效 skill 的 preset。其中 review-animations… |
| [blender-model](https://github.com/liu8969/blender-model) · | 「Blender 建模」preset 专用的结构校验与多角度出图工具。入口 bm。 |
| [dsh-video](https://github.com/liu8969/dsh-video) · | 用代码与 AI 编排做视频的内容管线工作区。 |

### 📦 实验与归档

<sub>试过、参考过，或已停用；留作历史</sub>

| 仓库 | 说明 |
|---|---|
| **[Anti-Clog-Printer](https://github.com/liu8969/Anti-Clog-Printer)** | 定时自动打印彩色测试页，防止喷墨打印机喷嘴堵塞。支持 macOS 桌面 GUI 和 Docker Web 管理两种运行方式。 |
| [todo-list](https://github.com/liu8969/todo-list) · |  |
| [pdf--codex](https://github.com/liu8969/pdf--codex) · | 把 PDF 里的所有文本自动提取出来、用 DeepSeek 并发翻译成中文，再把译文插回原文所在的位置，输出一份与原文档版… |
| **[test1](https://github.com/liu8969/test1)** | 这是一个简单的测试项目，旨在尝试合作 |
| **[share](https://github.com/liu8969/share)** |  |
| [dsh-share](https://github.com/liu8969/dsh-share) · | 旧的"一次性导出"设施，被本仓库取代；保留作历史与 Windows 安装脚本参考。 |
| **[awesome-design-md](https://github.com/liu8969/awesome-design-md)** | Collection of DESIGN.md files that capture design systems fro… |
| **[claw-code](https://github.com/liu8969/claw-code)** | Better Harness Tools, not merely storing the archive of leake… |
| **[claude-code-source-code](https://github.com/liu8969/claude-code-source-code)** | Claude Code v2.1.88 Source Code |

---

<sub>这份目录由 `dsh-sync` 的清单生成 —— 真源只有那份清单一份，这里只是它的一个视图。</sub>
