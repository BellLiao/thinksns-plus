# Music消息对照表

在程序中，所有请求接口都是使用了状态码约定不同的错误状态，下面将列出所有的状态码，以便调用接口过程中随时查询。

## 代码规则

代码采用的是 Module + Function block + Code number 方式排列总长度占4位，不足0不齐，如下：
- module 占1位，因为属于四位长度首位，加上考虑int类型规则，范围是1-9，服务器总体模块，目前不会超过9个大模块。
- function 占1位，范围0-9十个模块，分属于大模块下的小功能块，一个大功能块，划分不超过10个小功能块。
- code number，2位，这个代码范围定义为模糊定位，范围00-99，总状态数量为100个，一个功能块下状态很难超过100个状态。

## 模块列表

* 8*** - [音乐模块](#音乐模块)

### 音乐模块
| code  | message  |
|-------|:--------|
| 8001  | 专辑不存在或已删除 |
| 8002  | 歌曲不存在或已删除 |
| 8003  | 已赞过该歌曲 |
| 8004  | 未对歌曲点赞 |



