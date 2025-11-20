# 🔌 PRÁCTICA: DISEÑO Y SIMULACIÓN DE CIRCUITOS ELÉCTRICOS
**Módulo:** CMO-313 - Robótica  
**Ciclo Formativo:** SMR1 - Sistemas Microinformáticos y Redes  
**Profesor:** Ezequiel Llarena Borges  
**Duración:** 3 horas  
**Fecha:** `__________________`

---

## 🎯 OBJETIVOS DE APRENDIZAJE

### Objetivos Conceptuales
- [ ] Comprender las leyes fundamentales de circuitos eléctricos (Ley de Ohm, Kirchhoff)
- [ ] Diferenciar circuitos serie, paralelo y mixto
- [ ] Identificar componentes electrónicos básicos y su simbología

### Objetivos Procedimentales
- [ ] Diseñar circuitos eléctricos en plataforma de simulación TinkerCAD
- [ ] Realizar mediciones de voltaje, corriente y resistencia con polímetros virtuales
- [ ] Verificar experimentalmente las leyes de circuitos eléctricos

### Objetivos Actitudinales
- [ ] Desarrollar precisión en mediciones y cálculos
- [ ] Fomentar el método científico en la verificación de teorías
- [ ] Promover el trabajo sistemático en diseño electrónico

---

## 📋 CRITERIOS DE EVALUACIÓN

| Criterio | Ponderación | Evidencias |
|----------|-------------|------------|
| Diseño correcto circuitos en TinkerCAD | 30% | Capturas de pantalla circuitos funcionales |
| Mediciones precisas con polímetros | 35% | Tablas de datos completas y correctas |
| Cálculos y verificaciones teóricas | 25% | Comprobación leyes Ohm y Kirchhoff |
| Documentación y presentación | 10% | Informe completo y organizado |

---

## 🛠️ MATERIAL Y HERRAMIENTAS

