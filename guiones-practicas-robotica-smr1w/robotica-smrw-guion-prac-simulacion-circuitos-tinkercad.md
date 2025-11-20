# Práctica: DISEÑO Y SIMULACIÓN DE CIRCUITOS ELÉCTRICOS
**Módulo:** Informática aplicada a sistemas eléctrónicos - Robótica (CMO-313)  
**Ciclo Formativo:** Sistemas Microinformáticos y Redes (SMR1W)
**Profesor:** Ezequiel Llarena Borges  
**Duración:** 3 horas  
**Fecha:** `  ...  `

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

## 1. OBJETIVOS DE APRENDIZAJE

### 1.1. Objetivos conceptuales
- [ ] Comprender las leyes fundamentales de circuitos eléctricos (Ley de Ohm, Kirchhoff)
- [ ] Diferenciar circuitos serie, paralelo y mixto
- [ ] Identificar componentes electrónicos básicos y su simbología

### 1.2. Objetivos procedimentales
- [ ] Diseñar circuitos eléctricos en plataforma de simulación Tinkercad
- [ ] Realizar mediciones de voltaje, corriente y resistencia con polímetros virtuales
- [ ] Verificar experimentalmente las leyes de circuitos eléctricos

### 1.3. Objetivos actitudinales
- [ ] Desarrollar precisión en mediciones y cálculos
- [ ] Fomentar el método científico en la verificación de teorías
- [ ] Promover el trabajo sistemático en diseño electrónico

---

## 2. CRITERIOS DE EVALUACIÓN

| Criterio | Ponderación | Evidencias |
|----------|-------------|------------|
| Diseño correcto circuitos | 30% | Capturas de pantalla circuitos funcionales |
| Mediciones precisas con polímetros | 35% | Tablas de datos completas y correctas |
| Cálculos y verificaciones teóricas | 25% | Comprobación leyes Ohm y Kirchhoff |
| Documentación y presentación | 10% | Informe completo y organizado |

---

## 3. HERRAMIENTAS Y MATERIAL NECESARIO

