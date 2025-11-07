# Resume-agentic-ai

## 📋 Overview

**Agentic Career Copilot** is a revolutionary multi-agent AI system that transforms the job search experience into an autonomous, intelligent workflow. Built on the principle of **Perceive → Decide → Act → Learn**, this SaaS application manages everything from resume creation to interview scheduling without requiring constant user intervention.

### 🎯 Why Agentic Career Copilot?

Traditional job search is time-consuming and repetitive. Our agentic AI system:
- ✅ **Automates** the entire job application process
- 🎯 **Optimizes** your resume for each job using ATS scoring
- 🤖 **Communicates** with recruiters on your behalf
- 📅 **Schedules** interviews automatically
- 📈 **Learns** continuously from outcomes to improve results
- 🔒 **Protects** your privacy with ethical AI practices

---

## 🌟 Key Features

### 🧾 Resume Intelligence
| Agent | Description |
|-------|-------------|
| **Automatic Resume Builder** | Creates and formats personalized resumes for different job types |
| **ATS Scoring System** | Evaluates resumes against job descriptions (0-100 score) |
| **Real-Time Scorer** | Live ATS score updates as you edit your resume |
| **Enhancement Assistant** | Suggests improvements using hiring trend data |
| **Dynamic Variant Creator** | Generates multiple role-specific resume versions |
| **Trend-Based Enhancer** | Adds emerging skills and keywords automatically |

### 💼 Job Discovery & Application
- **Job Recommendation Engine**: Scans LinkedIn, Indeed, Naukri, and ranks jobs by match quality
- **Portal Integrator**: Real-time job fetching from multiple platforms
- **Autonomous Application Agent**: Applies to jobs on your behalf (with consent)
- **Cover Letter Generator**: Creates personalized cover letters for each application
- **Privacy Manager**: Ensures GDPR-compliant, ethical AI operations

### 📧 Recruiter Communication
- **Smart Communication Agent**: Composes and sends professional emails automatically
- **Follow-Up Agent**: Sends polite follow-ups after 3-5 days of no response
- **Interview Scheduler**: Syncs with Google/Outlook Calendar for automatic booking

### 🔗 Profile Optimization
- **LinkedIn Optimizer**: Suggests headline, summary, and skill improvements
- **Auto-Updater**: Keeps LinkedIn profile in sync with resume changes

### 🧠 Career Intelligence
- **Career Path Predictor**: Recommends next career moves based on market trends
- **Skill Gap Analyzer**: Identifies missing skills for target roles
- **Auto-Learning Scheduler**: Books learning sessions in your calendar
- **Interview Prep Bot**: Generates role-specific interview questions

---

## 🏗️ System Architecture

### Agentic Workflow
```
┌─────────────────────────────────────────────────────────────────┐
│                    USER INITIALIZATION                          │
│              (Upload Resume / Set Career Goals)                 │
└──────────────────────────┬──────────────────────────────────────┘
                           │
                           ▼
┌─────────────────────────────────────────────────────────────────┐
│  PERCEPTION LAYER: Career Path Predictor & Skill Gap Analyzer  │
└──────────────────────────┬──────────────────────────────────────┘
                           │
                           ▼
┌─────────────────────────────────────────────────────────────────┐
│     DECISION LAYER: Resume Builder & ATS Optimization Agent    │
└──────────────────────────┬──────────────────────────────────────┘
                           │
                           ▼
┌─────────────────────────────────────────────────────────────────┐
│    ACTION LAYER: Job Discovery → Application → Communication   │
└──────────────────────────┬──────────────────────────────────────┘
                           │
                           ▼
┌─────────────────────────────────────────────────────────────────┐
│  LEARNING LAYER: Feedback Analysis & Continuous Improvement    │
└──────────────────────────┬──────────────────────────────────────┘
                           │
                           ▼ (Loop Back)
```

### Multi-Agent Coordination

Our system uses **orchestrated agent collaboration** where specialized AI agents work together:

1. **Coordinator Agent**: Manages overall workflow and agent communication
2. **Resume Agents**: Build, score, and optimize resumes
3. **Job Agents**: Discover, filter, and apply to positions
4. **Communication Agents**: Handle recruiter interactions
5. **Learning Agents**: Analyze outcomes and improve strategies

---

