# Acuerdo de trabajo por ramas

Este documento describe cómo trabaja el equipo en el repositorio.

## Ramas

| Rama | Uso |
|---|---|
| `main` | Versión estable del proyecto. **No se trabaja directamente sobre ella.** |
| `develop` | Rama de integración. Aquí se unen las funcionalidades antes de pasar a `main`. |
| `feature/nombre` | Una rama por funcionalidad. Ej.: `feature/registro-cliente`, `feature/carrito`, `feature/gestion-dispositivos`. |
| `fix/nombre` | Corrección de errores. Ej.: `fix/validacion-registro`. |
| `docs/nombre` | Cambios de documentación. Ej.: `docs/readme`. |

Los nombres de rama van en minúscula, sin tildes y separados por guiones.

## Flujo de trabajo

1. Actualizar `develop` antes de empezar:
   ```
   git checkout develop
   git pull origin develop
   ```
2. Crear la rama de la funcionalidad:
   ```
   git checkout -b feature/nombre-funcionalidad
   ```
3. Hacer commits pequeños y descriptivos.
4. Subir la rama:
   ```
   git push origin feature/nombre-funcionalidad
   ```
5. Abrir un **Pull Request hacia `develop`** en GitHub.
6. Al menos **otro integrante** revisa el PR (código, prueba funcional, estilos) antes de aprobarlo.
7. Si hay observaciones o conflictos, se corrigen en la misma rama.
8. Una vez aprobado, se hace el merge y se borra la rama.
9. Antes de cada entrega, `develop` se une a `main` mediante un PR revisado por el equipo.

## Mensajes de commit

Formato: `tipo: descripción corta en presente`

| Tipo | Ejemplo |
|---|---|
| `feat` | `feat: agrega formulario de registro de cliente` |
| `fix` | `fix: corrige validación de correo duplicado` |
| `docs` | `docs: actualiza instrucciones de ejecución` |
| `style` | `style: ajusta estilos del catálogo` |
| `refactor` | `refactor: mueve lógica del carrito al servicio` |

No se aceptan commits vacíos o con mensajes como "cambios", "avance" o "asdf".

## Reglas del equipo

- Cada integrante trabaja con **su propia cuenta** de GitHub.
- Las historias de usuario o tareas se registran como **Issues** y se asignan a un responsable.
- Un PR debe hacer referencia al issue o historia que resuelve (ej.: `Cierra #5 – HU-06`).
- No se suben contraseñas, tokens ni credenciales reales.
- Se hace `git pull` de `develop` con frecuencia para evitar conflictos acumulados.
