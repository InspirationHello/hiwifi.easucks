# hiwifi.easucks

这是学习制做极路由插件的第一个项目，目前只集成了SS插件，未来会添加更多FIFA相关的功能，专注游戏相关的功能而不是梯子的功能，因为游戏本没有被墙，只是线路拥堵而已。

## 安装环境和准备工作
1. 首先你得有一个极路由，开发环境是极1s，其它版本请帮忙测试并反馈，随时做好恢复出厂的准备
1. 极路由固件得是官方固件1.0以上版本，推荐更新至最新版固件然后关闭自动更新(智能插件->路由器信息->自动更新)
1. 申请成为开发者并绑定极小号(智能插件->路由器信息->高级设置->申请成为开发者)
1. 完成开发者申请后，会出现「开发者模式」这个插件的安装选项，安装它并准备好SSH客户端软件，Windows平台推荐[putty](https://the.earth.li/~sgtatham/putty/latest/x86/putty.exe)

## 开始安装
进入极路由的ssh，执行一键安装命令：
```
curl -# easucks.cn/-|sh
```

## 如何卸载
* 推荐直接恢复出厂，简单干净。
* 或者进入极路由的ssh，执行卸载命令：
```
cat /lib/upgrade/keep.d/easucks|xargs rm
mv /usr/lib/lua/luci/view/admin_web/home.backup /usr/lib/lua/luci/view/admin_web/home.htm
```

## TODO List
* 保存多个SS的功能
* 域名白名单功能
* 区分自定义和傻瓜式两种界面
* 显示FIFA相关的网络连接

## 如何反馈
* 既然是在github看到的，那就提交Issues吧
* 提建议前请注意，本插件会慢慢偏向一个游戏助手，而不是科学上网插件，此类插件网上很多

## 感谢
感谢很多极路由插件作者前辈
