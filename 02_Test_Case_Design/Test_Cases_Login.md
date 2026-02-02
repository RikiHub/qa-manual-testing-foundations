# Test Cases – Login

## 1. Introducción

Este documento contiene los **casos de prueba manuales** para la funcionalidad de **Inicio de Sesión (Login)** de una aplicación web.

El objetivo es validar que el sistema permita el acceso a usuarios registrados, maneje correctamente credenciales inválidas y muestre mensajes claros al usuario.

## 2. Supuestos y Alcance

- El usuario ya está registrado en el sistema
- El login se realiza mediante **correo electrónico y contraseña**
- El sistema muestra mensajes de error ante credenciales inválidas

## 3. Casos de Prueba

### 🧪 TC-LOGIN-001 – Login exitoso con credenciales válidas

| Campo | Detalle |
|-------|-----------|
| Test Case ID | TC-LOGIN-001 |
| Test Case Name | Login exitoso con credenciales válidas |
| Módulo | Autenticación |
| Requerimiento | RF-LOGIN-01 |
| Prioridad | Alta |
| Tipo de Prueba | Funcional |
| Precondiciones | Usuario registrado y activo |
| Ambiente | QA |

**Pasos de Prueba**

| Paso | Acción | Datos de Prueba | Resultado Esperado |
|------|--------|-----------------|--------------------|
| 1 | Ingresar correo válido | user@test.com | Campo acepta el valor |
| 2 | Ingresar contraseña válida | Password123 | Campo acepta el valor |
| 3 | Hacer clic en “Login” | — | Usuario accede al sistema |

**Resultado Esperado Final**  
El sistema permite el acceso y redirige al dashboard principal.

### 🧪 TC-LOGIN-002 – Login con contraseña incorrecta

| Campo | Detalle |
|-------|---------|
| Test Case ID | TC-LOGIN-002 |
| Test Case Name | Login con contraseña incorrecta |
| Módulo | Autenticación |
| Requerimiento | RF-LOGIN-02 |
| Prioridad | Alta |
| Tipo de Prueba | Negativa |
| Precondiciones | Usuario registrado |
| Ambiente | QA |

**Pasos de Prueba**

| Paso | Acción | Datos de Prueba | Resultado Esperado |
|------|--------|-----------------|--------------------|
| 1 | Ingresar correo válido | user@test.com | Campo acepta el valor |
| 2 | Ingresar contraseña inválida | WrongPass | Campo acepta el valor |
| 3 | Hacer clic en “Login” | — | Se muestra mensaje de error |

**Resultado Esperado Final**  
El sistema no permite el acceso y muestra un mensaje de credenciales incorrectas.

### 🧪 TC-LOGIN-003 – Login con correo no registrado

| Campo | Detalle |
|-------|---------|
| Test Case ID | TC-LOGIN-003 |
| Test Case Name | Login con correo no registrado |
| Módulo | Autenticación |
| Requerimiento | RF-LOGIN-03 |
| Prioridad | Media |
| Tipo de Prueba | Negativa |
| Precondiciones | Ninguna |
| Ambiente | QA |

**Resultado Esperado**  
El sistema muestra mensaje indicando que el usuario no existe.

### 🧪 TC-LOGIN-004 – Login con campos vacíos

| Campo | Detalle |
|-------|---------|
| Test Case ID | TC-LOGIN-004 |
| Test Case Name | Login con campos vacíos |
| Módulo | Autenticación |
| Requerimiento | RF-LOGIN-04 |
| Prioridad | Alta |
| Tipo de Prueba | Validación |
| Precondiciones | Ninguna |
| Ambiente | QA |

**Resultado Esperado**  
El sistema muestra mensajes de validación indicando que los campos son obligatorios.

### 🧪 TC-LOGIN-005 – Login con formato de correo inválido

| Campo | Detalle |
|-------|---------|
| Test Case ID | TC-LOGIN-005 |
| Test Case Name | Login con correo inválido |
| Módulo | Autenticación |
| Requerimiento | RF-LOGIN-05 |
| Prioridad | Media |
| Tipo de Prueba | Validación |
| Precondiciones | Ninguna |
| Ambiente | QA |

**Datos de Prueba**  
Correo: `user@com`

**Resultado Esperado**  
El sistema no permite continuar y muestra mensaje de formato inválido.

### 🧪 TC-LOGIN-006 – Sensibilidad a mayúsculas en contraseña

| Campo | Detalle |
|-------|---------|
| Test Case ID | TC-LOGIN-006 |
| Test Case Name | Validar sensibilidad de mayúsculas en contraseña |
| Módulo | Autenticación |
| Requerimiento | RF-LOGIN-06 |
| Prioridad | Media |
| Tipo de Prueba | Funcional |
| Precondiciones | Usuario registrado |
| Ambiente | QA |

**Resultado Esperado**  
El sistema distingue entre mayúsculas y minúsculas en la contraseña.

## 4. Consideraciones Adicionales

- Estos casos cubren escenarios positivos y negativos
- Se aplican principios de **partición de equivalencia**
- Se priorizan flujos críticos por impacto al usuario

## 5. Conclusión

La funcionalidad de Login representa un **punto crítico del sistema**, por lo que requiere pruebas exhaustivas y bien priorizadas para minimizar riesgos de acceso y experiencia negativa del usuario.