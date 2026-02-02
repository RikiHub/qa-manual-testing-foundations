# Sample Bug Reports

Este documento contiene ejemplos de bugs reportados utilizando el **Bug Report Template**, mostrando escenarios comunes en pruebas de una aplicación web.

## 🐞 Bug 001 – Login con contraseña incorrecta

| Campo | Detalle |
|-------|---------|
| Bug ID | BUG-001 |
| Título | Login no bloquea acceso con contraseña incorrecta |
| Módulo | Autenticación |
| Requerimiento | RF-LOGIN-02 |
| Reportado por | QA Analyst |
| Fecha | 02/02/2026 |
| Prioridad | Alta |
| Severidad | Crítica |
| Estado | Nuevo |

**Descripción Detallada**

- **Resumen:** El sistema permite el acceso incluso con contraseña incorrecta.  
- **Comportamiento Actual:** Usuario puede iniciar sesión con cualquier contraseña.  
- **Comportamiento Esperado:** Usuario no debe poder acceder; se debe mostrar mensaje de error.

**Pasos para Reproducir**

1. Abrir la página de login  
2. Ingresar correo válido `user@test.com`  
3. Ingresar contraseña inválida `WrongPass123`  
4. Hacer clic en “Login”

**Datos de Prueba**

- Usuario: `user@test.com`  
- Contraseña: `WrongPass123`  
- Navegador: Chrome 111  
- Ambiente: QA

**Evidencia**

- Captura de pantalla mostrando acceso exitoso con contraseña incorrecta

**Observaciones**

- Impacto crítico: afecta seguridad y experiencia del usuario

## 🐞 Bug 002 – Mensaje de error genérico en login

| Campo | Detalle |
|-------|---------|
| Bug ID | BUG-002 |
| Título | Mensaje de error poco claro al ingresar correo no registrado |
| Módulo | Autenticación |
| Requerimiento | RF-LOGIN-03 |
| Reportado por | QA Analyst |
| Fecha | 02/02/2026 |
| Prioridad | Media |
| Severidad | Media |
| Estado | Nuevo |

**Descripción Detallada**

- **Resumen:** Mensaje de error dice “Error” en lugar de indicar que el usuario no existe.  
- **Comportamiento Actual:** “Error”  
- **Comportamiento Esperado:** “El usuario no está registrado”

**Pasos para Reproducir**

1. Abrir la página de login  
2. Ingresar correo no registrado `fakeuser@test.com`  
3. Ingresar cualquier contraseña  
4. Hacer clic en “Login”

**Datos de Prueba**

- Correo: `fakeuser@test.com`  
- Contraseña: `AnyPass123`  
- Navegador: Chrome 111  
- Ambiente: QA

**Evidencia**

- Captura de pantalla mostrando mensaje “Error”

**Observaciones**

- Mejora UX: cambiar mensaje a algo descriptivo reduce confusión

## 🐞 Bug 003 – Recuperación de contraseña con enlace expirado

| Campo | Detalle |
|-------|---------|
| Bug ID | BUG-003 |
| Título | Enlace de recuperación de contraseña expira inmediatamente |
| Módulo | Recuperación de contraseña |
| Requerimiento | RF-PASSWORD-01 |
| Reportado por | QA Analyst |
| Fecha | 02/02/2026 |
| Prioridad | Alta |
| Severidad | Alta |
| Estado | Nuevo |

**Descripción Detallada**

- **Resumen:** Al enviar solicitud de recuperación, el enlace recibido no funciona o expira inmediatamente.  
- **Comportamiento Actual:** El enlace no permite restablecer la contraseña.  
- **Comportamiento Esperado:** El enlace debe ser válido durante al menos 24 horas.

**Pasos para Reproducir**

1. Abrir página de recuperación de contraseña  
2. Ingresar correo registrado `user@test.com`  
3. Hacer clic en “Enviar”  
4. Abrir enlace recibido en email  
5. Intentar restablecer la contraseña

**Datos de Prueba**

- Usuario: `user@test.com`  
- Navegador: Chrome 111  
- Ambiente: QA

**Evidencia**

- Captura de pantalla del mensaje de enlace inválido

**Observaciones**

- Impacto crítico: usuarios no pueden recuperar acceso

### 🔹 Notas finales

- Estos ejemplos muestran la aplicación de **Prioridad y Severidad**  
- Incluyen **evidencia y pasos reproducibles**  
- Permiten a un desarrollador replicar y corregir rápidamente los bugs