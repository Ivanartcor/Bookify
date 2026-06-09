# Bookify — Frontend

Bookify es una plataforma web para la gestión de citas entre clientes, empresas y empleados. El objetivo del proyecto es ofrecer una solución intuitiva para buscar empresas y servicios, reservar citas, gestionar disponibilidad, consultar citas asignadas y facilitar la comunicación entre los distintos perfiles de usuario.

Este repositorio contiene el frontend de la aplicación, desarrollado con Angular.

---

## Descripción general

Bookify está diseñado como una plataforma multirol:

* **Clientes:** pueden buscar empresas, consultar servicios, reservar citas, gestionar su perfil y revisar sus citas.
* **Empresas:** pueden administrar servicios, empleados, disponibilidad, citas, categorías y datos asociados a su negocio.
* **Empleados:** pueden consultar y gestionar las citas que tienen asignadas.
* **Usuarios no autenticados:** pueden acceder a secciones informativas como contacto, FAQ o política de privacidad.

La aplicación se comunica con una API REST desarrollada en NestJS y MySQL.

Repositorio backend:
`https://github.com/Ivanartcor/bookify-backend`

---

## Tecnologías utilizadas

* Angular 16
* TypeScript
* HTML
* SCSS
* Bootstrap
* Bootstrap Icons
* RxJS
* FullCalendar
* Chart.js
* ECharts / ngx-echarts
* Angular Router
* Guards de autenticación y roles
* Servicios HTTP para comunicación con API REST

---

## Funcionalidades principales

* Autenticación de usuarios.
* Separación de vistas por rol: cliente, empresa y empleado.
* Rutas protegidas mediante guardias de autenticación.
* Gestión de perfil de usuario.
* Gestión de empresas y servicios.
* Reserva y consulta de citas.
* Gestión de citas por cliente, empresa y empleado.
* Visualización de calendarios.
* Formularios y validaciones.
* Secciones informativas: FAQ, contacto y política de privacidad.
* Interfaz responsive orientada a una experiencia clara y funcional.

---

## Estructura general del proyecto

```text
src/
├── app/
│   ├── core/              # Guards, servicios base y lógica compartida
│   ├── features/
│   │   ├── auth/          # Login, registro y autenticación
│   │   ├── client/        # Área de cliente
│   │   ├── company/       # Área de empresa
│   │   ├── employee/      # Área de empleado
│   │   ├── contacto/      # Página de contacto
│   │   ├── faq/           # Preguntas frecuentes
│   │   └── politica-privacidad/
│   ├── shared/            # Componentes o recursos compartidos
│   └── app-routing.module.ts
```

---

## Instalación y ejecución

### Requisitos previos

* Node.js
* npm
* Angular CLI

### Instalar dependencias

```bash
npm install
```

### Ejecutar en desarrollo

```bash
ng serve
```

La aplicación estará disponible en:

```text
http://localhost:4200/
```

---

## Conexión con el backend

Este frontend está pensado para trabajar junto al backend de Bookify:

```text
https://github.com/Ivanartcor/bookify-backend
```

Antes de ejecutar la aplicación completa, asegúrate de tener el backend configurado y levantado correctamente.

---

## Scripts disponibles

```bash
npm start
```

Ejecuta la aplicación en modo desarrollo.

```bash
npm run build
```

Genera la versión compilada de producción.

```bash
npm test
```

Ejecuta las pruebas configuradas en Angular.

---

## Estado del proyecto

Proyecto desarrollado como plataforma full stack de gestión de citas, con enfoque en arquitectura por roles, consumo de API REST, diseño responsive y organización modular del frontend.



