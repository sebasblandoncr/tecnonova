# TecnoNova – Tienda en línea de dispositivos electrónicos

Proyecto final del curso **SC-403 Desarrollo de Aplicaciones Web y Patrones** – Universidad Fidélitas.

## Descripción

TecnoNova es una aplicación web transaccional para la venta de dispositivos electrónicos (laptops, celulares, tablets, audio, smartwatch y accesorios). Permite a los clientes registrarse, consultar el catálogo, filtrar productos, gestionar un carrito y confirmar pedidos. El administrador gestiona los dispositivos y el inventario.

## Objetivo

Desarrollar una solución web con Java y Spring Boot que facilite la venta en línea de dispositivos electrónicos y el control de inventario, aplicando arquitectura MVC, persistencia con JPA, autenticación por roles e internacionalización.

## Integrantes

| Nombre | Usuario de GitHub |
|---|---|
| Sebastián Blandón | @sebasblandoncr |
| Nombre Apellido | @usuario |
| Nombre Apellido | @usuario |
| Nombre Apellido | @usuario |

## Roles del sistema

- **Cliente:** registro, inicio de sesión, catálogo, carrito, pedidos e historial de compras.
- **Administrador:** gestión de dispositivos (CRUD) e inventario.

## Tecnologías previstas

- Java 21 + Spring Boot
- Thymeleaf (plantillas y fragmentos)
- Bootstrap
- Spring Data JPA / Hibernate
- MySQL
- Spring Security (autenticación y roles)
- Internacionalización con archivos `messages.properties` (español / inglés)
- Git y GitHub

## Estructura del proyecto (prevista)

```
src/main/java/com/tecnonova/
├── controller/
├── service/
├── repository/
└── domain/
src/main/resources/
├── templates/
├── static/
├── messages.properties
└── application.properties
```

## Ejecución (preliminar)

1. Clonar el repositorio:
   ```
   git clone https://github.com/USUARIO/tecnonova.git
   ```
2. Crear la base de datos `tecnonova` en MySQL.
3. Configurar usuario y contraseña de la base de datos en `application.properties` (no subir credenciales reales).
4. Ejecutar el proyecto desde NetBeans / IntelliJ o con:
   ```
   mvn spring-boot:run
   ```
5. Abrir `http://localhost:8080` en el navegador.

## Estado del proyecto

**Avance 1 (semana 5):** historias de usuario, prototipo, mapa de navegación, modelo preliminar de datos y repositorio inicial.

## Forma de trabajo

El acuerdo de trabajo por ramas está en [CONTRIBUTING.md](CONTRIBUTING.md).
