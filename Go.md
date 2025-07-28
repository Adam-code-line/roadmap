# Go 后端学习路线
> Tips：环境安装可以自行搜索
## Go 语法
### 文档
1. [Go by Example](https://gobyexample-cn.github.io/)
    <br/> 通过例子了解Golang的语法，适合快速上手。
    <br/> 最基础的看到`错误处理`一节即可，但是到这只是能满足你将Golang作为一门普通的语言去使用。
    <br/> 想要进阶可以把后面有关`channel`的部分一并看完
    <br/>余下的内容可选，有需要时再看也不迟

### 视频教程
1. [8小时转职Golang工程师](https://www.bilibili.com/video/BV1gf4y1r79E/?vd_source=2d780bafbc8783777d10d823f1cb5010)
   <br/>说是8小时，但实际上Go的语法还是比较简单的，可能花不到一半时间就能学会
   <br/>这个教程后面还有一个小项目，可以看看

### 练手项目
1. [gin-vue-admin](https://github.com/flipped-aurora/gin-vue-admin)
   <br/>一个比较完整，涵盖了各种实际开发中所需要的功能的项目。比较完整但难度不会很大，可以作为刚开始
   <br/>做项目的起步。
   > 由[lyydsheep](https://github.com/lyydsheep)学长提供
2. [定时微服务](https://github.com/lyydsheep/micro-tt)
   <br/>其中的 tick-tock 微服务是复现 github 上的一个开源项目，涵盖了本人阅读原项目时做的各种图，建议结合原项目阅读学习。
3. [go-chat](https://github.com/LockGit/gochat)
   <br/> 使用纯go实现的轻量级im系统。项目的 readme 很详细，便于快速上手 Go 项目。

--- 

## MySQL
TODO 补充完善

（需要涉及相应的框架）

---

## Redis
### 教程

1. [Redis 官方文档](https://redis.io/docs/latest/develop/) - Redis的官方文档写的非常好，根据官方文档学习基本用法完全没有问题

2. [Redis 学习之旅](https://dinglz.cn/tags/redis/) - [dinglz](https://github.com/dingdinglz)的Redis学习记录，涵盖内容包括redis的使用，以及在go中如何使用redis（redis-go），每个教程中都有小例子帮你理解学习该Redis类型的意义是什么 

### 框架

1. [go-redis](https://github.com/redis/go-redis) - 建议搭配Redis学习之旅食用

### 视频教程

1. [Redis应用场景总结](https://www.bilibili.com/video/BV1x4MmzUEJt) - 真实项目中你该如何去使用redis，请完成redis的基础学习后再观看本视频

---

## Go Web
### 教程

1. [从0开始敲一个go web项目：教程](https://github.com/TIC-DLUT/2025_spring_backend) - 这是一个例会项目，是一个ai对话项目的后端，项目中有完整的包含语法、结构、数据库、ai调用的教程，完整地跟着该项目的readme敲完整个教程后，独立开发简单的go web项目不成问题

2. [7天用Go从零实现Web框架Gee教程](https://geektutu.com/post/gee.html) - 亲手设计框架后更能更好地使用其他框架，掌握原理，该教程适合想要深层次进阶的同学，该栏目下其他几个七天项目也十分推荐

### 框架推荐（深入学习其中一个即可，思路互通）

- [Gin框架](https://gin-gonic.com/zh-cn/docs/introduction/)
- [Fiber框架](https://docs.gofiber.io/)

---

## MQ
TODO 补充完善

---

## Docker、Kubernetes

- [Docker视频教程](https://www.bilibili.com/video/BV1gr4y1U7CY/?spm_id_from=333.337.search-card.all.click&vd_source=a15269894d9b8114cb5f9bb663d22be9)
- [Kubernetes视频教程(强烈推荐(✧∀✧))](https://www.bilibili.com/video/BV1GSu7zLE4F?spm_id_from=333.788.videopod.episodes&vd_source=a15269894d9b8114cb5f9bb663d22be9)
- [Kubernetes知识点](https://www.yuque.com/lyydsheep/kyeikv/cnxtgcz3edmxnemq?singleDoc#)
    - pdf格式，在线预览即可
- [Kubernetes-combat](https://github.com/crossoverJie/k8s-combat)

## 其他
- [Go八股文](https://golangstar.cn/go_series/introduction.html)
- [项目解读器](https://zread.ai/)