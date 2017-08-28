# Cecil
Welcome To nightvale, im stuck in the ethernet

var Discord = require('discord.io');

var bot = new Discord.Client({
    token: "",
    autorun: true
});

bot.on('ready', function() {
    console.log('Logged in as %s - %s\n', bot.Cecil, bot.id);
});

bot.on('message', function(user, userID, channelID, message, event) {
    if (message === "Hello Cecil") {
        bot.sendMessage({
            to: channelID,
            message: "Hello Listeners, and welcome."
        });
    }
});
