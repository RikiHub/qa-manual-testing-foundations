# Test Reports Samples

Este documento contiene **ejemplos prácticos de reportes de pruebas** generados durante el proyecto de QA, incluyendo **Test Execution Report** y **Test Summary Report**.  
Estos reportes muestran evidencia, resultados y métricas, reflejando **profesionalismo en la documentación de QA**.

## 1. Sample – Test Execution Report

| Test Case ID | Test Case Name | Resultado | Evidencia | Defecto Asociado | Observaciones |
|--------------|----------------|-----------|-----------|------------------|---------------|
| TC-LOGIN-001 | Login exitoso | Pass | Screenshot_Login_001.png | — | — |
| TC-LOGIN-002 | Contraseña incorrecta | Fail | Screenshot_Login_002.png | BUG-001 | Usuario pudo ingresar con contraseña incorrecta |
| TC-LOGIN-003 | Correo no registrado | Pass | Screenshot_Login_003.png | — | — |
| TC-REG-001 | Registro exitoso | Pass | Screenshot_Registro_001.png | — | — |
| TC-REG-002 | Correo duplicado | Fail | Screenshot_Registro_002.png | BUG-002 | Mensaje de error poco claro |

> Nota: La evidencia consiste en capturas de pantalla numeradas, videos y logs del sistema.

## 2. Sample – Test Summary Report

| Módulo | Casos Planificados | Ejecutados | Pass | Fail | % Cobertura |
|--------|--------------------|------------|------|------|-------------|
| Login | 6 | 6 | 5 | 1 | 100% |
| Registro | 7 | 7 | 6 | 1 | 100% |
| **Total** | 13 | 13 | 11 | 2 | 100% |

**Defectos Reportados:**

| Bug ID | Descripción | Severidad | Prioridad | Estado |
|--------|-------------|-----------|-----------|--------|
| BUG-001 | Login permitió acceso con contraseña incorrecta | Crítica | Alta | Nuevo |
| BUG-002 | Mensaje de error poco claro en registro | Media | Media | Nuevo |

**Conclusiones:**

- La funcionalidad principal cumple con la mayoría de los requerimientos.  
- Los defectos críticos requieren atención antes del release.  
- Todos los casos fueron ejecutados y documentados con evidencia.

## 3. Ejemplo de Evidencia Adjunta

1. Capturas de pantalla: `Screenshot_Login_001.png`, `Screenshot_Registro_002.png`  
2. Videos de flujo crítico (opcional)  
3. Logs relevantes del sistema durante la ejecución  

> Esta evidencia respalda los resultados reportados y permite replicar cualquier fallo por el equipo de desarrollo.

## 4. Beneficios de estos Reportes

- Permiten **visualizar rápidamente la salud del sistema**  
- Facilitan **auditorías y revisiones de QA**  
- Proporcionan **trazabilidad completa de la ejecución de pruebas**  
- Demuestran **profesionalismo y organización** en el proceso QA