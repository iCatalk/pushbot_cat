## Pushbot, a simple and stable push message api for telegram
### How to use it
1. Sign in [Pushbot.cat](https://pushbot.cat/) by you telegram account.
2. Automatic get PushKey and start push message by our API.

### API
#### Push text message
```
https://pushbot.cat/api/push/text/{your_key}?text=YOUR_TEXT
```
To support markdown message or push message longer than 256 character, add "content" param
```
https://pushbot.cat/api/push/text/{your_key}?text=TITLE&content=YOUR_TEXT
```

#### Push picture
```
https://pushbot.cat/api/push/img/{your_key}?url=PIC_NET_URL
```
Give your picture a description, add "content" param
```
https://pushbot.cat/api/push/img/{your_key}?url=PIC_NET_URL&content=PIC_DESCRIPTION
```
More API usage can be found at [our website](https://pushbot.cat/documentation)

#### All API support GET and POST, it will return

success:
```
{
   "code": 1,
   "msg": "success"
}
```
fail:
```
{
   "code": 0,
   "msg": "error message"
}
```
