# 微电网课程大作业 · 静态网站

作者：**吴浩辉** ｜ 学号：**202410132011**

本目录包含两次大作业的完整静态网站，均为纯前端（HTML + CSS + JavaScript）实现，无任何外部依赖，可离线打开，也可直接部署到任意静态托管平台。

## 已部署网址（GitHub Pages）

- 作品导航：<https://huihuhi669.github.io/microgrid-hw/>
- 第二次作业（控制框图仿真）：<https://huihuhi669.github.io/microgrid-hw/hw2-control/>
- 第三次作业（EMS 界面）：<https://huihuhi669.github.io/microgrid-hw/hw3-ems/>

## 目录结构

```
sites/
├── index.html          作品导航首页（可选，把两次作业串在一起）
├── hw2-control/        第二次大作业：第四章 微电网控制技术 框图仿真
│   └── index.html
├── hw3-ems/            第三次大作业：微电网能量管理系统（EMS）
│   └── index.html
└── README.md
```

## 本地预览

直接双击 `sites/index.html` 即可在浏览器中打开；无需安装任何环境。

> 若浏览器对本地文件有限制，可在 `sites` 目录下执行 `python -m http.server 8000`，然后访问 `http://localhost:8000/`。

## 部署为长期有效的网址

### 方案 A：GitHub Pages（推荐，免费且长期有效）

1. 登录 GitHub，新建公开仓库，例如 `microgrid-hw`。
2. 将本 `sites` 目录中的全部内容上传到仓库根目录（网页上传或 `git push` 均可）。
3. 打开仓库 **Settings → Pages**：
   - Source 选择 **Deploy from a branch**
   - Branch 选择 `main`，目录选择 `/ (root)`
4. 等待约 1 分钟，得到网址：
   - 首页：`https://<你的用户名>.github.io/microgrid-hw/`
   - 第二次作业：`https://<你的用户名>.github.io/microgrid-hw/hw2-control/`
   - 第三次作业：`https://<你的用户名>.github.io/microgrid-hw/hw3-ems/`

### 方案 B：Netlify Drop（最快，拖拽即可）

1. 打开 <https://app.netlify.com/drop>。
2. 把整个 `sites` 文件夹拖入页面。
3. 立即得到形如 `https://xxxx-yyyy.netlify.app/` 的网址，其中：
   - `/hw2-control/` 为第二次作业
   - `/hw3-ems/` 为第三次作业
4. 注册账号后可将站点“Claim”并长期保留（建议把站点名改成有意义的名字）。

### 方案 C：Cloudflare Pages

1. 打开 Cloudflare Dashboard → Workers & Pages → Create → Pages → Upload assets。
2. 上传 `sites` 文件夹内容，得到 `https://<项目名>.pages.dev/` 网址。

## 交付要求核对

- [x] 第二次作业：第四章控制框图 → 可交互界面 → 可仿真（波形、频率、功率动态）
- [x] 第三次作业：微电网能量管理系统界面（24 h 调度、储能 SoC、电价、消纳率）
- [x] 每个页面均显示姓名 **吴浩辉** 与学号 **202410132011**（页头、页脚、网页标题、meta 作者）
- [x] 纯静态网站，无外部 CDN 依赖，长期可访问、可离线运行
