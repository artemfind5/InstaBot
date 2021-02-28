# InstaBot - Massliking and more
[closed the API]: http://developers.instagram.com/post/133424514006/instagram-platform-update
[LevPasha]: https://github.com/LevPasha
[jaguar754's edits]: https://github.com/jaguar754/instabot.py
Instagram bot. Works without Instagram API.

After Instagram [closed the API] (new checkout process), there was a problem: automatically like, comment and subscribe.

This version is a revision to [LevPasha]'s project and [jaguar754's edits] (instabot-py).

By 2021, the implementation of authorization and search for media data objects have become irrelevant.
This version is working correctly.

This InstaBot runs on https://www.instagram.com and only requires your username and password.

# Example
1. Set the value of the like_per_day, more_than_likes, tag_list, max_like_for_one_tag and log_mod that you need:
```python
def __init__(self, login, password,
                like_per_day=100,
                more_than_likes=10000,
                tag_list=['cat', 'dog'],
                max_like_for_one_tag = 5,
                log_mod = 0):
```

2. Create a class object with login and password arguments and run:
```python
bot = InstaBot('username', 'password')
bot.auto_mod()
```
