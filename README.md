# Parte II — Componente Práctico

## Ejercicio 1 — Repositorio en parejas: CV en HTML

Trabajo en parejas. El objetivo es aplicar el flujo completo de Git (local y remoto) sobre un proyecto real: una página HTML de una sola vista (one-page) que funcione como hoja de vida (CV).

### Roles

- **Persona principal**: crea el repositorio, la estructura inicial del proyecto y el remoto.
- **Persona de apoyo**: clona el repositorio, contribuye con ramas propias y valida los cambios de la persona principal.
- Los roles se intercambian a la mitad del ejercicio, de modo que ambas personas ejecuten tanto el flujo de 'principal' como el de 'apoyo'.

### Pasos sugeridos

1. La persona principal crea la carpeta del proyecto, ejecuta `git init` y agrega un archivo `index.html` con la estructura base del CV (nombre, foto o inicial, resumen, experiencia, educación, contacto).
2. Primer commit: `git add index.html` y `git commit -m "Estructura base del CV"`.
3. La persona principal crea el repositorio remoto (vacío) y lo conecta con `git remote add origin <url>`, luego sube el historial con `git push -u origin master`.
4. La persona de apoyo clona el repositorio con `git clone <url>`.
5. Cada persona crea al menos una rama propia para agregar una sección o mejora distinta (por ejemplo, `seccion-habilidades` o `estilos-css`), y confirma sus cambios con commits descriptivos.
6. Cada rama se sube al remoto con `git push -u origin <rama>`.
7. La persona principal integra ambas ramas en `master` con `git merge`, resolviendo a mano cualquier conflicto que surja (por ejemplo, si ambas tocaron la misma sección del HTML).
8. La persona de apoyo trae los cambios finales con `git pull` y confirma, con `git log --oneline --graph --all`, que su copia local refleja el trabajo integrado de ambas.

### Entregables del Ejercicio 1

- Enlace o acceso al repositorio remoto con el proyecto HTML del CV.
- Historial de commits visible que muestre la participación de ambas personas (nombre/correo configurados en cada commit).
- Captura o registro de al menos un conflicto de merge resuelto manualmente.
- Breve reflexión escrita (5-8 líneas) sobre la experiencia de alternar entre los roles de principal y apoyo.
