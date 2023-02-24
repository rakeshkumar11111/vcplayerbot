# Telegram VCPlayer Bot
Play any media(song, video, live, remote) directly into your group voice chat.

Official Bot : [VCPlayerBot](https://telegram.me/vcplayerbot)   |   Discussion Group : [VoiceChat Music Player Support](https://telegram.me/voicechatsupport)

<p align="center">
  <img width="200" height="200" src="https://github.com/kshubham506/vcplayerbot/blob/master/etc/logo.jpg?raw=true">
</p>

[Checkout AutoForwarder Bot](https://sktechhub.com/auto-forward) | [Try Code Compile Bot](https://t.me/codecompilebot)


# Requirements
1. Telegram Api Id and Hash [ Get it from http://my.telegram.org ]
2. A Telegram Bot Token. Get it from [@botfather] 6261297005:AAEnfm0uI-mbcYKc_qDSJQNDyPJ7_X1jyZE
3. Python 3.6+
4. [ Optional, only use if you are an advanced user ] Mongo DB [ Create free account from mongo website and get your connection string. ] 

# Deploying To Heroku
1. Get your telegram API ID and API HASH from my.telegram.org and the BOT TOKEN from [@botfather](https://t.me/botfather)
2. Generate your telegram session string using the `Run on Repl` button below (Click on run after opening the url below) or use the `generateSession.py` file or read the steps [mentioned here](get_session_string.md).

- [![Run on Repl.it](https://repl.it/badge/github/rakesh11111
- 


/music](https://replit.com/@rakesh11111/GenerateSession?lite=1&outputonly=1)


3. Click on the `Deploy to Heroku` button below. Fill in the required fields on the website that opens.

- [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

4. Add the bot to your group and send the [commands](https://github.com/kshubham506/vcplayerbot#features) to start using the VCPlayer Bot :)


# Steps To Setup on VPC or Locally
1. Read the steps [mentioned here](get_session_string.md) to get your session string.
2. Rename `.env copy` to `.env` and fill all the values there. You can leave the `MONGO_URL` line as it is (only fill if you know what you are doing)


# Steps to Run
1. After the setup is done.
2. Install the requirements : `pip3 install -U -r requirements.txt`
3. Run the service by : 
  - Run `python3 main.py -env prod` 
  
  - (make sure `-env prod` flag is provided, if not rename `.env` file to `.env.copy`)

# Environmental Variables

Starting from command line:
- python3 main.py -env `prod|local`

Available env variables
- `Mandataory` **API_ID** :  27874394
- `Mandataory` **API_HASH** : 7d34cfcde089859977200f3d818532b1
- `Mandataory` **BOT_TOKEN** : 6261297005:AAEnfm0uI-mbcYKc_qDSJQNDyPJ7_X1jyZE
- `Mandataory` **USERBOT_SESSION** :  [mentioned here](get_session_string.md) BQBdI0mowmYj3KvnHPp-dzlHGCcB_KotAu9TZKAJNPG-tNop6xvn-uB56sP8QP63Etc0moUR50oLpXbWk7PHbJHwhdUL_8zIM_FXa82JscN0cxwMQfEBAAGRJXtEeFh7k4Kdt3RVaguz5l4_aKenrC7lsKrpwP6sqM9rXO6QpXm4jZs9QFs7AJsrA-UsHCZsKuIkX-yPva_uoZGrESNT4_K0WJl6yIKXYTrz2MFAHQKmedolNIeHIsA6npj-6oHUwr2AleZgE6g4Ilss8V4eqrUAdDEcIT7kY4jcJqNDPVrTcemnuLAfovxggb45C1ytB36AMz4Kx3v_P_3H6A-WnTRlAAAAAVFqOdYA
- `Optional` **MONGO_URL** : connection url for mongo databse. needed if you wnat to run the service in single mode

- Many other optional variables, check [Config.py](utils/Config.py) file for details.

# Features
Streams directly from url, Playlist support

Command | Description
------------ | -------------
/start , /help | Lists the available commands.
/play song_name/song_url -res[num] | Starts the song in the voice chat, num specifies the audio resolution. eg. `/play coldplay -res256` → plays coldplay song in 256 bit rate
/play song_name/song_url -video -res[num] | Starts the video in the voice chat, num specifies the video resolution. eg. `/play coldplay -res2480` → plays coldplay video in 480p
/skip | Skip the current media playback.
/stop | Stops the playback.



<p align="center">
  <img width="500" height="300" src="https://github.com/kshubham506/vcplayerbot/blob/master/etc/signs_of_time.jpg?raw=true">
</p>

# Developer
[Shubham Kumar](https://github.com/rakesh11111)

For any issues/questions please contact [here](https://telegram.me/voicechatsupport)

Pull Requests are more than welcome.


 ### [A SkTechHub Product](https://sktechhub.com)
