# Boundary Value Analysis (BVA)

## 1. Introducción

El **Boundary Value Analysis (BVA)** es una técnica de diseño de casos de prueba que se centra en **los valores en los límites de entrada de un campo o rango de datos**.  
Se basa en la idea de que los errores tienden a ocurrir en los **límites de los rangos**, no necesariamente en los valores intermedios.

Esta técnica es ampliamente utilizada en QA profesional para **maximizar cobertura con mínimo esfuerzo**.

## 2. Principios de BVA

1. Se identifican los **rangos válidos e inválidos** para cada campo.  
2. Se seleccionan **valores en los límites**: mínimo, máximo, justo dentro y justo fuera.  
3. Se generan **casos de prueba positivos y negativos** basados en estos límites.  
4. La técnica complementa otras como **partición de equivalencia**.

## 3. Pasos para aplicar BVA

1. Identificar el campo o entrada a evaluar.  
2. Determinar el **rango permitido** (mínimo y máximo).  
3. Elegir los valores del límite:  
   - Valor mínimo válido  
   - Valor máximo válido  
   - Valor justo por debajo del mínimo (inválido)  
   - Valor justo por encima del máximo (inválido)  
4. Documentar cada caso de prueba con resultado esperado.  
5. Ejecutar los casos y registrar evidencia.

## 4. Ejemplos Prácticos

### 4.1 Registro de Usuario – Campo “Nombre”

- Requerimiento: Nombre entre 2 y 50 caracteres  
- BVA:

| Caso | Entrada | Resultado Esperado |
|------|---------|--------------------|
| TC-BVA-001 | 1 caracter | Error: nombre demasiado corto |
| TC-BVA-002 | 2 caracteres | Aceptado |
| TC-BVA-003 | 50 caracteres | Aceptado |
| TC-BVA-004 | 51 caracteres | Error: nombre demasiado largo |

### 4.2 Login – Campo “Contraseña”

- Requerimiento: Contraseña entre 8 y 20 caracteres  
- BVA:

| Caso | Entrada | Resultado Esperado |
|------|---------|--------------------|
| TC-BVA-005 | 7 caracteres | Error: contraseña demasiado corta |
| TC-BVA-006 | 8 caracteres | Aceptado |
| TC-BVA-007 | 20 caracteres | Aceptado |
| TC-BVA-008 | 21 caracteres | Error: contraseña demasiado larga |

### 4.3 Edad de Usuario – Campo “Edad” (ejemplo numérico)

- Requerimiento: Edad entre 18 y 60 años  
- BVA:

| Caso | Entrada | Resultado Esperado |
|------|---------|--------------------|
| TC-BVA-009 | 17 | Error: edad inválida |
| TC-BVA-010 | 18 | Aceptado |
| TC-BVA-011 | 60 | Aceptado |
| TC-BVA-012 | 61 | Error: edad inválida |

## 5. Beneficios de BVA

- Detecta errores en **valores límite**, que suelen ser problemáticos  
- Permite **maximizar cobertura con menos casos**  
- Facilita pruebas **repetibles y trazables**  
- Complementa otras técnicas de diseño como **partición de equivalencia**

## 6. Conclusión

El **Boundary Value Analysis** es una técnica esencial en QA manual, especialmente en aplicaciones donde los **rangos de datos son críticos**.  
Su aplicación demuestra **pensamiento estructurado y estratégico**, lo que es altamente valorado en entrevistas y proyectos reales.