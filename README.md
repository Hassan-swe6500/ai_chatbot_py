# ai_chatbot_py

def get_reply(user_input):
    """User ke message ke hisab se reply return karta hai."""
    msg = user_input.lower().strip()

    if msg == "hello" or msg == "hi":
        return "Hi!"
    elif msg == "how are you":
        return "I'm fine, thanks!"
    elif msg == "what is your name":
        return "I'm a simple chatbot."
    elif msg == "bye":
        return "Goodbye!"
    elif msg == "what are you doing":
        return"I am chatting with you!"
    else:
        return "Sorry, I didn't understand that."


def main():
    print("Chatbot: Hello! Type 'bye' to exit.")

    while True:
        user_input = input("You: ")
        reply = get_reply(user_input)
        print("Chatbot:", reply)

        if user_input.lower().strip() == "bye":
            break


main()
