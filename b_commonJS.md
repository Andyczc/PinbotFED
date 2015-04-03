# Pinbot B端公共JS组件（基于jQuery）

>
以上样式定义皆为beta版本，后期会不断完善。
>
pb.common.js包含jquery-1.11.1.min.js与basic.js等，这里只讲basic.js部分；

## $.LayerOut
含义：弹出一个空白的层;
>
使用方法 $.LayerOut({config})

## $.alert
含义：弹出一个确认框（$.LayerOut再封装）;
>
使用方法 $.alert( html , onOk , title , setting )

## $.confirm
含义：弹出一个确认框（$.LayerOut再封装）;
>
使用方法 $.confirm( html , onOk , onCancel , title , setting )

## $.Click
含义：基于JQuery对html元素点击事件的再封装,实现了防止重复点击等功能;
>
使用方法 $.Click({ dom | before | callback })

## $.Ajax
含义：基于JQuery对ajax请求事件的再封装;
>
使用方法 $.Ajax({ url | form | callDom | method | data | failed | successed | verify | callback })

## $.commonAjax
含义：$.Click与$.Ajax组合封装，通过在html元素本身配置相关参数，实现了简单get与复杂post请求的功能;
>
使用方法 $.commonAjax()，函数体内this指向调用函数的html元素，参数都在调用函数的html元素身上配置；

## filterXss
含义：过滤xss代码;
>
使用方法 filterXss(str)；

## $.loadBgImg
含义：加载背景图片;
>
使用方法：$.loadBgImg({ attr | loadImg | imgList | callback })，可不带参数；

## $.lazyImg
含义：图片懒加载;
>
使用方法：$.lazyImg({ attr | loadType | count | scrollLimit | isLock | scrollTop | scrollBorder | callback })，可不带参数；

***
>
[Pinbot B端公共JS组件参数详解与实例](https://github.com/Andyczc/PinbotFED/blob/master/test/commonJS.html)
