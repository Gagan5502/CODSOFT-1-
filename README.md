# CODSOFT-1-
# ChatBot: Rule-Based Bot

def chatbot(user_input):
    msg = user_input.lower().strip()

    if "hello" in msg or "hi" in msg:
        return "Hello! I'm ChatBot. How can I assist you today?"
    elif "how are you" in msg:
        return "I'm doing great, thanks for asking! 😊 What about you?"
    elif "your name" in msg:
        return "I'm ChatBot, made by Gagan !"
    elif "help" in msg:
        return "Sure! You can ask me about weather, time, jokes, or just chat!"
    elif "bye" in msg or "exit" in msg:
        return "Goodbye! Have a wonderful day ahead!"
    else:
        return "Hmm... I'm not sure how to answer that. Try rephrasing?"

# Run Loop
print("🤖 ChatBot is online! Type 'bye' to exit.")
while True:
    user = input("You: ")
    response = g_chatbot(user)
    print("Bot:", response)
    if "bye" in user.lower():
        break
