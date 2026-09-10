# 数据结构与计算机网络可视化学习实验室

一个面向数据结构与计算机网络课程的本地可视化学习工具。项目将算法动画、C99 示例代码、章节知识、网络知识图谱和课程材料组织在同一个网页工作台中，下载完整包后可以直接在 Windows 上运行。

## 项目简介
<img width="1257" height="695" alt="image" src="https://github.com/user-attachments/assets/5119a3ff-7c05-41aa-b944-a898509d2e8d" />


这个项目希望把抽象的算法过程和网络概念变得更直观。学习者可以逐步观察数据结构的状态变化，对照示例代码理解实现，也可以通过交互式知识图谱梳理计算机网络章节之间的关系。

完整交付包已经包含便携 Node.js 运行环境和配套 PPT，无需安装 Node.js，也不需要执行 `npm install`。启动后服务只在本机运行，以本地WEB形式呈现，适合课程复习、课堂演示和个人实验。

## 主要功能

### 数据结构
<img width="1271" height="699" alt="image" src="https://github.com/user-attachments/assets/f2c4ceb5-0614-43f7-b00f-9a8f1de6ed85" />


- 覆盖 DS1–DS9 的章节内容、算法动画和状态演示。
- 提供 37 份 C99 示例源码，涵盖线性表、栈与队列、字符串、树、图、查找和排序。
- 支持逐步执行算法，并同步观察关键数据状态。

### 计算机网络
<img width="1268" height="704" alt="image" src="https://github.com/user-attachments/assets/e22601e2-f66b-4473-ad76-8df4ececf142" />


- 提供独立的英文课程界面和章节导航。
- 包含重点词汇中英对译与点击式知识图谱。
- 可定位原始 PPT 证据页，并提供 596 张课程材料索引缩略图。

### 本地学习工作台
<img width="1071" height="368" alt="image" src="https://github.com/user-attachments/assets/3b2344af-7a7a-4522-8665-bb3a37199a27" />


- 支持 AI 伴学、用量统计和“我的工作区”。
- 两门课程共享本机 AI 接口配置，但会自动使用当前科目的课程上下文。
- 自定义内容保存在本地，聊天记录保留在当前浏览器中。

### AI伴学聊天框
<img width="389" height="704" alt="image" src="https://github.com/user-attachments/assets/35536f6d-177b-473e-9a3d-78c2bf4bcc47" />

- 内置SKILL.可以自动同步左侧可视化交换界面的学习章节，直接提问即可回答相关知识。
- 在数据结构学习栏目中，与AI聊天或询问到相关知识时，可在输出文字里面自动生成相应的链接，您点击以后即可自动跳转到相应的可视化交互界面并自动播放（计算机网络学习界面暂未开发此功能）。

## 下载完整可运行包

- [直接下载 ZIP](https://github.com/999dy999-create/visual-learning-lab/releases/download/full-package-v1.0.0/data-structures-network-full-package.zip)
- [查看 Release 页面](https://github.com/999dy999-create/visual-learning-lab/releases/tag/full-package-v1.0.0)
- 原始文件名：`数据结构&计网_压缩包.zip`
- GitHub 附件名：`data-structures-network-full-package.zip`
- 文件大小：270,254,753 字节（约 257.74 MiB）
- SHA-256：`8D07B7AA5D7200E606E6BBC7BB37262CAA31FC732B92DBA9DFAB263C572E6DA7`

GitHub 为确保下载链接兼容性使用了英文附件名；压缩包内容没有修改，SHA-256 与本地原文件一致。

## 解压后如何运行

1. 下载完整 ZIP 并解压，保持文件夹结构不变。
2. 双击根目录的 `00_启动学习实验室.cmd`。
3. 启动脚本会使用包内自带的 Node.js，无需安装依赖。
4. 本地服务就绪后浏览器会自动打开，若不能打开，请复制cmd里面的本地网址到浏览器自行打开。默认端口为 `4173`；端口被占用时会自动选择其他端口。
5. 若需AI伴学，请打开AI伴学助手侧边栏，并点击右上角的设置按钮，填写API密钥，保存配置即可使用。

请不要直接双击 `WEB/index.html`。使用 `file://` 打开只能读取部分静态内容，无法可靠连接本地 API。启动失败时可以查看 `WEB/.local-data/server.log`。

## 压缩包主要内容

```text
数据结构学习实验室_可交付包/
├── 00_启动学习实验室.cmd       # 推荐启动入口
├── WEB/                        # 网页应用与本地服务
│   ├── runtime/node.exe        # 便携 Node.js
│   ├── network/                # 计算机网络课程模块
│   └── assets/slides/          # 课程材料索引缩略图
├── DS0.ppt ... DS9.ppt         # 数据结构课程材料
├── 计算机网络/                 # 计算机网络课程材料
├── PROJECT_GUIDE.md            # 架构与维护说明
└── README_交付包运行说明.md     # 包内运行说明
```

## 隐私与配置

- 压缩包不包含 API Key、Token 或个人 AI 服务配置。
- 如需使用 AI 助手，请在解压后的网页设置中填写自己的接口、模型和密钥。
- API 密钥只保存在使用者自己的浏览器中。
- 工作区内容保存在 `WEB/data/custom-sections.json`，AI 聊天历史保存在当前浏览器。

## 技术栈

- HTML5、CSS3、原生 JavaScript
- Node.js 内置 `http` 模块
- C99 示例程序
- PowerPoint COM 自动化（Windows）

## 作者

- 华中科技大学人工智能与自动化学院 徐多泽
