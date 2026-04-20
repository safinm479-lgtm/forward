from telegram import Update
from telegram.ext import Application, MessageHandler, filters, ContextTypes

TOKEN = "8700311212:AAG_cwTFMpJNac6J2pHocbYefy445gyXPFQ"
CHANNEL = "@ottzivvionline"

async def copy(update: Update, context: ContextTypes.DEFAULT_TYPE):
    await context.bot.send_message(
        chat_id=CHANNEL,
        text=update.message.text
    )

app = Application.builder().token(TOKEN).build()
app.add_handler(MessageHandler(filters.TEXT, copy))

app.run_polling()
