# Test Plan

## 1. Introducción

Este documento describe el **Plan de Pruebas** para una aplicación web ficticia orientada a usuarios finales, cuyo objetivo es permitir el registro, autenticación y acceso a funcionalidades básicas del sistema.

El propósito de este Test Plan es definir el **alcance, enfoque, recursos y cronograma** de las actividades de testing, asegurando que el producto cumpla con los requerimientos funcionales y de calidad esperados antes de su liberación.

## 2. Objetivo del Testing

El objetivo principal de las pruebas es:

- Validar que las funcionalidades principales del sistema funcionen correctamente
- Detectar defectos en etapas tempranas
- Reducir riesgos de fallas en producción
- Asegurar una experiencia de usuario consistente y confiable

## 3. Alcance del Testing

### 3.1 Funcionalidades incluidas

Las pruebas cubrirán las siguientes funcionalidades:

- Registro de usuario
- Inicio de sesión (Login)
- Validación de campos en formularios
- Mensajes de error y confirmación
- Navegación básica entre pantallas

### 3.2 Funcionalidades excluidas

Quedan fuera del alcance de este ciclo de pruebas:

- Pruebas de rendimiento y carga
- Pruebas de seguridad avanzadas (pentesting)
- Pruebas de compatibilidad con dispositivos móviles
- Integraciones con sistemas externos

## 4. Estrategia de Testing

El enfoque de testing será **manual**, basado en:

- Análisis de requerimientos
- Diseño de casos de prueba
- Ejecución controlada de pruebas
- Reporte y seguimiento de defectos

Se aplicarán técnicas de diseño de pruebas como:

- Partición de equivalencia
- Análisis de valores límite
- Pruebas basadas en riesgo
- Testing exploratorio


## 5. Tipos de Pruebas

- Pruebas funcionales
- Pruebas de regresión (manual)
- Pruebas exploratorias
- Pruebas de validación de UI básica


## 6. Entorno de Pruebas

- Tipo de aplicación: Web
- Navegador principal: Google Chrome
- Sistema operativo: Windows 11
- Ambiente: Testing / QA
- Base de datos: Simulada (datos de prueba)

## 7. Criterios de Entrada y Salida

### 7.1 Criterios de Entrada

- Requerimientos funcionales disponibles
- Ambiente de pruebas estable
- Acceso a la aplicación
- Casos de prueba diseñados y revisados

### 7.2 Criterios de Salida

- 100% de casos de prueba ejecutados
- Defectos críticos y altos corregidos
- Evidencia de pruebas documentada
- Test Summary Report aprobado

## 8. Roles y Responsabilidades

| Rol        | Responsabilidad |
|------------|-----------------|
| QA Analyst | Diseño y ejecución de pruebas, reporte de defectos |
| Developer  | Corrección de defectos |
| Product Owner | Validación de requerimientos |

## 9. Gestión de Defectos

Los defectos serán registrados y documentados con la siguiente información mínima:

- ID del defecto
- Título
- Descripción detallada
- Pasos para reproducir
- Resultado esperado
- Resultado actual
- Severidad y prioridad
- Evidencia (capturas o videos)

## 10. Riesgos y Mitigación

| Riesgo | Impacto | Mitigación |
|------|--------|-----------|
| Requerimientos incompletos | Alto | Revisión temprana con PO |
| Cambios de última hora | Medio | Pruebas de regresión focalizadas |
| Tiempo limitado | Medio | Priorización basada en riesgo |

## 11. Entregables

- Casos de prueba documentados
- Reportes de defectos
- Evidencia de ejecución
- Test Execution Report
- Test Summary Report

## 12. Aprobación

Este Test Plan será considerado aprobado una vez revisado y aceptado por las partes involucradas.
