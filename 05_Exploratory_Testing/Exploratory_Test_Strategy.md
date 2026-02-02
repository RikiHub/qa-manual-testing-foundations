# Exploratory Testing Strategy

## 1. Introducción

La estrategia de **Exploratory Testing** define cómo se realizarán sesiones de exploración de la aplicación, con objetivos claros, técnicas aplicadas y registro de hallazgos.  
Su propósito es **descubrir bugs no cubiertos por casos de prueba predefinidos** y mejorar la **experiencia de usuario**.

## 2. Objetivos

- Identificar bugs críticos y secundarios que no aparecen en los casos formales  
- Evaluar la **usabilidad y robustez** del sistema  
- Generar insights para mejorar **requerimientos y documentación QA**  
- Complementar el **Test Plan y Test Strategy** con hallazgos prácticos

## 3. Alcance

- Módulos explorados: **Login, Registro de Usuario y Gestión de Sesiones**  
- Áreas de enfoque:  
  - Flujo funcional principal  
  - Manejo de errores y validaciones  
  - Experiencia de usuario (mensajes, alertas, feedback)  
  - Seguridad básica y restricciones de acceso

## 4. Preparación

- Ambiente de pruebas estable y accesible  
- Credenciales de prueba y datos de usuario disponibles  
- Herramientas para captura de evidencia: capturas, videos y logs  
- Registro de hallazgos en formato estandarizado (Bug Report Template o notas de sesión)

## 5. Técnicas de Exploración Aplicadas

1. **Session-Based Testing:**  
   - Dividir la exploración en sesiones de 60 minutos por módulo  
   - Cada sesión con objetivo específico (p. ej., login válido/incorrecto)  

2. **Error Guessing:**  
   - Intentar inputs fuera de rango, vacíos o inválidos  
   - Probar combinaciones no contempladas en casos predefinidos  

3. **Checklist-Driven:**  
   - Uso de checklist de validaciones críticas: campos obligatorios, longitud, formatos, seguridad  

4. **Ad-Hoc / Freestyle:**  
   - Explorar libremente para detectar problemas de UX, consistencia de mensajes y flujo

## 6. Plan de Sesiones

| Sesión | Módulo | Objetivo | Tiempo Estimado | Técnica |
|--------|--------|----------|-----------------|---------|
| 1 | Login | Validar flujo de login con credenciales válidas e inválidas | 60 min | Session-Based / Error Guessing |
| 2 | Registro | Completar registro con datos válidos e inválidos | 60 min | Session-Based / Checklist |
| 3 | Gestión de Sesiones | Verificar expiración de sesión y logout | 45 min | Ad-Hoc / Freestyle |

## 7. Registro de Hallazgos

Cada hallazgo será documentado con:

| ID | Sesión | Descripción | Severidad | Evidencia | Estado |
|----|--------|-------------|-----------|-----------|--------|
| BUG-EXPL-001 | Login | Acceso permitido con contraseña incorrecta | Crítica | Screenshot_Login_002.png | Nuevo |
| BUG-EXPL-002 | Registro | Mensaje de correo duplicado poco claro | Media | Screenshot_Registro_002.png | Nuevo |

## 8. Beneficios de la Estrategia

- Permite **explorar de manera sistemática**, no aleatoria  
- Documenta **hallazgos con trazabilidad y evidencia**  
- Complementa casos de prueba formales (Test Plan, BVA, EP)  
- Mejora la **robustez, seguridad y UX** del sistema

## 9. Conclusión

Una estrategia de **Exploratory Testing bien definida** asegura que las pruebas no estructuradas aporten **valor real al proyecto**, detectando bugs, mejorando la calidad y demostrando profesionalismo y pensamiento crítico del QA Analyst.