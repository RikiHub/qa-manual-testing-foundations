# Coverage Analysis – User Management Module

## 1. Introducción

El **Coverage Analysis** evalúa la **efectividad de la ejecución de pruebas**, verificando que los casos cubran todos los requerimientos y detectando riesgos y bugs.  
Permite al equipo QA **tomar decisiones basadas en datos** y garantizar trazabilidad completa desde requerimientos hasta hallazgos.

## 2. Alcance

- Evaluación de cobertura de pruebas de los módulos de **Login y Registro de Usuario**  
- Análisis de resultados de ejecución, bugs y severidad  
- Identificación de riesgos y gaps en la cobertura  
- Complemento de la **Requirements Traceability Matrix (RTM)**

## 3. Cobertura de Casos de Prueba

| Módulo | Casos Planificados | Ejecutados | Pass | Fail | % Cobertura |
|--------|-----------------|------------|------|------|------------|
| Login | 6 | 6 | 5 | 1 | 100% |
| Registro | 7 | 7 | 6 | 1 | 100% |
| Total | 13 | 13 | 11 | 2 | 100% |

> Nota: Todos los casos críticos fueron ejecutados y documentados.

## 4. Análisis de Bugs

| Bug ID | Descripción | Severidad | Prioridad | Estado | Impacto |
|--------|-------------|-----------|-----------|--------|---------|
| BUG-001 | Login permitió acceso con contraseña incorrecta | Crítica | Alta | Nuevo | Bloquea funcionalidad principal |
| BUG-002 | Mensaje de correo duplicado poco claro | Media | Media | Nuevo | UX y claridad del sistema |

**Observaciones:**

- Los bugs críticos requieren corrección inmediata antes del release.  
- La mayoría de los bugs son de severidad media y afectan UX, pero no bloquean la funcionalidad principal.

## 5. Cobertura por Requerimiento

| Req ID | Descripción | Caso Asociado | Ejecutado | Resultado | Comentarios |
|--------|-------------|---------------|-----------|-----------|-------------|
| RQ-001 | Login válido | TC-LOGIN-001 | Sí | Pass | — |
| RQ-002 | Contraseña incorrecta | TC-LOGIN-002 | Sí | Fail | Necesita corrección |
| RQ-004 | Registro de usuario | TC-REG-001 | Sí | Pass | — |
| RQ-005 | Correo duplicado | TC-REG-002 | Sí | Fail | Mensaje de error poco claro |

> Esto asegura trazabilidad completa y visibilidad de cobertura real.

## 6. Análisis de Riesgos

| Riesgo | Probabilidad | Impacto | Mitigación |
|--------|--------------|---------|------------|
| Login con contraseña incorrecta permite acceso | Alta | Crítico | Corrección inmediata y re-ejecución de prueba |
| Mensajes de error poco claros | Media | Medio | Ajuste de UX y validación en próxima iteración |
| Requerimientos no cubiertos | Baja | Medio | Revisar RTM y crear casos faltantes |

## 7. Conclusiones

- La cobertura de pruebas es **completa respecto a los casos planificados y requerimientos críticos**  
- Existen **bugs críticos y medios** que deben corregirse antes del release  
- El análisis de cobertura y riesgos permite **priorizar acciones y asegurar calidad del sistema**  
- La documentación y trazabilidad reflejan **profesionalismo y madurez en QA**