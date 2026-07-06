# 个人主页（用于 AAAI / OpenReview 注册）

一个纯静态的学术个人主页，用 GitHub Pages 免费托管后会得到一个公开网址，
填进 AAAI / OpenReview 注册页的「Homepage / Personal Website」一栏即可。

## 一、先改内容

用记事本 / VS Code 打开 `index.html`，把里面的占位信息改成你自己的：

- 标题 `<title>` 和页面里的 **Your Name / 你的姓名**
- 邮箱 `you@example.edu`、单位、研究方向
- GitHub / Google Scholar / ORCID 链接（没有的可以删掉那一行）
- 有证件照就把图片命名为 `photo.jpg` 放到同目录，并按 `index.html` 里第 128 行附近的注释把头像换成 `<img>`
- 填完后删掉页面顶部那个黄色的「填写提示」框

> 重要：主页上的**姓名、邮箱要和你在 AAAI/OpenReview 里填的一致**，审核才容易通过。

本地预览：直接双击 `index.html` 用浏览器打开即可。

## 二、放到 GitHub（两种方式，选一种）

### 方式 A：个人站点（网址最短，推荐）
仓库名必须叫 `你的用户名.github.io`，网址就是 `https://你的用户名.github.io/`。

```bash
# 在本文件夹（homepage）里执行
git init
git add .
git commit -m "Add personal homepage"
git branch -M main
git remote add origin https://github.com/你的用户名/你的用户名.github.io.git
git push -u origin main
```
在 GitHub 网页里进入这个仓库 → Settings → Pages，Source 选 `main` 分支、`/ (root)`，保存。
等一两分钟后访问 `https://你的用户名.github.io/`。

### 方式 B：项目站点（仓库名随意，比如 homepage）
网址是 `https://你的用户名.github.io/homepage/`。
命令同上，只是 remote 换成你建的那个仓库地址，push 后在 Settings → Pages 里同样开启即可。

## 三、把网址填进 AAAI

拿到 `https://你的用户名.github.io/...` 这个网址后，
在 AAAI / OpenReview 注册时填到「Homepage」或「Personal Website URL」那一栏。
