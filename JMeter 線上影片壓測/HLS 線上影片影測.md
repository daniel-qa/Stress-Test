# 1、安裝 BlazeMeter – HLS Plugin 

JMeter 插件管理器搜索 **BlazeMeter – HLS Plugin** 進行下載，完成安裝後重啟jMeter

# 2、添加取樣器 bzm – Streaming Sampler

# 3、填寫bzm – Streaming Sampler取樣器內容

![image](https://github.com/daniel-qa/Stress-Test/blob/master/JMeter%20%E7%B7%9A%E4%B8%8A%E5%BD%B1%E7%89%87%E5%A3%93%E6%B8%AC/JMeter_bzm_request.png)

# 一、HLS是什么
**HTTP Live Streaming（缩写是HLS)**
```
是一个由苹果公司提出的基于HTTP的流媒体网络传输协议。​是苹果公司QuickTime X和iPhone软件系统的一部分。 
它的工作原理是把整个流分成一个个小的基于HTTP的文件来下载，每次只下载一些。当媒体流正在播放时，
客户端可以选择从许多不同的备用源中以不同的速率下载同样的资源，允许流媒体会话适应不同的数据速率。

在开始一个流媒体会话时，客户端会下载一个包含元数据的extended M3U (m3u8)playlist文件，用于寻找可用的媒体流。
HLS只请求基本的HTTP报文，与实时传输协议（RTP)不同，HLS可以穿过任何允许HTTP数据通过的防火墙或者代理服务器。​
它也很容易使用内容分发网络来传输媒体流。

RTMP指Adobe的RTMP(Realtime Message Protocol)，广泛应用于低延时直播，也是编码器和服务器对接的实际标准协议，
在PC（Flash）上有最佳观看体验和最佳稳定性。

HLS指Apple的HLS(Http Live Streaming)，本身就是Live（直播）的，不过Vod（点播）也能支持。
HLS是Apple平台的标准流媒体协议，和RTMP在PC上一样支持得天衣无缝。
————————————————
版权声明：本文为CSDN博主「郎涯技术」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/aoshilang2249/article/details/82012187

```


**HTTP 狀態代碼 206**

表示由於客戶端發送的範圍標頭，服務器僅交付客戶端請求的部分資源。


