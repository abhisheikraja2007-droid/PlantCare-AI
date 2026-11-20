# PlantCare AI - Intelligent Botanical Health & Diagnostic Assistant

An intelligent, full-stack plant health diagnostic and maintenance platform powered by the Google Gemini API, Express, Vite, React, and TypeScript. PlantCare AI acts as an always-on digital agronomist and botanical doctor, combining multimodal computer vision diagnosis with predictive watering and soil telemetry schedules.

---

## Key Features

- **Gemini Multimodal Leaf Diagnostics:** Upload or capture leaf photos to identify leaf scorch, nitrogen deficiency, spider mites, fungal infections, and root rot with structured remedy plans.
- **Interactive Plant Doctor Chat:** Conversational botanical AI with contextual memory of individual plants, watering histories, and species requirements.
- **Smart Hydration & Environment Tracking:** Adaptive watering reminders based on species, ambient temperature, humidity, and pot size.
- **High-Performance Architecture:** Express API bridge with `@google/genai` SDK and React 18 frontend bundled via Vite with Tailwind CSS.
- **Containerized Deployment:** Ready-to-run `docker-compose.yml` for unified frontend and backend deployment.

---

## Tech Stack

- **Frontend:** React 18, TypeScript, Tailwind CSS, Lucide Icons, Vite
- **Backend:** Node.js, Express, `@google/genai` (Gemini 1.5 / 2.0 Flash)
- **Containerization:** Docker, Docker Compose
- **Tooling:** Bun / npm, ESLint, TypeScript Compiler

---

## Getting Started

### Prerequisites

- Node.js (v18+) or Bun
- Google Gemini API Key ([Google AI Studio](https://aistudio.google.com/))

### Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/abhisheikraja2007-droid/PlantCare-AI.git
   cd PlantCare-AI
   ```

2. **Configure Environment Variables:**
   ```bash
   cp .env.example .env.local
   ```
   Set your API credentials in `.env.local`:
   ```env
   GEMINI_API_KEY=your_gemini_api_key_here
   PORT=3000
   ```

3. **Install Dependencies:**
   ```bash
   npm install
   ```

4. **Launch Development Server:**
   ```bash
   npm run dev
   ```
   Open `http://localhost:3000` in your browser.

---

## Docker Deployment

Run the complete application inside Docker containers:

```bash
docker compose up -d --build
```

---

## API Endpoints

- `GET /api/health` - Server health status and timestamp.
- `POST /api/gemini/doctor` - Context-aware botanical diagnostic chat.
- `POST /api/gemini/diagnose-image` - Multimodal image classification and pathology report.

---

## License

This project is licensed under the MIT License.
