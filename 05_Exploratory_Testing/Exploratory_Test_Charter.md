# Exploratory Test Charter – User Management Module

## 1. Introducción

El **Exploratory Test Charter** define los objetivos, alcance y enfoque de una sesión de exploración específica para el módulo de **Login y Registro de Usuario**.  
Sirve como guía para asegurar que la sesión sea **estructurada, medible y documentada**.

## 2. Sesión de Exploración

| Campo | Detalle |
|-------|---------|
| Módulo | Login y Registro de Usuario |
| Fecha | 2026-02-02 |
| Duración | 60-90 minutos por sesión |
| QA Analyst | [Nombre del QA] |
| Técnica | Session-Based Testing + Error Guessing + Checklist |

## 3. Objetivos de la Sesión

- Verificar **flujos funcionales principales**  
- Identificar **errores y bugs** no cubiertos por casos predefinidos  
- Evaluar **usabilidad y experiencia de usuario**  
- Revisar **validaciones y restricciones de seguridad**

## 4. Alcance

- Login con credenciales válidas e inválidas  
- Registro de nuevos usuarios  
- Manejo de errores (campos vacíos, longitud de datos, duplicados)  
- Experiencia de usuario y consistencia de mensajes

## 5. Restricciones

- Ambiente QA estable (no producción)  
- Uso de datos de prueba proporcionados  
- Tiempo limitado de sesión (60-90 minutos)  
- Reporte de hallazgos debe ser resumido y con evidencia mínima (capturas/logs)

## 6. Plan de Acción

| Objetivo | Acción | Resultado Esperado |
|----------|--------|-------------------|
| Login válido | Ingresar usuario y contraseña correctos | Acceso exitoso |
| Login inválido | Contraseña o correo incorrecto | Error mostrado y acceso denegado |
| Registro válido | Completar todos los campos correctamente | Usuario registrado |
| Registro inválido | Correo duplicado o campos inválidos | Mensaje de error claro |
| Manejo de sesión | Logout y expiración de sesión | Redirección a login |

## 7. Registro de Hallazgos

- Cada hallazgo será documentado con:  
  - ID del bug  
  - Descripción  
  - Severidad y prioridad  
  - Evidencia (capturas, logs, videos)  
  - Estado (nuevo, en progreso, cerrado)

## 8. Beneficios del Test Charter

- Proporciona **claridad y enfoque** durante la sesión de exploración  
- Garantiza **registro de hallazgos con trazabilidad**  
- Permite medir efectividad y cobertura de la sesión  
- Complementa los casos de prueba formales y la estrategia QA general

## 9. Conclusión

El **Exploratory Test Charter** es una herramienta esencial para que las sesiones de pruebas exploratorias sean **efectivas, organizadas y con resultados claros**, demostrando profesionalismo y pensamiento crítico en QA.