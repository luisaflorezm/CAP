# Sistema Automatizado para la Gestión de Datos Clínicos y Neuropsicológicos

## Descripción del Proyecto

El proyecto "Sistema Automatizado para la Gestión de Datos Clínicos y Neuropsicológicos" tiene como objetivo desarrollar una solución eficiente para gestionar y analizar datos clínicos y resultados de pruebas neuropsicológicas en la Universidad Pontificia Bolivariana. El sistema está diseñado para facilitar el diagnóstico y seguimiento de pacientes con condiciones neuropsicológicas, optimizando el tiempo de los profesionales de la salud y reduciendo el trabajo manual.

## Integrantes del proyecto
[Camilo Velásquez Hincapié](https://github.com/CAMsay234)

[Luis Alejandro Londoño Martinez](https://github.com/alejolondonm) 

[Luisa María Flórez Múnera](https://github.com/luisaflorezm) 

[Mariana Gómez Mejía](https://github.com/MariGomezMe) 

## Objetivo general del proyecto:
Desarrollar un sistema automatizado para la gestión y análisis de datos clínicos y neuropsicológicos en la Universidad Pontificia Bolivariana; facilitando el diagnóstico y seguimiento de pacientes, obteniendo una eficiencia en la atención clínica de los profesionales de la salud.

## Objetivos claves:
•	Establecer una ruta crítica definiendo las herramientas y tecnologías para la implementación del proyecto, asegurando un funcionamiento óptimo y garantizando la sostenibilidad y evolución futura del sistema.

•	Implementar un motor de base de datos adecuado para el funcionamiento local, diseñando un esquema de base de datos detallado, y asegurando la integración eficiente con el backend del sistema.

•	Desarrollar una interfaz de usuario intuitiva y un backend robusto para la gestión segura y precisa de datos del paciente, garantizando la entrada, actualización y visualización efectiva de la información.

•	Crear un módulo de visualización de datos que permita a los neuropsicólogos la interpretación y el análisis de la información contenida en las historias clínicas a través de gráficos y visualizaciones claras y efectivas.

•	Implementar un sistema de autenticación estableciendo protocolos de seguridad para la protección de los datos clínicos y sensibles, asegurando el acceso controlado y la privacidad de la información.

## Metodología SCRUM
1. **Épica 1: Configuración y Preparación Inicial**
   - Configuración del entorno de desarrollo.
   - Establecimiento del repositorio y control de versiones.
   - Desarrollo de un prototipo en Figma para la interfaz del sistema.

2. **Épica 2: Diseño y Elección del Motor y Base de Datos**
   - Selección del motor de base de datos adecuado.
   - Diseño e implementación del esquema de la base de datos.
   - Configuración y prueba de la base de datos en el entorno de desarrollo.

3. **Épica 3: Gestión de Datos del Paciente**
   - Desarrollo de la interfaz de usuario para la introducción de datos.
   - Implementación del backend para la gestión de datos de pacientes.
   - Integración de mecanismos de validación y almacenamiento seguro de datos.

4. **Épica 4: Análisis y Visualización de Datos**
   - Diseño y desarrollo del módulo de visualización de datos.
   - Creación de gráficos y herramientas para el análisis de datos clínicos.

5. **Épica 5: Autenticación y Seguridad de Datos**
   - Implementación de un sistema de autenticación para diferentes roles de usuario.
   - Establecimiento de protocolos de seguridad para el manejo de datos clínicos.

6. **Épica 6: Pruebas y Refinamiento**
   - Realización de pruebas funcionales y de integración.
   - Ajustes y optimizaciones basadas en los resultados de las pruebas.

## Ruta crítica
## Fase 1: Definición y Prototipo
**Objetivo**: Crear una versión mínima viable (MVP) de la aplicación que permita almacenar, consultar y gestionar historias clínicas de forma local.
### Tecnología:
- Flask se utilizará para manejar la lógica de negocio y las interacciones con la base de datos (SQLite), pero el enfoque será ejecutar Flask localmente en la máquina del usuario.
- Usa PyInstaller o similar para generar un ejecutable local que el usuario final pueda ejecutar sin necesidad de instalar Python.
### Interfaz:
- Puedes optar por PyQt o Tkinter para desarrollar una interfaz gráfica nativa (GUI), o mantener Flask como backend con una interfaz web local.
### Tareas:
- Diseñar el flujo básico de la aplicación: Creación/edición de historias clínicas.
- Prototipar la lógica de Flask y las rutas principales (CRUD de historias clínicas).
- Si eliges usar Flask con interfaz web local, desarrollarla en HTML/CSS/JavaScript.
- Si eliges una GUI nativa, desarrollar ventanas y formularios con PyQt o Tkinter.
- Probar todo en entorno local antes de empaquetar.
- Empaquetar la aplicación en un ejecutable usando PyInstaller o py2exe.

---
## Fase 2: Desarrollo de Funcionalidades Avanzadas

**Objetivo**: Implementar las características avanzadas (evaluaciones neuropsicológicas, diagnósticos, seguimientos).
### Interfaz gráfica:
- Si estás usando una interfaz gráfica nativa (PyQt/Tkinter), diseña pantallas adicionales y formas de navegación entre las distintas secciones (evaluación neuropsicológica, áreas, etc.).
- Si mantienes la interfaz web local con Flask, expande el frontend usando tecnologías web.
### Tareas:
- Desarrollar el módulo de pruebas y subpruebas.
- Crear interfaces para registrar y visualizar diagnósticos, hipótesis y seguimientos.
- Pruebas de rendimiento local: Asegúrate de que la aplicación responde bien con diferentes volúmenes de datos en SQLite.
- Pruebas de empaquetado: Cada vez que completes una nueva característica, vuelve a empaquetar la aplicación con PyInstaller para probar la distribución.

---

## Fase 3: Pruebas de Seguimiento y Optimización
**Objetivo**: Asegurar que la aplicación local pueda escalar y que funcione correctamente bajo diversas condiciones.
### Escalabilidad local:
- Aunque SQLite puede manejar datos locales con facilidad, asegúrate de probar cómo funciona cuando tienes muchas historias clínicas o consultas frecuentes.
### Tareas:
- Realizar pruebas de carga local: Ver cómo reacciona la base de datos y la interfaz con muchos registros.
- Optimizar el manejo de archivos locales, si es necesario (copia de seguridad de la base de datos SQLite, gestión de archivos adjuntos o imágenes).
- Actualizar el empaquetado: Cada vez que optimices el sistema, prueba empaquetar nuevamente con PyInstaller para asegurarte de que sigue funcionando.

---

## Fase 4: Implementación del Seguimiento Futuro
**Objetivo**: Si deseas agregar seguimiento remoto o en línea en el futuro, este paso preparará tu aplicación para interactuar con una red.
### Decisiones:
- Aunque la aplicación será local inicialmente, podrías agregar funcionalidades de red más adelante (como sincronización con una base de datos central o la posibilidad de realizar copias de seguridad remotas).
- En esta fase podrías migrar a un sistema más escalable, si el crecimiento lo requiere.
### Tareas:
- Definir qué partes de la aplicación (si alguna) se podrían mover a la nube o necesitarían seguimiento remoto.
- Si es necesario, integrar un módulo para hacer copias de seguridad remotas (por ejemplo, usando una API web en un servidor externo).

---

## Estructura del proyecto
```bash
my_project/
│
├── app/
│   ├── _init_.py           # Inicializa la aplicación Flask
│   ├── routes/               # Directorio para las rutas (endpoints)
│   │   ├── _init_.py       # Importa todas las rutas
│   │   ├── pacientes.py      # Rutas para la entidad Pacientes
│   │   ├── historias_clinicas.py  # Rutas para Historias Clínicas
│   │   └── pruebas.py        # Rutas para Pruebas y Subpruebas
│   ├── models/               # Directorio para los modelos (tablas)
│   │   ├── _init_.py       # Importa todos los modelos
│   │   ├── paciente.py       # Modelo para la tabla Pacientes
│   │   ├── historia_clinica.py # Modelo para la tabla Historias Clínicas
│   │   └── prueba.py         # Modelo para la tabla Pruebas y Subpruebas
│   └── static/               # Archivos estáticos (CSS, JS, imágenes)
│
├── tests/                    # Pruebas unitarias y funcionales
│   ├── test_app.py           # Pruebas del backend de Flask
│   ├── test_gui.py           # Pruebas de la interfaz gráfica
│   └── test_database.py      # Pruebas de la base de datos
│
├── config.py                 # Configuraciones de la aplicación
├── app.py                    # Punto de entrada de la aplicación Flask
├── requirements.txt          # Dependencias del proyecto
└── README.md                 # Descripción general del proyecto
```
## Estado Actual del Proyecto

- **Épica 1 y 2:** Completas
- **Épica 3:** En progreso
- **Épica 4, 5 y 6:** No iniciadas

**Porcentaje de Avance:** 33.33%

## Cronograma y Planificación

- **Sprint 0 (15 de agosto - 30 de agosto):** Configuración y Preparación Inicial
- **Sprint 1 (31 de agosto - 13 de septiembre):** Diseño y Elección del Motor y Base de Datos
- **Sprint 2 (14 de septiembre - 27 de octubre):** Gestión de Datos del Paciente
- **Sprint 3 (27 de octubre - 14 de noviembre):** Pruebas y Refinamiento

Para consultar el cronograma detallado y la planificación del proyecto, por favor visita los siguientes enlaces:

- [Cronograma del Proyecto](https://upbeduco-my.sharepoint.com/my?id=%2Fpersonal%2Fluisa%5Fflorezm%5Fupb%5Fedu%5Fco%2FDocuments%2FProyecto%20CAP%2FCalendario%202024%20Proyecto%20CAP%2Epdf&parent=%2Fpersonal%2Fluisa%5Fflorezm%5Fupb%5Fedu%5Fco%2FDocuments%2FProyecto%20CAP&ga=1)
- [Tablero de Trello](https://trello.com/invite/b/66ce4e632567d46e7b3dadbd/ATTI91ce7cb6bb54337a79656335e98acbf358C4F0EE/proyecto-cap)

## Instrucciones para el Desarrollo

## Documentación

## Contacto

## Licencia

