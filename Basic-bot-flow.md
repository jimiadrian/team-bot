1. User actions something in talk room, or beacon event is fired (it sends the action to the LINE server)
2. The LINE server sends the  `event(s)` to `callback url` of your bot server as webhook. The event corresponds to users action
3. Your bot server receives `event(s)` and should handle it

When you create a bot, you should do three phases.

1. Receive webhook
2. Parse `event(s)`  that is via webhook by [\LINE\LINEBot#parseEventRequest()](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.html#_parseEventRequest). You must pass the body of webhook and the signature to the method. The signature is included in the `X_LINE_SIGNATURE` HTTP header
3. Switch processing depending on the type of event and do your domain

See also
--

- [[Event|Event]]
- [EchoBot/Route](https://github.com/line/line-bot-sdk-php/blob/e16d9ca/examples/EchoBot/src/LINEBot/EchoBot/Route.php)
- [KitchenSink/Route](https://github.com/line/line-bot-sdk-php/blob/e16d9ca/examples/KitchenSink/src/LINEBot/KitchenSink/Route.php)