# 🤖 AI Gmail Assistant using n8n + Gemini Pro

A smart Gmail automation system that fetches specific emails (like "Hackathon"), summarizes them using **Gemini Pro**, and replies with AI-generated responses — all in a **no-code workflow** built in [n8n](https://n8n.io).

![Demo](./photo.jpeg)

---

## 📌 Features

- 🔍 Search Gmail for specific email content (e.g., "mails related to hackathon")
- 🧠 Summarize email content using Gemini Pro AI
- ✉️ Send AI-generated replies via Gmail
- 🧩 Fully built using n8n workflow automation
- 💸 100% free setup — **no billing info required**

---

## 📹 Demo Video

Watch the working demo here:  
🎥 [Google Drive Folder](https://drive.google.com/drive/folders/1csgF2dCoj_dq6qWLiibObRiZAs0w7U8U?usp=sharing)

---

## ⚙️ Tech Stack

- [n8n](https://n8n.io) – workflow automation tool
- [Google Gemini Pro](https://ai.google.dev/) – for AI summarization & response
- [Gmail API](https://developers.google.com/gmail/api) – for email access and sending
- [OAuth2 + HTTP Request Node] – integrated via n8n credentials

---

## 🧠 AI Prompt Used

This is the system prompt used with Gemini Pro to generate responses:

```
You are an email assistant. Read the Gmail message content provided and:
1. Summarize it concisely.
2. Generate a short, polite, and relevant reply.
3. Mention if the email appears urgent or casual.

Only reply with the summary and the response text, clearly separated.
```

---

## 🚀 How It Works

1. **Trigger**: Starts manually or on schedule
2. **Gmail Search Node**: Searches for specific keywords (e.g., "hackathon")
3. **Extract Content**: Gets subject + body of matching emails
4. **Gemini Pro Node**: Sends the email content to Gemini and receives a summary + reply
5. **Send Gmail Node**: Sends the AI-generated reply email to the original sender

---

## 🛠️ Setup Instructions

1. Clone this repo or download the `README.md` + image
2. Set up an [n8n Cloud](https://n8n.io/) or self-hosted instance
3. Import your workflow into n8n
4. Add the following credentials:
   - **Gmail OAuth2** (for reading/sending mail)
   - **Gemini Pro API Key** (for AI responses)
5. Customize the keyword in the Gmail node (e.g., `"hackathon"`)
6. Run the workflow and enjoy automation!

---



## 💡 Use Cases

- Auto-reply for Hackathon emails
- Internship or Job mail assistant
- Daily summary and triage of unread emails
- Support ticket replies
- Notification analyzer


---

## 📜 License

This project is open-source under the [MIT License](https://opensource.org/licenses/MIT).  
Feel free to fork, remix, and build on it.

---

## 🙋‍♂️ Author

Made with 💡 and automation power by **[Your Name]**  
Let’s connect on [LinkedIn]([https://linkedin.com](https://www.linkedin.com/in/anikesh-kumar-289aaa290))
