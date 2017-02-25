You can get user's profile by the `user_id`.

Doc
--

https://devdocs.line.me/en/#bot-api-get-profile

Code Example
--

```php
$bot = new \LINE\LINEBot(new CurlHTTPClient('your-channel-token'), [
    'channelSecret' => 'your-channel-secret'
]);

$res = $bot->getProfile('user-id');
if ($res->isSucceeded()) {
    $profile = $res->getJSONDecodedBody();
    $displayName = $profile['displayName'];
    $statusMessage = $profile['statusMessage'];
    $pictureUrl = $profile['pictureUrl'];
}
```