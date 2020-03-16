<img src="werewolf.jpg"/>

>### *A [discord.py](http://discordpy.readthedocs.io/en/latest/) bot focused on providing CTF tools for collaboration in Discord servers (ctftime.org commands, team setup, utilites, etc)!  If you have a feature request, make it a GitHub issue.*

[Invite to your server](https://discordapp.com/api/oauth2/authorize?client_id=688958016447447057&permissions=2100817008&scope=bot)


#  How to Use
>This bot has commands for encoding/decoding, ciphers, and other commonly accessed tools during CTFs.  But, the main use for NullCTF is to easily set up a CTF for your discord server to play as a team.  The following commands listed are probably going to be used the most.

* `>ctf create "ctf name"`  This is the command you'll use when you want to begin a new CTF.  This command will make a text channel with your supplied name under the category 'CTF' (If the category doesn't exist it will be created).  *Must have permissions to manage channels*

*NOTE: the following ctf specific commands will only be accepted under the channel created for that ctf.  This is to avoid clashes with multiple ctfs going on in the same server.*

 * `>ctf join/leave` Using this command will either give or remove the role of a created ctf to/from you.

 
 * `>ctf challenge add/working/solved/remove "challenge name"` Allows users to add or remove challenges to a list, and then set the status of that challenge. *Use quotations*
 
 * `>ctf challenge list` This is the list command that was previously mentioned, it displays the added challenges, who's working on what, and if a challenge is solved (and by who).

 > NOTE: There is shorthand!  challenge -> chal/chall, add -> a, working -> w, solved -> s, remove -> r

 * `>ctf end` Delete the ctf info from the db, and remove the role from your server.  *Must have permissions to manage channels*

---
>The following commands use the api from [ctftime](https://ctftime.org/api)

 * `>ctftime countdown/timeleft` Countdown will return when a selected CTF starts, and timeleft will return when any currently running CTFs end in the form of days hours minutes and seconds.

* `>ctftime upcoming <number>` Uses the api mentioned to return an embed up to 5 upcoming CTFs.  If no number is provided the default is 3.

* `>ctftime current` Displays any currently running CTFs in the same embed as previously mentioned.

* `>ctftime top <year>`  Shows the ctftime leaderboards from a certain year *(dates back to 2011)*.
---
>Utility commands
* `>magicb filetype` Returns the mime and magicbytes of your supplied filetype. Useful for stegonography challenges where a filetype is corrupt.

* `>rot  "a message" <right/left>` Returns all 25 possible rotations for a message with an optional direction (defaults to left).

* `>b64 encode/decode "message"`  Encode or decode in base64 *(at the time of writing this, if there are any unprintable characters this command will not work, this goes for all encoding/decoding commands).*

* `>binary encode/decode "message"` Encode or decode in binary.

* `>hex encode/decode "message"` Encode or decode in hex.

* `>url encode/decode "message"` Encode or decode with url parse.  This could be used for generating XSS payloads.

* `>reverse "message"` Reverse a message.

* `>counteach "message"` Count the occurrences of each character in the supplied message.

* `>characters "message"` Count the amount of characters in your message.

* `>wordcount a test` Counts the amount of words in  your message (don't use quotations).

* `>cointoss` Get a 50/50 cointoss to make all your life's decisions.

* `>request/report "a feature"/"a bug"` Dm's the creator (nullpxl#3928) with your feature/bug  request/report.

* `>help` Returns the help page


