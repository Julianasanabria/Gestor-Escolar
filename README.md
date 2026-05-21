<div align="center">
  <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Travel%20and%20places/School.png" alt="School" width="90" />
  <h1>EduGestion API • Backend</h1>
  
  <p>
    <a href="https://nodejs.org/"><img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" /></a>
    <a href="https://expressjs.com/"><img src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white" /></a>
    <a href="https://www.mongodb.com/"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" /></a>
    <a href="https://jwt.io/"><img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=JSON%20web%20tokens&logoColor=white" /></a>
    <a href="https://jestjs.io/"><img src="https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=Jest&logoColor=white" /></a>
  </p>
  
  <blockquote>
    <strong>EduGestion</strong> es una API REST diseñada para la administración integral de instituciones educativas. Facilita la gestión de matrículas, carga académica, calificaciones y la generación automatizada de boletines escolares en PDF, sirviendo como la columna vertebral tecnológica para plataformas educativas modernas.
  </blockquote>
</div>

<br/>

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Travel%20and%20places/Rocket.png" alt="Rocket" width="25" /> Características Clave

*   **🔐 Autenticación y Seguridad:** Registro e inicio de sesión seguros con cifrado de contraseñas mediante **Bcrypt** y autorización basada en roles utilizando **JSON Web Tokens (JWT)**.
*   **📚 Gestión de Carga Académica:** Asignación flexible de docentes a grupos, sedes y asignaturas específicas.
*   **📝 Calificaciones:** Control detallado de notas con indicadores de logro personalizados y cálculo de promedios periódicos.
*   **📄 Boletines en Tiempo Real:** Motor de generación de reportes académicos en formato PDF de alta densidad utilizando **PDFKit**.
*   **✉️ Notificaciones:** Integración con **Nodemailer** para validación de servicios y envío automático de correos.
*   **🛡️ Validación de Datos:** Sanitización y validación de payloads en cada endpoint con **Express-Validator**.
*   **🧪 Pruebas Automatizadas:** Pruebas unitarias y de integración implementadas con **Jest** y **Supertest**.

<br/>

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Hammer%20and%20Wrench.png" alt="Tools" width="25" /> Stack Tecnológico

![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![Jest](https://img.shields.io/badge/-jest-%23C21325?style=for-the-badge&logo=jest&logoColor=white)

*   **Runtime:** Node.js (v18+)
*   **Framework Web:** Express.js (v5.x)
*   **Base de Datos:** MongoDB & Mongoose (ODM)
*   **Herramientas Extra:** PDFKit, Nodemailer, ES Modules

<br/>

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Open%20File%20Folder.png" alt="Folder" width="25" /> Arquitectura del Proyecto (MVC)

El proyecto sigue una estructura limpia y mantenible basada en **Modelo-Vista-Controlador (MVC)**:

```bash
├── 📁 controllers      # Lógica de negocio
├── 📁 models           # Esquemas de datos (Mongoose)
├── 📁 routes           # Endpoints de la API REST
├── 📁 middlewares      # Validadores (JWT, roles)
├── 📁 services         # Servicios de terceros
├── 📁 helpers          # Utilidades reutilizables
├── 📁 utils            # Clases utilitarias
├── 📁 tests            # Suite de pruebas (Jest)
├── 📄 app.js           # Configuración del servidor
└── 📄 package.json     # Dependencias y scripts
```

<br/>

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Vertical%20Traffic%20Light.png" alt="Traffic Light" width="25" /> Endpoints Principales

| Entidad | Endpoint Base | Operaciones Soportadas |
| :--- | :--- | :--- |
| **Usuarios** | `/api/users` | Registro, Login, Gestión de Roles |
| **Carga Académica** | `/api/academicLoad` | Asignación de docentes a materias |
| **Estudiantes** | `/api/registration` | Procesos de matrícula |
| **Grupos / Grados** | `/api/groups` | Creación de cursos |
| **Calificaciones** | `/api/qualifications` | Registro y edición de notas |
| **Boletines** | `/api/bulletins` | Generación de PDFs |
| **Indicadores** | `/api/indicators` | Gestión de logros académicos |
| **Materias** | `/api/subjects` | Administración del pensum |

<br/>

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Gear.png" alt="Gear" width="25" /> Instalación Local

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/ProyectoAdsoSocorro/Proyecto-final.git
   cd Proyecto-final
   ```

2. **Instalar dependencias:**
   ```bash
   npm install
   ```

3. **Variables de entorno (`.env`):**
   ```env
   PORT=3000
   MONGO_URL=tu_cadena_de_conexion
   JWT_SECRET=tu_secreto_seguro
   EMAIL_HOST=smtp.tuservicio.com
   EMAIL_PORT=587
   EMAIL_USER=tu_correo@ejemplo.com
   EMAIL_PASS=tu_contraseña
   ```

4. **Iniciar Servidor / Pruebas:**
   ```bash
   npm start          # Modo producción
   npm test           # Ejecutar pruebas
   npm run test:watch # Pruebas en modo desarrollo
   ```

<br/>

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Smilies/Glowing%20Star.png" alt="Star" width="25" /> Buenas Prácticas Implementadas

- **Clean Code & SOLID:** Separación de responsabilidades.
- **Seguridad Activa:** Verificación JWT y roles jerárquicos.
- **Integridad de Datos:** `express-validator` y esquemas estrictos.
- **Async/Await:** Código asíncrono limpio, evitando callback hell.

<br/>

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/People/Bust%20in%20Silhouette.png" alt="Silhouette" width="25" /> Liderazgo y Desarrollo

Este sistema fue desarrollado como proyecto final de grado, marcando un paso invaluable en mi aprendizaje y mi transición hacia el desarrollo de software profesional. 

Durante su ejecución, tuve el gran reto y la oportunidad de asumir el rol de **Líder de Equipo**. Desde esta posición, colaboré activamente en la coordinación de la arquitectura del backend y facilité la distribución ágil de tareas junto con mis compañeros. Ha sido un proceso de mucho esfuerzo colectivo, donde mi objetivo fue asegurar la aplicación de conceptos avanzados y buenas prácticas de ingeniería, aprendiendo continuamente de los desafíos técnicos y del trabajo en equipo.

*   **GitHub:** [Julianasanabria](https://github.com/Julianasanabria)
*   **LinkedIn:** [Karen Juliana Sanabria](https://linkedin.com/in/karen-Juliana-Sanabria)

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=timeGradient&height=150&section=footer"/>
</p>
