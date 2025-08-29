## Ticket Booking – Dev Setup

### Prerequisites
- Python 3.10+
- Node.js 18+ and npm

### 1) Backend (Django + DRF)
```bash
cd "backend"
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt

# Run from the Django project folder containing manage.py
cd travels
python manage.py migrate
python manage.py runserver 0.0.0.0:8000
```
Backend runs at: http://127.0.0.1:8000/

### 2) Frontend (Vite + React)
Open a new terminal:
```bash
cd "frontend"
npm install
npm run dev
```
Frontend runs at: http://localhost:5173/

### Common Issues
- If `python manage.py` not found: ensure you are in `backend/travels` (where `manage.py` lives).
- If ports are busy: use `python manage.py runserver 8001` or `npm run dev -- --port 5174`.

### Git Quick Start
From the project root:
```bash
git add README.md
git commit -m "Add README with setup instructions"
```


