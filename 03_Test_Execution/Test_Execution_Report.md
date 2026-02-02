# Test Execution Report

## 1. Introducción

El **Test Execution Report** documenta los resultados de la ejecución de los casos de prueba, proporcionando evidencia de **éxitos, fallos y defectos identificados**.  
Este informe sirve como registro formal del estado de calidad del sistema bajo prueba.

## 2. Alcance

- Casos de prueba ejecutados en los módulos de **Login** y **Registro de Usuario**  
- Registro de resultados para **escenarios positivos y negativos**  
- Documentación de defectos encontrados utilizando el **Bug Report Template**  
- Evidencia asociada a cada caso de prueba (capturas, videos, logs)

## 3. Resumen de Ejecución

| Módulo | Casos Ejecutados | Pass | Fail | % Cobertura |
|--------|------------------|------|------|-------------|
| Login | 6 | 5 | 1 | 100% |
| Registro | 7 | 6 | 1 | 100% |
| Total | 13 | 11 | 2 | 100% |

> Nota: La cobertura refleja que todos los casos planeados fueron ejecutados.

## 4. Detalle de Ejecución por Caso

| Test Case ID | Test Case Name | Resultado | Evidencia | Defecto Asociado | Observaciones |
|--------------|----------------|-----------|-----------|------------------|---------------|
| TC-LOGIN-001 | Login exitoso | Pass | Screenshot_001.png | — | — |
| TC-LOGIN-002 | Contraseña incorrecta | Fail | Screenshot_002.png | BUG-001 | Sistema permitió acceso |
| TC-LOGIN-003 | Correo no registrado | Pass | Screenshot_003.png | — | — |
| TC-REG-001 | Registro exitoso | Pass | Screenshot_004.png | — | — |
| TC-REG-002 | Correo duplicado | Fail | Screenshot_005.png | BUG-002 | Mensaje de error no es claro |

> Continuar registro para todos los casos ejecutados

## 5. Defectos Encontrados

| Bug ID | Descripción | Severidad | Prioridad | Estado |
|--------|-------------|-----------|-----------|--------|
| BUG-001 | Login con contraseña incorrecta permitió acceso | Crítica | Alta | Nuevo |
| BUG-002 | Mensaje de error poco claro en registro | Media | Media | Nuevo |

> Todos los defectos se reportan siguiendo el **Bug Report Template** para trazabilidad.

## 6. Evidencia de Pruebas

- Capturas de pantalla numeradas (`Screenshot_001.png`, etc.)  
- Videos de flujo críticos si aplica  
- Logs relevantes del sistema durante ejecución

## 7. Observaciones Generales

- Todos los casos críticos fueron priorizados y ejecutados primero  
- Los defectos identificados requieren atención inmediata por parte del equipo de desarrollo  
- La ejecución se realizó en ambiente QA estable

## 8. Conclusión

El **Test Execution Report** permite consolidar resultados de manera profesional y proporciona:

- Evidencia clara de la ejecución  
- Identificación de defectos críticos y secundarios  
- Base para generar el **Test Summary Report** y tomar decisiones sobre release o corrección