### Software Requerido
- [ ] **TinkerCAD** (https://www.tinkercad.com/) - Plataforma online de simulación
- [ ] Navegador web actualizado (Chrome/Firefox recomendado)
- [ ] Cuenta en Autodesk (gratuita)

### Componentes Virtuales Necesarios
┌─────────────────────────────────────────────────────────────┐
│ COMPONENTES PARA TINKERCAD │
├──────────────────────┬──────────────────┬───────────────────┤
│ COMPONENTE │ CANTIDAD │ USO │
├──────────────────────┼──────────────────┼───────────────────┤
│ Batería/Pila 9V │ 3 unidades │ Fuente alimentación│
│ Resistencias varias │ 9 unidades │ Cargas circuito │
│ Polímetros │ 3 unidades │ Mediciones V, I, R│
│ Protoboard │ 3 unidades │ Montaje circuitos │
│ LEDs (opcional) │ 6 unidades │ Visualización │
│ Cables jumpers │ Múltiples │ Conexiones │
└──────────────────────┴──────────────────┴───────────────────┘

text

### Valores de Resistencia Recomendados
- **R1:** 220Ω (Rojo-Rojo-Marrón)
- **R2:** 330Ω (Naranja-Naranja-Marrón)  
- **R3:** 470Ω (Amarillo-Violeta-Marrón)
- **R4:** 1kΩ (Marrón-Negro-Rojo)
- **R5:** 2.2kΩ (Rojo-Rojo-Rojo)

---

## 📝 PROCEDIMIENTO PASO A PASO

### FASE 1: CONFIGURACIÓN INICIAL (20 minutos)

**Paso 1.1 - Acceso a TinkerCAD**
1. [ ] Abrir https://www.tinkercad.com
2. [ ] Iniciar sesión con cuenta Autodesk
3. [ ] Crear nuevo proyecto: "Circuitos_CC_SMR1"
4. [ ] Seleccionar "Circuitos" → "Crear nuevo circuito"

**Paso 1.2 - Familiarización con la Interfaz**
┌─────────────────────────────────────────────────────────────┐
│ INTERFAZ TINKERCAD - ZONAS │
├─────────────────────────────────────────────────────────────┤
│ ZONA SUPERIOR: Barra herramientas componentes │
│ ZONA CENTRAL: Área de trabajo - Protoboard virtual │
│ ZONA DERECHA: Panel propiedades componentes │
│ ZONA INFERIOR: Controles simulación (Iniciar/Detener) │
└─────────────────────────────────────────────────────────────┘

text

**Paso 1.3 - Configuración Polímetros**
- [ ] Arrastrar 3 polímetros al área de trabajo
- [ ] Configurar cada uno para diferentes mediciones:
  - Polímetro 1: Voltímetro (V)
  - Polímetro 2: Amperímetro (A)  
  - Polímetro 3: Óhmetro (Ω)

---

## 🔧 CIRCUITO 1: SERIE (45 minutos)

### Diseño del Circuito
┌─────────────────────────────────────────────────────────────┐
│ CIRCUITO SERIE - ESQUEMA │
├─────────────────────────────────────────────────────────────┤
│ +9V ---[R1]---[R2]---[R3]--- 0V │
│ | | | | │
│ V1 V2 V3 V4 │
└─────────────────────────────────────────────────────────────┘

text

**Paso 2.1 - Montaje en Protoboard**
1. [ ] Colocar batería 9V en protoboard
2. [ ] Conectar R1 (220Ω) en serie con R2 (330Ω)
3. [ ] Conectar R2 en serie con R3 (470Ω)
4. [ ] Completar circuito cerrado
5. [ ] Verificar conexiones correctas

**Paso 2.2 - Mediciones de Voltaje**
| Punto de Medición | Valor Teórico | Valor Medido | Diferencia |
|-------------------|---------------|--------------|------------|
| V1 (Total) | 9V | `_____ V` | `_____ V` |
| V_R1 | `_____ V` | `_____ V` | `_____ V` |
| V_R2 | `_____ V` | `_____ V` | `_____ V` |
| V_R3 | `_____ V` | `_____ V` | `_____ V` |
| **Suma V_R1+V_R2+V_R3** | **9V** | **`_____ V`** | **`_____ V`** |

**Paso 2.3 - Mediciones de Corriente**
- [ ] Colocar amperímetro en serie con R1: `_____ A`
- [ ] Colocar amperímetro en serie con R2: `_____ A`  
- [ ] Colocar amperímetro en serie con R3: `_____ A`
- [ ] **Verificación:** I_R1 = I_R2 = I_R3 = `_____ A`

**Paso 2.4 - Cálculos Teóricos**
Resistencia Total (R_T) = R1 + R2 + R3 = _____ Ω
Corriente Teórica (I) = V / R_T = 9V / _____ Ω = _____ A
Voltaje R1 Teórico = I × R1 = _____ A × 220Ω = _____ V
Voltaje R2 Teórico = _____ A × 330Ω = _____ V
Voltaje R3 Teórico = _____ A × 470Ω = _____ V

text

---

## ⚡ CIRCUITO 2: PARALELO (45 minutos)

### Diseño del Circuito
┌─────────────────────────────────────────────────────────────┐
│ CIRCUITO PARALELO - ESQUEMA │
├─────────────────────────────────────────────────────────────┤
│ +---[R1]---+ │
│ | | │
│ +9V +---[R2]---+ 0V │
│ | | │
│ +---[R3]---+ │
│ | | | │
│ I1 I2 I3 │
└─────────────────────────────────────────────────────────────┘

text

**Paso 3.1 - Montaje en Nueva Protoboard**
1. [ ] Colocar batería 9V
2. [ ] Conectar R1, R2, R3 en paralelo
3. [ ] Verificar que todas las resistencias tengan mismo voltaje

**Paso 3.2 - Mediciones de Corriente**
| Rama | Resistencia | Corriente Teórica | Corriente Medida | Diferencia |
|------|-------------|-------------------|------------------|------------|
| R1 | 220Ω | `_____ A` | `_____ A` | `_____ A` |
| R2 | 330Ω | `_____ A` | `_____ A` | `_____ A` |
| R3 | 470Ω | `_____ A` | `_____ A` | `_____ A` |
| **Total** | **`_____ Ω`** | **`_____ A`** | **`_____ A`** | **`_____ A`** |

**Paso 3.3 - Mediciones de Voltaje**
- [ ] Voltaje en R1: `_____ V`
- [ ] Voltaje en R2: `_____ V`
- [ ] Voltaje en R3: `_____ V`
- [ ] **Verificación:** V_R1 = V_R2 = V_R3 = 9V

**Paso 3.4 - Cálculos Teóricos**
1/R_T = 1/R1 + 1/R2 + 1/R3 = 1/220 + 1/330 + 1/470 = _____ Ω
R_Total = _____ Ω
I_Total = V / R_T = 9V / _____ Ω = _____ A
I_R1 = 9V / 220Ω = _____ A
I_R2 = 9V / 330Ω = _____ A
I_R3 = 9V / 470Ω = _____ A

text

---

## 🔄 CIRCUITO 3: MIXTO (45 minutos)

### Diseño del Circuito
┌─────────────────────────────────────────────────────────────┐
│ CIRCUITO MIXTO - ESQUEMA │
├─────────────────────────────────────────────────────────────┤
│ +9V ---[R1]---+---[R2]---+--- 0V │
│ | | │
│ [R3] [R4] │
│ | | │
│ +-----------+ │
└─────────────────────────────────────────────────────────────┘

text

**Valores Recomendados:** R1=1kΩ, R2=2.2kΩ, R3=330Ω, R4=470Ω

**Paso 4.1 - Montaje Complejo**
1. [ ] Colocar R1 en serie con combinación R2-R3-R4
2. [ ] Conectar R3 y R4 en paralelo entre R1 y R2
3. [ ] Verificar todas las conexiones

**Paso 4.2 - Mediciones Completas**
| Parámetro | Valor Teórico | Valor Medido | Diferencia |
|-----------|---------------|--------------|------------|
| V Total | 9V | `_____ V` | `_____ V` |
| V_R1 | `_____ V` | `_____ V` | `_____ V` |
| V_R2 | `_____ V` | `_____ V` | `_____ V` |
| V_R3 | `_____ V` | `_____ V` | `_____ V` |
| V_R4 | `_____ V` | `_____ V` | `_____ V` |
| I Total | `_____ A` | `_____ A` | `_____ A` |
| I_R1 | `_____ A` | `_____ A` | `_____ A` |
| I_R2 | `_____ A` | `_____ A` | `_____ A` |
| I_R3 | `_____ A` | `_____ A` | `_____ A` |
| I_R4 | `_____ A` | `_____ A` | `_____ A` |

**Paso 4.3 - Cálculos Avanzados**
R_paralelo = (R3 × R4) / (R3 + R4) = _____ Ω
R_total = R1 + R_paralelo + R2 = _____ Ω
I_total = 9V / R_total = _____ A
V_R1 = I_total × R1 = _____ V
V_paralelo = I_total × R_paralelo = _____ V
V_R2 = I_total × R2 = _____ V

text

---

## 💡 ACTIVIDAD OPCIONAL: CIRCUITO CON LEDs (25 minutos)

### Diseño con LEDs
┌─────────────────────────────────────────────────────────────┐
│ CIRCUITO LED - ESQUEMA │
├─────────────────────────────────────────────────────────────┤
│ +9V ---[R1 220Ω]---[LED Rojo]--- 0V │
│ [R2 330Ω]---[LED Verde]--- │
│ [R3 470Ω]---[LED Azul]---- │
└─────────────────────────────────────────────────────────────┘

text

**Paso 5.1 - Consideraciones LEDs**
- [ ] Los LEDs requieren resistencia limitadora de corriente
- [ ] Verificar polaridad (ánodo +, cátodo -)
- [ ] Observar intensidad luminosa según resistencia

**Paso 5.2 - Mediciones**
- [ ] Corriente en LED rojo: `_____ A`
- [ ] Corriente en LED verde: `_____ A`
- [ ] Corriente en LED azul: `_____ A`
- [ ] Voltaje en cada LED: `_____ V`

---

## 📊 FICHA DE TRABAJO DEL ALUMNO

**Nombre:** _________________________  
**Grupo:** ______ **Fecha:** __________

### CHECKLIST COMPLETACIÓN
| Circuito | Montaje | Mediciones | Cálculos | Capturas |
|----------|---------|------------|----------|----------|
| Serie | ☐ | ☐ | ☐ | ☐ |
| Paralelo | ☐ | ☐ | ☐ | ☐ |
| Mixto | ☐ | ☐ | ☐ | ☐ |
| LEDs (opc) | ☐ | ☐ | ☐ | ☐ |

### VERIFICACIÓN LEYES FUNDAMENTALES
| Ley | Circuito Serie | Circuito Paralelo | Circuito Mixto |
|-----|----------------|-------------------|----------------|
| **Ley de Ohm** (V=I×R) | ☐ Correcta | ☐ Correcta | ☐ Correcta |
| **Kirchhoff Voltajes** (ΣV=0) | ☐ Verificada | ☐ Verificada | ☐ Verificada |
| **Kirchhoff Corrientes** (ΣI=0) | ☐ Verificada | ☐ Verificada | ☐ Verificada |

### INCIDENCIAS Y OBSERVACIONES
Dificultades encontradas en el montaje:

Diferencias entre valores teóricos y medidos:

Comportamiento observado en circuitos:

text

---

## 🎓 RECURSOS DE APOYO

### 📚 Documentación Técnica
- [Guía oficial TinkerCAD Circuits](https://www.tinkercad.com/learn/circuits)
- [Tutorial mediciones con polímetro virtual](https://www.tinkercad.com/things/0xqL1dF2d7F)
- [Tabla código colores resistencias](https://www.allaboutcircuits.com/tools/resistor-color-code-calculator/)

### 🎥 Video Tutoriales
- [Introducción a TinkerCAD Circuits](https://youtube.com/watch?v=yaS7m
se me olvidarondos cosas una que el guion incluya un cuadro para que el alumno pueda insertar captura del circuito diseñado mostrando los polimetros con las mediciones. y ademas que pueda rellenar los valores en las tablas resultado y por ultimo un boton para que se pueda descargar en pd con nombre completo de alumno y grupo , fecha y nombre profesor
Guion de Práctica - Robótica CMO-313 (Versión Mejorada)
markdown
# 🔌 PRÁCTICA: DISEÑO Y SIMULACIÓN DE CIRCUITOS ELÉCTRICOS
**Módulo:** CMO-313 - Robótica  
**Ciclo Formativo:** SMR1 - Sistemas Microinformáticos y Redes  
**Profesor:** Ezequiel Llarena Borges  
**Duración:** 3 horas  
**Fecha:** `__________________`

---

<div class="student-info">
    <div class="info-field">
        <label>Nombre completo del alumno:</label>
        <input type="text" id="studentName" placeholder="Escribe tu nombre completo">
    </div>
    <div class="info-field">
        <label>Grupo:</label>
        <input type="text" id="studentGroup" placeholder="Ej: SMR1A">
    </div>
    <div class="info-field">
        <label>Fecha de realización:</label>
        <input type="date" id="practiceDate">
    </div>
</div>

---

## 🎯 OBJETIVOS DE APRENDIZAJE

### Objetivos Conceptuales
- [ ] Comprender las leyes fundamentales de circuitos eléctricos (Ley de Ohm, Kirchhoff)
- [ ] Diferenciar circuitos serie, paralelo y mixto
- [ ] Identificar componentes electrónicos básicos y su simbología

### Objetivos Procedimentales
- [ ] Diseñar circuitos eléctricos en plataforma de simulación TinkerCAD
- [ ] Realizar mediciones de voltaje, corriente y resistencia con polímetros virtuales
- [ ] Verificar experimentalmente las leyes de circuitos eléctricos

### Objetivos Actitudinales
- [ ] Desarrollar precisión en mediciones y cálculos
- [ ] Fomentar el método científico en la verificación de teorías
- [ ] Promover el trabajo sistemático en diseño electrónico

---

## 📋 CRITERIOS DE EVALUACIÓN

| Criterio | Ponderación | Evidencias |
|----------|-------------|------------|
| Diseño correcto circuitos en TinkerCAD | 30% | Capturas de pantalla circuitos funcionales |
| Mediciones precisas con polímetros | 35% | Tablas de datos completas y correctas |
| Cálculos y verificaciones teóricas | 25% | Comprobación leyes Ohm y Kirchhoff |
| Documentación y presentación | 10% | Informe completo y organizado |

---

## 🛠️ MATERIAL Y HERRAMIENTAS

### Software Requerido
- [ ] **TinkerCAD** (https://www.tinkercad.com/) - Plataforma online de simulación
- [ ] Navegador web actualizado (Chrome/Firefox recomendado)
- [ ] Cuenta en Autodesk (gratuita)

### Componentes Virtuales Necesarios
┌─────────────────────────────────────────────────────────────┐
│ COMPONENTES PARA TINKERCAD │
├──────────────────────┬──────────────────┬───────────────────┤
│ COMPONENTE │ CANTIDAD │ USO │
├──────────────────────┼──────────────────┼───────────────────┤
│ Batería/Pila 9V │ 3 unidades │ Fuente alimentación│
│ Resistencias varias │ 9 unidades │ Cargas circuito │
│ Polímetros │ 3 unidades │ Mediciones V, I, R│
│ Protoboard │ 3 unidades │ Montaje circuitos │
│ LEDs (opcional) │ 6 unidades │ Visualización │
│ Cables jumpers │ Múltiples │ Conexiones │
└──────────────────────┴──────────────────┴───────────────────┘

text

### Valores de Resistencia Recomendados
- **R1:** 220Ω (Rojo-Rojo-Marrón)
- **R2:** 330Ω (Naranja-Naranja-Marrón)  
- **R3:** 470Ω (Amarillo-Violeta-Marrón)
- **R4:** 1kΩ (Marrón-Negro-Rojo)
- **R5:** 2.2kΩ (Rojo-Rojo-Rojo)

---

## 🔧 CIRCUITO 1: SERIE (45 minutos)

### Diseño del Circuito
┌─────────────────────────────────────────────────────────────┐
│ CIRCUITO SERIE - ESQUEMA │
├─────────────────────────────────────────────────────────────┤
│ +9V ---[R1]---[R2]---[R3]--- 0V │
│ | | | | │
│ V1 V2 V3 V4 │
└─────────────────────────────────────────────────────────────┘

text

**Paso 2.1 - Montaje en Protoboard**
1. [ ] Colocar batería 9V en protoboard
2. [ ] Conectar R1 (220Ω) en serie con R2 (330Ω)
3. [ ] Conectar R2 en serie con R3 (470Ω)
4. [ ] Completar circuito cerrado
5. [ ] Verificar conexiones correctas

**Paso 2.2 - Mediciones de Voltaje**
| Punto de Medición | Valor Teórico | Valor Medido | Diferencia |
|-------------------|---------------|--------------|------------|
| V1 (Total) | 9V | <input type="text" class="measurement" data-circuit="serie" data-measure="v_total"> V | <input type="text" class="difference" readonly> V |
| V_R1 | <input type="text" class="theoretical" data-circuit="serie" data-measure="v_r1"> V | <input type="text" class="measurement" data-circuit="serie" data-measure="v_r1"> V | <input type="text" class="difference" readonly> V |
| V_R2 | <input type="text" class="theoretical" data-circuit="serie" data-measure="v_r2"> V | <input type="text" class="measurement" data-circuit="serie" data-measure="v_r2"> V | <input type="text" class="difference" readonly> V |
| V_R3 | <input type="text" class="theoretical" data-circuit="serie" data-measure="v_r3"> V | <input type="text" class="measurement" data-circuit="serie" data-measure="v_r3"> V | <input type="text" class="difference" readonly> V |
| **Suma V_R1+V_R2+V_R3** | **9V** | **<span id="sum_voltages_serie">0</span> V** | **<span id="diff_voltages_serie">0</span> V** |

**Paso 2.3 - Mediciones de Corriente**
- [ ] Colocar amperímetro en serie con R1: <input type="text" class="measurement" data-circuit="serie" data-measure="i_r1"> A
- [ ] Colocar amperímetro en serie con R2: <input type="text" class="measurement" data-circuit="serie" data-measure="i_r2"> A  
- [ ] Colocar amperímetro en serie con R3: <input type="text" class="measurement" data-circuit="serie" data-measure="i_r3"> A
- [ ] **Verificación:** I_R1 = I_R2 = I_R3 = <span id="current_verification_serie">___</span> A

**Paso 2.4 - Cálculos Teóricos**
Resistencia Total (R_T) = R1 + R2 + R3 = <input type="text" class="calculation" data-circuit="serie" data-calc="r_total"> Ω
Corriente Teórica (I) = V / R_T = 9V / <span id="r_total_serie"></span> Ω = <input type="text" class="calculation" data-circuit="serie" data-calc="i_total"> A
Voltaje R1 Teórico = I × R1 = <span id="i_total_serie"></span> A × 220Ω = <input type="text" class="calculation" data-circuit="serie" data-calc="v_r1_theo"> V
Voltaje R2 Teórico = <span id="i_total_serie2"></span> A × 330Ω = <input type="text" class="calculation" data-circuit="serie" data-calc="v_r2_theo"> V
Voltaje R3 Teórico = <span id="i_total_serie3"></span> A × 470Ω = <input type="text" class="calculation" data-circuit="serie" data-calc="v_r3_theo"> V

text

### 📸 CAPTURA CIRCUITO SERIE
<div class="screenshot-section">
    <div class="screenshot-instructions">
        <strong>Instrucciones para captura:</strong>
        <ol>
            <li>Completar el circuito en TinkerCAD</li>
            <li>Colocar polímetros mostrando mediciones</li>
            <li>Hacer captura de pantalla (Print Screen)</li>
            <li>Pegar en un documento y guardar como imagen</li>
        </ol>
    </div>
    <div class="screenshot-upload">
        <label>Insertar captura del circuito serie:</label>
        <input type="file" id="screenshotSerie" accept="image/*" class="screenshot-input">
        <div id="screenshotPreviewSerie" class="screenshot-preview"></div>
    </div>
</div>

---

## ⚡ CIRCUITO 2: PARALELO (45 minutos)

### Diseño del Circuito
┌─────────────────────────────────────────────────────────────┐
│ CIRCUITO PARALELO - ESQUEMA │
├─────────────────────────────────────────────────────────────┤
│ +---[R1]---+ │
│ | | │
│ +9V +---[R2]---+ 0V │
│ | | │
│ +---[R3]---+ │
│ | | | │
│ I1 I2 I3 │
└─────────────────────────────────────────────────────────────┘

text

**Paso 3.1 - Montaje en Nueva Protoboard**
1. [ ] Colocar batería 9V
2. [ ] Conectar R1, R2, R3 en paralelo
3. [ ] Verificar que todas las resistencias tengan mismo voltaje

**Paso 3.2 - Mediciones de Corriente**
| Rama | Resistencia | Corriente Teórica | Corriente Medida | Diferencia |
|------|-------------|-------------------|------------------|------------|
| R1 | 220Ω | <input type="text" class="theoretical" data-circuit="paralelo" data-measure="i_r1_theo"> A | <input type="text" class="measurement" data-circuit="paralelo" data-measure="i_r1"> A | <input type="text" class="difference" readonly> A |
| R2 | 330Ω | <input type="text" class="theoretical" data-circuit="paralelo" data-measure="i_r2_theo"> A | <input type="text" class="measurement" data-circuit="paralelo" data-measure="i_r2"> A | <input type="text" class="difference" readonly> A |
| R3 | 470Ω | <input type="text" class="theoretical" data-circuit="paralelo" data-measure="i_r3_theo"> A | <input type="text" class="measurement" data-circuit="paralelo" data-measure="i_r3"> A | <input type="text" class="difference" readonly> A |
| **Total** | **<span id="r_total_paralelo">___</span> Ω** | **<input type="text" class="theoretical" data-circuit="paralelo" data-measure="i_total_theo"> A** | **<input type="text" class="measurement" data-circuit="paralelo" data-measure="i_total"> A** | **<input type="text" class="difference" readonly> A** |

**Paso 3.3 - Mediciones de Voltaje**
- [ ] Voltaje en R1: <input type="text" class="measurement" data-circuit="paralelo" data-measure="v_r1"> V
- [ ] Voltaje en R2: <input type="text" class="measurement" data-circuit="paralelo" data-measure="v_r2"> V
- [ ] Voltaje en R3: <input type="text" class="measurement" data-circuit="paralelo" data-measure="v_r3"> V
- [ ] **Verificación:** V_R1 = V_R2 = V_R3 = 9V

**Paso 3.4 - Cálculos Teóricos**
1/R_T = 1/R1 + 1/R2 + 1/R3 = 1/220 + 1/330 + 1/470 = <input type="text" class="calculation" data-circuit="paralelo" data-calc="r_parallel"> Ω
R_Total = <span id="r_total_calc_paralelo"></span> Ω
I_Total = V / R_T = 9V / <span id="r_total_for_current"></span> Ω = <input type="text" class="calculation" data-circuit="paralelo" data-calc="i_total_theo"> A
I_R1 = 9V / 220Ω = <input type="text" class="calculation" data-circuit="paralelo" data-calc="i_r1_theo"> A
I_R2 = 9V / 330Ω = <input type="text" class="calculation" data-circuit="paralelo" data-calc="i_r2_theo"> A
I_R3 = 9V / 470Ω = <input type="text" class="calculation" data-circuit="paralelo" data-calc="i_r3_theo"> A

text

### 📸 CAPTURA CIRCUITO PARALELO
<div class="screenshot-section">
    <div class="screenshot-upload">
        <label>Insertar captura del circuito paralelo:</label>
        <input type="file" id="screenshotParalelo" accept="image/*" class="screenshot-input">
        <div id="screenshotPreviewParalelo" class="screenshot-preview"></div>
    </div>
</div>

---

## 🔄 CIRCUITO 3: MIXTO (45 minutos)

### Diseño del Circuito
┌─────────────────────────────────────────────────────────────┐
│ CIRCUITO MIXTO - ESQUEMA │
├─────────────────────────────────────────────────────────────┤
│ +9V ---[R1]---+---[R2]---+--- 0V │
│ | | │
│ [R3] [R4] │
│ | | │
│ +-----------+ │
└─────────────────────────────────────────────────────────────┘

text

**Valores Recomendados:** R1=1kΩ, R2=2.2kΩ, R3=330Ω, R4=470Ω

**Paso 4.1 - Montaje Complejo**
1. [ ] Colocar R1 en serie con combinación R2-R3-R4
2. [ ] Conectar R3 y R4 en paralelo entre R1 y R2
3. [ ] Verificar todas las conexiones

**Paso 4.2 - Mediciones Completas**
| Parámetro | Valor Teórico | Valor Medido | Diferencia |
|-----------|---------------|--------------|------------|
| V Total | 9V | <input type="text" class="measurement" data-circuit="mixto" data-measure="v_total"> V | <input type="text" class="difference" readonly> V |
| V_R1 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="v_r1_theo"> V | <input type="text" class="measurement" data-circuit="mixto" data-measure="v_r1"> V | <input type="text" class="difference" readonly> V |
| V_R2 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="v_r2_theo"> V | <input type="text" class="measurement" data-circuit="mixto" data-measure="v_r2"> V | <input type="text" class="difference" readonly> V |
| V_R3 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="v_r3_theo"> V | <input type="text" class="measurement" data-circuit="mixto" data-measure="v_r3"> V | <input type="text" class="difference" readonly> V |
| V_R4 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="v_r4_theo"> V | <input type="text" class="measurement" data-circuit="mixto" data-measure="v_r4"> V | <input type="text" class="difference" readonly> V |
| I Total | <input type="text" class="theoretical" data-circuit="mixto" data-measure="i_total_theo"> A | <input type="text" class="measurement" data-circuit="mixto" data-measure="i_total"> A | <input type="text" class="difference" readonly> A |
| I_R1 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="i_r1_theo"> A | <input type="text" class="measurement" data-circuit="mixto" data-measure="i_r1"> A | <input type="text" class="difference" readonly> A |
| I_R2 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="i_r2_theo"> A | <input type="text" class="measurement" data-circuit="mixto" data-measure="i_r2"> A | <input type="text" class="difference" readonly> A |
| I_R3 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="i_r3_theo"> A | <input type="text" class="measurement" data-circuit="mixto" data-measure="i_r3"> A | <input type="text" class="difference" readonly> A |
| I_R4 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="i_r4_theo"> A | <input type="text" class="measurement" data-circuit="mixto" data-measure="i_r4"> A | <input type="text" class="difference" readonly> A |

**Paso 4.3 - Cálculos Avanzados**
R_paralelo = (R3 × R4) / (R3 + R4) = <input type="text" class="calculation" data-circuit="mixto" data-calc="r_parallel"> Ω
R_total = R1 + R_paralelo + R2 = <span id="r_total_mixto">___</span> Ω
I_total = 9V / R_total = <input type="text" class="calculation" data-circuit="mixto" data-calc="i_total_theo"> A
V_R1 = I_total × R1 = <input type="text" class="calculation" data-circuit="mixto" data-calc="v_r1_theo"> V
V_paralelo = I_total × R_paralelo = <input type="text" class="calculation" data-circuit="mixto" data-calc="v_parallel_theo"> V
V_R2 = I_total × R2 = <input type="text" class="calculation" data-circuit="mixto" data-calc="v_r2_theo"> V

text

### 📸 CAPTURA CIRCUITO MIXTO
<div class="screenshot-section">
    <div class="screenshot-upload">
        <label>Insertar captura del circuito mixto:</label>
        <input type="file" id="screenshotMixto" accept="image/*" class="screenshot-input">
        <div id="screenshotPreviewMixto" class="screenshot-preview"></div>
    </div>
</div>

---

## 💡 ACTIVIDAD OPCIONAL: CIRCUITO CON LEDs (25 minutos)

### Diseño con LEDs
┌─────────────────────────────────────────────────────────────┐
│ CIRCUITO LED - ESQUEMA │
├─────────────────────────────────────────────────────────────┤
│ +9V ---[R1 220Ω]---[LED Rojo]--- 0V │
│ [R2 330Ω]---[LED Verde]--- │
│ [R3 470Ω]---[LED Azul]---- │
└─────────────────────────────────────────────────────────────┘

text

**Paso 5.1 - Consideraciones LEDs**
- [ ] Los LEDs requieren resistencia limitadora de corriente
- [ ] Verificar polaridad (ánodo +, cátodo -)
- [ ] Observar intensidad luminosa según resistencia

**Paso 5.2 - Mediciones**
- [ ] Corriente en LED rojo: <input type="text" class="measurement" data-circuit="leds" data-measure="i_led_rojo"> A
- [ ] Corriente en LED verde: <input type="text" class="measurement" data-circuit="leds" data-measure="i_led_verde"> A
- [ ] Corriente en LED azul: <input type="text" class="measurement" data-circuit="leds" data-measure="i_led_azul"> A
- [ ] Voltaje en cada LED: <input type="text" class="measurement" data-circuit="leds" data-measure="v_led"> V

### 📸 CAPTURA CIRCUITO LEDs
<div class="screenshot-section">
    <div class="screenshot-upload">
        <label>Insertar captura del circuito con LEDs:</label>
        <input type="file" id="screenshotLEDs" accept="image/*" class="screenshot-input">
        <div id="screenshotPreviewLEDs" class="screenshot-preview"></div>
    </div>
</div>

---

## 📊 FICHA DE TRABAJO DEL ALUMNO

### CHECKLIST COMPLETACIÓN
| Circuito | Montaje | Mediciones | Cálculos | Capturas |
|----------|---------|------------|----------|----------|
| Serie | ☐ | ☐ | ☐ | ☐ |
| Paralelo | ☐ | ☐ | ☐ | ☐ |
| Mixto | ☐ | ☐ | ☐ | ☐ |
| LEDs (opc) | ☐ | ☐ | ☐ | ☐ |

### VERIFICACIÓN LEYES FUNDAMENTALES
| Ley | Circuito Serie | Circuito Paralelo | Circuito Mixto |
|-----|----------------|-------------------|----------------|
| **Ley de Ohm** (V=I×R) | ☐ Correcta | ☐ Correcta | ☐ Correcta |
| **Kirchhoff Voltajes** (ΣV=0) | ☐ Verificada | ☐ Verificada | ☐ Verificada |
| **Kirchhoff Corrientes** (ΣI=0) | ☐ Verificada | ☐ Verificada | ☐ Verificada |

### INCIDENCIAS Y OBSERVACIONES
<textarea id="observations" placeholder="Describe aquí las dificultades encontradas, diferencias entre valores teóricos y medidos, y comportamientos observados en los circuitos..." rows="4" style="width: 100%; padding: 10px; border: 1px solid #ddd; border-radius: 5px; margin: 10px 0;"></textarea>

---

## 🎓 RECURSOS DE APOYO

### 📚 Documentación Técnica
- [Guía oficial TinkerCAD Circuits](https://www.tinkercad.com/learn/circuits)
- [Tutorial mediciones con polímetro virtual](https://www.tinkercad.com/things/0xqL1dF2d7F)
- [Tabla código colores resistencias](https://www.allaboutcircuits.com/tools/resistor-color-code-calculator/)

### 🎥 Video Tutoriales
- [Introducción a TinkerCAD Circuits](https://youtube.com/watch?v=yaS7m84YeD8)
- [Mediciones con polímetro virtual](https://youtube.com/watch?v=2-4L0gTjXsQ)
- [Circuitos serie, paralelo y mixto](https://youtube.com/watch?v=7vfd

