If application receives event that has a type that is not supported by this SDK, it encapsulates the event to `UnknownEvent'. `UnknownMessage` is also the same.

So if you want to handle unknown type events and messages, you should check type of instance like so;

### For unknown event

```php
if ($event instanceof MessageEvent) {
    // do something...
} elseif ($event instanceof UnknownEvent) {
    // implement here!

    $eventBody = $event->getEventBody(); // <= array of raw event payload
    // do something...
}
```

###　For unknown message

```php
if ($event instanceof MessageEvent) {
    if ($event instanceof TextMessage) {
        // do something
    } elseif ($event instanceof UnknownMessage) {
        // implement here!

        $messageBody = $event->getMessageBody(); // <= array of raw message payload 
        // do something
    }
}
```

`UnknownMessage#getEventBody` returns the array of raw event payload. It makes you to be able to implement the behavior of the event even if this SDK doesn't support the event type　（`UnknownMessage#getMessageBody` is also）.