# Risk Analysis

## 1. Introducción

Este documento describe el **análisis de riesgos** asociado a una aplicación web orientada a usuarios finales.  
El objetivo del análisis es **identificar, evaluar y priorizar riesgos** que puedan afectar la calidad del producto, la experiencia del usuario o los objetivos del negocio.

El análisis de riesgos permite enfocar los esfuerzos de testing en las áreas de **mayor impacto y probabilidad de falla**.

## 2. Objetivo del Análisis de Riesgos

- Identificar funcionalidades críticas del sistema
- Priorizar las pruebas de acuerdo al impacto y probabilidad
- Reducir el riesgo de defectos en producción
- Optimizar el tiempo y esfuerzo de testing

## 3. Metodología de Evaluación

Cada riesgo es evaluado considerando dos factores:

### 3.1 Impacto
Grado en que el defecto afecta al usuario o al negocio.

- **Alto**: Bloquea el uso del sistema o afecta datos
- **Medio**: Afecta funcionalidad importante con alternativa
- **Bajo**: Impacto menor o visual

### 3.2 Probabilidad
Posibilidad de que el defecto ocurra.

- **Alta**: Funcionalidad compleja o frecuentemente usada
- **Media**: Funcionalidad común con lógica moderada
- **Baja**: Funcionalidad simple o poco usada

## 4. Matriz de Riesgos

| Funcionalidad | Riesgo | Impacto | Probabilidad | Nivel de Riesgo |
|---------------|--------|---------|--------------|-----------------|
| Registro de usuario | Fallo en validación de campos obligatorios | Alto | Alta | Alto |
| Login | Autenticación incorrecta                                 | Alto | Alta | Alto |
| Recuperación de contraseña | Enlace inválido o expirado          | Alto | Media | Alto |
| Mensajes de error | Mensajes poco claros                         | Medio | Media | Medio |
| Navegación | Enlaces rotos                                       | Medio | Baja | Bajo |
| UI | Problemas de alineación visual                              | Bajo | Media | Bajo |

## 5. Riesgos Críticos Identificados

### 5.1 Registro de Usuario
- Riesgo de creación de cuentas inválidas
- Impacto directo en la experiencia del usuario
- Riesgo de datos inconsistentes

**Mitigación:**  
Pruebas exhaustivas de validación, valores límite y escenarios negativos.

### 5.2 Inicio de Sesión (Login)
- Riesgo de bloqueo de acceso al sistema
- Riesgo de mensajes de error incorrectos

**Mitigación:**  
Casos de prueba positivos, negativos y pruebas exploratorias enfocadas en credenciales inválidas.

### 5.3 Recuperación de Contraseña
- Riesgo de que el usuario no pueda recuperar el acceso
- Riesgo de confusión por mensajes incorrectos

**Mitigación:**  
Validación de flujos completos y mensajes al usuario.

## 6. Estrategia de Mitigación de Riesgos

Para reducir los riesgos identificados se aplicarán las siguientes acciones:

- Priorización de pruebas en funcionalidades críticas
- Mayor cobertura de casos negativos
- Pruebas de regresión focalizadas
- Testing exploratorio en áreas de alto riesgo


## 7. Relación con la Estrategia de Testing

Este análisis de riesgos sirve como base para:

- Definir el orden de ejecución de pruebas
- Asignar mayor esfuerzo a funcionalidades críticas
- Justificar decisiones de testing ante stakeholders

## 8. Conclusión

El análisis de riesgos permite enfocar el proceso de testing en las áreas que representan **mayor valor y mayor riesgo**, contribuyendo a una entrega de software más estable y confiable.

Este enfoque demuestra un pensamiento QA orientado al negocio y a la prevención de defectos críticos.