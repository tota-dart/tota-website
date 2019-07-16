---
title: "Host on Netlify | Tota"
template: "docs"
public: true
---

# Host on Netlify

Netlify provides a global CDN, continuous deployment, automatic HTTPS, a pleasant UI and CLI tool, and quite a generous free plan.

<br>

## Create an account

If you have already signed up, you can skip this step. Otherwise, go to [app.netlify.com](https://app.netlify.com/) and select your preferred signup method.

<br>

## Create an access token

Tota needs your authorization to deploy a site to your Netlify account. You can generate an access token
for this purpose within the Netlify admin UI by following the steps in this help article.

* [How to create an access token on Netlify](/articles/how-to-create-an-access-token-on-netlify)

Once you have created your access token, add it to your Tota config.

```bash
TOTA_NETLIFY_TOKEN="54686520717569636b2062726f776e20666f78206a756d7073206f7665722031"
```

<br>

## Create a site

Every site on Netlify is given a unique site name identified by its subdomain on Netlify's URL.
For example, **_tota_**.netlify.com. This namespace is shared among all Netlify user accounts,
so it has to be unique.

Add your chosen site name to the config.

```bash
TOTA_NETLIFY_SITE="tota"
```

On deploy, Tota will automatically create a site for you, if it doesn't already exist under your account.

<br>

## Deploy site

Once you have added your access token and site name to the Tota config, use the [deploy command](/docs/commands#deploy)
to deploy your site.

```bash
tota deploy --host netlify
```
