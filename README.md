🎙️ AI Podcast Clipper
Created by Radhika Borigam
🔗 GitHub Repository

🚀 Overview
AI Podcast Clipper is an AI-powered tool that transforms long podcast episodes into engaging short clips—automatically. Built for modern creators, it uses state-of-the-art models to detect viral moments, add subtitles, crop based on active speakers, and export vertical videos ready for TikTok, YouTube Shorts, and more.

No manual editing. No need to scrub through hours of audio. Just upload, sit back, and let the AI do the work.

✨ Features
🎬 AI Viral Moment Detection — Auto-identifies engaging stories, jokes, and questions using Gemini 2.5 Pro

🔊 Auto Subtitles — Adds accurate, synced captions powered by m-bain/whisperX

🧠 Speaker Detection — Uses Junhua-Liao/LR-ASD to track and crop based on active speaker

📱 Vertical Video Output — Optimized for TikTok, Instagram Reels, YouTube Shorts

⚡ Fast Rendering — GPU-accelerated using FFMPEGCV

💻 Responsive UI — Built with Next.js, Tailwind CSS, and Shadcn UI

📊 Queue System — Handles processing flow smoothly using Inngest

👤 User Authentication — Secure sign-up/login with session handling

💳 Credit-Based Access — Integrated credit system with Stripe support

☁️ Serverless GPU Backend — Runs entirely on Modal for simplicity and scale

🎛️ Dashboard Interface — Upload audio/video, track processing, manage clips

🧠 Tech Stack
Layer	Tools/Frameworks
Frontend	Next.js, Tailwind CSS, Shadcn UI
Backend	FastAPI, Modal (GPU), FFMPEGCV
AI Models	Gemini 2.5 Pro, whisperX, LR-ASD
Auth & Billing	Auth system + Stripe for payments
Queue	Inngest

⚙️ Getting Started
1️⃣ Clone the Repository
bash
Copy
Edit
git clone --recurse-submodules https://github.com/Radhika-borigam/ai-podcast-clipper-saas.git
🧩 Backend Setup
🔧 Setup Python Environment (Python 3.12 recommended)
cd ai-podcast-clipper-backend
python -m venv venv
source venv/bin/activate  # Use `venv\Scripts\activate` on Windows
pip install -r requirements.txt
🚀 Modal Setup
modal setup
modal run main.py         # Test run
modal deploy main.py      # Deploy the backend
🎨 Frontend Setup
cd ai-podcast-clipper-frontend
npm install
npm run dev               # Starts on http://localhost:3000
📊 Queue (Inngest)
To run local development server for queue handling:


cd ai-podcast-clipper-frontend
npm run inngest-dev
✅ Summary of Folder Structure
bash
Copy
Edit
ai-podcast-clipper-saas/
├── ai-podcast-clipper-backend/     # FastAPI + Modal (AI + processing logic)
│   └── main.py                     # Modal functions and podcast logic
├── ai-podcast-clipper-frontend/    # Next.js web dashboard
│   ├── pages/                      # Routes and views
│   ├── components/                 # Reusable UI elements
│   ├── inngest/                    # Event-based queue handling
│   └── utils/                      # Helpers (e.g., upload, validation)
└── README.md                       # This file
🧪 Example Workflow
User logs in via the frontend

Uploads a podcast episode (audio/video)

Backend triggers Modal + Inngest

Viral segments are extracted and rendered with subtitles

Final vertical video clips are shown on the dashboard

Download or share directly from the interface

📜 License
Licensed under the MIT License

🙌 Contributions Welcome!
If you’d like to contribute, improve the UI, suggest new features, or fix bugs:

Fork this repo

Create a new branch

Make your changes

Open a pull request 🚀

Let me know if you'd like help creating:

📽️ A video demo script

🧾 A pitch deck description

📄 A Notion-based documentation version

🌐 A landing page in HTML/React

I'm happy to help you make this shine even more!
