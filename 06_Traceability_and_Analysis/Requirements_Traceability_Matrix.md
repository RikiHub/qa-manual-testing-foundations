# Requirements Traceability Matrix (RTM) – User Management Module

## 1. Introducción

La **Requirements Traceability Matrix (RTM)** es un documento que asegura la **completa cobertura de pruebas respecto a los requerimientos** del sistema.  
Permite relacionar cada requerimiento con sus casos de prueba asociados y los resultados de ejecución.

## 2. Objetivos

- Garantizar que **todos los requerimientos** tengan casos de prueba asociados  
- Facilitar **auditorías y revisiones de QA**  
- Identificar **áreas no cubiertas o de riesgo**  
- Proveer **trazabilidad completa desde requerimientos hasta resultados**

## 3. Matriz de Trazabilidad

| Req ID | Descripción del Requerimiento | Caso(s) de Prueba Asociado(s) | Resultado de Ejecución | Defectos Asociados |
|--------|-------------------------------|-------------------------------|------------------------|--------------------|
| RQ-001 | Login con usuario válido y contraseña correcta | TC-LOGIN-001 | Pass | — |
| RQ-002 | Manejo de contraseña incorrecta | TC-LOGIN-002 | Fail | BUG-001 |
| RQ-003 | Correo no registrado | TC-LOGIN-003 | Pass | — |
| RQ-004 | Registro de nuevo usuario | TC-REG-001 | Pass | — |
| RQ-005 | Validación de correo duplicado | TC-REG-002 | Fail | BUG-002 |
| RQ-006 | Campos obligatorios | TC-REG-003 | Pass | — |
| RQ-007 | Longitud máxima de nombre | TC-REG-004 | Pass | — |
| RQ-008 | Manejo de expiración de sesión | TC-LOGIN-004 | Pass | — |

> Nota: Esta matriz puede actualizarse en tiempo real para reflejar resultados de ejecución y defectos descubiertos.

## 4. Beneficios de la RTM

- Permite **ver rápidamente qué requerimientos han sido validados**  
- Facilita la **identificación de gaps o áreas sin cobertura**  
- Proporciona **trazabilidad completa para auditorías o revisiones**  
- Ayuda a **priorizar corrección de defectos críticos**  

## 5. Conclusión

Una **Requirements Traceability Matrix** bien documentada asegura que el proceso QA **sea completo, organizado y auditable**, demostrando profesionalismo y rigor en la gestión de pruebas.