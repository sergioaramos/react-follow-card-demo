# Twitter Follow Card Demo

Este proyecto es una demostración de un componente de React que simula las tarjetas de seguimiento de usuarios de Twitter (ahora X). El componente muestra información de un usuario, su avatar y un botón para seguir/dejar de seguir.

## Características

- Componente reutilizable para mostrar tarjetas de usuarios
- Estado de seguimiento que se puede cambiar al hacer clic en el botón
- Efecto visual al pasar el cursor sobre el botón de "Dejar de seguir"
- Avatares dinámicos que se cargan desde unavatar.io

## Tecnologías utilizadas

- React 18
- Vite
- CSS puro para los estilos

## Instalación

Para ejecutar este proyecto localmente:

```bash
# Clonar el repositorio
git clone https://github.com/sergioaramos/react-follow-card-demo.git

# Navegar al directorio del proyecto
cd react-follow-card-demo

# Instalar dependencias
npm install

# Iniciar servidor de desarrollo
npm run dev
```

## Uso del componente

El componente `TwitterFollowCard` puede ser reutilizado de la siguiente manera:

```jsx
<TwitterFollowCard 
  userName="nombreusuario" 
  initialIsFollowing={true|false}
>
  Nombre del usuario
</TwitterFollowCard>
```

### Props

- `userName`: El nombre de usuario para mostrar y usar en la URL del avatar
- `initialIsFollowing`: Estado inicial del botón de seguimiento (true/false)
- `children`: Contenido que se mostrará como el nombre del usuario

## Estructura del proyecto

- `src/App.jsx`: Componente principal que renderiza una lista de tarjetas de usuario
- `src/TwitterFollowCard.jsx`: Componente reutilizable para mostrar cada tarjeta
- `src/App.css`: Estilos específicos para el componente TwitterFollowCard
- `src/index.css`: Estilos globales de la aplicación

## Scripts disponibles

- `npm run dev`: Inicia el servidor de desarrollo
- `npm run build`: Compila la aplicación para producción
- `npm run preview`: Previsualiza la versión compilada

## Licencia

MIT