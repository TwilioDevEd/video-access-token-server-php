# Video Quickstart for PHP

This application should give you a ready-made starting point for writing your
own video apps with Twilio Video. Before we begin, we need to collect
all the config values we need to run the application:

| Config Value  | Description |
| :-------------  |:------------- |
Configuration Profile SID | Identifier for a set of config properties for your video application - [find yours here](https://www.twilio.com/console/video/profiles).
Account SID | Your primary Twilio account identifier - find this [in the console here](https://www.twilio.com/console).
API Key | Used to authenticate - [generate one here](https://www.twilio.com/console/video/dev-tools/api-keys).
API Secret | Used to authenticate - [just like the above, you'll get one here](https://www.twilio.com/console/video/dev-tools/api-keys).

## A Note on API Keys

When you generate an API key pair at the URLs above, your API Secret will only
be shown once - make sure to save this in a secure location, 
or possibly your `~/.bash_profile`.

## Setting Up The PHP Application

Create a configuration file for your application:

```bash
cp config.example.php config.php
```

Edit `config.php` with the four configuration parameters we gathered from above.

Next, we'll need to install the Twilio Helper library via [Composer](https://getcomposer.org/).

```bash
composer install
```

Now we should be all set! Run the application using the `php -S` command.

```bash
php -S 127.0.0.1:8000
```

Alternately, you could simply place the contents of this project directly in the
webroot of your server and visit `index.html`.

Your application should now be running at [http://localhost:8000](http://localhost:8000).
Select any room name and join the room. Join the same room with another user in another browser tab or window to start video chatting!

![screenshot of chat app](https://s3.amazonaws.com/com.twilio.prod.twilio-docs/images/video2.original.png)

## License

MIT
