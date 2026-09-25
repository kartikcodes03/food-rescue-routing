# FoodRescue

React + Tailwind (Vite) → FastAPI → PostgreSQL

## 1. Database
    docker compose up -d

## 2. Backend  (http://localhost:8000/docs)
    cd backend
    python -m venv venv && source venv/bin/activate   # Windows: venv\Scripts\activate
    pip install -r requirements.txt
    uvicorn app.main:app --reload
Tables apne aap ban jaate hain. Admin login: `admin@foodrescue.local` / `admin123` (.env me badlein).

## 3. Frontend  (http://localhost:5173)
    cd frontend
    npm install
    npm run dev

## Demo flow
1. NGO register karo -> location set karo -> "Request food" post karo
2. Donor register karo -> food post karo -> Matching Engine turant NGO se jod deta hai
3. Volunteer register karo -> location set karo -> Accept -> Picked up -> Delivered
4. Home page (Dashboard) par live numbers badhte dikhenge
