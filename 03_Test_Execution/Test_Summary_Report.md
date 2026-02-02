# Test Summary Report

## 1. Introducción

El **Test Summary Report** proporciona un resumen ejecutivo de la ejecución de pruebas, destacando la cobertura, Bugs encontrados, métricas y conclusiones generales.  
Este documento sirve para **Stakeholders, Product Owners y QA Leads** como evidencia del estado de calidad del sistema.

## 2. Alcance

- Módulos evaluados: **Login** y **Registro de Usuario**  
- Casos de prueba ejecutados: positivos, negativos, BVA y EP  
- Bugs reportados y categorizados  
- Evidencia documentada para auditoría y revisión

## 3. Resumen de Ejecución

| Módulo | Casos Planificados | Ejecutados | Pass | Fail | % Ejecución |
|--------|--------------------|------------|------|------|-------------|
| Login | 6 | 6 | 5 | 1 | 100% |
| Registro | 7 | 7 | 6 | 1 | 100% |
| **Total** | 13 | 13 | 11 | 2 | 100% |

> Todos los casos planificados fueron ejecutados. La cobertura completa asegura trazabilidad de la calidad.

## 4. Resumen de Bugs

| Bug ID | Descripción | Severidad | Prioridad | Estado |
|--------|-------------|-----------|-----------|--------|
| BUG-001 | Login permitió acceso con contraseña incorrecta | Crítica | Alta | Nuevo |
| BUG-002 | Mensaje de error poco claro en registro | Media | Media | Nuevo |

**Observaciones:**  
- BUG-001 impacta la seguridad y flujo crítico, requiere atención inmediata.  
- BUG-002 impacta UX y claridad, corregible en la próxima iteración.

## 5. Cobertura de Pruebas

- Todos los casos de prueba críticos se ejecutaron  
- Se aplicaron técnicas de **BVA** y **EP**  
- Los casos negativos se ejecutaron para validar robustez y manejo de errores

## 6. Métricas Clave

| Métrica | Valor |
|---------|-------|
| Casos Planificados | 13 |
| Casos Ejecutados | 13 |
| Casos Pass | 11 |
| Casos Fail | 2 |
| Bugs Críticos | 1 |
| Bugs Medios | 1 |
| Porcentaje de Ejecución | 100% |
| Porcentaje de Éxito | 84.6% |

## 7. Conclusiones

1. La funcionalidad **Login y Registro** cumple en su mayoría con los requerimientos funcionales.  
2. Existen Bugs críticos y medios que requieren corrección antes de un release en producción.  
3. La evidencia recopilada asegura trazabilidad y soporte para decisiones de lanzamiento.  
4. La ejecución de pruebas demuestra **cobertura completa de escenarios positivos y negativos**, incluyendo técnicas de diseño avanzadas.

## 8. Recomendaciones

- Priorizar corrección de Bugs críticos antes de release  
- Ejecutar regresión tras corrección de bugs  
- Mantener trazabilidad y evidencia actualizada  
- Revisar mensajes de error y UX en el registro de usuario

## 9. Aprobaciones

| Rol | Nombre | Firma | Fecha |
|-----|--------|-------|-------|
| QA Lead | — | — | — |
| Product Owner | — | — | — |