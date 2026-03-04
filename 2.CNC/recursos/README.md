# Recursos CNC - CECATI No. 17

Documentación técnica de referencia para la programación de control numérico por computadora (CNC), enfocada en sistemas Fanuc estándar ISO.

---

## 📚 Manuales de Referencia

### 1. **guia-maestria-programacion-cnc.pdf**

**Contenido:** Guía completa de programación CNC con énfasis en códigos G y M.

#### Temas cubiertos:
- **Fundamentos del Lenguaje G&M**
  - Lenguaje G (movimiento y geometría)
  - Lenguaje M (acciones del hardware)
  - Estandarización ISO

- **Códigos para Tornos CNC**
  - G00: Posicionamiento rápido
  - G01/G03: Interpolación lineal y circular
  - G71/G76: Ciclos automáticos de desbaste y roscado
  - M03/M05: Control de husillo

- **Códigos para Fresadoras CNC**
  - G81/G83: Ciclos de taladrado (simple y profundo)
  - G90/G91: Sistemas de coordenadas (absoluto/incremental)
  - G15/G68: Funciones avanzadas
  - G41/G42: Compensación de radio

- **Ciclos Avanzados**
  - G71: Automatización de desbaste
  - G83: Picoteo (Peck Drilling)

- **Seguridad Industrial**
  - Normas innegociables en el área de trabajo
  - Procedimientos antes de ejecutar

- **Flujo de Trabajo Completo**
  - Diseño y codificación → Simulación → Setup físico → Ejecución

---

### 2. **lenguaje-cnc-codigos-g-m-visual.pdf**

**Contenido:** Guía visual con diagramas, ilustraciones y ejemplos prácticos.

#### Temas cubiertos:
- **Anatomía de un Bloque de Código**
  - Estructura: `N5 G01 X20 Y30 F150`
  - Desglose: Secuencia, función, destino, velocidad

- **La Dualidad del Control**
  - Código G: Define movimiento (dónde va la herramienta)
  - Código M: Gestiona acciones (enciende/apaga, cambia herramienta)

- **Sistemas de Coordenadas y Planos**
  - El "cero" pieza (G90: Absoluto)
  - El "cero" desplazamiento (G91: Incremental)
  - Planos de trabajo: XY (G17), XZ (G18), YZ (G19)

- **Coreografía Básica**
  - G00: Rápido (sin cortar)
  - G01: Lineal (cortando)
  - G02/G03: Arcos horarios/antihorarios

- **Compensación de Precisión**
  - G41/G42: Climb vs. Conventional Milling
  - G40: Cancelar compensación

- **Control de Máquina**
  - M03/M04/M05: Husillo ON/OFF
  - M06/T01: Cambio de herramienta
  - M08/M09: Refrigerante
  - M30: Fin y rebobinado

- **Variaciones: CNC vs. Impresión 3D**
  - Comparativa entre procesos sustractivos (fresado) y aditivos (3D)

- **Solución de Problemas**
  - Errores comunes: colisiones, cortes imprecisos, sintaxis

---

## 🎯 Cómo Usar Estos Recursos

### Para Principiantes:
1. Comienza con **lenguaje-cnc-codigos-g-m-visual.pdf** para entender conceptos con diagramas
2. Luego consulta **guia-maestria-programacion-cnc.pdf** para profundizar

### Para Referencia Rápida:
- Hoja de referencia rápida (Cheatsheet) al final de ambos documentos
- Búsqueda por código G o M específico

### Para Proyectos:
- Usar la guía maestra como referencia técnica durante la programación
- Verificar siempre en simulación antes de ejecutar en máquina real

---

## 📋 Códigos Más Frecuentes

| Código | Descripción | Documento |
|--------|-------------|-----------|
| **G00** | Posicionamiento rápido | Ambos |
| **G01** | Interpolación lineal (corte) | Ambos |
| **G02/G03** | Arcos horario/antihorario | Ambos |
| **G17/G18/G19** | Seleccionar plano de trabajo | Visual |
| **G41/G42** | Compensación de radio | Visual |
| **G71/G76** | Ciclos de torno | Maestra |
| **G81/G83** | Ciclos de taladrado | Maestra |
| **M03/M05** | Encender/apagar husillo | Ambos |
| **M06** | Cambio de herramienta | Visual |
| **M08/M09** | Refrigerante ON/OFF | Visual |

---

## 🔧 Estándar Utilizado

- **ISO 6983** (Código G estándar internacional)
- **Controladores:** Fanuc (estándar industrial)
- **Máquinas:** Tornos CNC, Fresadoras CNC, Impresoras 3D Marlin

---

## 📝 Notas Pedagógicas

Estos documentos están diseñados para complementar la experiencia práctica en CECATI No. 17:
- Teoría visual en el aula
- Práctica en simuladores (Denford FANUC v1.96)
- Ejecución en máquinas reales bajo supervisión

**Principio:** _Simular siempre antes de ejecutar en máquina._

---

**Última actualización:** Marzo 2026  
**Institución:** CECATI No. 17 - Querétaro  
**Área:** Control Numérico CNC