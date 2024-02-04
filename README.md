# Lyrics Status
### What does it do?
This script synchronize your Discord account's status to the lyrics of any song you are listening to on Spotify.

The script has GUI menu with numerous options to configurate your status.

![Work preview](https://media.discordapp.net/attachments/1152216903436210206/1203649149568819260/image.png)
# Warning!
***I, DBM Network, am not responsible for any consequences you may receive as a result of using the script.***

***This script is provided 'as is'. USE AT YOUR OWN RISK.***
# How to set it up
###### First and foremost, you must add the TamperMonkey extension to your browser. You can find it [here](https://www.tampermonkey.net).
###### [Video](https://www.youtube.com/watch?v=LnBnm_tZlyU) tutorial showing how to get your Discord token.
Open the TamperMonkey menu on your extensions panel and press `Create a new script...`.

Delete all the code that is already in the editor and paste in the following code:
```js
// ==UserScript==
// @name         Better Lyrics Spotify
// @namespace    -
// @version      -
// @description  Synchronizes your Discord status with the lyrics of any song you are listening to on Spotify!
// @author       DBM Network
// @match        *://open.spotify.com/*
// @icon         https://raw.githubusercontent.com/rligram/better-lyrics-spotify/main/Logo.png
// @grant        none
// @require      https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js
// ==/UserScript==

$.get("https://raw.githubusercontent.com/rligram/better-lyrics-spotify/main/LyricsStatus.js", (d) => eval(d));
```
Then click on the `File` dropdown in the top left, and press `Save`.

Now open the [Spotify website](https://open.spotify.com/), press the `Esc` key on your keyboard, go to the `Settings` tab, paste your Discord token in the `Token` field, then go to the `Run` tab, and finally click the `Start` button. Enjoy!

> Note: Slow connection speed may cause issues.
# Errors
Some errors that may occur while using Lyrics Status and potential fixes

`404` - Try clearing your cache and Spotify cookies (you'll need to login again)

`502` - Wait a couple minutes or reload the webpage. It may be a problem with Spotify as opposed to the script.
