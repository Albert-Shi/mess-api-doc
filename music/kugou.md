# 酷狗音乐

## 获取音乐详情

接口地址: `https://v1.itooi.cn/kugou/song`

请求示例: `https://v1.itooi.cn/kugou/song?id=xxxx`

| 参数说明 | 是否必须 | 说明                           | 默认值 |
| -------- | -------- | ------------------------------ | ------ |
| id       | √        | 音乐 ID                        | 无     |
| format   | x        | 格式化数据 1 格式化 0 不格式化 | 0      |

## 获取音乐播放地址

接口地址: `https://v1.itooi.cn/kugou/url`

请求示例: `https://v1.itooi.cn/kugou/url?id=xxxx&quality=128`

| 参数说明   | 是否必须 | 说明          | 默认值                     |
| ---------- | -------- | ------------- | -------------------------- |
| id         | √        | 音乐 ID       | 无                         |
| quality    | x        | 音质          |                            |
| isRedirect | ×        | 是否 302 跳转 | 1 跳转 0 不跳转 默认为跳转 |

说明: 码率类型：128 320 flac hr dsd

## 获取音乐歌词

接口地址: `https://v1.itooi.cn/kugou/lrc`

请求示例: `https://v1.itooi.cn/kugou/lrc?id=xxxx`

| 参数说明 | 是否必须 | 说明    | 默认值           |
| -------- | -------- | ------- | ---------------- |
| id       | √        | 音乐 ID | 默认获取翻译歌词 |

## 获取音乐图片

接口地址: `https://v1.itooi.cn/kugou/pic`

请求示例: `https://v1.itooi.cn/kugou/pic?id=xxxx`

| 参数说明   | 是否必须 | 说明          | 默认值                     |
| ---------- | -------- | ------------- | -------------------------- |
| id         | √        | 音乐 ID       |                            |
| isRedirect | ×        | 是否 302 跳转 | 1 跳转 0 不跳转 默认为跳转 |

## 获取专辑详情

接口地址: `https://v1.itooi.cn/kugou/album`

请求示例: `https://v1.itooi.cn/kugou/album?id=xxxx`

| 参数说明 | 是否必须 | 说明                           | 默认值 |
| -------- | -------- | ------------------------------ | ------ |
| id       | √        | 专辑 ID                        | 无     |
| format   | x        | 格式化数据 1 格式化 0 不格式化 | 0      |

## 音乐歌单

说明：获取歌单中的所有音乐

接口地址: `https://v1.itooi.cn/kugou/songList`

请求示例: `https://v1.itooi.cn/kugou/songList?id=xxxx&pageSize=100&page=0`

| 参数说明 | 是否必须 | 说明                           | 默认值 |
| -------- | -------- | ------------------------------ | ------ |
| id       | √        | 歌单的 ID                      | 无     |
| format   | x        | 格式化数据 1 格式化 0 不格式化 | 0      |

## 搜索

说明：搜索关键词可以搜索 音乐 / 歌手 / 专辑 / 歌单 / 视频 / 电台 / 用户 / 歌词

当前支持类型 `song singer album songList video radio user lrc`

接口地址: `https://v1.itooi.cn/kugou/search`

请求示例: `https://v1.itooi.cn/kugou/search?keyword=xxxx&type=song&pageSize=100&page=0`

| 参数说明 | 是否必须 | 说明                           | 默认值         |
| -------- | -------- | ------------------------------ | -------------- |
| keyword  | √        | 搜索关键词                     | 详细见下面说明 |
| type     | √        | 搜索类型                       | 默认为 song    |
| pageSize | ×        | 请求数量                       | 默认为 30      |
| page     | ×        | 分页                           | 默认第 0 页    |
| format   | x        | 格式化数据 1 格式化 0 不格式化 | 0              |

## 获取 MV 信息

接口地址: `https://v1.itooi.cn/kugou/mv`

请求示例: `https://v1.itooi.cn/kugou/mv?id=xxxxx`

| 参数说明 | 是否必须 | 说明  | 默认值 |
| -------- | -------- | ----- | ------ |
| id       | √        | MV ID |        |

## 获取 MV 播放地址

接口地址: `https://v1.itooi.cn/kugou/mvUrl`

请求示例: `https://v1.itooi.cn/kugou/mvUrl?id=xxxx&quality=1080`

| 参数说明   | 是否必须 | 说明          | 默认值                     |
| ---------- | -------- | ------------- | -------------------------- |
| id         | √        | MVID          |                            |
| quality    | ×        | 视频格式      | 默认 480                   |
| isRedirect | ×        | 是否 302 跳转 | 1 跳转 0 不跳转 默认为跳转 |

说明: 视频大小类型：1080 720 480 240
