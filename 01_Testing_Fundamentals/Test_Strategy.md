# Test Strategy

## 1. Introducción

Este documento define la **estrategia de pruebas** que se seguirá para asegurar la calidad de una aplicación web ficticia, enfocándose en pruebas manuales y en un enfoque basado en riesgo.

La estrategia establece el **cómo**, **cuándo** y **con qué prioridad** se realizarán las actividades de testing, alineándose con los objetivos del negocio y las limitaciones del proyecto.

## 2. Objetivo de la Estrategia de Testing

Los objetivos principales de esta estrategia son:

- Garantizar que las funcionalidades críticas del sistema funcionen correctamente
- Detectar bugs de alto impacto antes de la liberación
- Optimizar el tiempo de pruebas mediante priorización basada en riesgo
- Asegurar una experiencia de usuario estable y consistente

## 3. Enfoque de Testing

El enfoque de testing será **manual**, estructurado y progresivo:

1. Análisis de requerimientos
2. Identificación de funcionalidades críticas
3. Diseño de casos de prueba
4. Ejecución de pruebas
5. Reporte y seguimiento de bugs
6. Pruebas de regresión focalizadas

Este enfoque permite detectar bugs de forma temprana y reducir riesgos en producción.

## 4. Estrategia Basada en Riesgo

La priorización de las pruebas se realizará considerando:

- Impacto al usuario final
- Frecuencia de uso de la funcionalidad
- Complejidad técnica
- Historial de bugs (en proyectos reales)

### Funcionalidades de mayor riesgo

- Registro de usuarios
- Inicio de sesión
- Validaciones de formularios
- Manejo de errores y mensajes al usuario

Estas funcionalidades serán probadas primero y con mayor profundidad.

## 5. Técnicas de Diseño de Pruebas

Se utilizarán las siguientes técnicas:

- **Partición de equivalencia**  
  Para reducir el número de casos de prueba sin perder cobertura.

- **Análisis de valores límite**  
  Para validar comportamientos en los extremos de los rangos permitidos.

- **Casos positivos y negativos**  
  Para validar flujos esperados y escenarios de error.

- **Testing exploratorio**  
  Para descubrir bugs no cubiertos por casos predefinidos.

## 6. Tipos de Pruebas

La estrategia contempla los siguientes tipos de pruebas:
- Pruebas funcionales
- Pruebas de regresión manual
- Pruebas exploratorias
- Validación básica de interfaz de usuario (UI)

## 7. Niveles de Prueba

- **Pruebas de sistema**  
  Validación del sistema completo desde la perspectiva del usuario.

- **Pruebas de aceptación (UAT)**  
  Soporte al Product Owner para validar que el sistema cumple con los criterios de aceptación.

## 8. Entorno de Pruebas

- Aplicación web en ambiente de QA
- Navegador principal: Google Chrome
- Sistema operativo: Windows 11
- Datos de prueba controlados

## 9. Gestión de bugs

Los bugs serán clasificados según:

### Severidad
- Crítica
- Alta
- Media
- Baja

### Prioridad
- Alta
- Media
- Baja

Todos los bugs deberán incluir evidencia y pasos claros para su reproducción.

## 10. Comunicación y Seguimiento

- Los bugs críticos serán comunicados de forma inmediata
- Se dará seguimiento hasta su resolución
- Se validarán correcciones mediante pruebas de regresión

## 11. Criterios de Aceptación del Testing

El proceso de testing se considerará satisfactorio cuando:

- Las funcionalidades críticas estén validadas
- No existan bugs críticos o de severidad alta abiertos
- Los riesgos conocidos estén documentados y aceptados
- Se haya generado el Test Summary Report

## 12. Mejora Continua

Al finalizar el ciclo de pruebas se documentarán:

- Lecciones aprendidas
- Riesgos detectados
- Oportunidades de mejora para futuros ciclos

## 13. Conclusión

Esta estrategia de testing está diseñada para ser **realista, flexible y alineada a proyectos ágiles**, demostrando un enfoque profesional orientado a la calidad del producto y la satisfacción del usuario final.