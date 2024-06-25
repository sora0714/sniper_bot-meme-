<img width="64" height="64" align="left" style="float: left; margin: 10px 10px 0 0;" alt="Icon" src="https://imgur.com/dRSYp1f.png">

# Sniper

> An easy to run simple bot that lets you snipe messages in your Discord server.

## Setup

[Node.js 16.9.0](https://nodejs.org) or newer is required.

1. Run:

```bash
$ git clone https://github.com/DankMemer/sniper.git
$ cd ./sniper
```

2. Create config.json:

```json
{
	"token": "<Your bot's token>",
	"application_id": "<Your application's id>"
}
```

3. Run:

```bash
$ npm i
$ npm run register [guild id]
$ npm run bot
```

> Note:
> Without specifying [guild id], the snipe commands will be available to all of your app's guilds. They will fan out slowly across all guilds and will be guaranteed to be updated in an hour (due to Discord's cache).
> 
> With [guild id] they will be available only within the guild specified and will update instantly.

## Dockerfile instructions
An [example Dockerfile](Dockerfile.example) has been included. Modify line 12 to change the guild id. If you want to make the bot global, simply comment out line 12.

## License

[MIT](https://tldrlegal.com/license/mit-license)
