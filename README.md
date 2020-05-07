# BiliBili SuperChat WebAPI Document

是醒目留言的接口文档！

Prefix: `https://api.live.bilibili.com`

全部的`读取`接口使用 GET，`操作`接口使用 POST

## [/av/v1/SuperChat/getMessageList](https://api.live.bilibili.com/av/v1/SuperChat/getMessageList?room_id=14917277)

### Query

```json
{
  "room_id": 14917277
}
```

### Payload

```json
{
  "code": 0,
  "msg": "success",
  "message": "success",
  "data": {
    "list": [
      {
        "id": 544,
        "uid": 15045766,
        "background_image": "https://i0.hdslb.com/bfs/live/1aee2d5e9e8f03eed462a7b4bbfd0a7128bbc8b1.png",
        "background_color": "#F2FFFE",
        "background_icon": "",
        "background_bottom_color": "#427D9E",
        "background_price_color": "#7DA4BD",
        "font_color": "",
        "price": 50,
        "rate": 1000,
        "time": 104,
        "start_time": 1569249915,
        "end_time": 1569250035,
        "message": "翻出了2年不用的安卓，阿夸收下我的第一次",
        "message_jpn": "",
        "ts": 1569249931,
        "token": "A535A19F",
        "user_info": {
          "uname": "阿夸的召唤兽",
          "face": "https://i2.hdslb.com/bfs/face/5739fb353f4b631ccdd358e92de94fbf11bae34a.jpg",
          "face_frame": "",
          "guard_level": 0,
          "user_level": 23,
          "is_vip": 0,
          "is_svip": 0,
          "is_main_vip": 1
        }
      },
      {
        "id": 537,
        "uid": 7337516,
        "background_image": "https://i0.hdslb.com/bfs/live/1aee2d5e9e8f03eed462a7b4bbfd0a7128bbc8b1.png",
        "background_color": "#FFF4FB",
        "background_icon": "",
        "background_bottom_color": "#86105D",
        "background_price_color": "#AD5990",
        "font_color": "",
        "price": 100,
        "rate": 1000,
        "time": 28,
        "start_time": 1569249659,
        "end_time": 1569249959,
        "message": "夸夸傻夸，容我吃个桃子",
        "message_jpn": "大袈裟に自慢して、桃を食べさせてください。",
        "ts": 1569249931,
        "token": "F10A5EAE",
        "user_info": {
          "uname": "Hi-ero",
          "face": "https://i2.hdslb.com/bfs/face/104af82fd971dbc4e0e029f5eee4416b630faa42.jpg",
          "face_frame": "",
          "guard_level": 0,
          "user_level": 12,
          "is_vip": 0,
          "is_svip": 0,
          "is_main_vip": 1
        }
      }
    ]
  }
}
```

## [/av/v1/SuperChat/forMsgReason](https://api.live.bilibili.com/av/v1/SuperChat/forMsgReason)

### Payload

```json
{
  "code": 0,
  "msg": "ok",
  "message": "ok",
  "data": {
    "list": [
      { "id": 1, "reason": "违法违规", "reason_jpn": "法律に違反する" },
      { "id": 2, "reason": "低俗色情", "reason_jpn": "低俗な色情" },
      { "id": 3, "reason": "垃圾广告", "reason_jpn": "ごみの広告" },
      {
        "id": 4,
        "reason": "辱骂引战",
        "reason_jpn": "口汚くののしって戦を引きつける"
      },
      { "id": 5, "reason": "政治敏感", "reason_jpn": "政治が敏感である" },
      { "id": 6, "reason": "青少年不良信息", "reason_jpn": "青少年の不良情報" }
    ]
  }
}
```

## [/av/v1/SuperChat/getMessage](https://api.live.bilibili.com/av/v1/SuperChat/getMessage?order_id=1)

### Query

```json
{ "order_id": 1 }
```

### Payload

```json
{ "code": 404, "msg": "消息不存在", "message": "消息不存在", "data": [] }
```

## [/av/v1/SuperChat/messageInfo](https://api.live.bilibili.com/av/v1/SuperChat/messageInfo?id=16)

### Query

```json
{
  "id": "16"
}
```

### Payload

```json
{
  "code": 0,
  "msg": "",
  "message": "",
  "data": {
    "id": "16",
    "uid": "29608",
    "background_image": "https://i0.hdslb.com/bfs/live/1aee2d5e9e8f03eed462a7b4bbfd0a7128bbc8b1.png",
    "background_color": "#EDF5FF",
    "background_icon": "",
    "background_bottom_color": "#2A60B2",
    "background_price_color": "#7497CD",
    "font_color": "",
    "price": 30,
    "rate": 1000,
    "time": -50531,
    "start_time": 1569234681,
    "end_time": 1569234741,
    "message": "熊猫能吃辣吗？",
    "message_jpn": "パンダは辛いものが食べられますか？",
    "ts": 1569285272,
    "token": "73AFB519",
    "user_info": {
      "uname": "噶呜",
      "face": "https://i0.hdslb.com/bfs/face/4a3b67227dd1da6b8a0d7ba7c84d434c27067e69.jpg",
      "face_frame": "",
      "guard_level": 0,
      "user_level": 29,
      "level_color": "#5896de",
      "is_vip": 1,
      "is_svip": 1,
      "is_main_vip": 1,
      "title": "title-225-1",
      "manager": 0
    },
    "medal_info": {
      "target_id": 332704117,
      "medal_level": 15,
      "medal_name": "喵喵狐",
      "medal_color": "#ff86b2"
    }
  }
}
```

