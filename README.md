# Ava – Autism Skill Companion

## Overview
Ava is an interactive, AI-driven application tailored to help young children with Autism Spectrum Disorder (ASD) develop life skills such as speech, behavioral awareness, social-emotional learning, and potty-training. It provides personalized, engaging interactions for children aged 2-5, creating a safe and playful learning environment.

## Goals and Objectives
### Core Developmental Goals
- Improve conversational skills and expand vocabulary
- Enhance behavioral and social skills through emotional awareness and social cue recognition
- Facilitate effective potty training routines
- Provide continuous and adaptive positive reinforcement

### Application Objectives
- Deliver interactive experiences that keep children engaged
- Personalize AI interactions for autism spectrum developmental needs
- Offer clear and positive reinforcement with visual and auditory rewards
- Enable parental oversight and progress tracking through a dashboard

## User Experience and Interface
### Child-Focused UI/UX Design
- **Simple navigation** with large, colorful buttons and minimal text
- **Interactive characters**: Ava guides each interaction
- **Animated rewards** such as digital stickers and cheerful sounds

### Parent Dashboard
- Visual summaries of skill development
- Customization options for potty reminders, session length, and skill targets
- Clearly defined data privacy and security controls

## App Structure and Modules
| Section              | Description                                                |
|----------------------|------------------------------------------------------------|
| Home Screen          | Friendly greeting from Ava with simple module selection    |
| Speech & Conversation| Picture and prompt-based conversational activities        |
| Emotions & Social    | Games identifying emotions and social scenarios            |
| Potty Training       | Timely reminders, interactive routines, and reward system  |
| Play Zone            | Free-play interaction with Ava                             |

## AI Integration & Behavior
- **Compassionate & patient** personality
- **Adaptability** based on the child’s progress
- **Playful tone** with games, stories, and visuals

### AI Model & Framework
- Early training via Hugging Face models
- Main integration with OpenAI GPT models
- LangChain for managing interactions and conversational memory

## Technical Architecture
### Frontend
- Next.js framework
- Tailwind CSS and Shadcn/ui components for responsive design
- Framer Motion for subtle animations

### Backend
- Python 3.12 with FastAPI
- Handles interactions, logging, and session management
- Communicates with AI models through LangChain
- Secure RESTful API

### AI and ML Stack
- LangChain to manage conversation flow
- OpenAI & Hugging Face models for conversational capabilities
- Optional Azure Cognitive Services for speech features

### Deployment
- Docker containers deployed via Azure App Service
- GitHub Actions for CI/CD

## Potty Training Module
- Scheduled reminders every 30–60 minutes with visual/audio alerts
- Interactive potty timer with animated countdown
- Social story animations modeling potty routines
- Visual rewards and daily success trackers

## Analytics & Monitoring
- Tracks conversational progress, emotional responses, and potty-training outcomes
- Simple dashboard analytics with charts for parents
- Data privacy ensured through anonymization and secure storage

## Privacy and Security
- Minimal data collection limited to developmental insights
- Secure storage and transmission (HTTPS, encryption)
- Clear privacy policy for parents

## Project Roadmap
| Phase              | Description                                        | Timeline   |
|--------------------|----------------------------------------------------|-----------|
| Planning & Design  | Define objectives, modules, UI mockups, AI prompts  | 1–2 weeks |
| Initial Prototype  | Simple interaction prototypes (Speech, Potty)       | 2–4 weeks |
| Iterative Development | Frontend/backend integration, Hugging Face AI interaction | 4–6 weeks |
| Alpha Testing      | Internal testing, adjustments based on responses    | 1–2 weeks |
| Expansion to OpenAI| Refine interactions with advanced AI models         | 1–2 weeks |
| Beta Testing & Launch | Wider testing, parental dashboard setup          | 2 weeks    |
| Ongoing Enhancement| Feature enhancements and content updates           | Continuous |

## Example Prompt (AI Personality Definition)
> You are Ava, a kind, patient, playful educational assistant. Your primary mission is to help young children with autism develop conversational skills, recognize emotions, navigate social interactions, and master potty training through gentle, positive reinforcement, simple language, and engaging activities.

## Success Criteria
- Improved conversational clarity and increased frequency of speech
- Clearer emotional recognition demonstrated by the child
- Increased successful potty-training interactions

## Backend Setup
The backend uses **FastAPI** (Python 3.12). To install dependencies, create and activate a virtual environment and run:

```bash
pip install -r backend/requirements.txt
```

Start the development server with:

```bash
uvicorn app.main:app --reload --app-dir backend
```

