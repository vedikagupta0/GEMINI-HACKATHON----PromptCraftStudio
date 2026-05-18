# 🪄 PromptCraft Studio
**Built for the Gemma 4 Hackathon on Kaggle**

## 🌟 The Vision: Curing "Blank Page Syndrome"
Have you ever stared at an AI chat interface and suddenly forgotten exactly what you wanted to say? For neurodivergent individuals, people with ADHD, or anyone experiencing cognitive fatigue or anxiety, articulating a complex creative or technical thought from scratch can be deeply overwhelming. 

**PromptCraft Studio** is designed to completely eliminate the anxiety of the blank text box. Instead of forcing users to meticulously type out every detail of their vision, PromptCraft provides a structured, stress-free, and inspiring atmosphere. By simply typing a vague or brief idea, users can leverage the power of **Gemma 4** to automatically suggest relevant categories, stylistic modifiers, technical constraints, and even auto-expand their core intent into a beautifully detailed prompt. It transforms prompt engineering from a stressful typing exercise into an intuitive, visual, and highly accessible *building* process.

## 🚀 How It Works
PromptCraft Studio is a privacy-first, locally-hosted application that runs directly in your browser and interfaces with Ollama.

1. **Select Your Mode**: Choose between Image Generation, Text Writing, or Code Generation workspaces.
2. **State Your Intent**: Type a basic, rough idea into the prompt box (e.g., "a futuristic city" or "a python auth system").
3. **Let Gemma 4 Do the Heavy Lifting**: 
   - Select **"Generate Prompt"** to have Gemma auto-fill your core subject with a highly detailed, expansive 2-3 sentence foundation.
   - Select **"3 / cat"** to have Gemma dynamically generate tailored modifier chips across various categories (e.g., Lighting, Vibe, Frameworks, Architecture).
4. **Click to Build**: Browse the AI's suggestions and simply click the cards that match the vibe you were struggling to articulate. They instantly snap into your final prompt layout.
5. **Copy & Create**: Once your prompt is fully assembled, copy it with one click and use it in your favorite generation tools.

## 🧠 Relevance for the Gemma 4 Hackathon
This project serves as a perfect showcase for the unique strengths of the **Gemma 4** model:
- **Local & Private Accessibility**: By running via Ollama, it demonstrates Gemma 4's ability to run powerfully on consumer hardware without compromising user data, making AI accessible and safe.
- **Structured JSON Adherence**: The backend strictly forces Gemma 4 to output highly complex, multi-layered JSON structures on the fly, proving the model's exceptional instruction-following and formatting capabilities.
- **Contextual Awareness**: Gemma 4 actively analyzes the user's current prompt context and selected chips to ensure that its suggestions are hyper-relevant, non-repetitive, and never generic.

## 🛠️ Setup & Installation
1. Install [Ollama](https://ollama.com/) on your local machine.
2. Start the Ollama server with cross-origin requests enabled so the browser application can communicate with it:
   - **Windows (PowerShell)**: `$env:OLLAMA_ORIGINS="*"; ollama serve`
   - **Mac/Linux**: `OLLAMA_ORIGINS="*" ollama serve`
3. Ensure you have the `gemma4` model pulled locally (`ollama pull gemma4`).
4. Simply open `index.html` in your web browser. No complex build steps or external dependencies are required!
