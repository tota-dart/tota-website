---
title: "How to create an access token on Netlify"
date: "2019-06-23"
template: "posts.mustache"
public: true
---

# How to create an access token on Netlify

Before you can deploy your site to [Netlify](https://netlify.com/), you must
create an **access token** to allow Tota to authenticate on your behalf.

Note: _ensure that you have previously registered an account with Netlify before
following these steps._

<br>

## 1. Generate token

Head over to [your applications](https://app.netlify.com/user/applications) in
the Netlify admin panel, and click on the "**New access token**" button placed
beneath the "Personal access tokens" section.

![Enter a description](/assets/img/posts/create-access-token-netlify.png)

Add a description to remind yourself where this access token will be used,
and click "**Generate token**".

<br>

## 2. Add token to config

Take the access token generated in the previous step and add it to your Tota
configuration file (`.env`). For example:

```bash
TOTA_NETLIFY_TOKEN="54686520717569636b2062726f776e20666f78206a756d7073206f7665722031"
```

That's it! Now you're ready to deploy to Netlify.

