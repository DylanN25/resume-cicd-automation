# 🚀 Resume CI/CD Automation (LaTeX + GitHub Actions)



Este repositorio contiene un flujo de trabajo automatizado para gestionar, compilar y enviar múltiples versiones de un currículum (CV) profesional utilizando **LaTeX** y **GitHub Actions**. 



Diseñado originalmente para perfiles técnicos (Ingeniería de IA, Software y Automatización) que requieren adaptar su perfil a diferentes mercados como **Canadá** y **EE. UU.**.



## 🛠️ Características Principales



* **Multi-variante:** Gestión centralizada de diferentes versiones del CV (ej: AI Engineer, Software Developer, Industrial Automation).

* **Compilación Dinámica:** Permite seleccionar qué archivo `.tex` compilar mediante un menú desplegable en GitHub Actions.

* **Notificaciones por Email:** Envío automático del PDF generado a tu correo electrónico personal\[cite: 3].

* **Manejo de Errores:** Notificación vía email con logs detallados en caso de fallos de sintaxis en LaTeX.

* **Infraestructura como Código:** Elimina la dependencia de editores externos de pago como Overleaf.



## 🚀 Cómo usar este Repositorio



### 1. Requisitos Previos

* Una cuenta de **GitHub**.

* Una cuenta de **Gmail** con un *App Password* generado para el envío de correos.



### 2. Configuración de Secretos

En tu repositorio, ve a **Settings > Secrets and Variables > Actions** y añade:

* `MAIL_USERNAME`: Tu dirección de correo electrónico.

* `MAIL_PASSWORD`: Tu contraseña de aplicación de Google.



### 3. Ejecución del Workflow

1. Ve a la pestaña **Actions** en tu repositorio de GitHub.

2. Selecciona **"Dynamic Resume Builder"**.

3. Haz clic en **"Run workflow"**.

4. Selecciona la variante de CV que deseas (o selecciona `ALL` para todas).

5. En unos segundos, recibirás el PDF listo en tu bandeja de entrada[cite: 3].



## 🏗️ Estructura de Archivos

* `/src`: Contiene los archivos `.tex`. Los cambios realizados aquí disparan las validaciones del sistema.

* `.github/workflows/resume_builder.yml`: La lógica de automatización que utiliza contenedores Docker para compilar LaTeX.



---

*Desarrollado por Joseph Naranjo - Ndigitalhorizon*

