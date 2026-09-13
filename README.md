<div align="center">

# 🚀 Procrastinity — Enfoque, Hábitos & Control de Dopamina

<div align="center">
  <img width="512" height="512" alt="icon" src="https://github.com/user-attachments/assets/d4cddd70-83c5-4138-a338-2d4dd0e9ccfd" />
</div>


![Kotlin](https://img.shields.io/badge/Language-Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![Android Studio](https://img.shields.io/badge/IDE-Android%20Studio-3DDC84?style=for-the-badge&logo=android-studio&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Architecture](https://img.shields.io/badge/Architecture-Material%203-FF6F00?style=for-the-badge)
![UI/UX](https://img.shields.io/badge/Design-Cyber--Navy%20Dark-00C853?style=for-the-badge)

**Procrastinity** es una aplicación nativa de Android diseñada para la gestión del tiempo y la creación de hábitos productivos, desarrollada en **Android Studio** utilizando **Kotlin puro**. Combina **gamificación mediante mascotas virtuales** con mecánicas de **fricción cognitiva** para mitigar el consumo impulsivo de redes sociales y proteger tus bloques de estudio u trabajo sin depender de internet ni de suscripciones.

---

### 📲 Descargar Aplicación

[<img src="https://img.shields.io/badge/Descargar_Última_Versión-APK-2ea44f?style=for-the-badge&logo=android&logoColor=white" height="45">](https://github.com/markbn15/Procrastinity/releases)

</div>

---

## 🔒 1. Pilar Fundamental: Control de Dopamina y Privacidad Local

> [!IMPORTANT]
> **Tus hábitos y tus datos se quedan en tu dispositivo.**  
> Procrastinity opera bajo un modelo **totalmente local (*Offline-First*)**. Tu configuración de bloques, metas, selecciones de aplicaciones y estados de evolución de tu mascota permanecen en el almacenamiento interno sin enviar métricas a servidores externos.

* 🌐 **Arquitectura Offline-First:** Almacenamiento local mediante `SharedPreferences` persistentemente encriptadas por sesión.
* 🛡️ **Fricción Cognitiva:** Interfaz translucida (`FrictionOverlayActivity`) que interrumpe la apertura impulsiva de apps restringidas con una pausa de 15 segundos reales.
* 📑 **Lista Blanca Exclusiva:** Selección directa de herramientas del sistema exentas de bloqueo mediante la lectura del `PackageManager`.

---

## 🛠️ Especificaciones Técnicas

+---------------------------------------------------------------------------------+
|                                STACK TECNOLÓGICO                                |
+--------------------------+------------------------------------------------------+
| Lenguaje                 | Kotlin Puro                                          |
| Arquitectura             | Modular (Material 3 + Foreground Services)           |
| UI / Sistema de Diseño   | Dynamic Material Design 3 (Cyber-Navy Dark)          |
| Concurrencia & Alarmas   | AlarmManager, Broadcast Receivers & Android Threads  |
| Monitoreo de Sistema     | Foreground Service & PackageManager                  |
| Optimización de Layouts  | ConstraintLayout & ScrollView (fillViewport)         |
+--------------------------+------------------------------------------------------+

---

## ✨ Características Destacadas

### 🐾 2. Motor de Gamificación (`MascotGrowthManager`)
* 🐣 **Mascotas de Enfoque:** Elige entre **Árbol, Pez o Rana** al iniciar tu meta de estudio.
* 📈 **Evolución Adaptativa:** Crecimiento calculado en tres rangos precisos (**0–33%**, **34–66%**, **67–100%**) basados en el tiempo transcurrido vs. días restantes.
* ⚠️ **Penalización Reactiva:** Si rompes la sesión de enfoque interrumpiendo las restricciones, tu mascota sufrirá una involución visual.

### 🛡️ 3. Sistema de Bloqueo (`AppBlockerService`)
* ⏱️ **Retardo de 15 Segundos:** Ventana translucida al 90% de opacidad para romper la inercia del uso automático de apps.
* 🔍 **Gestión de Lista Blanca (`WhitelistActivity`):** Buscador en tiempo real con selectores `MaterialSwitch` para mantener activas las aplicaciones esenciales.
* ⚙️ **Monitoreo en Segundo Plano:** Servicio de primer plano (*Foreground Service*) optimizado para un bajo consumo de batería.

### 📅 4. Gestión de Rutinas y Salud (`MainActivity`)
* ⏱️ **Planificación de Bloques:** Organización de tiempo en categorías (**Estudio, Ocio, Ejercicio**) mediante `TimePickerDialog`.
* 💧 **Notificaciones de Hidratación (`HydrationReceiver`):** Recordatorios automáticos vinculados a `AlarmManager` al iniciar bloques de estudio para mantener el rendimiento intelectual.

### 🎨 5. Interfaz y Accesibilidad
* 🌙 **Tema Cyber-Navy:** Paleta oscura basada en tokens dinámicos (`?attr/colorSurface`) para reducir la fatiga visual.
* ♿ **Soporte Accesible:** Cadenas centralizadas en `strings.xml` (100% libre de textos *hardcoded*) e integración con `contentDescription` para lectores de pantalla.

---

## 🛠️ Requisitos de Instalación

* **S.O. Compatible:** Android 7.0 (API Nivel 24) o superior.
* **Permisos requeridos:**
  * 📊 `Acceso a Estadísticas de Uso`: Para detectar el uso de apps restringidas.
  * 🖼️ `Mostrar sobre otras aplicaciones`: Para desplegar la pantalla de retardo.
  * 🔔 `Notificaciones`: Para avisos del servicio en segundo plano e hidratación.

---

## 💻 Compilación e Instalación

```bash
# 1. Clona este repositorio
git clone [https://github.com/markbn15/Procrastinity.git](https://github.com/markbn15/Procrastinity.git)

# 2. Abre el proyecto en Android Studio

# 3. Sincroniza los archivos Gradle

# 4. Compila y ejecuta en un dispositivo o emulador
```
### ⭐ Apoya el Proyecto
Si Procrastinity te ha servido para estructurar tus hábitos o como referencia técnica de desarrollo en Android:

Dale una Estrella (⭐) a este repositorio en GitHub.

Comparte el proyecto con otros desarrolladores.

### 🤝 Créditos y Agradecimientos
Agradecimiento a las herramientas y tecnologías utilizadas:

🎨 Material Components for Android: Por la implementación de componentes de Material Design 3.

🤖 Android Jetpack: Por la infraestructura para servicios y alarmas del sistema.

🧑‍💻 Comunidad Open Source: Por la documentación y ejemplos de arquitectura.

Hecho con ❤️ para la comunidad de código abierto.

### 📄 Licencia
Este proyecto está distribuido bajo los términos de la Licencia Apache 2.0. Para más detalles, consulta el archivo LICENSE incluido en este repositorio.
