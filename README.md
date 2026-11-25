# 331KB 门面页

**给 AI API 中转站用的单文件落地页。**

只有一个 `index.html`，零外链、零网络请求，断网能开。背景是手写的 WebGL 粒子流与 3D 环，没引任何库。手机上首屏一屏 + 底部抽屉，桌面上左文案、右数据。

<img src="https://aka.doubaocdn.com/s/RenreADq0u" width="100%" alt="桌面首屏">
<img src="https://aka.doubaocdn.com/s/Lj8wdZMgmT" width="300" alt="手机首屏">

---

## 站长痛点

- 中转站默认面板丑得像十年前的测试后台，拿来当门面拿不出手。
- 手机端占了七成流量，访客点开只能捏着屏幕来回缩放。
- 请外包做官网花几百到几千，买完发现改一行文案都改不动。
- 模板站清一色 MUI 味，换个 Logo 就像同一家作坊批发的。

这套东西就是拿这四条做的。

---

## 特性

- **单文件交付**：整个站只有 1 个 `index.html`，327 KB。
- **零请求加载**：0 外链、0 网络请求。打开网络面板从头到尾是空的。
- **内置 30 个工具**：哈希、JWT、格式化、转换、生成器，全部真实现，不是占位卡片。
- **本地运行**：30 个工具都在浏览器里跑，不上传任何数据。
- **手写 WebGL**：0 第三方库，粒子流 + SDF 3D 环 + 透视地平线，约 3 KB 着色器。
- **双端两套骨架**：手机一屏 + 底部抽屉，桌面左文案右数据双栏。

---

## 改成你自己的中转站

三步，不用装任何环境：

1. **换颜色** —— 改 `<style>` 顶部一排变量，`--accent` 换掉就是你自己的品牌色。
2. **换内容** —— 中间 30 格工具区换成你的模型列表、价格表、充值入口；首屏左栏的标题、说明、按钮都是纯文本，直接改字。
3. **部署** —— 丢进 GitHub Pages、任意静态托管，或者直接给人发文件、拷 U 盘都行。

推送到 `main` 会自动触发 `.github/workflows/pages.yml` 部署。

---

## 内置的 30 个工具（demo 位）

| 区 | 工具 |
| --- | --- |
| 转换 | Base64、URL 编解码、JSON/YAML、CSV 转 JSON、时间戳 |
| 格式化 | JSON、SQL、HTML、CSS、Markdown 预览 |
| 加密 | SHA-1/256/512、HMAC、UUID v4、JWT 解码、bcrypt 校验 |
| 生成 | 二维码、密码、Lorem、slug、配色、meta 标签 |
| 开发 | 正则测试、文本 diff、字数统计、cron 构建、假数据、大小写转换 |

这 30 个是填位用的，证明这套骨架能装东西。中转站应该把它们换成模型和价格。

---

## 本地运行

双击 `index.html`。没有 `npm install`，没有构建步骤，没有 node_modules。

---

## English

A single-file landing page for AI API relay sites. One `index.html`, 327 KB, zero external links and zero runtime requests — it works offline. The background is hand-written WebGL: a particle field, an SDF 3D ring, a perspective floor, about 3 KB of shader code and no libraries. Mobile gets a one-screen hero with a bottom sheet; desktop gets a left-copy / right-data split. Swap the 30 demo tools for your own model list and pricing, change one accent variable, ship it anywhere.

---

## License

MIT
