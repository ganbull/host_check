# host_check
#Step 1. Enter @Botfather in the search tab and choose this bot.
#Click “Start” to activate BotFather bot.
#Choose a name for your bot — your subscribers will see it in the conversation. And choose a username for your bot — the bot can be found by its username in searches. The username must be unique and end with the word “bot.”
#edit file alert.sh, with name api and your id chat ( you can see id in URL)
#In ubuntu
sudo su
apt update
apt upgrade
apt install mc
cd /home
mcedit ping.sh
# then copy text from file ping.sh and past by shift+insert
mcedit alert.sh
# then copy text from file alert.sh and past by shift+insert
mcedit list.txt
# paste ip-address, what you want to check
crontab -e
#to the end file past: 
* * * * * /home/ping.sh
