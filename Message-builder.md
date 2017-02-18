As its name suggests, `MessageBuilder` is the builder of message.

The client of Messaging API (i.e. instance of `\LINE\LINEBot`) uses `MessageBuilder` as parameter to send message. The client of Messaging API builds and encode a JSON string according to `MessageBuilder` and send it as API request.

If you are an user of the client of Messaging API, you can treat `MessageBuilder` as message itself. In other words, user of the client should just create a `MessageBuilder` that corresponds to message and handle that as a parameter of the client.

The types of `MessageBuilder` is following. Please refer phpdoc for details.

- [TextMessageBuilder](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.MessageBuilder.TextMessageBuilder.html)
- [ImageMessageBuilder](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.MessageBuilder.ImageMessageBuilder.html)
- [AudioMessageBuilder](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.MessageBuilder.AudioMessageBuilder.html)
- [VideoMessageBuilder](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.MessageBuilder.VideoMessageBuilder.html)
- [LocationMessageBuilder](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.MessageBuilder.LocationMessageBuilder.html)
- [StickerMessageBuilder](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.MessageBuilder.StickerMessageBuilder.html)
- [TemplateMessageBuilder](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.MessageBuilder.TemplateMessageBuilder.html)
- [ImagemapMessageBuilder](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.MessageBuilder.ImagemapMessageBuilder.html)
- [MultiMessageBuilder](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.MessageBuilder.MultiMessageBuilder.html) (See also: [[Sending multiple messages|Sending-multiple-messages]])