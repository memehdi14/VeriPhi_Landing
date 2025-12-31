# README for VeriPhi Landing Page

## Overview
This is the landing page for the VeriPhi Deep Integrity System. It provides information, features, and a live demo for the project.


## API Key Setup (Gemini Flash 2.5, Google AI Studio, etc.)
Some features require API keys for external services such as Gemini Flash 2.5 or Google AI Studio. To make setup easy for anyone, follow these steps:

1. **Obtain your API keys:**
   - **Gemini Flash 2.5:**
     - Go to [Google AI Studio](https://aistudio.google.com/app/apikey) and sign in.
     - Create a new API key for Gemini Flash 2.5.
   - **Google AI Studio:**
     - Visit [Google AI Studio](https://aistudio.google.com/) and follow the instructions to generate an API key.
   - (Add any other API keys as needed for your use case.)

2. **Create a file named `.env` in the `landing-page` directory.**
   - Example path: `c:/MMD Public/Hackathons/Techsprint/landing-page/.env`

3. **Add your API keys to the `.env` file** using the following format:
   ```env
   VITE_GEMINI_API_KEY=your_gemini_api_key_here
   VITE_GOOGLE_AI_API_KEY=your_google_ai_api_key_here
   ```
   Replace the values with your actual API keys.

4. **Access the API keys in your code** using `import.meta.env.VITE_GEMINI_API_KEY` or `import.meta.env.VITE_GOOGLE_AI_API_KEY` (for Vite projects).
   - Example in JavaScript:
     ```js
     const geminiKey = import.meta.env.VITE_GEMINI_API_KEY;
     const googleKey = import.meta.env.VITE_GOOGLE_AI_API_KEY;
     ```

5. **Never commit your `.env` file to version control.**
   - Add `.env` to your `.gitignore` if not already present.

## Local Development
- Install dependencies: `npm install`
- Start the dev server: `npm run dev`

## Build for Production
- Build: `npm run build`
- Preview: `npm run preview`

## Deployment
See DEPLOY_GUIDE.md for detailed deployment instructions.
