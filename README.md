# AIUI - Unified AI Frontend

AIUI is a modern, full-featured frontend UI for interacting with AI models. It supports local models through Ollama, cloud-based LLMs via Groq, and Google's Gemini API. Perfect for developers and users who want a flexible, open-source interface to experiment with different AI models.

## Preview

![AIUI chat interface](images/pic3.jpeg)

## Features
- **Multi-Model Support**: Seamlessly switch between Ollama (local models), Groq (Llama 3), and Google Gemini APIs.
- **Local & Cloud Models**: Run models locally with Ollama or use cloud APIs—your choice.
- **Session Persistence**: Chat history is saved for authenticated users and guest sessions.
- **User Profiles & Customization**: Login, customize profiles, change backgrounds, organize with tags, and get contextual suggestions.
- **Modern Tech Stack**: Next.js App Router, TypeScript, Tailwind CSS, Prisma, Groq SDK, and Google Generative AI SDK.
- **Guest & User Modes**: Start chatting immediately as a guest, then sign in to sync your history.

## Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/SapiOwO/AIUI.git
cd AIUI
```

### 2. Install Dependencies
Make sure you have Node.js installed.
```bash
npm install
```

### 3. Set Up Environment Variables (Optional)
To use cloud APIs, create a `.env.local` file in the root directory. If you only want to use local Ollama models, you can skip this step.

```env
GROQ_API_KEY=your_groq_key_here
GEMINI_API_KEY=your_gemini_key_here
```

### 4. Configure Ollama (Optional)
If you want to use local Ollama models:
1. Download and install [Ollama](https://ollama.ai/)
2. Start the Ollama service (it runs on `http://127.0.0.1:11434` by default)
3. Pull your desired models: `ollama pull llama2`, `ollama pull mistral`, etc.

### 5. Run the Development Server
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to start chatting.

### 6. Optional Checks
```bash
npm run lint
npm run build
```

## Use Cases

AIUI can be used for a wide range of applications:
- **Local AI Development**: Test and experiment with Ollama models without cloud dependencies.
- **Research & Learning**: Compare different models side-by-side with an intuitive UI.
- **Content Creation**: Use AI as a writing assistant, brainstorm partner, or idea generator.
- **Problem Solving**: Get assistance with coding, math, analysis, and more.
- **Custom Applications**: Fork the repo and customize the UI for your specific AI use case.

## Customization

AIUI is built to be customizable:
- Modify `/src/components/` to change the UI and user experience.
- Update `/src/app/` to add new API routes or features.
- Adjust system prompts and model settings in `/src/lib/` utilities.
- Use the database schema (`/prisma/schema.prisma`) to extend user data and session tracking.

## Architecture

- **Frontend**: Next.js with React, TypeScript, and Tailwind CSS for a responsive, modern UI.
- **Backend**: API routes for session management, authentication, and model orchestration.
- **Database**: Prisma ORM with support for PostgreSQL, MySQL, and other databases.
- **Model Support**: Ollama (local), Groq APIs (Llama 3), and Google Generative AI (Gemini).

## License

[Check the LICENSE file for licensing details.]
