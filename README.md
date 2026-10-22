# App 下载页

直接用浏览器打开 `index.html` 即可预览，部署时把整个 `AppDownloadPage` 目录上传到静态服务器。

## 修改下载链接

打开 `index.html`，搜索以下注释即可定位：

- `iOS 下载地址`：修改 `id="iosDownload"` 的 `href`
- `Android 下载地址`：修改 `id="androidDownload"` 的 `href`

当前配置：

- iOS：`https://www.betaqr.com.cn/udid`
- Android：`https://fir.xcxwo.com/9lqecgy8`

## iOS UUID 弹窗

iOS 按钮默认会先弹出 UUID 说明，点击「确认并获取 UUID」后跳转到 `href` 配置的地址。

如果以后 iOS 改成可以直接下载的页面，不需要再提示 UUID，只需把 iOS 链接上的：

```html
data-uuid-notice="true"
```

改成：

```html
data-uuid-notice="false"
```

## 图标

`app-icon.jpg` 是 App 图标，替换时保持文件名不变即可。
