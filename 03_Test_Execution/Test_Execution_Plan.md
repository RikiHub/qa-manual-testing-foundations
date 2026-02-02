# Test Execution Plan

## 1. Introducción

El **Plan de Ejecución de Pruebas** define la estrategia para **ejecutar los casos de prueba**, registrar resultados y asegurar que el sistema cumple con los requerimientos definidos.

Este documento sirve como guía para QA Analysts, Test Leads y cualquier miembro del equipo que participe en la ejecución de pruebas.

## 2. Alcance

- Ejecución de casos de prueba para **Login, Registro y funcionalidades críticas**.  
- Cobertura de escenarios positivos, negativos y casos basados en **BVA y Partición de Equivalencia**.  
- Registro de resultados y evidencia.  
- Identificación de bugs y reporte utilizando **Bug Report Template**.

## 3. Entradas necesarias para la ejecución

- Casos de prueba documentados y aprobados (`Test_Cases_Login.md`, `Test_Cases_Registration.md`)  
- Ambiente de prueba configurado y estable  
- Datos de prueba listos  
- Accesos y credenciales  
- Herramientas para evidencias (capturas de pantalla, videos, logs)

## 4. Criterios de Inicio de Ejecución

- Todos los casos de prueba están revisados y aprobados  
- El ambiente de pruebas está operativo y estable  
- Los datos de prueba están cargados y verificados  
- La versión del sistema a probar está desplegada y estable

## 5. Criterios de Pausa o Suspensión

La ejecución de pruebas puede suspenderse si:

- El ambiente de prueba se vuelve inestable  
- Hay bugs críticos que impiden continuar la ejecución  
- Se requiere esperar corrección de bloqueos  
- Cambios de requerimientos no planificados afectan los casos actuales

## 6. Estrategia de Ejecución

1. Priorizar la ejecución de **casos críticos y de alta prioridad**  
2. Ejecutar casos de prueba según la secuencia definida en los módulos  
3. Registrar **resultados y evidencias** de cada caso  
4. Documentar bugs siguiendo el **Bug Report Template**  
5. Repetir la ejecución de casos afectados tras la corrección de bugs  
6. Actualizar el **Test Execution Report** diariamente

## 7. Herramientas y Recursos

- Navegadores y dispositivos configurados para pruebas  
- Herramientas de captura de pantalla / video  
- Sistema de gestión de pruebas (opcional: TestRail, Jira, Zephyr)  
- Herramienta de reporte de bugs (Jira o Excel)  

## 8. Registro de Resultados

Cada caso de prueba será registrado con:

| Campo | Descripción |
|-------|-------------|
| Test Case ID | Identificador único |
| Resultado | Pass / Fail |
| Evidencia | Capturas, videos, logs |
| Defecto Asociado | Bug ID si aplica |
| Observaciones | Comentarios adicionales |

## 9. Frecuencia y Responsables

- QA Analyst: Ejecuta los casos, documenta resultados y evidencia  
- Test Lead: Supervisa la ejecución, revisa resultados críticos y reportes diarios  
- Product Owner / Stakeholders: Reciben reporte final de ejecución  

## 10. Beneficios del Plan de Ejecución

- Estandariza la ejecución de pruebas  
- Mejora trazabilidad y control del ciclo QA  
- Permite priorizar recursos y esfuerzos  
- Garantiza documentación completa y evidencia de calidad

## 11. Conclusión

Un **Plan de Ejecución de Pruebas** bien definido asegura que la ejecución sea **estructurada, eficiente y medible**, permitiendo identificar bugs de manera efectiva y generar reportes confiables para la toma de decisiones.