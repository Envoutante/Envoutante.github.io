## 准备

1.在 demo 中填写 APPID、APISecret、APIKey，可到控制台-我的应用-大模型页面获取 2.安装 nodejs

## 本地运行

1.打开 cmd，进入 demo 目录，执行如下命令

```
npm i
npm run dev
```

> npm i 中有一段会从 github 上下载内容，但是有个 node-sass 被墙掉了，挂 VPN 也不行。解决方法：[参考这篇博客](https://blog.csdn.net/weixin_42132439/article/details/115720095?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522171066392416800197057823%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=171066392416800197057823&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduend~default-1-115720095-null-null.142^v99^pc_search_result_base3&utm_term=Downloading%20binary%20from%20https%3A%2F%2Fgithub.com%2Fsass%2Fnode-sass%2Freleases%2Fdownload%2Fv4.14.1%2Fwin32-x64-83_binding.node%20Cannot%20download%20https%3A%2F%2Fgithub.com%2Fsass%2Fnode-sass%2Freleases%2Fdownload%2Fv4.14.1%2Fwin32-x64-83_&spm=1018.2226.3001.4187)

2.在 chrome 浏览器中打开本机 IP 地址，可打开 cmd 输入 ipconfig 获取，例如
http://127.0.0.1:8080/index.html
ip 和端口以返回的信息为准

## 部署到服务器

1. 决定部署到服务器的文件夹。
   如果是根目录直接运行第二步，
   如果非根目录，如：test，请将 build/config 中的 build.assetsPublicPath 改为/test/，然后运行第二步
2. 打开 cmd，进入 demo 目录，执行如下命令

```
npm install
npm i cross-env@3.0.0
npm run build
```

3.  将第二步编译后的 dist 文件夹中的内容（非 dist）复制到指定的文件夹

## 注意事项

1.请使用 chrome 浏览器测试。 2.如程序报错 5 位错误码，请到文档或错误码链接查询
https://www.xfyun.cn/doc/spark/Web.html#_1-%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E
https://www.xfyun.cn/document/error-code
