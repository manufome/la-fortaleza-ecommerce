🏰 La Fortaleza — Plataforma E-commerce (Repositorio Contenedor)

La Fortaleza es una plataforma de comercio electrónico desarrollada con una arquitectura Headless, donde el frontend (Vue.js / Nuxt) y el backend (Django / DRF) se mantienen como aplicaciones independientes, comunicándose mediante una API REST.

Este repositorio funciona como punto central de documentación, enlazando ambos proyectos y ofreciendo una vista general del sistema.

🔗 Repositorios del Proyecto
🖥️ Frontend — Tienda (Vue.js / Nuxt)

Interfaz del cliente, catálogo, carrito, checkout y autenticación.

➡️ Repositorio: https://github.com/manufome/ecommerce-vue

(Incluye README completo con instalación, capturas y documentación.)

⚙️ Backend — API (Django / DRF)

Servicios REST, gestión de usuarios, productos, carrito, pedidos y autenticación JWT.

➡️ Repositorio: https://github.com/manufome/ecommerce-django

(Incluye instalación detallada, documentación Swagger y estructura interna.)

🧱 Arquitectura General
la-fortaleza-ecommerce/
│
├── frontend/        → App de cliente (Vue + Nuxt)
└── backend/         → API REST (Django + DRF)


Características de la arquitectura:

Comunicación vía API REST

Frontend desacoplado del backend (Headless Commerce)

Despliegue independiente por servicio

Fácil integración con apps móviles o paneles administrativos futuros

🚀 Ejecución Rápida en Local
1. Clonar este repositorio
git clone https://github.com/manufome/la-fortaleza-ecommerce
cd la-fortaleza-ecommerce

2. Levantar el Backend (API)
git clone https://github.com/manufome/ecommerce-django backend
cd backend

python -m venv venv
source venv/bin/activate     # Windows: venv\Scripts\activate

pip install -r requirements.txt
python manage.py migrate
python manage.py runserver


API disponible en:
👉 http://localhost:8000

3. Levantar el Frontend (Tienda)
git clone https://github.com/manufome/ecommerce-vue frontend
cd frontend

npm install
npm run dev


Tienda disponible en:
👉 http://localhost:3000

🛠️ Tecnologías Principales

Frontend: Vue.js, Nuxt 2, Vuex, Axios, SCSS

Backend: Django, Django Rest Framework, Simple JWT, PostgreSQL

Arquitectura: Headless, REST API, SSR, PWA
