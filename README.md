# Proyecto de Práctica - Gestión de Ramas en GitHub

---

title: "Gestión de Ramas y Pull Request en GitHub"
author: "Gael Espinosa"
fecha: "16/10/2025"
rama_respaldo: "respaldo-161024-GE"
repositorio: "https://github.com/GaelZ23/practica-rama-Gael"

---

## 🎯 Objetivo
Demostrar competencia en el manejo de ramas en GitHub, incluyendo la creación, fusión y resolución de conflictos, aplicando el concepto de *pull request* de trabajo colaborativo.

---

## 🧩 Flujo de trabajo realizado

### 🟦 Fase 1: Configuración Inicial
- Se creó el repositorio **practica-ramas-gael** en GitHub.
- Se clonó el repositorio localmente con `git clone`.
- Se configuró el usuario con `git config --global`.

### 🟩 Fase 2: Desarrollo en la rama `main`
- Se creó el archivo inicial `README.md` con la estructura base.
- Se añadió el archivo `funciones.js` con la función:
  ```js
  function saludar() { return 'Hola desde MAIN'; }

### 🟩 Fase 3: Trabajo con múltiples ramas
- Se creó la rama desarrollo y se reemplazó el contenido de funciones.js:
  ```js
  function saludar() { return 'Hola Mundo'; }
- Se creó la rama feature/validacion y se añadió:
  ```js
  function validarEmail(email) { return email.includes('@'); }
- Se realizaron commits en cada rama con mensajes descriptivos.


### 🟩 Fase 4: Respaldo y simulación de Pull Request
- Se creó la rama de respaldo: respaldo-161024-GE
- Se subió al repositorio remoto.
- Se documentó el respaldo dentro del README.md:
    # Fecha: 16/10/2025
    # Rama: respaldo-161024-GE
    # Contenido: desarrollo hasta función de validación.

### 🟩 Fase 5: Fusión y resolución de conflictos
- Se fusionó feature/validacion dentro de desarrollo.
- Se modificó funciones.js en main para generar un conflicto:
  ```js
     function saludar() { return 'Hola desde MAIN con cambios'; }
- Luego, al fusionar main en desarrollo, se produjo un conflicto.
- Se resolvió manualmente el conflicto y se dejó la versión final:
  ```js
     function saludar() { return 'Hola Mundo con validación'; }
     function validarEmail(email) { return email.includes('@'); }
- Commit final de resolución:
    *fix: resolver conflicto en funciones.js*

### 🟩 Fase 6: Limpieza y documentación
- Se eliminó la rama temporal feature/validacion.
- Se actualizó este archivo README.md con el flujo completo.
- Se realizó el push final de la rama desarrollo.

---