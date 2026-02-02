# Equivalence Partitioning (EP)

## 1. Introducción

La **Partición de Equivalencia** (Equivalence Partitioning, EP) es una técnica de diseño de casos de prueba que **divide los datos de entrada en clases equivalentes**, de manera que un solo caso de prueba represente toda la clase.

El objetivo es **reducir la cantidad de casos necesarios** sin perder cobertura significativa, enfocándose en valores representativos de cada grupo.

## 2. Principios de la EP

1. Identificar todas las posibles entradas o condiciones de un campo.  
2. Dividir las entradas en **clases válidas** y **clases inválidas**.  
3. Seleccionar **uno o dos valores representativos** de cada clase para las pruebas.  
4. Documentar cada clase y su resultado esperado.  

> Nota: Esta técnica se aplica tanto a campos **numéricos, alfabéticos, combinados y booleanos**.

## 3. Pasos para aplicar EP

1. Analizar los requisitos del campo.  
2. Definir **clases de equivalencia válidas e inválidas**.  
3. Seleccionar valores representativos de cada clase.  
4. Diseñar los casos de prueba usando esos valores.  
5. Ejecutar pruebas y registrar resultados.

## 4. Ejemplos Prácticos

### 4.1 Registro de Usuario – Campo “Edad” (numérico)

- Requerimiento: Edad entre 18 y 60 años

| Clase de Equivalencia | Tipo | Ejemplo de valor | Resultado Esperado |
|-----------------------|------|------------------|--------------------|
| Edad válida | Válida | 25 | Aceptado |
| Edad menor al mínimo | Inválida | 17 | Error: edad inválida |
| Edad mayor al máximo | Inválida | 61 | Error: edad inválida |

### 4.2 Registro de Usuario – Campo “Correo Electrónico” (alfabético / formato)

- Requerimiento: Formato válido de correo electrónico

| Clase de Equivalencia | Tipo | Ejemplo de valor | Resultado Esperado |
|-----------------------|------|------------------|--------------------|
| Correo válido | Válida | user@test.com | Aceptado |
| Correo sin “@” | Inválida | usertest.com | Error: formato inválido |
| Correo sin dominio | Inválida | user@ | Error: formato inválido |

### 4.3 Login – Campo “Contraseña” (alfanumérico)

- Requerimiento: Contraseña de 8 a 20 caracteres

| Clase de Equivalencia | Tipo | Ejemplo de valor | Resultado Esperado |
|-----------------------|------|------------------|--------------------|
| Contraseña válida | Válida | Password123 | Aceptado |
| Contraseña < 8 caracteres | Inválida | Pass12 | Error: contraseña demasiado corta |
| Contraseña > 20 caracteres | Inválida | Password123456789012345 | Error: contraseña demasiado larga |

## 5. Beneficios de EP

- Reduce la **cantidad de casos de prueba** manteniendo cobertura efectiva  
- Permite **enfocar esfuerzos en valores representativos**  
- Complementa otras técnicas como **BVA**  
- Facilita pruebas **estructuradas y repetibles**  

## 6. Conclusión

La **partición de equivalencia** es esencial para diseñar pruebas eficientes y efectivas.  
Aplicar EP demuestra que un QA puede **maximizar cobertura con menos esfuerzo**, minimizando redundancia y manteniendo calidad en el proceso de testing.