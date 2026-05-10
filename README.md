# 郑嘉铭个人主页

这个目录已经整理成可以直接部署到 `GitHub Pages` 的静态个人主页。

## 当前文件

- `index.html`：主页主文件
- `styles.css`：页面样式
- `.nojekyll`：告诉 GitHub Pages 按纯静态站点发布

## 怎么本地看效果

最简单的方法：

1. 进入这个目录
2. 双击 `index.html`
3. 浏览器会直接打开页面

如果你想用本地服务器方式预览，可以在这个目录打开终端后运行：

```powershell
python -m http.server 8000
```

然后访问 `http://localhost:8000`

## 怎么上传到 GitHub

最省事的是直接用网页上传：

1. 登录 GitHub
2. 点右上角 `+`
3. 选择 `New repository`
4. 仓库名建议填：
   - `zhengjiaming-homepage`
   - 或者如果你想要更标准的个人站网址，可以用 `你的GitHub用户名.github.io`
5. 仓库建议设为 `Public`
6. 创建仓库后，进入仓库主页
7. 点击 `Add file`
8. 选择 `Upload files`
9. 把这个文件夹里的这几个文件拖进去：
   - `index.html`
   - `styles.css`
   - `.nojekyll`
10. 等上传完成后，点击页面底部 `Commit changes`

## 怎么开启 GitHub Pages

根据 GitHub Docs 当前流程：

1. 进入你刚创建的仓库
2. 点击仓库上方的 `Settings`
3. 在左侧找到 `Pages`
4. 在 `Build and deployment` 里：
   - `Source` 选择 `Deploy from a branch`
   - `Branch` 选择 `main`
   - `Folder` 选择 `/(root)`
5. 点击 `Save`
6. 等待几十秒到几分钟，GitHub 会自动发布

## 发布后网址是什么

如果你的仓库名是普通名字，比如：

- `zhengjiaming-homepage`

那网址通常是：

- `https://你的用户名.github.io/zhengjiaming-homepage/`

如果你的仓库名直接就是：

- `你的用户名.github.io`

那网址通常就是：

- `https://你的用户名.github.io/`

## 之后如果要继续改

你只需要重新上传并覆盖这几个文件，再提交一次，页面就会自动更新。

## 备注

如果你后面要加头像、项目图、简历 PDF 下载，我建议再补一个 `assets/` 文件夹专门放图片和附件。
