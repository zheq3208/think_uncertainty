# haha.github.io 静态站点说明

这个目录里放的是一个可直接部署到 GitHub Pages 的静态页面。

## 你需要做的事

### 1) 先确认你的目标网址是否真的能是 `https://haha.github.io/`
只有在 **GitHub 用户名或组织名本身就是 `haha`** 的情况下，仓库名创建为 `haha.github.io`，最终网址才会是这个地址。

如果你的 GitHub 用户名不是 `haha`，那会有两种情况：
- 个人/组织主页：`https://你的用户名.github.io/`
- 项目页：`https://你的用户名.github.io/仓库名/`

### 2) 新建仓库
在 GitHub 新建一个仓库：
- 如果你账号名就是 `haha`：仓库名用 `haha.github.io`
- 否则：随便起名，比如 `haha-site`

### 3) 上传文件
把当前目录里的 `index.html` 上传到仓库根目录。

### 4) 开启 GitHub Pages
GitHub 仓库里进入：
- Settings
- Pages
- Build and deployment
- Source 选 `Deploy from a branch`
- Branch 选 `main`
- Folder 选 `/ (root)`

保存后等几十秒到几分钟即可访问。

## 当前版本的特点
- 已经尽量复刻原站的学术主页布局。
- 页面顶部站点名已经改成了 `haha.github.io`。
- 当前图片直接引用的是原站公开图片 URL，部署后能立刻看到效果。
- 这意味着它依赖原站继续在线。更稳妥的做法是把图片下载到你自己的仓库里，再改成本地路径。

## 你接下来最适合做的两件事

### A. 最快上线
直接上传 `index.html`，先让站点跑起来。

### B. 做成真正独立版本
把这些远程图片下载后放到你的仓库里：
- `https://pyspatial.github.io/static/img/teaser.png`
- `https://pyspatial.github.io/static/img/example.png`
- `https://pyspatial.github.io/static/img/robotDemo.png`
- `https://pyspatial.github.io/static/img/icons/connector.svg`
- `https://pyspatial.github.io/static/img/icons/visual.svg`
- `https://pyspatial.github.io/static/img/icons/eval.svg`
- `https://pyspatial.github.io/static/img/icons/recipe.svg`

然后把 `index.html` 里的这些 URL 改成例如：
- `assets/img/teaser.png`
- `assets/img/example.png`
- `assets/img/robotDemo.png`
- `assets/img/icons/connector.svg`

## 最常改的地方
在 `index.html` 里搜索这些内容：
- `haha.github.io`：站点显示名
- `<title>haha.github.io</title>`：浏览器标签名
- `<h1>pySpatial</h1>`：页面主标题
- 各个论文链接、作者链接、图片链接

