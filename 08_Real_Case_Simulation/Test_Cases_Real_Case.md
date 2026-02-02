# Casos de Prueba – Simulación de Caso Real QA Manual

## 1. Introducción

Este documento contiene los **casos de prueba manuales** diseñados para validar las funcionalidades del **Sistema de Gestión de Usuarios**.

Los casos de prueba están alineados con los requerimientos del sistema y siguen buenas prácticas de QA para asegurar claridad, trazabilidad y correcta ejecución.

## 2. Convenciones

- **TC ID:** Identificador único del caso de prueba
- **Precondición:** Estado necesario antes de ejecutar el caso
- **Resultado esperado:** Comportamiento esperado del sistema
- **Resultado actual:** Comportamiento observado durante la ejecución
- **Estado:** Pass / Fail

## 3. Casos de Prueba – Login

### TC-LOGIN-001 – Inicio de sesión con credenciales válidas (Happy Path)

- **Precondición:** Usuario registrado y activo
- **Pasos:**
  1. Acceder a la página de login
  2. Ingresar correo válido
  3. Ingresar contraseña válida
  4. Hacer clic en “Iniciar sesión”
- **Resultado esperado:** El usuario accede al sistema correctamente
- **Resultado actual:** —
- **Estado:** —

### TC-LOGIN-002 – Inicio de sesión con contraseña incorrecta

- **Precondición:** Usuario registrado
- **Pasos:**
  1. Acceder a la página de login
  2. Ingresar correo válido
  3. Ingresar contraseña incorrecta
  4. Hacer clic en “Iniciar sesión”
- **Resultado esperado:** El sistema muestra mensaje de error y no permite el acceso
- **Resultado actual:** —
- **Estado:** —

### TC-LOGIN-003 – Inicio de sesión con correo no registrado

- **Precondición:** Ninguna
- **Pasos:**
  1. Acceder a la página de login
  2. Ingresar correo no registrado
  3. Ingresar cualquier contraseña
  4. Hacer clic en “Iniciar sesión”
- **Resultado esperado:** Mensaje de usuario no encontrado
- **Resultado actual:** —
- **Estado:** —

## 4. Casos de Prueba – Registro de Usuario

### TC-REG-001 – Registro con datos válidos (Happy Path)

- **Precondición:** Correo no registrado
- **Pasos:**
  1. Acceder a la página de registro
  2. Ingresar datos válidos en todos los campos
  3. Hacer clic en “Registrar”
- **Resultado esperado:** Usuario registrado correctamente
- **Resultado actual:** —
- **Estado:** —

### TC-REG-002 – Registro con correo duplicado

- **Precondición:** Correo previamente registrado
- **Pasos:**
  1. Acceder a la página de registro
  2. Ingresar un correo ya registrado
  3. Completar el resto de campos
  4. Hacer clic en “Registrar”
- **Resultado esperado:** El sistema muestra mensaje de error indicando correo duplicado
- **Resultado actual:** —
- **Estado:** —

### TC-REG-003 – Registro con campos obligatorios vacíos

- **Precondición:** Ninguna
- **Pasos:**
  1. Acceder a la página de registro
  2. Dejar uno o más campos obligatorios vacíos
  3. Hacer clic en “Registrar”
- **Resultado esperado:** El sistema muestra mensajes de validación
- **Resultado actual:** —
- **Estado:** —

## 5. Notas

- Los resultados actuales y estados se completan durante la fase de ejecución
- Los defectos detectados serán documentados en el archivo de **Bug Reports**
- Los casos pueden ampliarse según se identifiquen nuevos escenarios