## [/av/v1/SuperChat/remove](https://api.live.bilibili.com/av/v1/SuperChat/remove?id=1)

### Query

```json
{ "id": 1 }
```

### Payload

```json
{
  "code": 4,
  "msg": "您没有权限",
  "message": "您没有权限",
  "data": { "status": 0 }
}
```

## /av/v1/SuperChat/report

### Query

```json
{ "id": 1, "room_id": 1, "reason": "", "ts": 1 }
```

## /av/v1/SuperChat/config

### Query

```json
{ "room_id": 916226, "ruid": 2304086, "parent_area_id": 1, "area_id": 1 }
```

### Payload

```json
{
    "code": 0,
    "msg": "success",
    "message": "success",
    "data": {
        "title": "发送醒目留言",
        "rate": 1000,
        "placeholder": "通过醒目留言传递自己的心意吧！",
        "introduce_url": "",
        "button_text": "购买并发送",
        "trans_status": 1,
        "ranked_mark": 0,
        "rank_version_sign": "",
        "gift_id": 12000,
        "gift_name": "醒目留言",
        "user_info": {
            "uname": "RootChannel",
            "face": "http://i2.hdslb.com/bfs/face/c14360f12cf183287d8c0562ced414dddec39b87.png",
            "face_frame": "",
            "guard_level": 0,
            "user_level": 30,
            "is_vip": 0,
            "is_svip": 0,
            "is_main_vip": 1,
            "title": "title-221-1",
            "manager": 0
        },
        "medal_info": {
            "target_id": 32890488,
            "medal_level": 10,
            "medal_name": "白帽子",
            "medal_color": "#a068f1"
        },
        "price_configs": [
            {
                "id": 8,
                "level": 1,
                "price": 30,
                "second": "60",
                "limit": 40,
                "background_image": "http://i0.hdslb.com/bfs/live/1aee2d5e9e8f03eed462a7b4bbfd0a7128bbc8b1.png",
                "background_color": "#EDF5FF",
                "background_icon": "",
                "background_bottom_color": "#2A60B2",
                "background_price_color": "#7497CD",
                "font_color": ""
            },
            {
                "id": 2,
                "level": 2,
                "price": 50,
                "second": 120,
                "limit": 50,
                "background_image": "https://i0.hdslb.com/bfs/live/1aee2d5e9e8f03eed462a7b4bbfd0a7128bbc8b1.png",
                "background_color": "#DBFFFD",
                "background_icon": "",
                "background_bottom_color": "#427D9E",
                "background_price_color": "#7DA4BD",
                "font_color": ""
            },
            {
                "id": 3,
                "level": 3,
                "price": 100,
                "second": 300,
                "limit": 60,
                "background_image": "https://i0.hdslb.com/bfs/live/1aee2d5e9e8f03eed462a7b4bbfd0a7128bbc8b1.png",
                "background_color": "#FFF1C5",
                "background_icon": "",
                "background_bottom_color": "#E2B52B",
                "background_price_color": "#ECCF75",
                "font_color": ""
            },
            {
                "id": 4,
                "level": 4,
                "price": 500,
                "second": 1800,
                "limit": 80,
                "background_image": "https://i0.hdslb.com/bfs/live/1aee2d5e9e8f03eed462a7b4bbfd0a7128bbc8b1.png",
                "background_color": "#FFEAD2",
                "background_icon": "https://i0.hdslb.com/bfs/live/e12e931ed8d9e5189ab6d1a3a1da35af4f8a55af.png",
                "background_bottom_color": "#E09443",
                "background_price_color": "#E8AF79",
                "font_color": ""
            },
            {
                "id": 5,
                "level": 5,
                "price": 1000,
                "second": 3600,
                "limit": 90,
                "background_image": "https://i0.hdslb.com/bfs/live/1aee2d5e9e8f03eed462a7b4bbfd0a7128bbc8b1.png",
                "background_color": "#FFE7E4",
                "background_icon": "https://i0.hdslb.com/bfs/live/0cf7b5fdc7084c9ae05f7a371ea2438118529d66.png",
                "background_bottom_color": "#E54D4D",
                "background_price_color": "#EE8B8B",
                "font_color": ""
            },
            {
                "id": 6,
                "level": 6,
                "price": 2000,
                "second": 7200,
                "limit": 100,
                "background_image": "https://i0.hdslb.com/bfs/live/1aee2d5e9e8f03eed462a7b4bbfd0a7128bbc8b1.png",
                "background_color": "#FFD8D8",
                "background_icon": "https://i0.hdslb.com/bfs/live/0d9cbbdbad7d3371266cd5b568065415415316ae.png",
                "background_bottom_color": "#AB1A32",
                "background_price_color": "#C86A7A",
                "font_color": ""
            }
        ]
    }
}
```

## [/av/v1/SuperChat/ownMessageList](https://api.live.bilibili.com/av/v1/SuperChat/ownMessageList?room_id=14917277)

### Query

```json
{ "room_id": 14917277 }
```

### Payload

```json
{ "code": 0, "msg": "success", "message": "success", "data": { "list": [] } }
```

## [/userext/v1/Conf/getExchangeRate](https://api.live.bilibili.com/userext/v1/Conf/getExchangeRate)

### Payload

```json
{ "code": 0, "msg": "", "message": "", "data": { "exchange_rate": 14.7 } }
```
