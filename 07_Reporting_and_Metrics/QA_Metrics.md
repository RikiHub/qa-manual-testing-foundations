# QA Metrics (and Reports)

## 1. Introducción

Las métricas de QA permiten **medir la calidad del software**, evaluar la eficiencia del proceso de testing y apoyar la toma de decisiones.  
Este documento describe las métricas utilizadas en el proyecto de **Login y Registro de Usuario**, así como los reportes generados.

## 2. Objetivos de las Métricas

- Evaluar la **efectividad de la ejecución de pruebas**  
- Medir la **densidad y severidad de defectos**  
- Facilitar **toma de decisiones basada en datos**  
- Mejorar procesos futuros y priorizar áreas críticas

## 3. Métricas Clave

### 3.1 Ejecución de Casos de Prueba

| Métrica | Fórmula | Valor |
|---------|---------|-------|
| Casos Planificados | Conteo total de casos de prueba | 13 |
| Casos Ejecutados | Conteo de casos ejecutados | 13 |
| Casos Pass | Casos exitosos | 11 |
| Casos Fail | Casos fallidos | 2 |
| Porcentaje de Ejecución | (Casos Ejecutados / Casos Planificados) * 100 | 100% |
| Porcentaje de Éxito | (Casos Pass / Casos Ejecutados) * 100 | 84.6% |

### 3.2 Defect Density (Densidad de Defectos)

- Fórmula: **# Defectos / # Casos Ejecutados**  
- Valor: 2 / 13 ≈ **0.154 defectos por caso**

### 3.3 Severidad y Prioridad de Defectos

| Severidad | Alta | Media | Baja | Total |
|-----------|------|-------|-----|-------|
| Cantidad | 1 | 1 | 0 | 2 |

| Prioridad | Alta | Media | Baja | Total |
|-----------|------|-------|-----|-------|
| Cantidad | 1 | 1 | 0 | 2 |

> Estas métricas ayudan a priorizar corrección y planificación de release.

### 3.4 Requerimientos Cubiertos

- % de requerimientos validados por pruebas: 100%  
- Todos los casos críticos fueron ejecutados y validados

## 4. Tipos de Reportes Generados

1. **Test Execution Report** – resultados detallados de cada caso  
2. **Bug Reports** – defectos documentados con severidad, prioridad y evidencia  
3. **Test Summary Report** – consolidación ejecutiva de métricas, cobertura y conclusiones  
4. **QA Metrics Report** – análisis de eficiencia, densidad de defectos y priorización

## 5. Beneficios del Reporte de Métricas

- Permite **visualizar rápidamente la salud del sistema**  
- Facilita **identificación de áreas de riesgo**  
- Mejora **planificación de corrección y release**  
- Genera **trazabilidad objetiva para auditorías**  

## 6. Conclusión

Las métricas y reportes de QA proporcionan un **análisis cuantitativo y cualitativo** del proceso de testing, mostrando eficiencia, cobertura y calidad del producto.  
La documentación clara de estas métricas refuerza tu portfolio mostrando **profesionalismo y madurez en QA**.