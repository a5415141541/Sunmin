# Sunmin

#iOS开发
#第一站,发布的就是M3U8加密视频的开发和步骤     
#之后会慢慢上传播放M3U8加密,解密，创建key，创建.M3U8文件等代码
1:本地服务器就是从网上下载HTTPServer文件包(本地服务器是指用第三方代码开启本地服务器)

2:问题

   1:为什么要开启本地服务器进行播放视频

   2:M3U8视频到底是什么格式的URL

   3:M3U8如何进行解析播放

   4:M3U8如何进行加密和解密

在线播放     

把后台给你返回的那么字符串放到文本里面生成.m3u8文件(格式应该懂吧@网上一大推)
key的地址(这个就是密钥)  16字节，自己生成这个文件就ok
http://localhost:12345/segmen/segmen.m3u8   这个就是本地服务器的地址/后面是segmen文件，在后面就是M3U8的文件

使用本地服务器播放M3U8就是把M3U8文件移动到本地服务器或者是把当前生成在本地的M3U8文件地址设置成本地服务器地址就OK了

然后播放上面的地址就可以进行播放视频了,直播推流一个道理

加密和解密    推荐几种 AES加密 AES解密（128的）

 这个需要咱们app端和后台进行商量来，如何进行M3U8这么多字符串的加密和解密的,Key是放到哪里的,怎么样取到key生成文件，取到M3U8生成.m3u8文件，这样就一目了然

说白了,就是字符串的截取在截取.生成文件,放到本地服务器进行播放。
