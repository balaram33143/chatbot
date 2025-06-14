## 💬 Sample Chatbot Code (Python)

Below is a simple chatbot using `nltk.chat.util`:

```python
from nltk.chat.util import Chat, reflections

pairs = [
    ["hi|hello", ["Hello!", "Hi there!"]],
    ["what is your name ?", ["I am your chatbot."]],
    ["how are you ?", ["I'm good, thank you!"]],
    ["bye", ["Goodbye!", "See you later!"]],
    ["(.*)", ["I'm not sure I understand that."]]
]

def start_chat():
    print("Hi! I am PyBot. Type 'quit' to exit.")
    chat = Chat(pairs, reflections)
    chat.converse()

start_chat()
