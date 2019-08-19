## 请求说明

以下所有接口请求域名为 `v1.itooi.cn`,为了降低使用门槛，所有请求为`GET`请求,你也可以试用其他请求方式

注意: 请求头中 `Content-type` 为 `application/x-www-form-urlencoded`

请求地址 = 域名 + 接口地址 + 参数

域名：`https://v1.itooi.cn`

接口地址：`https://v1.itooi.cn/netease/song`

参数：`id=37239038`

示例： `https://v1.itooi.cn/netease/song?id=37239038`

## 通用参数

### 地址重定向(isRedirect)

参数名称：isRedirect

参数说明：是否重定向到获取的 http 地址，目前所有音乐接口中获取歌曲播放地址、图片地址、Mv 播放地址均可使用该参数，具体以每个接口的说明为准

参数值说明：

-   0 :不进行 302 重定向跳转
-   1 :进行 302 重定向跳转

### 格式化(format)

参数名称：format

参数说明：格式化返回的 JSON 数据

参数值说明：

-   0 :不格式化,默认为该值
-   1 :进行格式化地址

## 支持平台

-   网易云音乐 http://music.163.com
-   QQ 音乐 http://y.qq.com
-   酷狗音乐 http://www.kugou.com
-   酷我音乐 http://www.kuwo.cn
-   咪咕音乐 http://www.migu.cn
-   百度音乐 http://music.taihe.com/

> 音乐平台音质： 未注明则为官方不支持或未找到该音质资源,`免费版不支持无损音乐`,如果使用`无损音质`版本请加群了解

| 支持平台 | 普通(48) | 普通(64) | 标准(96) | 标准（128） | 较高（192） | 极高（320） | 无损（ape） | 无损（flac） | Hi-Res(flac) | DSD(dff) |
| -------- | -------- | -------- | -------- | ----------- | ----------- | ----------- | ----------- | ------------ | ------------ | -------- |
| 网易     |          |          |          | mp3         | mp3         | mp3         |             | flac         |              |          |
| Q Q      | m4a      |          | m4a      | mp3         | m4a         | mp3         | ape         | flac         |              |          |
| 酷狗     |          |          |          | mp3         |             | mp3         |             | flac         | flac         | dff      |
| 酷我     | aac      |          |          | mp3         | mp3         | mp3         | mp3         | flac         |              |          |
| 咪咕     |          | mp3      |          | mp3         |             | mp3         |             | flac         |              |          |
| 百度     | aac(64)  |          |          | mp3         |             | mp3         |             |              |              |          |
