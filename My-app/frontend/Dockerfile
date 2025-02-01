# Usa Node.js como imagen base
FROM node:18-alpine

# Establece el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia el archivo package.json y package-lock.json antes de instalar dependencias
COPY package.json package-lock.json ./

# Instala las dependencias
RUN npm install --legacy-peer-deps

# Copia el resto del código fuente después de instalar dependencias
COPY . .

# Expone el puerto en el que correrá la app
EXPOSE 3000

# Comando por defecto para ejecutar en modo desarrollo
CMD ["npm", "start"]
