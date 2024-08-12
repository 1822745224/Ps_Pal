# PsPal
## 初衷

解决“被打赏人”在收到打赏后无法立刻回应或者回馈“打赏人”问题，同时分享一个除使用主流数据库的数据处理方案。

> 当前支持：微信打赏
> 
> MadDogQQ交流群：591668872

## 前言

  + 哥哥姐姐们，项目是全开源的，连各个模块都全部开源，该项目仅供学习和个人使用，重点是不可以用于商用更不能非法使用！！！感谢！！！

## 打赏端：

> 技术思路(使用Web方式展示接收打赏的信息，由HTML和原生JS以及EMQ的MQTT库实现！)：
> 
1、index.html 为展示创建打赏的过程，由变量（打赏唯一识别号、打赏数额、同步地址、异步地址、通信秘钥）生成打赏内容信息，并通过sha256使用通信秘钥生成唯一签名，避免恶意提交。

2、PsPal.html 通过得到的内容生成打赏内容信息并通过WebSocket协议对MQTT协议服务器发送打赏数据，由服务端验证并在对应的Topic返回识别信息和打赏成功信息。




GitHub 演示：https://maddog888.github.io/ps_pal/  


