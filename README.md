<div align="center">
  
![QLDependency Logo](https://cdn.jsdelivr.net/gh/youink/QL-Dependency@main/assets/QQ20220115-203256.png)

</div>

<!--Trap--:)-->
<a href="https://github.com/404"><img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif"></a>

<!-- ![青龙面板](https://user-images.githubusercontent.com/94276146/142231757-380c5221-7569-468e-9f68-2d09afeef538.png) -->

***

<h1 align="center">【青龙】全依赖环境一键安装脚本 | QLDependency </h1>

<div align="center">

A timed task management panel that supports typescript, javaScript, python3, and shell.（支持python3、javaScript、shell、typescript 的定时任务管理面板）

[![docker docker version][docker-version-image]][docker-version-url]

<!-- [![docker version][docker-version-image]][docker-version-url] [![docker pulls][docker-pulls-image]][docker-pulls-url] [![docker stars][docker-stars-image]][docker-stars-url] [![docker image size][docker-image-size-image]][docker-image-size-url] -->
<!-- [![docker image size][docker-image-size-image]][docker-image-size-url] -->
<!-- [docker-pulls-image]: https://img.shields.io/docker/pulls/whyour/qinglong?style=flat -->
<!-- [docker-pulls-url]: https://hub.docker.com/r/whyour/qinglong -->
[docker-version-image]: https://img.shields.io/docker/v/whyour/qinglong?style=flat
[docker-version-url]: https://hub.docker.com/r/whyour/qinglong/tags?page=1&ordering=last_updated
<!-- [docker-stars-image]: https://img.shields.io/docker/stars/whyour/qinglong?style=flat -->
<!-- [docker-stars-url]: https://hub.docker.com/r/whyour/qinglong -->
![GitHub Repo stars](https://img.shields.io/github/stars/youink/QL-Dependency)
![GitHub forks](https://img.shields.io/github/forks/youink/QL-Dependency)
![GitHub Workflow Status](https://img.shields.io/github/workflow/status/youink/QL-Dependency/Release)
[![docker-image-size-image]][docker-image-size-url]
![GitHub](https://img.shields.io/github/license/youink/QL-Dependency)
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FFlechazoPh%2FQLDependency.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FFlechazoPh%2FQLDependency?ref=badge_shield)

![GitHub Repo stars](https://img.shields.io/github/stars/whyour/qinglong)

[docker-image-size-image]: https://img.shields.io/docker/image-size/whyour/qinglong?style=flat
[docker-image-size-url]: https://hub.docker.com/r/whyour/qinglong
 
  
<h2 <b>本仓库原地址【 https://github.com/FlechazoPh/QLDependency 】</b> </h2><br>

<details>
<summary>链接文档 点我展开</summary>


<b>【Gitee 仓库地址(方便国内小伙伴访问)】https://gitee.com/exting/QLDependency </b> <br>

【GitBook 文档仓库地址】https://doc.flechazo.ml/青龙/2021-11-17-青龙依赖一键安装脚本.html <br>

【Telegram 群组】:airplane: https://t.me/github_chats <br>


</div>

<br>

</details>

欢迎前往原作者仓库右上角点 <b>⭐ Star 收藏和 关注 Follow</b>

# QLDependency
# 青龙全依赖一键安装脚本 部署文档


**[安装报错等常见问题参考](#常见问题)**


<!-- 文档地址： [GitBook 文档](https://doc.flechazo.ml/青龙/2021-11-17-青龙依赖一键安装脚本.html) -->


## 特别声明

<details>
<summary>特别声明 点我展开</summary>


- 本项目内所有资源文件，禁止任何公众号、自媒体进行任何形式的转载、发布。

- 本人对任何脚本问题概不负责，包括但不限于由任何脚本错误导致的任何损失或损害。

- 间接使用脚本的任何用户，包括但不限于建立VPS或在某些行为违反国家/地区法律或相关法规的情况下进行传播, 本人对于由此引起的任何隐私泄漏或其他后果概不负责。

- 请勿将本仓库的任何内容用于商业或非法目的，否则后果自负。

- 如果任何单位或个人认为该项目的脚本可能涉嫌侵犯其权利，则应及时通知并提供身份证明，所有权证明，我们将在收到认证文件后删除相关脚本。

- 任何以任何方式查看此项目的人或直接或间接使用该项目的任何脚本的使用者都应仔细阅读此声明。本人保留随时更改或补充此免责声明的权利。一旦使用并复制了任何相关脚本或Script项目的规则，则视为您已接受此免责声明。

**您必须在下载后的24小时内从计算机或手机中完全删除以下内容**
</details>

> ***您使用或者复制了本仓库且本人制作的任何脚本，则视为 `已接受` 以上声明，请仔细阅读***


***

新版本的青龙(2.10.2+ )，在运行脚本的时候，经常出现

```bash

“ Cannot find module 'xxxx' ” 

or

“ 'xxxx' module not found ” 

```

的报错问题 ，原因就是缺少 xxxx 模块，mudole的名字就是报错的 xxxx。

为解决新版本依赖问题，可以在安装时直接一键部署全部所需的依赖，以免后患：




一键安装单独青龙的依赖
国内版：


```bash

docker exec -it qinglong bash -c "$(curl -fsSL https://ghproxy.com/https://raw.githubusercontent.com/youink/QL-Dependency/main/Shell/QLOneKeyDependency.sh | bash)"

```





国外版：

```bash

docker exec -it qinglong bash -c "$(curl -fsSL https://raw.githubusercontent.com/youink/QL-Dependency/main/Shell/QLOneKeyDependency.sh | bash)"

```


**【更新】** 版本号 2.12+ 的新版本青龙安装失败请尝试：

```bash

docker exec -it qinglong bash -c "$(curl -fsSL https://raw.githubusercontent.com/youink/QL-Dependency/main/Shell/XinQLOneKey.sh | bash)"

```


## 具体执行方法：

> 安装拉取青龙镜像的就不说了，教程都有 `` docker pull whyour/qinglong:latest ``

0. 点击本页面 右上方的 **Star**

1. SSH 进入服务器（或群辉，或软路由等终端环境），输入 `` docker ps ``，查看 青龙 Docker 是否正常运行，记下青龙 Docker的容器名字 ，然后进入下一步。

![Docker](https://user-images.githubusercontent.com/94276146/142231910-c2d71ab6-869c-4153-b9bf-29bcd40ca2a4.png)


2. 输入一键安装命令，如果你的青龙容器不叫 qinglong，需要替换为相应的容器名字（国外鸡，可以使用上面的国外脚本，速度比较快）： 
```bash

docker exec -it qinglong bash -c "$(curl -fsSL https://ghproxy.com/https://raw.githubusercontent.com/youink/QL-Dependency/main/Shell/QLOneKeyDependency.sh | bash)"

```
3. 查看输出日志：
![SSH](https://user-images.githubusercontent.com/94276146/142231876-b842d1a5-bdbb-45e3-9fa5-38ba956f1dbf.png)


4. 等进度条走完，等待的时候因机器性能而异，性能差有的时间可能会非常长...

![npm](https://user-images.githubusercontent.com/94276146/142231949-56302ec2-f169-44a0-92d3-e0b778afbec3.png)



5. 最后输出，就完成了，重启下青龙 Docker ：

```bash

docker restart qinglong

```



6. 依赖安装完毕...

End

不介意的话顺手点个 **★ Star ** (本页面顶部右上方 ★ ), **方便以后收到脚本更新~**


## 常见问题

安装报错等常见问题请参考： 
* [常见问题答疑](https://github.com/youink/QL-Dependency/issues?q=is%3Aissue+is%3Aclosed)

## 附：
有新的需要的依赖，请测试完成后提交pull request，等待审核通过合并到项目中


## 鸣谢

* [qinglong](https://github.com/whyour/qinglong)

* [crontab-ui](https://github.com/alseambusher/crontab-ui)

* ![logo](https://github.com/youink/QL-Dependency/assets/94276146/050e2f90-60bb-438f-a5e3-6ecd964c341c)
  
* [DartNode](https://dartnode.com)




## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FFlechazoPh%2FQLDependency.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FFlechazoPh%2FQLDependency?ref=badge_large)