### 3.1. Software necesario
- [ ] **TinkerCAD** (https://www.tinkercad.com/) - Plataforma online de simulación
- [ ] Navegador web actualizado (Chrome/Firefox recomendado)
- [ ] Cuenta en Autodesk (gratuita)

### 3.2. Componentes Virtuales Necesarios
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

### 3.3. Valores de resistencia recomendados
- **R1:** 220Ω `rojo-rojo-marrón`
- **R2:** 330Ω `naranja-naranja-marrón` 
- **R3:** 470Ω `amarillo-violeta-marrón`
- **R4:** 1kΩ `marrón-negro-rojo`
- **R5:** 2.2kΩ `rojo-rojo-rojo`

---

## 4. CIRCUITO 1: SERIE
_Duración estimada: 45 minutos_

### 4.1. Diseño del circuito
┌─────────────────────────────────────────────────────────────┐
│ CIRCUITO SERIE - ESQUEMA │
├─────────────────────────────────────────────────────────────┤
│ +9V ---[R1]---[R2]---[R3]--- 0V │
│ | | | | │
│ V1 V2 V3 V4 │
└─────────────────────────────────────────────────────────────┘

**Paso 4.1.1 - Montaje en Protoboard**
1. [ ] Colocar batería 9V en protoboard
2. [ ] Conectar R1 (220Ω) en serie con R2 (330Ω)
3. [ ] Conectar R2 en serie con R3 (470Ω)
4. [ ] Completar circuito cerrado
5. [ ] Verificar conexiones correctas

**Paso 4.1.2 - Mediciones de Voltaje**
| Punto de Medición | Valor Teórico | Valor Medido | Diferencia |
|-------------------|---------------|--------------|------------|
| V1 (Total) | 9V | <input type="text" class="measurement" data-circuit="serie" data-measure="v_total"> V | <input type="text" class="difference" readonly> V |
| V_R1 | <input type="text" class="theoretical" data-circuit="serie" data-measure="v_r1"> V | <input type="text" class="measurement" data-circuit="serie" data-measure="v_r1"> V | <input type="text" class="difference" readonly> V |
| V_R2 | <input type="text" class="theoretical" data-circuit="serie" data-measure="v_r2"> V | <input type="text" class="measurement" data-circuit="serie" data-measure="v_r2"> V | <input type="text" class="difference" readonly> V |
| V_R3 | <input type="text" class="theoretical" data-circuit="serie" data-measure="v_r3"> V | <input type="text" class="measurement" data-circuit="serie" data-measure="v_r3"> V | <input type="text" class="difference" readonly> V |
| **Suma V_R1+V_R2+V_R3** | **9V** | **<span id="sum_voltages_serie">0</span> V** | **<span id="diff_voltages_serie">0</span> V** |

**Paso 4.1.3 - Mediciones de Corriente**
- [ ] Colocar amperímetro en serie con R1: <input type="text" class="measurement" data-circuit="serie" data-measure="i_r1"> A
- [ ] Colocar amperímetro en serie con R2: <input type="text" class="measurement" data-circuit="serie" data-measure="i_r2"> A  
- [ ] Colocar amperímetro en serie con R3: <input type="text" class="measurement" data-circuit="serie" data-measure="i_r3"> A
- [ ] **Verificación:** I_R1 = I_R2 = I_R3 = <span id="current_verification_serie">___</span> A

**Paso 4.1.4 - Cálculos teóricos**
Resistencia Total (R_T) = R1 + R2 + R3 = <input type="text" class="calculation" data-circuit="serie" data-calc="r_total"> Ω
Corriente Teórica (I) = V / R_T = 9V / <span id="r_total_serie"></span> Ω = <input type="text" class="calculation" data-circuit="serie" data-calc="i_total"> A
Voltaje R1 Teórico = I × R1 = <span id="i_total_serie"></span> A × 220Ω = <input type="text" class="calculation" data-circuit="serie" data-calc="v_r1_theo"> V
Voltaje R2 Teórico = <span id="i_total_serie2"></span> A × 330Ω = <input type="text" class="calculation" data-circuit="serie" data-calc="v_r2_theo"> V
Voltaje R3 Teórico = <span id="i_total_serie3"></span> A × 470Ω = <input type="text" class="calculation" data-circuit="serie" data-calc="v_r3_theo"> V

### 4.2. Capatura circuito 1 (Serie)
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

## 5. CIRCUITO 2: PARALELO 
_Duración estimada: 45 minutos_

### 5.1. Diseño del circuito
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

**Paso 5.1.1 - Montaje en nueva Protoboard**
1. [ ] Colocar batería 9V
2. [ ] Conectar R1, R2, R3 en paralelo
3. [ ] Verificar que todas las resistencias tengan mismo voltaje

**Paso 5.1.2 - Mediciones de Corriente**
| Rama | Resistencia | Corriente Teórica | Corriente Medida | Diferencia |
|------|-------------|-------------------|------------------|------------|
| R1 | 220Ω | <input type="text" class="theoretical" data-circuit="paralelo" data-measure="i_r1_theo"> A | <input type="text" class="measurement" data-circuit="paralelo" data-measure="i_r1"> A | <input type="text" class="difference" readonly> A |
| R2 | 330Ω | <input type="text" class="theoretical" data-circuit="paralelo" data-measure="i_r2_theo"> A | <input type="text" class="measurement" data-circuit="paralelo" data-measure="i_r2"> A | <input type="text" class="difference" readonly> A |
| R3 | 470Ω | <input type="text" class="theoretical" data-circuit="paralelo" data-measure="i_r3_theo"> A | <input type="text" class="measurement" data-circuit="paralelo" data-measure="i_r3"> A | <input type="text" class="difference" readonly> A |
| **Total** | **<span id="r_total_paralelo">___</span> Ω** | **<input type="text" class="theoretical" data-circuit="paralelo" data-measure="i_total_theo"> A** | **<input type="text" class="measurement" data-circuit="paralelo" data-measure="i_total"> A** | **<input type="text" class="difference" readonly> A** |

**Paso 5.1.3 - Mediciones de Voltaje**
- [ ] Voltaje en R1: <input type="text" class="measurement" data-circuit="paralelo" data-measure="v_r1"> V
- [ ] Voltaje en R2: <input type="text" class="measurement" data-circuit="paralelo" data-measure="v_r2"> V
- [ ] Voltaje en R3: <input type="text" class="measurement" data-circuit="paralelo" data-measure="v_r3"> V
- [ ] **Verificación:** V_R1 = V_R2 = V_R3 = 9V

**Paso 5.1.4 - Cálculos teóricos**
1/R_T = 1/R1 + 1/R2 + 1/R3 = 1/220 + 1/330 + 1/470 = <input type="text" class="calculation" data-circuit="paralelo" data-calc="r_parallel"> Ω
R_Total = <span id="r_total_calc_paralelo"></span> Ω
I_Total = V / R_T = 9V / <span id="r_total_for_current"></span> Ω = <input type="text" class="calculation" data-circuit="paralelo" data-calc="i_total_theo"> A
I_R1 = 9V / 220Ω = <input type="text" class="calculation" data-circuit="paralelo" data-calc="i_r1_theo"> A
I_R2 = 9V / 330Ω = <input type="text" class="calculation" data-circuit="paralelo" data-calc="i_r2_theo"> A
I_R3 = 9V / 470Ω = <input type="text" class="calculation" data-circuit="paralelo" data-calc="i_r3_theo"> A

### 5.1.5. Captura circuito 2 (Paralelo)
<div class="screenshot-section">
    <div class="screenshot-upload">
        <label>Insertar captura del circuito paralelo:</label>
        <input type="file" id="screenshotParalelo" accept="image/*" class="screenshot-input">
        <div id="screenshotPreviewParalelo" class="screenshot-preview"></div>
    </div>
</div>

---

## 6. CIRCUITO 3: MIXTO
_Duración estimada: 45 minutos_

### 6.1. Diseño del circuito
┌─────────────────────────────────────────────────────────────┐
│ CIRCUITO MIXTO - ESQUEMA │
├─────────────────────────────────────────────────────────────┤
│ +9V ---[R1]---+---[R2]---+--- 0V │
│ | | │
│ [R3] [R4] │
│ | | │
│ +-----------+ │
└─────────────────────────────────────────────────────────────┘

**6.1.1. Valores Recomendados:**
- R1 = 1 kΩ
- R2 = 2.2 kΩ
- R3 = 330 Ω
- R4 = 470 Ω

**Paso 6.1.2 - Montaje**
1. [ ] Colocar R1 en serie con combinación R2-R3-R4
2. [ ] Conectar R3 y R4 en paralelo entre R1 y R2
3. [ ] Verificar todas las conexiones

**Paso 6.1.3 - Mediciones**
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

**Paso 6.1.4 - Cálculos**
R_paralelo = (R3 × R4) / (R3 + R4) = <input type="text" class="calculation" data-circuit="mixto" data-calc="r_parallel"> Ω
R_total = R1 + R_paralelo + R2 = <span id="r_total_mixto">___</span> Ω
I_total = 9V / R_total = <input type="text" class="calculation" data-circuit="mixto" data-calc="i_total_theo"> A
V_R1 = I_total × R1 = <input type="text" class="calculation" data-circuit="mixto" data-calc="v_r1_theo"> V
V_paralelo = I_total × R_paralelo = <input type="text" class="calculation" data-circuit="mixto" data-calc="v_parallel_theo"> V
V_R2 = I_total × R2 = <input type="text" class="calculation" data-circuit="mixto" data-calc="v_r2_theo"> V

### 6.1.5. Captura circuito 3 (Mixto)
<div class="screenshot-section">
    <div class="screenshot-upload">
        <label>Insertar captura del circuito mixto:</label>
        <input type="file" id="screenshotMixto" accept="image/*" class="screenshot-input">
        <div id="screenshotPreviewMixto" class="screenshot-preview"></div>
    </div>
</div>

---

## 7. ACTIVIDAD OPCIONAL: CIRCUITO CON DIODOS LED
_Duración estimada: 25 minutos_

### 7.1. Diseño con led (diodo emisor de luz)
┌─────────────────────────────────────────────────────────────┐
│ CIRCUITO LED - ESQUEMA │
├─────────────────────────────────────────────────────────────┤
│ +9V ---[R1 220Ω]---[LED Rojo]--- 0V │
│ [R2 330Ω]---[LED Verde]--- │
│ [R3 470Ω]---[LED Azul]---- │
└─────────────────────────────────────────────────────────────┘

**Paso 7.1.1. Consideraciones Leds**
- [ ] Los LEDs requieren resistencia limitadora de corriente
- [ ] Verificar polaridad (ánodo +, cátodo -)
- [ ] Observar intensidad luminosa según resistencia

**Paso 7.1.2 - Mediciones**
- [ ] Corriente en LED rojo: <input type="text" class="measurement" data-circuit="leds" data-measure="i_led_rojo"> A
- [ ] Corriente en LED verde: <input type="text" class="measurement" data-circuit="leds" data-measure="i_led_verde"> A
- [ ] Corriente en LED azul: <input type="text" class="measurement" data-circuit="leds" data-measure="i_led_azul"> A
- [ ] Voltaje en cada LED: <input type="text" class="measurement" data-circuit="leds" data-measure="v_led"> V

### 7.1.3. Captura circuito con leds
<div class="screenshot-section">
    <div class="screenshot-upload">
        <label>Insertar captura del circuito con LEDs:</label>
        <input type="file" id="screenshotLEDs" accept="image/*" class="screenshot-input">
        <div id="screenshotPreviewLEDs" class="screenshot-preview"></div>
    </div>
</div>

---

## 8. FICHA DE TRABAJO DEL ALUMNO

### 8.1. CHECKLIST DE COMPLETACIÓN
| Circuito | Montaje | Mediciones | Cálculos | Capturas |
|----------|---------|------------|----------|----------|
| Serie | ☐ | ☐ | ☐ | ☐ |
| Paralelo | ☐ | ☐ | ☐ | ☐ |
| Mixto | ☐ | ☐ | ☐ | ☐ |
| LEDs (opc) | ☐ | ☐ | ☐ | ☐ |

### 8.2. VERIFICACIÓN LEYES FUNDAMENTALES
| Ley | Circuito Serie | Circuito Paralelo | Circuito Mixto |
|-----|----------------|-------------------|----------------|
| **Ley de Ohm** (V=I×R) | ☐ Correcta | ☐ Correcta | ☐ Correcta |
| **Kirchhoff Voltajes** (ΣV=0) | ☐ Verificada | ☐ Verificada | ☐ Verificada |
| **Kirchhoff Corrientes** (ΣI=0) | ☐ Verificada | ☐ Verificada | ☐ Verificada |

### 8.3. INCIDENCIAS Y OBSERVACIONES
<textarea id="observations" placeholder="Describe aquí las dificultades encontradas, diferencias entre valores teóricos y medidos, y comportamientos observados en los circuitos..." rows="4" style="width: 100%; padding: 10px; border: 1px solid #ddd; border-radius: 5px; margin: 10px 0;">```Describe aquí las dificultades encontradas, diferencias entre valores teóricos y medidos, y comportamientos observados en los circuitos...```</textarea>

---

## 9. RECURSOS DE APOYO

### 9.1. Documentación técnica
- [Guía oficial TinkerCAD Circuits](https://www.tinkercad.com/learn/circuits)
- [Tutorial mediciones con polímetro virtual](https://www.tinkercad.com/things/0xqL1dF2d7F)
- [Tabla código colores resistencias](https://www.allaboutcircuits.com/tools/resistor-color-code-calculator/)

### 9.2. Videotutoriales
- [Introducción a TinkerCAD Circuits](https://youtube.com/watch?v=yaS7m84YeD8)
- [Mediciones con polímetro virtual](https://youtube.com/watch?v=2-4L0gTjXsQ)
- [Circuitos serie, paralelo y mixto](https://youtube.com/watch?v=7vfd

