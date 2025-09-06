
import telebot

# tu wstaw swój token
TOKEN = "7311991999:AAGbRwrMD40KW2ObOFXUMW1x55LelpxioIU"
bot = telebot.TeleBot(TOKEN)

@bot.message_handler(commands=['start'])
def start(message):
    bot.reply_to(message, "Bot działa!")

print("Bot wystartował...")
bot.polling()
