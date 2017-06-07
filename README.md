# resin-docker-webhooks-demo

> Webhooks demo from a Resin.io Docker container

## Prerequisites

1) Install [node](https://nodejs.org/en/)
2) Install [git](https://git-scm.com/downloads)
3) Install [yarn](https://yarnpkg.com/lang/en/docs/install/)

## Getting started

1) clone this repo

```bash
git clone https://github.com/thegreatsunra/resin-docker-webhooks-demo.git
cd resin-docker-webhooks-demo
```

2) install dependencies

```bash
yarn
```

## Make it work

1) start the endpoint server in one window

```bash 
node ./endpoint.js
```

2) start the messenging server in another window

```bash
node ./messenger.js
```

### Set up resin.io and push your project to get it on a device

1) [Sign up for a resin.io account][signup-page]

2) Create an app on resin.io. Look at their [Getting Started tutorial][gettingStarted-link] for help

3) Set up a device (e.g. a Raspberry Pi 3) on resin.io

4) Add your resin.io application's remote repository to your project repo

```bash
# run this command from your resin-docker-webhooks-demo folder
git remote add resin username@git.resin.io:username/myapp.git
```

5) Push your changes to the newly added remote to kick off a build:

```bash
git push resin master
```

It will take a few minutes for the code to push, build, deploy to your device, and for your device to start your app

## License

The MIT License (MIT)

Copyright (c) 2017 Dane Petersen

[resin-link]:https://resin.io/
[signup-page]:https://dashboard.resin.io/signup
[gettingStarted-link]:http://docs.resin.io/#/pages/installing/gettingStarted.md
