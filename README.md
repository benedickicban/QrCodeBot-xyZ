# QrCodeBot-xyZ
- This is a Discord bot that will provide a QR Code to your Axie Infinity scholars.
- This version of the bot is compatible with ronin!

- If you want to use it with Ethereum information instead:

In submitSignaure function, change "mainnet":"ronin" to "mainnet":"ethereum"

# Setup
1. Run Ubuntu on AWS ec2 instance
2. Clone the file by running:
* `git clone https://github.com/benedickicban/QrCodeBot-xyZ.git`
3. Install the requierements by running in to correct path:
* `chmod +x install-ubuntu.sh`
* `sudo ./install-ubuntu.sh`
4. Follow this tutorial to create and add a bot to your Discord Server:
* `https://discordpy.readthedocs.io/en/stable/discord.html`
5. Update the SecretStorage.py file in repo with the Token of your bot and with the information of your scholars.
6. Run the script by running in to correct path:
* `python3 ./QrCodeBot-xyZ.py`

# bug to fix
- [x] Current time isn't displayed correcly
- [x] Fix edge case where the bot could send a wrong code
- This could've happen in extreme edge cases where a lot of scholars were asking for a code simultaniously and axie server didn't respond in a timely manner!
- This was fixed by making sure every QRCode was saved using the scholars DiscordUUID 

Please tell me if you experience any bugs...

