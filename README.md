# 🧠 Headless Shopify – Next.js + TypeScript

Este es un proyecto personal para construir una tienda **headless** con Shopify como backend y un frontend completamente custom usando **Next.js + React + TypeScript**. No se utiliza Hydrogen, Remix ni ningún framework adicional: el objetivo es **aprender desde cero** cómo conectar Shopify a un frontend desacoplado, con foco en rendimiento, escalabilidad y SEO.

---

## 👨‍💻 ¿Por qué este proyecto?

Trabajo como desarrollador frontend y UX/UI en **Onestic**, donde usamos temas Shopify personalizados basados en Dawn. Pero quería entender cómo construir **una tienda headless real**, desde cero, sin dependencias, para mejorar mis habilidades en:

- Arquitectura headless
- GraphQL y Storefront API
- SEO y renderizado en servidor
- Rutas dinámicas con Next.js
- Estilos con CSS Modules y diseño escalable

---

## 🧱 ¿Qué estoy construyendo?

Una tienda ecommerce desacoplada con:

- Navegación pública: home, colecciones, productos
- Datos en tiempo real desde Shopify Storefront API
- Carrito de compra y redirección al checkout
- Filtros, variantes y lógica de producto dinámica
- Responsive, accesible y optimizada para SEO

---

## 🚀 Stack técnico

- [Next.js](https://nextjs.org/) (con Pages Router)
- [React](https://react.dev/)
- [TypeScript](https://www.typescriptlang.org/)
- [CSS Modules](https://nextjs.org/docs/basic-features/built-in-css-support#adding-component-level-css)
- [Shopify Storefront API](https://shopify.dev/docs/api/storefront)
- [GraphQL](https://graphql.org/)

---

## 📁 Estructura inicial del proyecto

``
headless-shopify/
├── public/ # Archivos estáticos
├── src/
│ ├── components/ # Componentes reutilizables
│ ├── lib/ # Cliente Shopify y funciones de API
│ ├── pages/ # Home, producto, colección, etc.
│ ├── styles/ # CSS Modules
│ └── types/ # Tipos TypeScript compartidos
├── .env.local # Claves privadas (Storefront Token)
├── next.config.js
├── tsconfig.json
└── package.json
``


---

## 📍 Estado del proyecto

✅ Proyecto Next.js + TS configurado  
🔜 Conexión a Storefront API (en proceso)  
🔜 Primera query a productos  
🔜 Routing dinámico (`/products/[handle]`)  
🔜 Carrito y lógica de checkout  

---

## 🛠️ Cómo ejecutarlo localmente

1. Crea un archivo `.env.local` en la raíz con estas claves:

``
SHOPIFY_STORE_DOMAIN=your-store.myshopify.com
SHOPIFY_STOREFRONT_TOKEN=your_storefront_token
SHOPIFY_API_VERSION=2024-04
``


2. Instala dependencias y ejecuta el entorno:

```bash
npm install
npm run dev

