# Jeremy Keith

- Piece of history about DOM, Javascript and JQuery

### The code is just an translation... its about the code

## Introduction

- Service workers - How does it work

  - Phone -> network -> server -> network -> phone
  - Serviceworkers: Intercepting request and do stuf in between
  - Only for https

- Register a service worker
  - Do not write `<script src="someUrl"></script>`
  - DO write `<script>navigator.serviceWorker.register("DO NOT SET URLS IN HERE!")</script>`
  - Do feature detecture with an `if()` statement around your script
  - Triggers an event and eneble for example caching
    - We have now cache API -> Create your own cache
      - You can precache during the installation
      - Phone -> network -> server -> network -> _CACHE STORAGE_ -> phone
      - Must be async!!
      - intall -> event -> `cache.open` -> `cache.addAll` => we've cached files now
      - Try fetch for cache frist || fetch from network

## Using this way of caching, you can litterly browser offline

- Dont use this for whole websites
- Do use this for css / icons etc.
- For HTML network first || network backup page
- You can me a custom offline page

  ![alt text](https://res.cloudinary.com/rowin648/image/upload/v1558079448/staro/hyjppc2l9niep30tvrey.png 'Logo Title Text 1')

Notice

- HTML => freshness fist
- CSS => speed first

If you have a https, service worker and have manifest file you will get a progressive web app => Awesome ... Lets dismiss the message and never use this..
