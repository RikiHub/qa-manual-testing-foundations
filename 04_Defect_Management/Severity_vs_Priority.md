# Severity vs Priority

## 1. Introducción

En QA, **Severidad** y **Prioridad** son conceptos fundamentales para clasificar y gestionar defectos.  
Aunque a menudo se confunden, tienen significados distintos y sirven para **tomar decisiones objetivas** sobre el ciclo de pruebas y la corrección de bugs.

## 2. Definiciones

### 2.1 Severidad (Severity)

- Se refiere al **impacto técnico** que tiene el defecto sobre el sistema.  
- Determina qué tan grave es el fallo desde el punto de vista del **funcionamiento del software**.

**Clasificación común:**

| Nivel | Descripción |
|-------|-------------|
| Crítica | Bloquea completamente el sistema; datos corruptos; falla de seguridad grave |
| Alta | Funcionalidad importante dañada; afecta flujo principal |
| Media | Funcionalidad secundaria afectada; inconveniente para el usuario |
| Baja | Defecto menor, UI o errores estéticos; no afecta el flujo principal |

### 2.2 Prioridad (Priority)

- Se refiere al **orden en que el defecto debe ser solucionado**.  
- Determina la **urgencia de corrección**, generalmente definida por Product Owner o QA Lead.

**Clasificación común:**

| Nivel | Descripción |
|-------|-------------|
| Alta | Debe corregirse inmediatamente, antes de la próxima release |
| Media | Corregir en próxima iteración / sprint |
| Baja | Puede corregirse más adelante; no bloquea release |

## 3. Diferencias Clave

| Aspecto | Severidad | Prioridad |
|---------|-----------|-----------|
| Qué mide | Impacto en el sistema | Urgencia de corrección |
| Quién lo define | QA Analyst / Tester | Product Owner / QA Lead |
| Relación | Independiente de prioridad | Puede depender de severidad, pero no siempre |
| Ejemplo | Login no funciona = Crítica | Release urgente = Prioridad Alta |

## 4. Ejemplos Prácticos

| Bug | Severidad | Prioridad | Justificación |
|-----|-----------|-----------|---------------|
| Login bloquea acceso | Crítica | Alta | Impacta flujo principal y usuarios no pueden acceder |
| Error de ortografía en pantalla | Baja | Baja | No afecta funcionalidad, se puede corregir luego |
| Mensaje de error confuso | Media | Media | Afecta UX, pero no bloquea flujo principal |
| Enlace de recuperación de contraseña expira inmediatamente | Alta | Alta | Afecta acceso al usuario; crítico en experiencia |

## 5. Consideraciones

- **Severidad alta no siempre implica prioridad alta**, y viceversa.  
- Es importante documentar **ambos campos en los Bug Reports** para que dev y PO tengan claridad.  
- Esta clasificación permite gestionar **bugs de manera objetiva** y priorizar esfuerzos de desarrollo.

## 6. Conclusión

Comprender la diferencia entre Severidad y Prioridad demuestra **pensamiento crítico y profesionalismo en QA**.  
Un buen QA asegura que los defectos sean reportados de manera clara, correcta y con criterios que faciliten la toma de decisiones por el equipo.