# tiktok-users-info
A dead-simple PHP package gives TikTok users statistics


### Usage

```php
<?php

// require __DIR__ . '/src/Users.php';

$getTiktokUser = new TikTok\Users();

echo $getTiktokUser->details('@emxh');
```

### Example responses 

###### HTTP_CODE 200

```json
{
    "code": 200,
    "user": {
        "id": "7265945350605997074",
        "username": "emxh",
        "profileName": "Mohammad.",
        "avatar": "https://p16-sign-sg.tiktokcdn.com/aweme/720x720/tos-alisg-avt-0068/2f5e7abcdb14360bd2a42a9d7deb8b02.jpeg?x-expires=1695189600&x-signature=WZtOV6RYHZbWqWsowZXR8mRyWUY%3D",
        "description": "",
        "region": "US",
        "verified": false
    },
    "stats": {
        "following": 0,
        "follower": 505,
        "video": 1,
        "like": 17
    }
}
```

###### HTTP_CODE 404

```json
{
  "code": 404,
  "error": "This account cannot be found."
}
```

### Version

```code
0.0.1
0.0.1 — Fixed User-Agent.

0.0.2 — Fixed User-Agent.
        Fixed (regex) lookup of JSON data on the page.
```

### Orginal

###### nothing
