# GraminRide — GitHub-ready (UI3 Hybrid)

This package is prepared for GitHub and Render deployment.

## How to use
1. Extract and inspect folders `backend/` and `frontend/` at repo root.
2. Commit and push to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial GraminRide UI3 ready for deploy"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo>.git
   git push -u origin main
   ```
3. On Render.com:
   - Create a **Web Service** for backend with Root: `backend`, Build: `npm install`, Start: `npm start`
   - Create a **Static Site** for frontend with Root: `/frontend`

## Notes
- Backend uses SQLite; `backend/data.sqlite` will be created on first run.
- Update frontend fetch calls if needed to point to backend URL (SEARCH for `/api/` in frontend files).
