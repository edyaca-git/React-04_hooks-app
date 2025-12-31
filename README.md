# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Temas puntuales
Esta sección tiene por objetivo reforzar el conocimiento de los hooks tradicionales y especializarlos en los "custom hooks"
Puntualmente veremos:
  o  useState
  o  useRef
  o  useEffect
  o  Custom Hooks como:
  o  useCounter
  o  usePokemon
  o  useTrafficLight
Conectar múltiples custom hooks entre sí
Y mucho más..

Proyecto React hooksApp
1.- npm create vite
    o  Project name:
    |  04_hooks-app
    o  Select a framework:
    |  React
    o  Select a variant:
    |  TypeScript + SWC
    
    cd 04_hooks-app
    npm install
    npm run dev
2.- eliminar :
     - assets
     - App.css
     - App.tsx
    quitar contenido de
     - index.css
    quitar las llamadas que ya no existen
     - main.tsx
    crear en  src
     - HookApp.tsx
3.- Los estilos se haran con
      o  https://tailwindcss.com/
         click en [Get started] y asegurate que este seleccionado [Using Vite]
      o  instalar tailwindcss
         C:\Projects\Git\React\04_hooks-app>npm install tailwindcss @tailwindcss/vite
         click en [Get started] y asegurate que este seleccionado [Using Vite]
      o  en el archivo vite.config.ts agregar las lineas (esta)
            import { defineConfig } from 'vite'
            import tailwindcss from '@tailwindcss/vite'   (esta)

            export default defineConfig({
            plugins: [
                tailwindcss(),      (esta)
            ],
            })     
      o  en el index.css agregar
          @import "tailwindcss";
        y agregas esta linea que contiene muchos stilos de Tailwind que dio el instructor
        .bg-gradient {
        @apply bg-gradient-to-br from-slate-900 via-gray-900 to-slate-800 min-h-screen flex items-center justify-center p-4 text-white;
        }          
