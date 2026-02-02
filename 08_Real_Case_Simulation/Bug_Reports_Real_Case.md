# Reportes de Bugs – Simulación de Caso Real QA Manual

## 1. Introducción

Este documento contiene ejemplos de **reportes de bugs** detectados durante la ejecución de pruebas manuales del **Sistema de Gestión de Usuarios**.

Los bugs están documentados siguiendo buenas prácticas de QA, incluyendo pasos claros para reproducir, resultados esperados, severidad, prioridad e impacto en el negocio.

## 2. Convenciones

- **Bug ID:** Identificador único del defecto
- **Severidad:** Impacto del defecto en el sistema
- **Prioridad:** Urgencia de corrección
- **Estado:** Nuevo / En Progreso / Resuelto / Cerrado

## 3. Reporte de Bug – BUG-001

- **Título:** El sistema permite iniciar sesión con contraseña incorrecta
- **Módulo:** Login
- **Severidad:** Crítica
- **Prioridad:** Alta
- **Estado:** Nuevo

### Pasos para reproducir:
1. Acceder a la página de login
2. Ingresar correo válido
3. Ingresar una contraseña incorrecta
4. Hacer clic en “Iniciar sesión”

### Resultado esperado:
El sistema debe mostrar un mensaje de error y no permitir el acceso.

### Resultado actual:
El sistema permite el acceso con credenciales incorrectas.

### Impacto:
Compromete la seguridad del sistema y bloquea la liberación del producto.

## 4. Reporte de Bug – BUG-002

- **Título:** Mensaje poco claro al intentar registrar un correo duplicado
- **Módulo:** Registro
- **Severidad:** Media
- **Prioridad:** Media
- **Estado:** Nuevo

### Pasos para reproducir:
1. Acceder a la página de registro
2. Ingresar un correo previamente registrado
3. Completar el resto de los campos
4. Hacer clic en “Registrar”

### Resultado esperado:
Mensaje claro indicando que el correo ya está registrado.

### Resultado actual:
Mensaje genérico que no indica claramente el error.

### Impacto:
Afecta la experiencia del usuario y puede generar confusión.

## 5. Observaciones Generales

- Los bugs críticos deben corregirse antes del release
- Los bugs de severidad media pueden evaluarse según impacto y tiempo
- Todos los bugs deben re-ejecutarse después de su corrección

## 6. Conclusión

El reporte adecuado de bugs permite una **comunicación clara entre QA, desarrollo y negocio**, reduciendo tiempos de corrección y mejorando la calidad del producto.