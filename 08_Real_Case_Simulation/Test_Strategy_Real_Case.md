# Estrategia de Pruebas – Simulación de Caso Real QA Manual

## 1. Introducción

Este documento define la **estrategia de pruebas** para la simulación de un proyecto real de QA Manual aplicado a una **Aplicación Web de Gestión de Usuarios**.

La estrategia establece el **enfoque, alcance, prioridades, tipos de pruebas y criterios de calidad**, con el objetivo de asegurar que el sistema cumpla con los requerimientos funcionales antes de su liberación.

## 2. Objetivos de la Estrategia de Pruebas

- Validar las funcionalidades críticas del sistema
- Detectar bugs en etapas tempranas
- Asegurar una adecuada cobertura de pruebas
- Priorizar pruebas basadas en riesgo
- Garantizar una experiencia de usuario correcta
- Apoyar la toma de decisiones para el release del producto

## 3. Enfoque de Pruebas

El enfoque de pruebas será **manual**, utilizando técnicas de diseño de casos y pruebas exploratorias.

### Estrategias aplicadas:
- Pruebas basadas en requerimientos
- Pruebas basadas en riesgo
- Pruebas positivas y negativas
- Pruebas exploratorias complementarias

## 4. Tipos de Pruebas Incluidas

- Pruebas funcionales
- Pruebas de validación de campos
- Pruebas de regresión manual
- Pruebas de usabilidad básicas
- Pruebas exploratorias
- Pruebas de smoke testing

## 5. Priorización Basada en Riesgo

Las pruebas se priorizan considerando:
- Impacto en el negocio
- Frecuencia de uso de la funcionalidad
- Complejidad técnica
- Historial de bugs

### Funcionalidades críticas:
- Inicio de sesión
- Registro de usuario
- Validaciones de credenciales
- Manejo de errores

## 6. Ambientes de Pruebas

- **Ambiente:** QA / Staging
- **Navegadores:** Chrome, Edge
- **Sistema Operativo:** Windows 11
- **Datos de prueba:** Cuentas válidas, inválidas y límites

## 7. Roles y Responsabilidades

| Rol | Responsabilidad |
|-----|-----------------|
| QA Analyst | Diseño, ejecución, reporte y análisis de pruebas |
| Developer | Corrección de bugs |
| Product Owner | Validación de requerimientos y aprobación |

## 8. Herramientas Utilizadas

- Documentación en Markdown
- Navegadores web
- Herramientas de seguimiento de bugs (simulado)
- Capturas de pantalla como evidencia

## 9. Gestión de bugs

- Todos los bugs serán documentados con:
  - Pasos para reproducir
  - Resultado esperado vs actual
  - Severidad y prioridad
  - Evidencia
- Los bugs críticos bloquearán el release

## 10. Criterios de Entrada

- Requerimientos aprobados
- Ambiente estable
- Casos de prueba definidos
- Datos de prueba disponibles

## 11. Criterios de Salida

- 100% de casos críticos ejecutados
- No existen bugs críticos abiertos
- Bugs medios evaluados y aceptados
- Reporte de ejecución generado

## 12. Riesgos y Mitigación

| Riesgo | Mitigación |
|--------|------------|
| Requerimientos ambiguos | Revisión y aclaración previa |
| Cambios tardíos | Re-ejecución de pruebas críticas |
| Falta de tiempo | Priorización por riesgo |
| Bugs críticos | Bloqueo de liberación |

## 13. Conclusión

Esta estrategia asegura un **proceso de pruebas estructurado, controlado y alineado a buenas prácticas de QA**, permitiendo evaluar la calidad del sistema antes de su liberación y reduciendo riesgos para el negocio.