## 🛠️ Tech Stack

### Frontend
- **React.js** - UI framework
- **Next.js** - Server-side rendering & routing
- **TailwindCSS** - Utility-first styling
- **Shadcn/ui** - Component library

### Backend
- **Python** - Core backend language
- **FastAPI** - High-performance API framework
- **PostgreSQL** - Primary database
- **Redis** - Caching & session management

### AI & ML
- **GPT-4** - Language understanding & generation
- **Claude** - Complex reasoning tasks
- **LangChain** - Agent orchestration framework
- **CrewAI** - Multi-agent coordination
- **OpenAI Embeddings** - Semantic search

### Integrations
- **LinkedIn API** - Profile optimization & job scraping
- **Indeed API** - Job listings
- **Naukri API** - Indian job market
- **Gmail API** - Email automation
- **Google Calendar API** - Interview scheduling
- **Outlook Calendar API** - Alternative scheduling

### DevOps
- **Docker** - Containerization
- **GitHub Actions** - CI/CD
- **AWS/Vercel** - Cloud hosting

---

## 🚀 Installation

### Prerequisites
```bash
node >= 18.0.0
python >= 3.10
postgresql >= 14
redis >= 6.0
```

### 1. Clone the Repository
```bash
git clone https://github.com/AnujS394/Resume-agentic-ai.git
cd Resume-agentic-ai
```

### 2. Backend Setup
```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

Create `.env` file:
```env
# AI API Keys
OPENAI_API_KEY=your_openai_key
ANTHROPIC_API_KEY=your_anthropic_key

# Database
DATABASE_URL=postgresql://user:password@localhost:5432/career_copilot
REDIS_URL=redis://localhost:6379

# Integration APIs
LINKEDIN_CLIENT_ID=your_linkedin_id
LINKEDIN_CLIENT_SECRET=your_linkedin_secret
GMAIL_CLIENT_ID=your_gmail_id
GMAIL_CLIENT_SECRET=your_gmail_secret
GOOGLE_CALENDAR_API_KEY=your_calendar_key

# Job Portals
INDEED_API_KEY=your_indeed_key
NAUKRI_API_KEY=your_naukri_key
```

Run migrations:
```bash
alembic upgrade head
```

Start backend:
```bash
uvicorn main:app --reload
```

### 3. Frontend Setup
```bash
cd ../frontend
npm install
```

Create `.env.local`:
```env
NEXT_PUBLIC_API_URL=http://localhost:8000
NEXT_PUBLIC_APP_URL=http://localhost:3000
```

Start frontend:
```bash
npm run dev
```

---

## 📖 Usage

### 1. Initial Setup
```bash
# Visit http://localhost:3000
# Create account or sign in
# Upload existing resume or create new one
```

### 2. Configure Preferences
- Set target job roles
- Define salary expectations
- Choose job locations
- Set application frequency (daily/weekly)

### 3. Activate Agents
```bash
# Enable autonomous mode
✅ Auto-apply to jobs
✅ Auto-respond to recruiters
✅ Auto-schedule interviews
```

### 4. Monitor Dashboard
- View ATS scores
- Track applications sent
- See recruiter responses
- Check upcoming interviews

### 5. Continuous Improvement
The system learns from:
- Interview outcomes
- Recruiter response rates
- Job offer conversions
- Resume performance metrics

---

## 🧪 API Documentation

### Resume Endpoints
```http
POST   /api/v1/resume/create        # Create new resume
GET    /api/v1/resume/{id}          # Get resume
PUT    /api/v1/resume/{id}          # Update resume
POST   /api/v1/resume/{id}/score    # Get ATS score
GET    /api/v1/resume/{id}/variants # Get all variants
```

### Job Endpoints
```http
GET    /api/v1/jobs/search          # Search jobs
POST   /api/v1/jobs/apply           # Apply to job
GET    /api/v1/jobs/applications    # Get user applications
```

### Agent Endpoints
```http
POST   /api/v1/agents/trigger       # Manually trigger agent
GET    /api/v1/agents/status        # Get agent status
PUT    /api/v1/agents/config        # Update agent settings
```

Full API documentation: `http://localhost:8000/docs`

---

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines
- Follow PEP 8 for Python code
- Use ESLint for JavaScript/React
- Write unit tests for new features
- Update documentation

