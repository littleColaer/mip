# mip-video（ToDo）

mip-video 用来支持在 mip 中增加视频内容。

该视频组件支持在文本中插入一个视频，插入的视频不先定大小与尺寸，自动生成按照屏幕尺寸缩放的缩略图，点击多略图可以播放视频。

描述|替换html5的video标签; 只用于能直接用HTML5播放的视频文件.
----|----
可用性|开发中
支持布局| 响应式
示例|官网上线后增加示例

## 1. 使用

mip-video 根据标签的src在组件的runtime中进行懒加载，能够像html5的video标签一样控制

```
<mip-video 
    width=400 
    height=300 
    src="https://yourhost.com/yourvideo.mp4"
    poster="yourvideo.jpg">
    <div fallback>
        <p>你的浏览器不支持html5 video</p>
    </div>
  <source type="video/mp4" src="foo.mp4">
  <source type="video/webm" src="foo.webm">
</mip-video>
```

## 2. 属性

视频组件所涉及的属性有：视频地址（src），封面图地址（poster），自动播放开关（autoplay），菜单开关（controls），循环播放开关（loop）以及（muted）

- **视频地址（src）**

    - 是否必填：是

    - 说明：视频源地址，必须是https资源

- **封面图地址（poster）**

    - 是否必填：是

    - 说明：视频播放前默认展示图片

- **自动播放开关（autoplay）**

    - 是否必填：否

    - 说明：默认？ //待完善 需要说明几种选择的值是什么

- **菜单开关（controls）**

    - 是否必填：否

    - 说明：默认？ //待完善 需要说明几种选择的值是什么


- **循环播放开关（loop）**

    - 是否必填：否

    - 说明：默认？ //待完善 需要说明几种选择的值是什么

- **muted**

    - 是否必填：否

    - 说明：默认？ //待完善 需要说明几种选择的值是什么

## 3. 验证

暂不支持

