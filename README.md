# Take Home Assignment: Scheduler with Recurring Slots


## Mockup 
<img width="379" height="807" alt="Screenshot 2025-09-02 at 12 43 10 AM" src="https://github.com/user-attachments/assets/d84bd942-3628-4984-a33e-f774bde85eac" />


## Objective
Build a scheduler system with recurring weekly slots. Each day can contain up to 2 slots (start and end times). The system should support creating, updating, deleting, and managing these slots, while handling modifications as exceptions to the recurring pattern.

You need to implement both **frontend (React + TypeScript + Tailwind)** and **backend (Node.js + TypeScript + PostgreSQL with Knex)**. The app should be fully functional and deployed live.

---

## Requirements

### Scheduler Logic
1. A schedule is created for a specific day with a start and end time.  
   - Example: Create a slot on **Monday at 9 AM - 11 AM**.
   - This slot should **automatically replicate for all upcoming Mondays**.

2. Each date can have a maximum of **2 slots**.

3. If a slot is **edited or deleted**, it should be treated as an **exception** for that specific date, without affecting other recurring slots.

4. The UI should display:
   - Current week’s dates with their slots.
   - On scrolling forward, load the next week’s dates (infinite scroll).

---

### Frontend
- Framework: **React + TypeScript**.
- Styling: **TailwindCSS**.
- Show a weekly calendar view with slots per day.
- Support infinite scroll to fetch upcoming weeks.
- Users should be able to **create, update, and delete slots** through the UI.
- Changes should be reflected immediately (optimistic updates are a plus).

---

### Backend
- Framework: **Node.js + TypeScript**.
- Database: **PostgreSQL**
- Expose REST APIs for:
  - Creating a slot.
  - Fetching slots for a given week.
  - Updating a slot (creates exception).
  - Deleting a slot (creates exception).
- Ensure recurring logic and exception handling are done at the backend.

---

### Deployment
- **Backend**: Deploy on [Render](https://render.com/) (or similar).  
- **Frontend**: Deploy on [Vercel](https://vercel.com/) or [Netlify](https://www.netlify.com/).  
- **Database**: Use a free PostgreSQL instance (e.g., Render).

---

## Deliverables
- A live **frontend link** and **backend API link**.
- A GitHub repository containing both frontend and backend code.

---

## Timeframe
You have **20 days** to complete and submit this assignment at `admin@dilsaycare.in`

---
