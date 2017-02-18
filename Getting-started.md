How to create an API client of bot
--

```php
$bot = new \LINE\LINEBot(new CurlHTTPClient('your-channel-token'), [
    'channelSecret' => 'your-channel-secret'
]);
```

Simple replying
--

```php
$textMessageBuilder = new \LINE\LINEBot\MessageBuilder\TextMessageBuilder('hello');
$response = $bot->replyMessage('your-reply-token', $textMessageBuilder);
```

Documents
--

See the official API documentation for more information.

- English: [https://devdocs.line.me/en/](https://devdocs.line.me/en/)
- Japanese: [https://devdocs.line.me/ja/](https://devdocs.line.me/ja/)

Sample projects
--

### [Echo bot](https://github.com/line/line-bot-sdk-php/tree/master/examples/EchoBot)

A sample echo bot implementation.

### [Kitchen sink](https://github.com/line/line-bot-sdk-php/tree/master/examples/KitchenSink)

A full-stack LINE Messaging API sample implementation. This sample shows you a practical use of the LINE Messaging API.
