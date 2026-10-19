# 📝 App de Publicaciones

Aplicación web para crear, ver, editar y eliminar publicaciones, desarrollada con **React** y **Supabase** como backend. Incluye validación de formularios, manejo de estados de carga y error, y navegación entre páginas.

## ✨ Características

- **CRUD completo:** crear, listar, editar y eliminar publicaciones.
- **Formulario reutilizable** para crear y editar, con validación de campos obligatorios usando React Hook Form.
- **Estados de interfaz cuidados:** indicadores de carga, mensajes de error, botón de reintentar y mensaje cuando no hay publicaciones.
- **Navegación con React Router**, incluyendo rutas dinámicas (`/editar/:id`) y una página 404 personalizada.
- **Estilos modulares** con CSS Modules, sin conflictos de nombres entre componentes.
- **Capa de servicios** separada (`services/Publicaciones`) para aislar la comunicación con la base de datos.

## 🛠️ Tecnologías

| Tecnología | Uso |
|---|---|
| React | Interfaz de usuario |
| Vite | Entorno de desarrollo y build |
| React Router | Enrutamiento |
| React Hook Form | Manejo y validación de formularios |
| Supabase | Base de datos y backend |
| CSS Modules | Estilos con alcance local |

## 📁 Estructura del proyecto
src/
├── components/
│ └── CardPublicacion/ # Tarjeta de cada publicación
├── pages/
│ ├── InicioPagina/ # Listado de publicaciones
│ ├── FormularioPublicacion/# Crear / editar publicación
│ └── NoEncontrada/ # Página 404
├── services/
│ └── Publicaciones.js # Funciones de acceso a Supabase
└── main.jsx

## 🚀 Instalación y uso

1. Clonar el repositorio:
```bash
   git clone https://github.com/tu-usuario/tu-repositorio.git
   cd tu-repositorio
```
2. Instalar dependencias:
```bash
   npm install
```
3. Crear un archivo `.env` en la raíz con tus credenciales de Supabase:
```env
   VITE_SUPABASE_URL=tu_url_de_supabase
   VITE_SUPABASE_ANON_KEY=tu_clave_anonima
```
4. Crear en Supabase una tabla `publicaciones` con las columnas `id`, `titulo` y `contenido`.
5. Iniciar el servidor de desarrollo:
```bash
   npm run dev
```
   La app queda disponible en `http://localhost:5173`.

## 🧠 Lo que practiqué en este proyecto

- Integración de React con un backend como servicio (Supabase).
- Formularios controlados con validación declarativa.
- Manejo de efectos y estados asíncronos con `useEffect` y `useState`.
- Organización del código en páginas, componentes y servicios.

## 🔮 Próximas mejoras

- Autenticación de usuarios.
- Búsqueda y paginación de publicaciones.
- Confirmación antes de eliminar.
- Despliegue en Vercel o Netlify.

## 👤 Autor

**Guillermo Sanchez Apaza** · [LinkedIn](https://www.linkedin.com/in/guille-apaza-9569b0355/) · [GitHub](https://github.com/Guillermovgs)
