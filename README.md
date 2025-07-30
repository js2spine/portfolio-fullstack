# portfolio-fullstack
Инструкция по запуску и деплою Portfolio
Portfolio Fullstack Gallery

Полноценное fullstack-портфолио на Node.js + React (Vite) с галереей изображений, pop-up, swipe и деплоем на Render + Vercel.

🔧 Стек технологий
- Backend: Node.js + Express
- Frontend: React + Vite + TailwindCSS + shadcn/ui + Framer Motion
- Деплой: Render (backend), Vercel (frontend)
- CI/CD: GitHub Actions

🚀 Быстрый старт локально
1. Установи зависимости:
cd backend && npm install
cd ../frontend && npm install

2. Запусти backend:
cd ../backend && node index.js

3. Запусти frontend:
cd ../frontend && npm run dev

4. Пример .env:
VITE_API_URL=http://localhost:3000/api/gallery

🌍 Деплой
Backend на Render:
- Создай Web Service в render.com
- Настройки: Build - npm install, Start - node index.js, Root - backend

Frontend на Vercel:
- Импортируй GitHub репозиторий
- Настройки: Vite, root: frontend, build: npm run build, dist: dist
- Добавь .env:
VITE_API_URL=https://your-backend.onrender.com/api/gallery

⚙️ CI/CD с GitHub Actions
1. Получи токены в Vercel:
- Personal Token
- Project ID
- Org ID

2. В GitHub → Secrets добавь:
VERCEL_TOKEN, VERCEL_ORG_ID, VERCEL_PROJECT_ID

3. Workflow уже есть: .github/workflows/deploy-vercel.yml

✅ Функциональность
- Галерея сеткой
- Pop-up с описанием и доп. изображениями
- Swipe по главному изображению

==> Available at your primary URL https://portfolio-backend-23pv.onrender.com
portfolio-fullstack-eight-navy.vercel.app
portfolio-fullstack-zuz5i1u6s-leopolds-projects-84ed9406.vercel.app

backend
https://dashboard.render.com/web/srv-d22c5963jp1c738o86o0/deploys/dep-d22c59e3jp1c738o8700


- Backend API
- CI/CD автодеплой
