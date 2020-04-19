# AK47 Commands
The default command prefix is `+`.

<> = required\
[] = optional\
| = or\
... = accepts spaces\
*italic* = replace with your own value

## Account

### Log In
> login <*exchange code*>

Aliases: `i`, `signin`\
Logs in to an Epic account using exchange code (make one on https://www.epicgames.com/id/login?redirectUrl=https%3A%2F%2Fwww.epicgames.com%2Fid%2Fapi%2Fexchange).

Example:
* `login aabbccddeeff11223344556677889900`

### Log Out
> logout

Aliases: `o`, `signout`\
Logs out the Epic account.

### Devices
> devices <list|create|delete>

Aliases: `device`\
Device auth operation commands.

### Save Login
> savelogin

Redirects to `devices create`.

### Delete Saved Login
> deletesavedlogin

Redirects to `devices delete <registered device ID>`.

### Claim Two-Factor Authentication Reward
> claim2fa

Aliases: `claimmfa`, `boogiedown`\
Claim 2fa reward (Boogie down emote) on your account.

### Generate Exchange Code
> exchange

Generates an exchange code.

## Fortnite Core

### Gift History
> gifthistory

Aliases: `gifth`\
Check how much gifting slots is remaining along with a history of sent/received gifts.

### Support-a-Creator
> sac [*new code*|clear]

Displays or changes the Support a Creator code. Use `clear` to unset the code.

### V-Bucks Balance
> vbucks

Aliases: `v`, `balance`, `bal`, `mtx`, `vbucksbalance`\
Tells you how much V-Bucks the account has on all platforms.

### V-Bucks Platform
> vbucksplatform <WeGame|EpicPCKorea|Epic|EpicPC|EpicAndroid|PSN|Live|IOSAppStore|Nintendo|Samsung|Shared>

Aliases: `vp`, `mtxplatform`\
Changes the V-Bucks platform.

## Fortnite Battle Royale

### Purchase Battle Pass/Tiers
> battlepass <1|2|3>

Aliases: `bp`\
Purchase battlepass or tiers.

### Purchase Item
> buy <*item number*> [*quantity*] [*price index*]

Aliases: `b`, `purchase`\
Purchases a shop entry from the Battle Royale or Save the World Item Shop. Argument `price index` defaults to and starts from 1 and is applicable for non dynamic bundle entries.

### Gift Item
> gift <*item number*> <*friend 1*[;*friend 2*[;*friend 3*[;*friend 4*]]]>

Aliases: `g`\
Gifts up to 4 friends a shop entry from current Battle Royale item shop.\
Argument `friend` accepts Epic display name (spaces allowed), email, account ID, or friend number.\
Epic Games has removed the gift message text field from the game, so the gift message will be the default one.

Example:
* Single recipient with one word display name:\
  `g 5 noobmaster69`

* 4 recipients with varying types of identification:\
  `g 5 noobmaster69;I take wall;ramirez@gmail.com;d43dce39c5044b8f84bf24f2493fd393`

### Locker
> locker

Generate images of all Battle Royale items in the account.

### Item Shop
> shop

Aliases: `s`\
Displays current Battle Royale item shop image.

### Item Shop (as Text)
> shoptext

Aliases: `st`\
Sends the current item shop items as a text.

### Cancel Purchase
> cancelpurchase

Aliases: `refund`, `undo`\
Cancel your last purchase.

## Fortnite Save the World

### Claim STW Daily Rewards
> claimdaily

Aliases: `daily`\
Claims the STW daily reward.

### Edit Homebase Name
> homebasename [*new name...*]

Displays or changes the homebase name. (STW owning accounts only)

### STW Item Shop
> stwshop

Sends the current Save the World item shop items as a text.

## Friends
Base command: **friends**. Aliases: **f**.

### List Friends
> friends list [friends|incoming|outgoing|suggested|blocklist]

Aliases: `f`\
Lists friends in the account along with their account IDs. Defaults to accepted friends (`friends`) if no second argument were specified.

### Add Friend
> friends add <*display name...*|*email*|*account ID*>

Lookup a user and send them/accept their friend request.

### Remove Friend
> friends remove <*display name...*|*email*|*account ID*>

Lookup a user and unfriend them if you're friends.

### Accept Incoming Friend Request
> friends accept <*display name...*|*email*|*account ID*|all>

Lookup a user and accept their friend request if there is any.

### Reject Incoming Friend Request
> friends reject <*display name...*|*email*|*account ID*|all>

Lookup a user and reject their friend request if there is any.

### Cancel Outgoing Friend Request
> friends cancel <*display name...*|*email*|*account ID*|all>

Lookup a user and cancel your outgoing friend request if there is any.

## Public
> host

Host custom matchmaking games (codes sent to verified users only). (Server admins only)
### Steps :
**1.** Start by making a channel for custom games then do the command `host`
**2.** Write down your GameMode name ,then your game rules
**3.** The bot will dm you with your custom matchmaking code, go in game and start hosting the match with the same code the bot sent
**4.** Tell your viewers/friends to react to the custom matchmaking message to enroll to the match
**5.** After getting enough number of player, go to the channel you hosted in, do the command `start` to start spreading your custom code to your players
**Disclaimer** : Non-Verified user will not receive the code, only verified members will. 

> prefix <*new prefix*>

Aliases: `akprefix`\
Change prefix for the server/user. (Server admins only)

> shop

Aliases: `s`\
Displays current Battle Royale item shop image.

> vmessage [more text (can be another languages)]

Send message to instruct people about verify themselves

> verify

Verify your ownership for your Epic account. (DMs only)
### Steps :
**1.** Start dming AK47 with command `verify`
**2.** Write down your epic username after a couple of seconds you will receive a friend request from `AK47-BOT`
**3.** After accepting the friend request `whisper` the bot with the verification code you received from ak47 on discord
**4.** AllGood!, You are now verified (Epic Linked To Discord), And you can now receive custom code from your favourite streamer/hoster.
