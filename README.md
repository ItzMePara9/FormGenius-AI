# ⚡ FormGenius AI

<div align="center">

### ✨ Your AI-Powered Google Forms Builder

**Turn ideas into professional Google Forms with AI.**

Generate, customize, edit, and publish beautiful Google Forms using natural language, Gemini, and OpenAI-compatible models — all from your own self-hosted dashboard.

<br/>

![Version](https://img.shields.io/badge/version-1.0.0-8b5cf6?style=for-the-badge)
![Node.js](https://img.shields.io/badge/Node.js-24.x-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-Enabled-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![License](https://img.shields.io/badge/License-Apache--2.0-blue?style=for-the-badge)

<br/>

**🤖 AI Generation • 📝 Smart Editing • 🔗 Google Forms Integration • 🔒 Self-Hosted**

</div>

---

## 🌟 Overview

**FormGenius AI** is a modern, self-hosted AI-powered Google Forms builder that transforms natural-language instructions into professional, ready-to-publish Google Forms.

Instead of manually creating questions, configuring answer types, and organizing sections, simply describe what you need and let AI do the work.

Whether you're creating job applications, student registrations, customer feedback surveys, event registrations, or employee questionnaires, FormGenius AI makes the entire process faster and easier.

### 💡 How It Works

1. ✍️ Describe the form you want using a natural-language prompt.
2. 🤖 Select your preferred AI model.
3. ⚡ Let AI generate a structured form with questions and sections.
4. 🎨 Preview, customize, and edit your generated form.
5. 💬 Use the AI Copilot to make changes through conversation.
6. 🚀 Publish directly to your connected Google account.
7. 🔗 Get your Google Forms sharing link.

**Your infrastructure. Your AI models. Your Google account. Your control.**

---

## ✨ Features

### 🤖 AI-Powered Form Generation

- Generate complete forms using natural-language prompts.
- Automatically generate relevant questions and descriptions.
- Intelligent question-type selection.
- Automatic section organization.
- Support for multiple languages.
- Customizable form complexity.
- Structured JSON generation with schema validation.

### 🧠 Multi-Provider AI Support

Connect your own AI providers and models.

**Supported integrations:**

- OpenAI-compatible APIs.
- Google AI Studio.
- Gemini models.
- Groq.
- Together AI.
- DeepSeek.
- LocalAI.
- Ollama-compatible endpoints.
- Other compatible providers.

**Model management:**

- Unlimited custom model configurations.
- Custom API Base URLs.
- Custom API keys.
- Custom Model IDs.
- Custom model nicknames.
- Connection testing.
- Default model selection.
- Easy model switching.
- Encrypted API key storage.

### ✨ Google AI Studio Presets

Get started quickly with built-in Gemini model presets.

| Model | Model ID |
|---|---|
| Gemini 2.5 Flash | `gemini-2.5-flash` |
| Gemini 2.5 Pro | `gemini-2.5-pro` |
| Gemini 2.0 Flash | `gemini-2.0-flash` |

Presets are configurable, allowing you to update model IDs as provider availability changes.

### 🔗 Google Forms Integration

Publish generated forms directly to your Google account.

- Google OAuth 2.0 authentication.
- Secure Google account connection.
- Automatic access-token refreshing.
- Google Forms API integration.
- Automatic form creation.
- Question and section publishing.
- Public form URL retrieval.
- Google Form editing URL.
- Connection status management.
- Secure account disconnection.

**No Gmail App Passwords required.**

FormGenius AI uses Google's official authorization system rather than Gmail SMTP credentials.

### 🎨 Interactive Form Editor

Customize your generated forms before publishing.

Supported question types include:

- Short Answer
- Paragraph
- Multiple Choice
- Checkboxes
- Dropdown
- Date
- Time
- Linear Scale
- Rating
- Sections

**Editing capabilities:**

- Add and remove questions.
- Duplicate questions.
- Reorder questions.
- Edit titles and descriptions.
- Change question types.
- Configure answer options.
- Set required questions.
- Organize multiple sections.
- Live form preview.

### 💬 AI Copilot

Modify existing forms using conversational instructions.

Examples:

- "Add a GitHub profile question."
- "Make the phone number mandatory."
- "Create a separate education section."
- "Rewrite all questions professionally."
- "Translate this form into Hindi."
- "Make this application suitable for freshers."

The AI works with your existing form structure instead of unnecessarily rebuilding everything.

### 📚 Templates Library

Get started with professionally structured templates.

Included starter templates:

- Job Application
- Employee Registration
- Customer Feedback
- Event Registration
- Course Registration
- Student Admission
- Contact Form
- Employee Survey
- Internship Application
- Product Feedback
- Website Feedback
- Interview Evaluation
- Workshop Registration

### 🕘 Version History

- Automatic form snapshots.
- Revision tracking.
- Previous version restoration.
- Form duplication.
- Publishing history.

### 🔐 Security & Privacy

Security is a core part of FormGenius AI.

- AES-256-GCM encryption for stored credentials.
- Secure password hashing.
- HTTP-only authentication cookies.
- OAuth state validation.
- Protected API endpoints.
- Input validation with Zod.
- Rate limiting.
- Secure HTTP headers.
- Environment-based secret management.
- No plaintext API keys or OAuth refresh tokens in database storage.

### 🖥️ Self-Hosted Architecture

Run FormGenius AI on your own infrastructure.

- Full administrative control.
- Local database storage.
- Configurable application port.
- Ubuntu VPS compatibility.
- PM2 process management.
- Nginx reverse proxy support.
- HTTPS deployment support.
- No mandatory external SaaS subscription.

---

## 🛠️ Technology Stack

| Component | Technology |
|---|---|
| Runtime | Node.js 24.22.1 |
| Frontend | React 19 |
| Language | TypeScript |
| Build Tool | Vite |
| Styling | Tailwind CSS 4 |
| Backend | Express.js |
| Database | SQLite |
| ORM | Prisma ORM 6 |
| AI SDK | OpenAI SDK |
| Gemini Integration | @google/genai |
| Google Integration | googleapis |
| Validation | Zod |
| Encryption | Node.js Crypto |
| Icons | Lucide |

---

## 📋 Requirements

Before installing FormGenius AI, make sure you have:

- Node.js 24.22.1 or higher.
- npm 10.x or higher.
- Git.
- A Google account.
- An AI provider API key.
- Google Cloud OAuth credentials for publishing forms.

---

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/ItzMePara9/FormGenius-AI.git

cd FormGenius-AI
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create your environment configuration:

```bash
cp .env.example .env
```

Edit the `.env` file:

```env
# Application
PORT=3000
APP_URL=http://localhost:3000

# Database
DATABASE_URL="file:./dev.db"

# Security
APP_SECRET=your-secure-encryption-secret
SESSION_SECRET=your-secure-session-secret

# Optional AI Configuration
GEMINI_API_KEY=
OPENAI_API_KEY=

# Google OAuth
GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=
GOOGLE_REDIRECT_URI=http://localhost:3000/api/google/callback
```

**Important:** Generate strong, unique production secrets. Never commit your `.env` file or share your credentials.

### 4. Initialize the Database

```bash
npm run prisma:push
```

### 5. Start the Application

```bash
npm run dev
```

Open the application:

**http://localhost:3000**

On the first launch, FormGenius AI will guide you through the administrator setup wizard.

---

## ☁️ Google Cloud OAuth Setup

To publish forms directly to your Google account, configure Google OAuth.

### Step 1 — Create a Google Cloud Project

Visit:

https://console.cloud.google.com/

Create a project named **FormGenius AI**.

### Step 2 — Enable APIs

Navigate to APIs & Services → Library.

Enable:

- Google Forms API
- Google Drive API

### Step 3 — Configure OAuth Consent

Navigate to Google Auth Platform and configure your OAuth consent screen.

Configure the required application information and add the necessary scopes:

```text
https://www.googleapis.com/auth/forms.body

https://www.googleapis.com/auth/drive.file

https://www.googleapis.com/auth/userinfo.email
```

### Step 4 — Create OAuth Credentials

Navigate to:

APIs & Services → Credentials → Create Credentials → OAuth Client ID.

Select:

**Application Type:** Web Application

Add your authorized redirect URI:

```text
https://forms.yourdomain.com/api/google/callback
```

For local development:

```text
http://localhost:3000/api/google/callback
```

### Step 5 — Connect Your Account

Copy your Google Client ID and Client Secret into FormGenius AI's Google integration settings.

Then click **Connect Google Account** and complete Google's authorization process.

> Note: Google OAuth applications in testing mode may require test-user configuration. Production use may require additional Google verification depending on the requested scopes and publishing setup.

---

## 🤖 AI Model Configuration

FormGenius AI allows you to configure your own AI providers.

Example OpenAI-compatible configuration:

| Setting | Example |
|---|---|
| Provider Name | My OpenAI |
| Base URL | `https://api.openai.com/v1` |
| API Key | Your API Key |
| Model ID | `gpt-4o` |
| Model Nickname | Form Creator Pro |

You can also configure Gemini through Google AI Studio.

Get your API key:

https://aistudio.google.com/apikey

All configured credentials should be encrypted before being stored.

---

## 🖥️ Production Deployment — Ubuntu VPS

### Step 1 — Install Node.js 24

```bash
curl -fsSL https://deb.nodesource.com/setup_24.x | sudo -E bash -

sudo apt-get update

sudo apt-get install -y nodejs git build-essential
```

Verify installation:

```bash
node -v
npm -v
```

### Step 2 — Clone the Project

```bash
sudo mkdir -p /var/www/formgenius

sudo chown -R $USER:$USER /var/www/formgenius

git clone https://github.com/ItzMePara9/FormGenius-AI.git /var/www/formgenius

cd /var/www/formgenius
```

### Step 3 — Configure Environment

```bash
npm install

cp .env.example .env

nano .env
```

Configure your production URL, database, and secure secrets.

### Step 4 — Initialize Database and Build

```bash
npm run prisma:push

npm run build
```

### Step 5 — Install PM2

```bash
sudo npm install -g pm2
```

Start FormGenius AI:

```bash
pm2 start npm --name formgenius -- start

pm2 save

pm2 startup
```

Check application status:

```bash
pm2 status
```

View logs:

```bash
pm2 logs formgenius
```

### Step 6 — Nginx Configuration

Create a configuration file:

```bash
sudo nano /etc/nginx/sites-available/formgenius
```

Add:

```nginx
server {
    listen 80;
    server_name forms.yourdomain.com;

    location / {
        proxy_pass http://127.0.0.1:3000;

        proxy_http_version 1.1;

        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
    }
}
```

Enable the configuration:

```bash
sudo ln -s /etc/nginx/sites-available/formgenius /etc/nginx/sites-enabled/

sudo nginx -t

sudo systemctl reload nginx
```

### Step 7 — Configure SSL

Install Certbot:

```bash
sudo apt install -y certbot python3-certbot-nginx
```

Generate your SSL certificate:

```bash
sudo certbot --nginx -d forms.yourdomain.com
```

Your application should now be accessible through HTTPS.

---

## ⚙️ Useful Commands

| Command | Description |
|---|---|
| `npm install` | Install dependencies |
| `npm run dev` | Start development server |
| `npm run build` | Build production frontend |
| `npm start` | Start production server |
| `npm run prisma:push` | Synchronize database schema |
| `npm run prisma:studio` | Open Prisma Studio |

*Commands depend on the scripts defined in the project package.json.*

---

## 🔒 Security Notes

- Never expose API keys in frontend code.
- Never commit `.env` files.
- Always use HTTPS in production.
- Keep encryption secrets secure.
- Use trusted AI providers.
- Review Google OAuth permissions before connecting.
- Regularly back up your database and encryption keys.

**Important:** Losing the encryption key may make previously stored credentials unrecoverable.

---

## 🗺️ Roadmap

- [x] Project concept and architecture
- [x] AI provider architecture planning
- [x] Google OAuth integration design
- [x] Form generation workflow design
- [ ] Complete authentication system
- [ ] AI model management
- [ ] Gemini presets
- [ ] Google account connection
- [ ] AI form generation
- [ ] Interactive form editor
- [ ] AI Copilot
- [ ] Google Forms publishing
- [ ] Template library
- [ ] Version history
- [ ] Production deployment testing

---

## 🤝 Contributing

Contributions, ideas, suggestions, and bug reports are welcome!

1. Fork the repository.
2. Create a feature branch.
3. Implement your changes.
4. Test your changes.
5. Submit a pull request.

For major changes, open an issue first to discuss your proposal.

---

## 📜 License

FormGenius AI is licensed under the **Apache License 2.0**.

You are free to use, modify, distribute, and build upon this project under the terms of the license.

See [LICENSE](LICENSE) for more information.

---

<div align="center">

### ⚡ FormGenius AI

**Stop building forms manually. Start building with AI.**

Made with ❤️ by **Para**

[GitHub](https://github.com/ItzMePara9) · [Repository](https://github.com/ItzMePara9/FormGenius-AI)

⭐ If you like this project, consider giving it a star!

</div>
