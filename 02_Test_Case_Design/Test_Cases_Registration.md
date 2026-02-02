# Test Cases – User Registration

## 1. Introducción

Este documento contiene los **casos de prueba manuales** para la funcionalidad de **Registro de Usuario** de una aplicación web.  
El objetivo es validar que los usuarios puedan registrarse correctamente, que las validaciones sean correctas y que el sistema maneje errores de manera adecuada.

## 2. Supuestos y Alcance

- El formulario de registro requiere: nombre completo, correo electrónico, contraseña, confirmación de contraseña.  
- Validaciones de formato y obligatoriedad de campos están activas.  
- Se aplican restricciones de seguridad mínima para la contraseña.  

## 3. Casos de Prueba

### 🧪 TC-REG-001 – Registro exitoso con datos válidos

| Campo | Detalle |
|-------|---------|
| Test Case ID | TC-REG-001 |
| Test Case Name | Registro exitoso |
| Módulo | Registro de Usuario |
| Requerimiento | RF-REG-01 |
| Prioridad | Alta |
| Tipo de Prueba | Funcional |
| Precondiciones | Ninguna |
| Ambiente | QA |

**Pasos de Prueba**

| Paso | Acción | Datos de Prueba | Resultado Esperado |
|------|--------|-----------------|--------------------|
| 1 | Ingresar nombre | Juan Pérez | Campo acepta valor |
| 2 | Ingresar correo | juan@test.com | Campo acepta valor |
| 3 | Ingresar contraseña | Password123! | Campo acepta valor |
| 4 | Confirmar contraseña | Password123! | Coincide con contraseña |
| 5 | Hacer clic en “Registrar” | — | Usuario registrado exitosamente |

**Resultado Esperado Final**  
Se muestra mensaje de confirmación y usuario es creado en el sistema.

### 🧪 TC-REG-002 – Registro con correo ya existente

| Campo | Detalle |
|-------|---------|
| Test Case ID | TC-REG-002 |
| Test Case Name | Correo duplicado |
| Módulo | Registro de Usuario |
| Requerimiento | RF-REG-02 |
| Prioridad | Alta |
| Tipo de Prueba | Negativa |
| Precondiciones | Usuario existente: juan@test.com |
| Ambiente | QA |

**Resultado Esperado Final**  
El sistema muestra mensaje de error: “El correo ya está registrado”.

### 🧪 TC-REG-003 – Registro con contraseña débil

| Campo | Detalle |
|-------|---------|
| Test Case ID | TC-REG-003 |
| Test Case Name | Contraseña débil |
| Módulo | Registro de Usuario |
| Requerimiento | RF-REG-03 |
| Prioridad | Media |
| Tipo de Prueba | Negativa |
| Precondiciones | Ninguna |
| Ambiente | QA |

**Datos de Prueba**  
Contraseña: `12345`

**Resultado Esperado Final**  
El sistema muestra mensaje: “La contraseña debe tener al menos 8 caracteres, incluir mayúsculas, minúsculas, un número y al menos un caracter especial”.

### 🧪 TC-REG-004 – Campos obligatorios vacíos

| Campo | Detalle |
|-------|---------|
| Test Case ID | TC-REG-004 |
| Test Case Name | Validación de campos vacíos |
| Módulo | Registro de Usuario |
| Requerimiento | RF-REG-04 |
| Prioridad | Alta |
| Tipo de Prueba | Validación |
| Precondiciones | Ninguna |
| Ambiente | QA |

**Resultado Esperado Final**  
El sistema indica qué campos son obligatorios y no permite continuar hasta completarlos.

### 🧪 TC-REG-005 – Formato de correo inválido

| Campo | Detalle |
|-------|---------|
| Test Case ID | TC-REG-005 |
| Test Case Name | Validación de formato de correo |
| Módulo | Registro de Usuario |
| Requerimiento | RF-REG-05 |
| Prioridad | Media |
| Tipo de Prueba | Validación |
| Precondiciones | Ninguna |
| Ambiente | QA |

**Datos de Prueba**  
Correo: `juan@test`  

**Resultado Esperado Final**  
El sistema no permite continuar y muestra mensaje: “Formato de correo inválido”.

### 🧪 TC-REG-006 – Confirmación de contraseña no coincide

| Campo | Detalle |
|-------|---------|
| Test Case ID | TC-REG-006 |
| Test Case Name | Contraseña y confirmación no coinciden |
| Módulo | Registro de Usuario |
| Requerimiento | RF-REG-06 |
| Prioridad | Alta |
| Tipo de Prueba | Negativa |
| Precondiciones | Ninguna |
| Ambiente | QA |

**Datos de Prueba**  
Contraseña: `Password123!`  
Confirmación: `Password124!`

**Resultado Esperado Final**  
El sistema muestra mensaje: “Las contraseñas no coinciden”.

### 🧪 TC-REG-007 – Registro con límite de caracteres en nombre

| Campo | Detalle |
|-------|---------|
| Test Case ID | TC-REG-007 |
| Test Case Name | Validación de longitud de nombre |
| Módulo | Registro de Usuario |
| Requerimiento | RF-REG-07 |
| Prioridad | Media |
| Tipo de Prueba | Validación / BVA |
| Precondiciones | Ninguna |
| Ambiente | QA |

**Datos de Prueba**  
Nombre: 2 caracteres (mínimo) / 50 caracteres (máximo)  

**Resultado Esperado Final**  
El sistema permite registrar nombres entre 2 y 50 caracteres y muestra mensaje de error si se excede o es menor al mínimo.

## 4. Consideraciones Adicionales

- Se aplican **partición de equivalencia** y **análisis de valores límite**  
- Priorización basada en **impacto al usuario**  
- Incluye casos positivos y negativos

## 5. Conclusión

El registro de usuarios es una **funcionalidad crítica**, y estos casos aseguran que el flujo sea robusto, seguro y con una **experiencia de usuario confiable**.