## Pushbot, a simple and stable push message api for telegram
### How to use it
1. Sign in [Pushbot.cat](https://pushbot.cat/?from=github) by you telegram account.
2. Automatic get PushKey and start push message by using API.

### API
#### Push text message
```
https://pushbot.cat/api/push/text/{your_key}?text=YOUR_TEXT
```
To support **Markdown message** or push message longer than 256 characters, add "content" param (limit 5000 characters)
```
https://pushbot.cat/api/push/text/{your_key}?text=TITLE&content=YOUR_TEXT
```

#### Push picture
```
https://pushbot.cat/api/push/img/{your_key}?url=PIC_NET_URL
```
Give your picture a description, add "content" param (limit 256 characters)
```
https://pushbot.cat/api/push/img/{your_key}?url=PIC_NET_URL&content=PIC_DESCRIPTION
```
More API usage can be found at [Pushbot.cat](https://pushbot.cat/documentation?from=github)

**GET** and **POST** requests are supported to send data to the API server, response

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
