# GitHub Actions
## Objetivo

Se hac creado un workflow de GitHub Actions para generar automáticamente la documentación de la tarea 0 de PPS con MkDocs cada vez que se realiza un push sobre la rama main.

## Archivo del workflow

El archivo se encuentra en:
```text
.github/workfows

```

## Funcionamiento
El workfow realiza automáticamente las siguientes tareas:
1. Descargar el respositorio
2. Configura Python
3. Instala MkDocs
4. Genera la documentación HTML
5. Publica la documentación en la rama gh-pages

Gracuas a GitHub Actions cada ve que se realiza cambios en los archivos Markdown y se hace push, la documentación se actualiza automáticamente sin necesidad de intervención manual.

Los detalles de implementación se encuentra en el PDF de la tarea.
