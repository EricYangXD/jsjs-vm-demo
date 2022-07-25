# jsjs-vm-demo
小程序绕过微信js解释器封锁，实现热更新

原文地址：https://zhuanlan.zhihu.com/p/539725089

2022年6月23号的时候，微信团队发了如下通知将禁止小程序使用 JavaScript 解释来动态更新代码。

为进一步提升小程序的安全性和用户体验，目前平台对提审的小程序均需进行安全检测，在检测过程中，发现有小程序采用内置 JavaScript 解释器（如eval5、estime、evil-eval等）的方式，动态执行JS代码、对小程序wxml代码进行热更新。对于使用解释器的小程序，平台将自「2022年7月6日」开始在代码审核环节进行「驳回」，请各位开发者于「7月6日」前完成自查、修复。

—— 摘自 「关于禁止小程序JavaScript解释器使用规范要求 | 微信开放社区」

https://developers.weixin.qq.com/community/minihome/doc/0000ae500e4fd0541f2ea33755b801
