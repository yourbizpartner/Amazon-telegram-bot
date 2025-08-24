import os
import telebot

# Telegram Bot Token (BotFather se liya hua)
BOT_TOKEN = os.getenv("BOT_TOKEN")

bot = telebot.TeleBot(BOT_TOKEN)

@bot.message_handler(commands=['start'])
def send_welcome(message):
    bot.reply_to(message, "Namaste 🙏, main Amazon Deals Bot hoon! ")

@bot.message_handler(commands=['deal'])
def send_deal(message):
    # yahan tum apna Amazon affiliate link dalna
    deal_link = "https://amzn.to/3XXXXXX"  # Example affiliate link
    bot.send_message(message.chat.id, f"Aaj ka Amazon Loot Deal 🔥\n{deal_link}")

bot.polling()
