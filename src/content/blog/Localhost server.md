---
title: Localhost server
date: '2020-03-26'
tags: ['Dev', 'localhost', 'SSH tunneling']
slug: localhost-server
image: ./images/bg-image-1.jpg
flip: false
dirction: ltr
excerpt: Research is the root of good process - Do it right and you might do everything right
---

Use a localhost server ****- A way to share your localhost and test on other devices 

[ngrok - secure introspectable tunnels to localhost](https://ngrok.com/)

I'm using this one

![Run gridsome develop](./Localhost-server/Screen_Shot_2020-04-21_at_17.30.35.png "After runnig gridsome develop")

If port `8080` is in use

![Run ngrok command](./Localhost-server/Screen_Shot_2020-04-21_at_17.32.03.png "Run ngrok command")

Then  run  `./ngrok http 8080`

![See ngrok link](./Localhost-server/Screen_Shot_2020-04-21_at_17.29.27.png "After runnig ngrok command")

Use Forwarding https link  and share