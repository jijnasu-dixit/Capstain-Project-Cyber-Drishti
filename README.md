# Cyber Drishti 👁️

**An anonymous platform for sharing and learning from real-world cyber incident stories.**

This project provides a safe space for victims of cybercrime to anonymously share their experiences. A guided AI chatbot helps them structure their story, which is then anonymized and shared with the community to help prevent others from falling for the same tactics.

![Project visual showing the concept of shedding light on unreported cybercrime](httpss://storage.googleapis.com/gemini-prod-images/652f1e29e830e201b1a329c29013532c)

---

## 🚀 The Problem

Cybercrime is a massive, multi-trillion dollar problem, but an estimated **85% of incidents go unreported** (source: U.S. Dept. of Justice).

Victims often remain silent due to:
* **Shame or embarrassment**
* **Fear of being blamed**
* **Believing authorities can't or won't help**
* **Not knowing where to turn**

This silence creates a critical "awareness gap" that allows attackers to reuse the same tactics successfully.

## 💡 The Solution: Cyber Drishti

**Cyber Drishti** (meaning "Cyber Vision") provides a 100% anonymous, safe, and simple platform to bridge this gap.

1.  **AI-Guided Sharing:** An empathetic AI chatbot gently guides a user to detail their experience.
2.  **Anonymous Story Generation:** The conversation is transformed into an anonymized, easy-to-read narrative (title, category, and story).
3.  **Community Learning:** The user reviews and posts their anonymous story, which then appears on a public feed to educate and empower the entire community.

---

## ✨ Key Features

* **AI Chatbot:** A conversational UI (powered by the Google Gemini API) helps users share their story naturally.
* **Anonymized Story Generation:** The AI summarizes the chat into a clean, first-person story, stripping any potential identifying information.
* **Community Story Feed:** A real-time, browsable feed of all incidents, filterable by category.
* **Anonymous Authentication:** Users are authenticated anonymously via Firebase, ensuring their identity is never known.
* **Fully Responsive:** A clean, modal-based UI that works on both desktop and mobile.

---

## 🛠️ Tech Stack

This project is a powerful single-page application built with modern, lightweight technologies.

* **Frontend:** **Vue.js 3** (loaded via CDN)
* **Styling:** **Tailwind CSS** (loaded via CDN)
* **Backend & Database:** **Firebase** (Firestore Database & Anonymous Authentication)
* **Generative AI:** **Google Gemini API** (for both the chatbot and the story generation)

---

## 📖 How It Works: The User Flow

1.  A user visits the site and can read all "Latest Reports" from the community.
2.  The user clicks **"Share Your Story"**.
3.  A chat modal opens. The user is anonymously authenticated in the background.
4.  The user talks to the AI, explaining what happened.
5.  When the conversation is complete (either by the AI detecting an end or the user clicking), the user is taken to a "Review" screen.
6.  The AI generates a `title`, `category`, and `story` for the user to review.
7.  If satisfied, the user clicks **"Post Anonymously"**.
8.  The story is saved to the Firestore database and instantly appears on the main feed for all other users to see.

---

## ⚙️ Local Setup and Installation

To run this project, you only need this `index.html` file and the credentials from Firebase and Google.

### Step 1: Clone the Project
```bash
git clone [https://your-repo-url.com/cyber-drishti.git](https://your-repo-url.com/cyber-drishti.git)
cd cyber-drishti
