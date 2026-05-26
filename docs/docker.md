# DOCJR NGINX

Se utilizó la imagen oficial de NGINX disponible en Docker Hub.

El contenedor se creó con el siguiente comando:
```text
docker run -d \
--name PPSUnidad0-Tarea_Isidro \
-p 8085:80 \
-v "$PWD":/usr/share/nginx/html:ro \
nginx
```

## Explicación del comando 

1. **docker run -d**
 Ejecuta el contenedor en segundo plano.

2. **--name PPSUnidad0-Tarea_Isidro**
 Asigna un nombre al contenedor.
**-p 8085:80**
 Redirige el puerto 8085 del anfitrión al puerto 80 interno del contenedor.
3. **-v "$PWD":/usr/share/nginx/html:ro**
 Monta el directorio actual dentro del directorio web de NGINX utilizando un Bind Mount en modo solo lectura.
4. **nginx**
 Imagen utilizada para crear el contenedor.


Para verificar que el contenedor estaba funcionando correctamente se utilizó: * docker ps *

La documentación quedó accesible desde: **http://localhost:8085**
