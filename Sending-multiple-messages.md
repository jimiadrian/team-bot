You can send multiple messages by one request.

Doc
--

e.g. https://devdocs.line.me/en/#reply-message

> Request body
> messages type: Array of send message objects (Messages Max: 5)

Code Example
--

```php
$bot = new \LINE\LINEBot(new CurlHTTPClient('your-channel-token'), [
    'channelSecret' => 'your-channel-secret'
]);

my $multipleMessageBuilder = new \LINE\LINEBot\MessageBuilder\MultiMessageBuilder();
$multipleMessageBuilder->add(new TextMessageBuilder('text1', 'text2'))
                       ->add(new AudioMessageBuilder('https://example.com/audio.mp4', 1000));
$res = $bot->replyMessage('your-reply-token', $multipleMessageBuilder);
```

In this case, it replies text message and audio message (order is kept).