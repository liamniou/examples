<!--
title: TODO
description: This example demonstrates how to setup an echo Telegram Bot using the Serverless Framework.
layout: Doc
framework: v1
platform: AWS
language: Python
priority: 10
authorLink: 'https://github.com/jonatasbaldin'
authorName: 'Jonatas Baldin'
authorAvatar: 'https://avatars3.githubusercontent.com/u/8570364?v=4&s=140'
-->
# Serverless Telegram Bot
This example demonstrates how to setup an echo Telegram Bot using the Serverless Framework ⚡🤖

## Usage

### What do I need?
- A AWS key configured locally, see [here](https://serverless.com/framework/docs/providers/aws/guide/credentials/).
- NodeJS. I tested with v8.9.0.
- A Telegram account.

### Installing
```

brew install node@14
brew link --overwrite node@14

brew install python3.7
echo 'export PATH="/usr/local/opt/python@3.7/bin:$PATH"' >> ~/.zshrc

npm install -g serverless@1.71.1

npm install

code ~/.aws/credentials
>>>
[ckl]
aws_access_key_id = KEY_ID
aws_secret_access_key = ACCESS_KEY

serverless deploy

# Install the necessary plugins
$ npm install

# Get a bot from Telegram, sending this message to @BotFather

# Put the token received into a file called serverless.env.yml, like this
$ cat serverless.env.yml
TELEGRAM_TOKEN: <your_token>

# Deploy it!
$ serverless deploy

# With the URL returned in the output, configure the Webhook
$ curl -X POST https://<your_url>.amazonaws.com/dev/set_webhook
```
