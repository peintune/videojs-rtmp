## videojs 播放 rtmp 实时视频流相关组件和Demo

测试结果： 
- 用video-js-0.2-0.1.swf 延迟 < 0.1s, 但丢帧概率变大，画面卡顿
- 用video-js-2-6.swf 延迟 ~ 2s, 但丢帧概率变小，画面流畅

```
说明： video-js-xx-xx.swf 中的 xx-xx 表示flash中的  bufferTime， bufferTimeMax
       即，flash中缓存的buffer相关设置，理论上，bufferTime越小，实时视频流延迟越小，但会出现丢帧和卡顿。
       此项目编译了不同bufferTime的swf插件，如果想自己编译，
       可以下载源码： https://github.com/peintune/video-js-swf 修改 Defaults.as 文件
```

- video.js 使用版本：7.7.6
- video-js.css 使用版本：7.7.6
- videojs-flash.js 使用版本：7.7.6