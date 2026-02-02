# Exploratory Testing – User Management Module

## 1. Introducción

El objetivo de esta sesión de **Exploratory Testing** es identificar bugs y comportamientos inesperados en los módulos de **Login y Registro de Usuario** mediante la exploración de la aplicación de forma libre, complementando los casos de prueba planificados.  

Se busca:

- Detectar errores no previstos en los casos formales  
- Evaluar la experiencia de usuario y usabilidad  
- Analizar robustez del sistema frente a entradas y escenarios no estándar  

## 2. Alcance

- Módulos evaluados: Login y Registro de Usuario  
- Tipos de pruebas exploratorias:  
  - Funcionalidad básica y flujo principal  
  - Manejo de errores y validaciones  
  - Experiencia de usuario y mensajes de alerta  
  - Restricciones de seguridad y accesos  

## 3. Preparación

- Ambiente QA estable y actualizado  
- Credenciales de prueba disponibles  
- Herramientas para captura de evidencia (pantalla, logs)  
- Registro de hallazgos y notas de sesión  

## 4. Sesiones de Exploración

### 4.1 Sesión 1 – Login

| Objetivo | Acción | Observaciones | Resultado |
|----------|--------|---------------|-----------|
| Verificar login válido | Ingresar usuario y contraseña correctos | Flujo OK | Pass |
| Contraseña incorrecta | Ingresar contraseña inválida | Sistema permitió acceso | Fail (BUG-EXPL-001) |
| Correo no registrado | Usar email inexistente | Mensaje correcto pero no claro | Medium |
| Sesión expirada | Intentar login tras logout automático | Sistema requiere reingreso | Pass |

### 4.2 Sesión 2 – Registro

| Objetivo | Acción | Observaciones | Resultado |
|----------|--------|---------------|-----------|
| Registro válido | Completar todos los campos correctamente | Flujo OK | Pass |
| Correo duplicado | Intentar registrar un correo existente | Mensaje de error poco claro | Medium (BUG-EXPL-002) |
| Contraseña débil | Ingresar `12345` | Sistema rechazó correctamente | Pass |
| Nombre demasiado largo | Más de 50 caracteres | Mensaje de error mostrado | Pass |
| Campos vacíos | Dejar campos obligatorios vacíos | Sistema indica campos requeridos | Pass |

## 5. Hallazgos Clave

- **BUG-EXPL-001** – Login permitió acceso con contraseña incorrecta  
- **BUG-EXPL-002** – Mensaje de correo duplicado poco claro  
- Flujo de registro y login en general estable  
- Validaciones BVA y EP aplicadas correctamente  
- Mejora sugerida: mensajes de error más claros y consistentes  

## 6. Beneficios de la Exploración

- Detecta bugs **que podrían no cubrir los casos predefinidos**  
- Mejora la **experiencia de usuario** y robustez del sistema  
- Permite registrar **insights y aprendizajes** para futuros casos de prueba  
- Complementa la estrategia QA formal, mostrando **pensamiento crítico y proactividad**