# Reporte de Ejecución de Pruebas – Simulación de Caso Real QA Manual

## 1. Introducción

Este documento presenta el **reporte de ejecución de pruebas manuales** realizadas sobre el **Sistema de Gestión de Usuarios**, como parte de la simulación de un proyecto real de QA.

El objetivo es mostrar el estado de la calidad del sistema tras la ejecución de los casos de prueba planificados.

## 2. Información General

- **Proyecto:** Sistema de Gestión de Usuarios
- **Tipo de pruebas:** Pruebas manuales funcionales
- **Ambiente:** QA / Staging
- **Fecha de ejecución:** Simulada
- **QA responsable:** QA Analyst

## 3. Resumen de Ejecución

| Métrica | Cantidad |
|---------|----------|
| Casos de prueba planificados | 6 |
| Casos de prueba ejecutados | 6 |
| Casos exitosos (Pass) | 4 |
| Casos fallidos (Fail) | 2 |
| Casos bloqueados | 0 |
| Cobertura de ejecución | 100% |

## 4. Detalle por Módulo

### Login

| Caso de Prueba | Resultado |
|----------------|-----------|
| TC-LOGIN-001 | Pass |
| TC-LOGIN-002 | Fail |
| TC-LOGIN-003 | Pass |

**Observación:**  
Se detectó un bug crítico relacionado con validación de credenciales.

### Registro de Usuario

| Caso de Prueba | Resultado |
|----------------|-----------|
| TC-REG-001 | Pass |
| TC-REG-002 | Fail |
| TC-REG-003 | Pass |

**Observación:**  
Se identificó un bug de severidad media relacionado con mensajes de error.

## 5. Bugs Detectados

| Bug ID | Módulo | Severidad | Prioridad | Estado |
|--------|--------|-----------|-----------|--------|
| BUG-001 | Login | Crítica | Alta | Nuevo |
| BUG-002 | Registro | Media | Media | Nuevo |

## 6. Análisis de Resultados

- La ejecución alcanzó el **100% de cobertura planificada**
- Se detectó un **bug crítico** que bloquea la liberación
- Los bugs encontrados fueron correctamente documentados
- La funcionalidad principal requiere corrección y re-ejecución

## 7. Riesgos Identificados

- Riesgo alto en seguridad del login
- Riesgo medio en experiencia de usuario durante el registro
- Necesidad de re-ejecución de pruebas críticas tras correcciones

## 8. Conclusión

El sistema **no está listo para liberación** en su estado actual debido a la presencia de un bug crítico.  
Se recomienda corregir los bugs detectados y ejecutar pruebas de regresión antes de considerar el release.