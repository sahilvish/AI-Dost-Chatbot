# 🤖 AI Dost: A Persistent Personalized Chatbot

**AI Dost** is a sophisticated AI companion designed to provide a human-like, supportive interaction experience. Built using Python and powered by the Mistral AI (mistral-small) model, this project bridges the gap between cold machine responses and friendly, personalized conversations.

## ✨ Key Features

* **🗣️ Natural Hinglish Interaction:** Expertly handles mixed Hindi and English inputs for a culturally relevant, "desi" conversational feel.
* **🧠 Persistent Memory:** Integrates with Google Drive and JSON file handling to ensure the AI remembers past interactions, user preferences, and personal details across sessions.
* **⏰ Contextual Awareness:** Features dynamic greeting logic that adjusts based on the time of day (IST), making the interaction feel timely and personal.
* **👤 Deep Personalization:** Remembers user identity (e.g., "Sahil bhai") and adapts its tone to be supportive and engaging.
* **📂 Cloud-Native Architecture:** Optimized for Google Colab with seamless data synchronization to Google Drive.

## 🛠️ Tech Stack

* **Language:** Python 3.x
* **AI Model:** Mistral AI API
* **Environment:** Google Colab
* **Data Storage:** Google Drive (JSON Persistence)
* **Libraries:** `mistralai`, `pytz`, `datetime`, `json`, `os`

## 🚀 How It Works

1. **Drive Synchronization:** The system mounts Google Drive to access `chat_memory.json`, which stores the conversation history.
2. **Temporal Logic:** Uses `pytz` and `datetime` to determine the user's local time and generate appropriate greetings.
3. **Inference Loop:** Processes user input through the Mistral API with custom system prompts to maintain a "friend-like" persona.
4. **Auto-Persistence:** Every exchange is automatically serialized back to the JSON file, ensuring no data loss if the session disconnects.

## 📝 Setup & Usage

1. **API Key:** Obtain your API key from the Mistral AI console.
2. **Colab Setup:** Open the provided `.ipynb` file in Google Colab.
3. **Authorization:** Run the drive mount cell to link your storage.
4. **Initialization:** Replace the placeholder API key with your own and start the conversation.

---
**Developed with ❤️ by Sahil**
