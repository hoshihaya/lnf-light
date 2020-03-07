# lnf-light

LINE Notify clinet light

## token settings

- 1. Issue token from https://notify-bot.line.me/my
- 2. Write the token to '~/.line/notify.token'.

```
mkdir ~/.line
vi ~/.line/notify.token
chmod 700 ~/.line
chmod 600 ~/.line/notify.token
```

## execute lnf

```
lnf your message
```

## one-liner

```
LINE_NOTIFY_ACCESS_TOKEN=$(cat ~/.line/notify.token); curl -X POST -H "Authorization: Bearer ${LINE_NOTIFY_ACCESS_TOKEN}" https://notify-api.line.me/api/notify -F "message=てすと"
```
