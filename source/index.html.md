---
title: Bucket API Reference

language_tabs:
  - shell

toc_footers:
  - <a href='https://github.com/tripit/slate' target="_blank">Documentation powered by Slate</a>

includes:
  - errors
  - sessions
  - users
  - tools
  - segmentation_funnels
  - quiz_types
  - outcomes
  - question_types
  - questions
  - sections

search: true
---

# Introduction



# Authentication

> To authorize, use this code:

```shell
# With shell, you can just pass the correct header with each request
curl "api_endpoint_here"
  -H "Authorization: meowmeowmeow"
```

> Make sure to replace `meowmeowmeow` with your API key.

Kittn expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: meowmeowmeow`

<aside class="notice">
You must replace <code>meowmeowmeow</code> with your personal API key.
</aside>
