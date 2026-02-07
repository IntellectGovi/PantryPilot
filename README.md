# PantryPilot 🥗  
**From pantry to plan.**

PantryPilot helps busy people plan their weekly meals using the ingredients they already have.  
Users enter what’s in their kitchen and their preferences, and the system generates a practical weekly meal plan along with a ready-to-use shopping list.

This project focuses on solving a real-world problem: **decision fatigue and food waste caused by manual meal planning**.

---

## Why PantryPilot?

Meal planning sounds simple, but in reality:
- People don’t know what to cook with what they already have
- Recipes are scattered and hard to adapt
- Planning a full week is mentally exhausting
- Groceries are often overbought, leading to waste

Existing solutions are either rigid, overly diet-focused, or require too much manual effort.

PantryPilot is built around a simple idea:
> Start with what you already have, then plan the rest intelligently.

---

## Key Features (MVP)

- Ingredient-first meal planning
- Weekly meal plan generation (7 days)
- Consolidated shopping list
- Recipe details with ingredients and instructions
- Graceful handling of missing or conflicting inputs
- Fast, responsive UI with clear loading and error states

---

## How It Works

1. User enters available ingredients and preferences
2. Backend fetches relevant recipes from an external API
3. OpenAI is used **only for planning logic**, not raw data
4. The system generates a structured weekly plan (JSON)
5. Frontend renders the plan and shopping list

AI is deliberately constrained to reasoning tasks, while data integrity and UX remain deterministic.

---

## Tech Stack

### Frontend
- React (Next.js)
- TypeScript
- Tailwind CSS
- Modern hooks-based state management

### Backend
- Node.js
- Express
- TypeScript
- OpenAI API
- External Recipe API

### Infrastructure
- RESTful API design
- Environment-based configuration
- Deployed on cloud hosting (Vercel / Render)

---

## Technical Challenges Solved

- Converting unstructured user input into structured data
- Enforcing strict JSON output from AI responses
- Handling partial failures from third-party APIs
- Managing async UI state and loading flows
- Designing a useful MVP without feature bloat

---

## Project Scope & Intentional Tradeoffs

What this project **does**:
- Focuses on core planning logic
- Solves a real, specific problem well
- Demonstrates full-stack decision making

What this project **intentionally avoids** (for MVP):
- User authentication
- Social features
- Drag-and-drop UI
- Over-automation

These can be added later, but were excluded to keep the MVP focused and shippable.

---

## Future Improvements

- Save plans to user accounts
- Drag-and-drop meal reordering
- Nutrition and calorie constraints
- Budget-based planning
- Image-based ingredient input
- Calendar and reminder integrations

---

## Why This Project Matters

PantryPilot is not a demo CRUD app.

It demonstrates:
- Product thinking
- System design
- AI integration with guardrails
- Real-world UX considerations
- Practical full-stack engineering

---

## Author

Built by **Govind**  
Frontend-focused engineer with backend experience in Node.js and APIs.

---
