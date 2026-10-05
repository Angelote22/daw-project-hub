# Pequeña página web para practicar un flujo profesional de trabajo con Git y Github.

Conexión SSH con GitHub: comprobada correctamente
## Instrucciones para abrir la página web

1. Clona el repositorio en tu equipo local si no lo has hecho aún:
   ```bash
   git clone git@github.com:Angelote22/daw-project-hub.git
   ## Diferencia entre fetch y pull

- **¿Qué hizo `git fetch`?** Descargó los nuevos commits y metadatos desde el repositorio remoto (`origin/main`) a la copia local, pero **sin modificar ni alterar** los archivos de trabajo actuales ni fusionar nada en la rama local.
- **¿Qué hizo `git pull`?** Realizó en un solo paso la descarga de novedades remota (`fetch`) y la fusión automática (`merge`) de la rama remota en la rama local activa.
- **¿Por qué `fetch` permite revisar antes de integrar?** Porque al no aplicar automáticamente los cambios sobre el directorio de trabajo, permite inspeccionar las diferencias (`git diff main origin/main`) e identificar posibles conflictos antes de decidir si fusionar.
- **Relación entre `pull`, `fetch` e integración:** El comando `git pull` es en esencia la combinación secuencial de dos operaciones: `git fetch` (descargar cambios remotos) seguido de `git merge` (integrar o fusionar esos cambios en la rama actual).

## Forks y colaboración

1. **¿Qué es un fork en GitHub?**  
   Es una copia completa de un repositorio ajeno que se guarda directamente dentro de tu propia cuenta de GitHub. Te permite experimentar o realizar cambios en un proyecto sin alterar el repositorio original.

2. **¿En qué se diferencia un fork de una rama?**  
   Una rama pertenece al mismo repositorio y la gestionan las personas con permisos sobre él. Un fork es una copia independiente alojada en la cuenta de otro usuario de GitHub.

3. **¿En qué cuenta se almacena un fork?**  
   Se almacena directamente en la cuenta personal del usuario que hace el fork (o en la organización donde este lo clone).

4. **¿Cuándo resulta útil trabajar mediante un fork?**  
   Es muy útil al colaborar en proyectos de código abierto (Open Source) o cuando quieres realizar aportaciones a un repositorio en el que no tienes permisos directos de escritura.

5. **¿Qué relación existe entre el repositorio original y el fork?**  
   Están vinculados mediante el historial de Git en GitHub. El fork sabe de qué repositorio original procede, lo que permite sincronizar actualizaciones posteriores o proponer cambios.

6. **¿Qué es el repositorio *upstream*?**  
   Es el término utilizado para referirse al repositorio original principal del cual hiciste el fork.

7. **¿Qué diferencia existe entre *origin* y *upstream*?**  
   * **`origin`**: Es la URL de tu propio fork (tu copia en GitHub).  
   * **`upstream`**: Es la URL del repositorio original del creador principal, de donde puedes descargar las novedades para mantener actualizado tu fork.

8. **¿Cómo se propone que un cambio del fork llegue al repositorio original?**  
   A través de un **Pull Request (PR)** enviado desde GitHub, solicitando a los mantenedores del proyecto original que revisen e integren tus modificaciones.

9. **¿Quién decide si se acepta la propuesta?**  
   Los administradores o mantenedores que tienen permisos de escritura en el repositorio original (*upstream*).

10. **¿Puede seguir evolucionando el repositorio original mientras existe el fork?**  
    Sí, de forma totalmente independiente. El repositorio original seguirá recibiendo avances de sus creadores y la persona que tiene el fork puede ir sincronizando esas novedades en su copia cuando lo necesite.
    