# 🟩 VitroxCraft — ViTrox Campus 2.0 方块教育世界

A web-based, Minecraft-education-style voxel world that recreates
**[ViTrox Campus 2.0 by CYC Architect](https://www.cycarch.com/vitrox-campus-20)**
(Batu Kawan, Penang, Malaysia) — playable in any desktop browser, no installation.

以 CYC Architect 设计的 ViTrox Campus 2.0 为蓝本的网页版 Minecraft 教育体验：
中央圆形庭院、放射状布局、环形景观坡道、无门入口、绿色屋顶，以及与圆形体量相交的矩形生产办公楼。

## ▶ 开始游玩 / Play

- **在线**（开启 GitHub Pages 后）：`https://<你的用户名>.github.io/vitroxcraft/`
- **本地**：下载 `index.html`，双击用 Chrome / Edge 打开（首次需联网加载 Three.js）

电脑键鼠体验最佳，手机/平板有触屏操作（摇杆 + 按钮）。完整操作说明、多人连线教程、FAQ 和课堂建议见 **[使用说明书 MANUAL.md](MANUAL.md)**。

## ✨ 功能 / Features

- 🏛 **建筑还原** — 按真实设计概念参数化生成：圆形庭院、两层环形楼与玻璃幕墙、螺旋景观坡道、屋顶花园与环形光伏雨棚、庭院楼梯塔、VITROX 方块招牌、食堂与洗碗棚、篮球场与两个停车场，以及东侧 Campus 3.0 扩建区（光伏屋顶板楼 + 鱼池庭院）
- 🌐 **三语界面** — 中文 / English / Bahasa Melayu，一键切换，界面与讲解全翻译（首次打开自动匹配浏览器语言）
- 🧑‍🤝‍🧑 **NPC 人物** — 8 位园区角色（保安、工程师、厨师、建筑师…）分布各处，走近会转身看你，按 E 三语对话并为你指路
- 📚 **教育模式** — 8 个金色信息点讲解建筑设计理念（放射布局、实与虚、几何并置、绿色建筑…），带任务清单与探索进度
- ⛏ **自由建造** — 挖/放 9 种方块，改动自动存档（localStorage），可一键重置
- 🌐 **多人连线** — 基于 WebRTC（PeerJS）点对点，房主建房间发 5 位代码，同学即可加入；位置与方块实时同步，无需服务器
- 📦 **单文件零构建** — 一个 `index.html`，Three.js 体素引擎，纹理全部程序化生成

## 🛠 Enable GitHub Pages

Settings → Pages → Source: **Deploy from a branch** → Branch: `main` / `(root)` → Save.
约一分钟后即可通过上面的网址访问。

---

*建筑原型版权归 CYC Architect / ViTrox 所有；本项目为教育用途的方块化演绎，非精确比例模型。*
