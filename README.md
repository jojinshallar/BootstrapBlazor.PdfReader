# Blazor Pdf Reader PDF阅读器 组件  

![image](https://user-images.githubusercontent.com/8428709/205808008-b3898c07-3f26-4f88-be5c-7836f8985174.png)

示例:

https://blazor.app1.es/pdfReaders

使用方法:

1.nuget包

```BootstrapBlazor.PdfReader```

2._Imports.razor 文件 或者页面添加 添加组件库引用

```@using BootstrapBlazor.Components```


3.razor页面
```
<PdfReader PdfFile="https://densen.es/test/webdev/pdf/sample.pdf" />
           
<PdfReader UrlBase="https://blazor.app1.es/"
           PdfFile="_content/DemoShared/sample.pdf" />

<PdfReader UrlBase="https://blazor.app1.es/"
           PdfFile="_content/DemoShared/sample.pdf" 
           EnableStreamingMode="true"/>

<pre>跨域最佳体验</pre>

<PdfReader UrlBase="https://blazor.app1.es/"
           PdfFile="_content/DemoShared/sample.pdf" 
           EnableStreamingMode="true"
           ForcePDFJS="true" />
```

4.参数说明

|  参数   | 说明  | 默认值  | 
|  ----  | ----  | ----  | 
| PdfStream  | 用于渲染的文件流,为空则用URL参数读取文件 |  | 
| PdfFile  | PDF文件路径, https://xx.com/sample.pdf | null | 
| Func<string, Task>? OnInfo | 信息回调 | |
| Func<string, Task>? OnError | 错误回调 |
| EnableStreamingMode  | 使用流化模式,可跨域读取文件 | false | 
| UrlBase  | PDF文件基础路径, (使用流化模式才需要设置),  https://xx.com |  | 
| Height  | 高 | 700 | 
| Page | 指定页码,如果浏览器支持，将加载PDF并自动滚动到第n页 | 1 |
| ForceIframe | 强制使用 Iframe | false |
| ForcePDFJS | 强制使用 PDF.js | false |
| PDFJS_URL | PDF.js 浏览器页面路径 | 内置 |
| Search | *查询字符串 | |
| View | *视图模式 | FitV |
| Pagemode | *页面模式 | thumbs |

*表示PDF.js 专有

**优先嵌入模式,不支持则回落倒pdf.js模式**

**跨域最佳体验:**  EnableStreamingMode=true , ForcePDFJS=true

---
#### Blazor 组件

[条码扫描 ZXingBlazor](https://www.nuget.org/packages/ZXingBlazor#readme-body-tab)
[![nuget](https://img.shields.io/nuget/v/ZXingBlazor.svg?style=flat-square)](https://www.nuget.org/packages/ZXingBlazor) 
[![stats](https://img.shields.io/nuget/dt/ZXingBlazor.svg?style=flat-square)](https://www.nuget.org/stats/packages/ZXingBlazor?groupby=Version)

[图片浏览器 Viewer](https://www.nuget.org/packages/BootstrapBlazor.Viewer#readme-body-tab)
  
[条码扫描 BarcodeScanner](Densen.Component.Blazor/BarcodeScanner.md)
   
[手写签名 Handwritten](Densen.Component.Blazor/Handwritten.md)

[手写签名 SignaturePad](https://www.nuget.org/packages/BootstrapBlazor.SignaturePad#readme-body-tab)

[定位/持续定位 Geolocation](https://www.nuget.org/packages/BootstrapBlazor.Geolocation#readme-body-tab)

[屏幕键盘 OnScreenKeyboard](https://www.nuget.org/packages/BootstrapBlazor.OnScreenKeyboard#readme-body-tab)

[百度地图 BaiduMap](https://www.nuget.org/packages/BootstrapBlazor.BaiduMap#readme-body-tab)

[谷歌地图 GoogleMap](https://www.nuget.org/packages/BootstrapBlazor.Maps#readme-body-tab)

[蓝牙和打印 Bluetooth](https://www.nuget.org/packages/BootstrapBlazor.Bluetooth#readme-body-tab)

[PDF阅读器 PdfReader](https://www.nuget.org/packages/BootstrapBlazor.PdfReader#readme-body-tab)

[文件系统访问 FileSystem](https://www.nuget.org/packages/BootstrapBlazor.FileSystem#readme-body-tab)

[光学字符识别 OCR](https://www.nuget.org/packages/BootstrapBlazor.OCR#readme-body-tab)

[电池信息/网络信息 WebAPI](https://www.nuget.org/packages/BootstrapBlazor.WebAPI#readme-body-tab)

#### AlexChow

[今日头条](https://www.toutiao.com/c/user/token/MS4wLjABAAAAGMBzlmgJx0rytwH08AEEY8F0wIVXB2soJXXdUP3ohAE/?) | [博客园](https://www.cnblogs.com/densen2014) | [知乎](https://www.zhihu.com/people/alex-chow-54) | [Gitee](https://gitee.com/densen2014) | [GitHub](https://github.com/densen2014)


![ChuanglinZhou](https://user-images.githubusercontent.com/8428709/205942253-8ff5f9ca-a033-4707-9c36-b8c9950e50d6.png)
