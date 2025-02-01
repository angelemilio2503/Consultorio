# Usar una imagen base de Node
FROM node:16

# Crear un directorio de trabajo
WORKDIR /app

# Copiar los archivos de package.json y package-lock.json
COPY package*.json ./

# Instalar las dependencias
RUN npm install

# Copiar el resto de los archivos
COPY . .

# Exponer el puerto
EXPOSE 5000

# Comando para iniciar el servidor del backend
CMD ["npm", "run", "dev"]
