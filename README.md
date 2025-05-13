<p align='center'>
  <img width='200' heigth='225' src='https://user-images.githubusercontent.com/62605744/171186764-43f7aae0-81a9-4b6e-b4ce-af963564eafb.png'>
</p>

# 🚀 Taller Desarrollo de Software III - React & GraphQL 👋

## 📝 Descripción

Aplicación web interactiva de saludos personalizados utilizando tecnologías modernas. La aplicación consta de un backend GraphQL con Express y un frontend en React que permite a los usuarios enviar mensajes y recibir saludos personalizados.

## ✨ Características

- 🔄 API GraphQL para consultas de saludos
- 🎨 Interfaz de usuario moderna construida con React y Bootstrap
- 🐳 Containerización con Docker para un despliegue sencillo
- 🌐 Arquitectura cliente-servidor con frontend y backend integrados

## 🛠️ Tecnologías Utilizadas

### Backend:
- 📊 Express.js - Framework web
- 🔍 Apollo Server - Servidor GraphQL
- 🧪 GraphQL - Lenguaje de consulta para APIs

### Frontend:
- ⚛️ React - Biblioteca de UI
- 📱 React Bootstrap - Componentes de UI responsivos
- 🔌 Apollo Client - Cliente GraphQL para React
- 🏗️ Vite - Herramienta de construcción rápida

## 🚦 Cómo ejecutar el proyecto

### Requisitos previos:
- Node.js (v14 o superior)
- npm o yarn

### Usando npm:

```bash
# Instalar dependencias del backend
npm install

# Instalar dependencias del frontend
cd saludofront-app
npm install
npm run build
cd ..

# Iniciar el servidor
npm start
```

### Usando Docker:

```bash
# Construir la imagen
docker build -t saludo-app .

# Ejecutar el contenedor
docker run -p 4000:4000 saludo-app
```

## 🌐 Acceso a la aplicación

Una vez que el servidor esté en funcionamiento, puedes acceder a:

- 🖥️ Aplicación web: http://localhost:4000
- 📊 Playground GraphQL: http://localhost:4000/graphql

## 📝 Ejemplos de consultas GraphQL

```graphql
# Consulta de saludo personalizado
query {
  hello(message: "Juan")
}

# Consulta de información sobre los creadores
query {
  aboutMarcelo
  aboutDiego
  aboutSebas
}
```