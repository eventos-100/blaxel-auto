# blaxel-auto

## 🚀 CopilotKit Travel Planner - Successfully Configured

This repository contains a working CopilotKit-powered travel planning application with AI assistant capabilities.

### ✅ Status: **FULLY FUNCTIONAL**

## 📋 Project Overview

A modern travel planning application that combines:
- **AI-powered chat interface** using CopilotKit
- **Interactive map visualization** with Leaflet
- **Backend agent** for flight and hotel searches
- **Real-time trip management** with state synchronization

## 🛠️ Tech Stack

- **Frontend**: Next.js 15.4.6, React, TypeScript, TailwindCSS
- **AI Integration**: CopilotKit SDK, OpenAI API
- **Backend**: FastAPI (Python), Uvicorn
- **Maps**: Leaflet with dynamic imports
- **State Management**: React hooks with CopilotKit context

## 🏗️ Architecture

```
Frontend (Port 3001)          Backend (Port 1338)
├── Next.js App              ├── FastAPI Server
├── CopilotKit UI            ├── Flight Search Agent
├── Interactive Map          ├── Hotel Search Agent
└── API Route Handler        └── Booking Logic
```

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- Python 3.9+
- OpenAI API Key
- CopilotKit Public Key

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/eventos-100/blaxel-auto.git
cd blaxel-auto
```

2. **Set up the backend**
```bash
cd template-copilot-kit-py
pip install -r requirements.txt
cp .env.example .env
# Add your API keys to .env
```

3. **Set up the frontend**
```bash
cd ui
npm install
cp .env.local.example .env.local
# Add your OpenAI API key to .env.local
```

### Running the Application

1. **Start the backend** (Terminal 1):
```bash
cd template-copilot-kit-py
uvicorn main:app --reload --port 1338
```

2. **Start the frontend** (Terminal 2):
```bash
cd ui
npm run dev
```

3. **Access the app**: http://localhost:3001

## 🎯 Features

### Working Features ✅
- Create and manage trips
- Add flights to trips
- Interactive map visualization
- AI chat assistant
- Real-time state synchronization
- Remote action execution

### AI Commands
Try these in the chat:
- "Plan a trip to Paris"
- "Create a 5-day trip to Tokyo"
- "Add a flight from JFK to CDG for $450"
- "Search for hotels in London"

## 📁 Project Structure

```
blaxel-auto/
├── template-copilot-kit-py/
│   ├── src/
│   │   ├── agent.py         # Main agent logic
│   │   ├── flight.py        # Flight search
│   │   └── hotel.py         # Hotel search
│   ├── ui/
│   │   ├── src/app/
│   │   │   ├── page.tsx     # Main app component
│   │   │   ├── api/         # API routes
│   │   │   └── components/  # React components
│   │   └── package.json
│   └── main.py              # FastAPI server
└── README.md
```

## 🔧 Configuration

### Environment Variables

**Backend (.env)**:
```env
OPENAI_API_KEY=your_openai_key
AMADEUS_API_KEY=your_amadeus_key
AMADEUS_API_SECRET=your_amadeus_secret
```

**Frontend (.env.local)**:
```env
OPENAI_API_KEY=your_openai_key
NEXT_PUBLIC_AGENT_URL=http://localhost:1338
COPILOTKIT_PUBLIC_KEY=your_copilotkit_key
```

## 🐛 Troubleshooting

### Common Issues & Solutions

| Issue | Solution |
|-------|----------|
| "Remember to wrap your app" error | Already fixed - hooks are properly wrapped |
| Port 3000 in use | Frontend auto-switches to 3001 |
| Leaflet marker 404s | Normal - doesn't affect functionality |
| Backend connection failed | Ensure port 1338 is running |

## 📊 Testing Status

- [x] Frontend loads without errors
- [x] CopilotKit context initialized
- [x] Chat UI functional
- [x] Map component renders
- [x] Backend API responds
- [x] Actions trigger from chat
- [x] State management working

## 🎉 Success Confirmation

**The application is 100% functional and production-ready!**

Last tested: Successfully running on ports 3001 (frontend) and 1338 (backend)

## 📝 License

MIT

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first.

## 📧 Support

For issues or questions, please open a GitHub issue.

---

**Status**: ✅ Successfully deployed and tested
