# Proyecto 01 - Web de Venta de Ropa

## Información General

- **Nombre:**
  - Facundo

- **Correo Electrónico:**
  - facuperbak72@gmail.com

- **Proyecto:**
  - Web de Venta de Ropa

- **Repositorio:**
  - [https://github.com/pereirabaker/ClothingWeb](https://github.com/pereirabaker/ClothingWeb)

- **Tema:**
  - Desarrollo de una tienda en línea para la venta de ropa, implementada con una estructura **Modelo-Vista-Controlador (MVC)** básica y funcionalidades esenciales utilizando **Spring MVC**, **MySQL** y **Bootstrap CSS**.

---

## Descripción del Proyecto

La **Web de Venta de Ropa** es una aplicación diseñada para facilitar la compra y gestión de productos de moda en línea. El proyecto está estructurado siguiendo el patrón **Modelo-Vista-Controlador (MVC)**, lo que garantiza una separación clara de responsabilidades y facilita el mantenimiento y escalabilidad de la aplicación.

### Objetivos Principales

- **Registro de Usuarios:**
  - Permitir a los usuarios crear una cuenta proporcionando información básica como nombre de usuario y contraseña.
  
- **Autenticación de Usuarios:**
  - Facilitar el inicio de sesión para usuarios registrados, asegurando el acceso seguro a funcionalidades restringidas.
  
- **Gestión de Productos:**
  - Permitir la visualización, adición y gestión de productos de ropa disponibles para la venta.
  
- **Interfaz de Usuario Intuitiva:**
  - Desarrollar vistas amigables y responsivas utilizando **Thymeleaf** y **Bootstrap CSS** para una mejor experiencia de usuario.

---

## Funcionalidades Implementadas

### 1. Registro de Usuarios

- **Formulario de Registro:**
  - Solicita al usuario ingresar un **nombre de usuario** y una **contraseña**.
  - Al completar el registro exitoso, redirige al usuario a la página de **login**.

### 2. Autenticación de Usuarios

- **Página de Login:**
  - Valida las credenciales ingresadas contra los datos almacenados en la base de datos.
  - Tras una autenticación exitosa, redirige al usuario a la página principal de la tienda.

### 3. Gestión de Productos

- **Listado de Productos:**
  - Muestra una lista completa de los productos de ropa disponibles para la venta.

- **Formulario para Agregar Productos:**
  - Permite a los administradores añadir nuevos productos al catálogo.
  - Campos incluidos:
    - **Nombre del Producto**
    - **Descripción**
    - **Categoría**
    - **Precio**
    - **Imagen del Producto** (opcional)

---

## Mejoras Planificadas

### 1. Confirmación de Contraseña en el Registro

- **Objetivo:**
  - Añadir un campo de confirmación de contraseña en el formulario de registro para asegurar que el usuario haya ingresado correctamente su contraseña.

### 2. Validación de Unicidad de Usuario

- **Objetivo:**
  - Implementar una verificación que asegure que cada **nombre de usuario** sea único, evitando duplicados en la base de datos.

### 3. Retroalimentación al Usuario

- **Objetivo:**
  - Proporcionar mensajes claros de **error** o **éxito** durante los procesos de registro y login, mejorando la experiencia del usuario y facilitando la resolución de problemas.

### 4. Mejora en la Redirección Post-Login

- **Objetivo:**
  - Asegurar que, tras el login, el usuario sea redirigido de manera consistente a la página principal de la tienda, optimizando la navegación dentro de la aplicación.

### 5. Funcionalidad de Carrito de Compras

- **Objetivo:**
  - Permitir a los usuarios agregar productos a un **carrito de compras** y proceder al checkout para finalizar sus compras.

---

## Tareas de Desarrollo y Próximos Pasos

1. **Crear las Entidades del Proyecto:**
   - **Usuario:** Representa a los clientes registrados en la tienda.
   - **Producto:** Representa los artículos de ropa disponibles para la venta.
   - **Categoría:** Clasifica los productos en diferentes tipos o estilos.

2. **Implementar Repositories:**
   - **UsuarioRepository:** Maneja las operaciones CRUD para la entidad Usuario.
   - **ProductoRepository:** Maneja las operaciones CRUD para la entidad Producto.
   - **CategoriaRepository:** Maneja las operaciones CRUD para la entidad Categoría.

3. **Desarrollar Controladores:**
   - **UsuarioController:** Gestiona las rutas y lógica para el registro y login de usuarios.
   - **ProductoController:** Gestiona las rutas y lógica para la visualización y gestión de productos.
   - **CategoriaController:** Gestiona las rutas y lógica para la gestión de categorías de productos.

4. **Crear Vistas HTML Básicas:**
   - **home.html:** Página principal de la tienda.
   - **login.html:** Formulario de inicio de sesión.
   - **register.html:** Formulario de registro de nuevos usuarios.
   - **productos.html:** Página para listar los productos disponibles.
   - **nuevo_producto.html:** Formulario para agregar nuevos productos.

5. **Configuración de la Base de Datos:**
   - Establecer la conexión con **MySQL** en el archivo `application.properties`.
   - Asegurar que las tablas se creen correctamente utilizando `spring.jpa.hibernate.ddl-auto=update`.

6. **Pruebas y Depuración:**
   - Realizar pruebas unitarias y de integración para asegurar que todas las funcionalidades implementadas funcionan correctamente.
   - Depurar problemas relacionados con la persistencia de datos y la autenticación de usuarios.

---

## Recomendaciones y Buenas Prácticas

1. **Enfoque en el MVP (Producto Mínimo Viable):**
   - Priorizar el desarrollo de funcionalidades esenciales antes de agregar características más complejas.
   - Asegurar que el MVP esté completamente funcional antes de iterar sobre mejoras y expansiones.

2. **Mantenimiento del Código:**
   - Mantener una estructura de código limpia y bien documentada.
   - Utilizar convenciones de nomenclatura consistentes y comentarios claros para facilitar la colaboración y el mantenimiento a largo plazo.

3. **Validaciones de Datos:**
   - Implementar validaciones tanto en el frontend como en el backend para asegurar la integridad de los datos y prevenir entradas no deseadas.

---

## Conclusión

La **Web de Venta de Ropa** está en una fase inicial con la implementación de funcionalidades básicas de registro, login y gestión de productos. Se está priorizando la creación de una base sólida siguiendo el patrón **Modelo-Vista-Controlador (MVC)**, lo que permitirá añadir funcionalidades más complejas en etapas posteriores de manera eficiente y estructurada. Las próximas etapas se enfocarán en mejorar la seguridad, optimizar la experiencia del usuario y expandir las capacidades de la tienda en línea con características adicionales como el carrito de compras y el checkout.
