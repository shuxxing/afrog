<h1 align="center">afrog</h1>
<p align="center">一款性能卓越、快速稳定、PoC 可定制化的漏洞扫描工具<br/>❤️不以物喜，不以己悲<br/>共 <b>[500]</b> 个<br/>🐸喜欢请点赞🌟⭐，不迷路</p>

<p align="center" dir="auto">
  <a href="https://github.com/zan8in/afrog/tree/main/pocs/afrog-pocs">PoC 仓库</a> •
  <a href="https://github.com/zan8in/afrog/blob/main/README_en.md">English Doc</a>
</p>


# 什么是 afrog

afrog 是一款性能卓越、快速稳定、PoC 可定制的漏洞扫描工具，PoC 包含 CVE、CNVD、默认口令、信息泄露、指纹识别、未授权访问、任意文件读取、命令执行等多种漏洞类型，帮助网络安全从业者快速验证并及时修复漏洞。

# 特点

* [x] 基于 xray 内核，又不像 xray（[**afrog 模板语法**](https://github.com/zan8in/afrog/blob/main/pocs/afrog-pocs/README.md)）
* [x] 性能卓越，快速稳定
* [x] 实时显示，扫描进度
* [x] 输出 html 报告，方便查看 `request` 和 `response`
* [x] 启动程序，自动更新本地 PoC 库
* [x] 长期维护、更新 PoC（[**afrog-pocs**](https://github.com/zan8in/afrog/tree/main/pocs/afrog-pocs)）
* [x] 二次开发，参考 `cmd/afrog/main.go` 或加入 **[交流群](https://github.com/zan8in/afrog#%E4%BA%A4%E6%B5%81%E7%BE%A4)**

# 下载

### [下载地址](https://github.com/zan8in/afrog/releases)

# 使用指南

### [查看指南](https://github.com/zan8in/afrog/blob/main/GUIDE.md)

# 例子

扫描单个目标
```
afrog -t http://127.0.0.1 -o result.html
```
![](https://github.com/zan8in/afrog/blob/main/images/onescan.png)

扫描多个目标

```
afrog -T urls.txt -o result.html
```
例如：`urls.txt`
```
http://192.168.139.129:8080
http://127.0.0.1
```
![](https://github.com/zan8in/afrog/blob/main/images/twoscan.png)

测试单个 PoC 文件

```
afrog -t http://127.0.0.1 -P ./testing/poc-test.yaml -o result.html
```
![](https://github.com/zan8in/afrog/blob/main/images/threescan.png)

测试多个 PoC 文件

```
afrog -t http://127.0.0.1 -P ./testing/ -o result.html
```
![](https://github.com/zan8in/afrog/blob/main/images/fourscan.png)

输出 html 报告

![](https://github.com/zan8in/afrog/blob/main/images/2.png)

![](https://github.com/zan8in/afrog/blob/main/images/3.png)

# 如何贡献 PoC？

### [查看教程](https://github.com/zan8in/afrog/blob/main/CONTRIBUTION.md)

# 免责声明

本工具仅面向**合法授权**的企业安全建设行为，如您需要测试本工具的可用性，请自行搭建靶机环境。

为避免被恶意使用，本项目所有收录的poc均为漏洞的理论判断，不存在漏洞利用过程，不会对目标发起真实攻击和漏洞利用。

在使用本工具进行检测时，您应确保该行为符合当地的法律法规，并且已经取得了足够的授权。**请勿对非授权目标进行扫描。**

如您在使用本工具的过程中存在任何非法行为，您需自行承担相应后果，我们将不承担任何法律及连带责任。

在安装并使用本工具前，请您**务必审慎阅读、充分理解各条款内容**，限制、免责条款或者其他涉及您重大权益的条款可能会以加粗、加下划线等形式提示您重点注意。 除非您已充分阅读、完全理解并接受本协议所有条款，否则，请您不要安装并使用本工具。您的使用行为或者您以其他任何明示或者默示方式表示接受本协议的，即视为您已阅读并同意本协议的约束。

# 交流群

<img src="https://github.com/zan8in/afrog/blob/main/images/afrog.jpg" width="33%" />
