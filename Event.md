`Event` is a request that is sent from the LINE server via webhook. The content of `Event` corresponds to the action of user.
`Event` identifies the event type, and also it can retrieve the content (e.g. message that corresponds the event type, reply token and etc.) from the `Event` .

The types of `Event` is following. Please refer phpdoc for details.

- [MessageEvent](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.Event.MessageEvent.html)
  - [TextMessage](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.Event.MessageEvent.TextMessage.html)
  - [ImageMessage](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.Event.MessageEvent.ImageMessage.html)
  - [AudioMessage](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.Event.MessageEvent.AudioMessage.html)
  - [VideoMessage](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.Event.MessageEvent.VideoMessage.html)
  - [LocationMessage](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.Event.MessageEvent.LocationMessage.html)
  - [StickerMessage](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.Event.MessageEvent.StickerMessage.html)
- [FollowEvent](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.Event.FollowEvent.html)
- [UnfollowEvent](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.Event.UnfollowEvent.html)
- [JoinEvent](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.Event.JoinEvent.html)
- [LeaveEvent](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.Event.LeaveEvent.html)
- [PostbackEvent](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.Event.PostbackEvent.html)
- [BeaconDetectionEvent](https://line.github.io/line-bot-sdk-php/class-LINE.LINEBot.Event.BeaconDetectionEvent.html)