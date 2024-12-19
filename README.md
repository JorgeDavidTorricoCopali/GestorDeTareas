# Gestor de Tareas

Un sistema completo para la gestión de usuarios y tareas, desarrollado en Java utilizando Swing para la interfaz gráfica. Este proyecto permite a los administradores y trabajadores gestionar tareas con facilidad y eficacia.

## Tabla de Contenidos

1. [Descripción](#descripción)
2. [Características](#características)
3. [Requisitos Previos](#requisitos-previos)
4. [Instalación](#instalación)
5. [Uso](#uso)
6. [Arquitectura del Proyecto](#arquitectura-del-proyecto)
7. [Estructura de Archivos](#estructura-de-archivos)
8. [Contribuciones](#contribuciones)
9. [Licencia](#licencia)

---

## Descripción

El **Gestor de Tareas** es una aplicación de escritorio que permite a los usuarios registrar cuentas, iniciar sesión, recuperar contraseñas, y gestionar tareas asignadas. Los roles incluyen:

- **Administrador**: Puede crear tareas para cualquier trabajador, modificarlas o eliminarlas.
- **Trabajador**: Puede ver y gestionar las tareas asignadas a sí mismo.

---

## Características

- **Gestión de Cuentas**:
  - Registro de cuentas para administradores y trabajadores.
  - Recuperación de contraseñas con validación por código de seguridad.
  
- **Gestión de Tareas**:
  - Asignación de tareas por parte de los administradores.
  - Visualización de tareas con filtrado y búsqueda.
  - Modificación y eliminación de tareas.

- **Interfaz Gráfica**:
  - Aplicación responsiva con un diseño limpio usando Swing.
  - Tablas con colores asignados a usuarios para mejor legibilidad.

---

## Requisitos Previos

Antes de comenzar, asegúrate de tener lo siguiente instalado:

- **Java JDK** (versión 8 o superior)
- **IDE** para Java (Eclipse, IntelliJ IDEA, o NetBeans)
- Sistema operativo Windows, macOS o Linux.

---

## Instalación

1. Clona este repositorio:
   ```bash
   git clone [https://github.com/tu-usuario/gestor-de-tareas.git](https://github.com/JorgeDavidTorricoCopali/GestorDeTareas/tree/08766d406768a169f9cc356fff910fa9df61e92c)
   ```

2. Abre el proyecto en tu IDE preferido.

3. Asegúrate de que los archivos `users.txt` y `tasks.txt` existan en el directorio raíz del proyecto. Si no, créalos manualmente.

4. Ejecuta el archivo `Login.java` para iniciar la aplicación.

---

## Uso

### Iniciar Sesión
1. Ejecuta `Login.java`.
2. Introduce tus credenciales o crea una cuenta nueva.

### Funciones Principales
#### Para Administradores
- Crear cuentas de trabajadores.
- Asignar tareas, con opciones para definir:
  - Descripción
  - Prioridad (Alta, Media, Baja)
  - Fecha límite
  - Estado (Pendiente, En proceso, Completada)

#### Para Trabajadores
- Visualizar y buscar tareas asignadas.
- Modificar estados de tareas según el progreso.

### Recuperar Contraseña
- Selecciona "Olvidé la contraseña".
- Introduce el nombre completo, nombre de usuario y código de seguridad para restablecerla.

---

## Arquitectura del Proyecto

El proyecto está dividido en las siguientes partes principales:

1. **Interfaz de Usuario**:
   - `Login.java`: Maneja el inicio de sesión.
   - `CreateAccountWindow.java`: Permite la creación de cuentas.
   - `AdminForm.java` y `WorkerForm.java`: Formularios para registro de usuarios.
   - `TaskManagementWindow.java`: Ventana principal para la gestión de tareas.
   - `PasswordRecovery.java`: Recuperación de contraseñas.

2. **Gestión de Archivos**:
   - `FileManager.java`: Lee y escribe información de usuarios y tareas en archivos.

3. **Lógica de Negocio**:
   - `Task.java`: Clase que representa las tareas, con atributos como descripción, prioridad y estado.

---

## Estructura de Archivos

```plaintext
src/
├── AdminForm.java
├── CreateAccountWindow.java
├── FileManager.java
├── Login.java
├── PasswordRecovery.java
├── Task.java
├── TaskManagementWindow.java
├── WorkerForm.java
resources/
├── users.txt       # Archivo para almacenamiento de usuarios
├── tasks.txt       # Archivo para almacenamiento de tareas
├── userColors.dat  # Archivo para colores personalizados
```

---

## Contribuciones

¡Contribuciones son bienvenidas! Por favor:

1. Haz un fork del repositorio.
2. Crea una rama (`git checkout -b feature/nueva-funcion`).
3. Realiza un pull request cuando tu función esté lista.


