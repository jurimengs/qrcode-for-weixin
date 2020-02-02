# qrcode-for-weixin
generate an qrcode picture with custom text, so that it can be recognized by long tap in wechat directly, and also can be save or transmit directly.

"qrcode-for-weixin.html" is a demo for acting how to use it,
Introduce:
At the year before last last year, there was a H5 page include a qrcode picture would be open in wechat , which must be save or transmit directly by long tap , and the picture must be wrote by some custom words, so I need to generate an qrcode pic with certain words before page was loaded. and I did it by javascript instead of doing it in server.


生成一个带自定义文本的二维码图片，当我们在微信中打开该页面时，可以直接长按识别二维码，且可以直接带文字保存转发

qrcode-for-weixin.html 用于演示生成带文字的二维码图片，

背景介绍 ：前前年写项目有个功能：
微信中打开 h5  页面后展示某链接的二维码，同时根据业务内容的不同，需要在二维码下方展示不同的文字，
麻烦在于需要在当前打开的页面， 直接长按就要能识别二维码并且要求可以保存，转发。
意味着，打开这个页面的时候，这个二维码必需是一张，带自定义内容的图片。
实现思路有两种：
后端实现
前端实现（所以就有了本案）

技术实现：
基于 jquery 和 jquery-qrcode-0.14.0 来生成二维码，
为了方便功能实现，对jquery-qrcode源码做了些微的改动(参见 fillIndividuationContent 函数)，为了与源码区分，更名为jquery-qrcode-custom.js, 为了表示对 jquery-qrcode 的尊重, 代码包里也包含了 jquery-qrcode.js 

交流邮箱： jurimengs@163.com, 微信交流号 jurimengs


jquery-qrcode 链接： https://github.com/lrsjng/jquery-qrcode
