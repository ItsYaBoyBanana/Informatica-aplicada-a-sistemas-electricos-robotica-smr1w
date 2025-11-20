# Unidad Práctica 1: Diseño y simulación de circuitos eléctricos en continua

**Módulo:** Informática aplicada a sistemas eléctrónicos - Robótica (CMO-313)  
**Ciclo Formativo:** Sistemas Microinformáticos y Redes (SMR1W)  
**Profesor:** Ezequiel Llarena Borges  
**Duración estimada:** 3 horas  
**Resultados de aprendizaje a trabajar:**  
- *RA2 - Analiza, diseña, simula y mide circuitos electrónicos en continua.*

---

## 1. Objetivos

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

## 2. Criterios de evaluación

| Criterio | Ponderación | Evidencias |
|----------|-------------|------------|
| Diseño correcto circuitos | 30% | Capturas de pantalla circuitos funcionales |
| Mediciones precisas con polímetros | 35% | Tablas de datos completas y correctas |
| Cálculos y verificaciones teóricas | 25% | Comprobación leyes Ohm y Kirchhoff |
| Documentación y presentación | 10% | Informe completo y organizado |

---

## 3. Herramientas y material necesario

### 3.1. Software
- [ ] [Plataforma online de simulación Tinkercad](https://www.tinkercad.com/)  
- [ ] Navegador web actualizado (Chrome/Firefox recomendado)
- [ ] Cuenta en Autodesk (gratuita)

### 3.2. Componentes virtuales 

| **Componente**      | **Cantidad** | **Uso**                |
| ------------------- | ------------ | ---------------------- |
| Batería/Pila 9 V    | 3 unidades   | Fuente de alimentación |
| Resistencias varias | 9 unidades   | Cargas del circuito    |
| Polímetros          | 3 unidades   | Mediciones V, I, R     |
| Protoboard          | 3 unidades   | Montaje de circuitos   |
| LEDs (opcional)     | 6 unidades   | Visualización          |
| Cables jumpers      | Múltiples    | Conexiones             |


### 3.3. Valores de resistencia recomendados
- **R1:** 220 Ω `rojo-rojo-marrón`
- **R2:** 330 Ω `naranja-naranja-marrón` 
- **R3:** 470 Ω `amarillo-violeta-marrón`
- **R4:** 1 kΩ `marrón-negro-rojo`
- **R5:** 2.2 kΩ `rojo-rojo-rojo`  

---

## 4. Diseño del Circuito en Serie CC
_Duración estimada: 45 minutos_

### 4.1. Esquema del circuito

             CIRCUITO EN SERIE

     +---[R1]---[R2]---[R3]---+
     |                        |
     |                        |
     +----------||------------+
              + 9 V -

### 4.2. Montaje en Protoboard
1. [ ] Colocar batería 9 V en protoboard
2. [ ] Conectar R1 (220 Ω) en serie con R2 (330 Ω)
3. [ ] Conectar R2 en serie con R3 (470 Ω)
4. [ ] Completar circuito cerrado
5. [ ] Verificar conexiones correctas

### 4.3. Mediciones de Voltaje 

- Caída de tensión en cada resistor: V<sub>R</sub> = I × R<sub>n</sub> 

| Punto de Medición | Valor Teórico | Valor Medido | Diferencia |
|-------------------|---------------|--------------|------------|
| V1 (Total) | 9 V | <input type="text" class="measurement" data-circuit="serie" data-measure="v_total"> V | <input type="text" class="difference" readonly> V |
| $V_R_1$ | <input type="text" class="theoretical" data-circuit="serie" data-measure="v_r1"> V | <input type="text" class="measurement" data-circuit="serie" data-measure="v_r1"> V | <input type="text" class="difference" readonly> V |
| V_R2 | <input type="text" class="theoretical" data-circuit="serie" data-measure="v_r2"> V | <input type="text" class="measurement" data-circuit="serie" data-measure="v_r2"> V | <input type="text" class="difference" readonly> V |
| V_R3 | <input type="text" class="theoretical" data-circuit="serie" data-measure="v_r3"> V | <input type="text" class="measurement" data-circuit="serie" data-measure="v_r3"> V | <input type="text" class="difference" readonly> V |
| **Suma V_R1 + V_R2 + V_R3** | **9 V** | **<span id="sum_voltages_serie">0</span> V** | **<span id="diff_voltages_serie">0</span> V** |

### 4.4. Mediciones de Corriente 
- [ ] Colocar amperímetro en serie con R1: <input type="text" class="measurement" data-circuit="serie" data-measure="i_r1"> ```   A```  
- [ ] Colocar amperímetro en serie con R2: <input type="text" class="measurement" data-circuit="serie" data-measure="i_r2"> ```   A```   
- [ ] Colocar amperímetro en serie con R3: <input type="text" class="measurement" data-circuit="serie" data-measure="i_r3"> ```   A```  
- [ ] **Verificación:** I_R1 = I_R2 = I_R3 = <span id="current_verification_serie"></span> ```   A```

### 4.5. Cálculos teóricos    

- Resistencia Total (R_T) = R1 + R2 + R3 = <input type="text" class="calculation" data-circuit="serie" data-calc="r_total"> ```   Ω```  
- Corriente teórica (I) = V / R_T = 9 V / <span id="r_total_serie"></span> Ω = <input type="text" class="calculation" data-circuit="serie" data-calc="i_total"> ```   A```  
- Voltaje R1 Teórico = I × R1 = <span id="i_total_serie"></span> A × 220 Ω = <input type="text" class="calculation" data-circuit="serie" data-calc="v_r1_theo"> ```   V```  
- Voltaje R2 Teórico = <span id="i_total_serie2"></span> A × 330 Ω = <input type="text" class="calculation" data-circuit="serie" data-calc="v_r2_theo"> ```   V```  
- Voltaje R3 Teórico = <span id="i_total_serie3"></span> A × 470 Ω = <input type="text" class="calculation" data-circuit="serie" data-calc="v_r3_theo"> ```   V```  

### 4.6. Captura del circuito (Serie)

<div class="screenshot-section">
    <div class="screenshot-instructions">
        <strong>Instrucciones para captura:</strong>
        <ol>
            <li>Completar el circuito en Tinkercad</li>
            <li>Colocar polímetros mostrando mediciones</li>
            <li>Hacer captura de pantalla (Print Screen)</li>
            <li>Pegar en un documento y guardar como imagen</li>
        </ol>
    </div>
    <div class="screenshot-upload">
        <label>Insertar captura del circuito serie:</label>
        <input type="file" id="screenshotSerie" accept="image/*" class="screenshot-input">
        <div id="screenshotPreviewSerie" class="screenshot-preview"><pre>circuito-serie.jpg</pre></div>
    </div>
</div>



---

## 5. Diseño del circuito en Paralelo CC 
_Duración estimada: 45 minutos_

### 5.1. Esquema del circuito

          CIRCUITO EN PARALELO

     +------------+-----[R1]-----+------------+
     |            |              |            |
     |            +-----[R2]-----+            |
     |            |              |            |
     +------------+-----[R3]-----+------------+
                  |                           | 
                  |       +  9 V  –           |
                  +----------||–--------------+  

### 5.2. Montaje en nueva Protoboard 
1. [ ] Colocar batería 9 V
2. [ ] Conectar R1, R2, R3 en paralelo
3. [ ] Verificar que todas las resistencias tengan mismo voltaje

### 5.3. Mediciones de Corriente      
| Rama | Resistencia | Corriente Teórica | Corriente Medida | Diferencia |
|------|-------------|-------------------|------------------|------------|
| R1 | 220 Ω | <input type="text" class="theoretical" data-circuit="paralelo" data-measure="i_r1_theo"> A | <input type="text" class="measurement" data-circuit="paralelo" data-measure="i_r1"> A | <input type="text" class="difference" readonly> A |
| R2 | 330 Ω | <input type="text" class="theoretical" data-circuit="paralelo" data-measure="i_r2_theo"> A | <input type="text" class="measurement" data-circuit="paralelo" data-measure="i_r2"> A | <input type="text" class="difference" readonly> A |
| R3 | 470 Ω | <input type="text" class="theoretical" data-circuit="paralelo" data-measure="i_r3_theo"> A | <input type="text" class="measurement" data-circuit="paralelo" data-measure="i_r3"> A | <input type="text" class="difference" readonly> A |
| **R_Total** | **<span id="r_total_paralelo">___</span> Ω** | **<input type="text" class="theoretical" data-circuit="paralelo" data-measure="i_total_theo"> A** | **<input type="text" class="measurement" data-circuit="paralelo" data-measure="i_total"> A** | **<input type="text" class="difference" readonly> A** |

### 5.4. Mediciones de Voltaje      
- [ ] Voltaje en R1: <input type="text" class="measurement" data-circuit="paralelo" data-measure="v_r1"> ```   V```  
- [ ] Voltaje en R2: <input type="text" class="measurement" data-circuit="paralelo" data-measure="v_r2"> ```   V```  
- [ ] Voltaje en R3: <input type="text" class="measurement" data-circuit="paralelo" data-measure="v_r3"> ```   V```  
- [ ] **Verificación:** V_R1 = V_R2 = V_R3 = 9 V

### 5.5. Cálculos teóricos    
- 1/R_T = 1/R1 + 1/R2 + 1/R3 = 1/220 + 1/330 + 1/470 = <input type="text" class="calculation" data-circuit="paralelo" data-calc="r_parallel"> Ω
- R_Total = <span id="r_total_calc_paralelo"></span> Ω
- I_Total = V / R_T = 9 V / <span id="r_total_for_current"></span> Ω = <input type="text" class="calculation" data-circuit="paralelo" data-calc="i_total_theo"> A
- I_R1 = 9 V / 220 Ω = <input type="text" class="calculation" data-circuit="paralelo" data-calc="i_r1_theo"> A
- I_R2 = 9 V / 330 Ω = <input type="text" class="calculation" data-circuit="paralelo" data-calc="i_r2_theo"> A
- I_R3 = 9 V / 470 Ω = <input type="text" class="calculation" data-circuit="paralelo" data-calc="i_r3_theo"> A

### 5.6. Captura del circuito (Paralelo)

   <div class="screenshot-upload">
        <label>Insertar captura del circuito paralelo:</label>
        <input type="file" id="screenshotSerie" accept="image/*" class="screenshot-input">
        <div id="screenshotPreviewSerie" class="screenshot-preview"><pre>circuito-paralelo.jpg</pre></div>
    </div>
</div>

---

## 6. Diseño del circuito combinado (serie-paralelo) en CC  
_Duración estimada: 45 minutos_

### 6.1. Esquema del circuito

                CIRCUITO ELÉCTRICO (SERIE-PARALELO)
                
                         I_total →
                 +----------[R1]-------------+
                 |  <----- V_R1 ----->       |  
                 |                      I2 → |
                 |                           |
                 |                 +------[R2]-------+ 
                 |                 |  <--- V_R2 ---> | 
                 |                 |                 |
                 |                 |  <--- V_R3 ---> |
                 |                 +-------[R3]------+
                 |                           |
                 |                      I3 → | 
                 |       +  9 V  –           |
                 +----------||–--------------+                 
                   
       
| Elemento        | Símbolo con subíndice | Descripción                     |
| --------------- | --------------------- | ------------------------------- |
| Corriente total | ( I_{\text{total}} )  | Corriente que entra al circuito |
| Corriente R2    | ( I_R2 )               | Corriente que pasa por R2       |
| Corriente R3    | ( I_R3 )               | Corriente que pasa por R3       |
| Voltaje R1      | ( V_{R1} )            | Caída de tensión en R1          |
| Voltaje R2      | ( V_{R2} )            | Caída de tensión en R2          |
| Voltaje R3      | ( V_{R3} )            | Caída de tensión en R3          |



### 6.2. Valores de resistencias recomendados:    
- R1 = 1 kΩ
- R2 = 2.2 kΩ
- R3 = 330 Ω
- R4 = 470 Ω

### 6.3. Montaje    
1. [ ] Colocar R1 en serie con combinación R2-R3-R4
2. [ ] Conectar R3 y R4 en paralelo entre R1 y R2
3. [ ] Verificar todas las conexiones

### 6.4. Mediciones    
| Parámetro | Valor Teórico | Valor Medido | Diferencia |
|-----------|---------------|--------------|------------|
| V Total | 9 V | <input type="text" class="measurement" data-circuit="mixto" data-measure="v_total"> V | <input type="text" class="difference" readonly> V |
| V_R1 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="v_r1_theo"> V | <input type="text" class="measurement" data-circuit="mixto" data-measure="v_r1"> V | <input type="text" class="difference" readonly> V |
| V_R2 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="v_r2_theo"> V | <input type="text" class="measurement" data-circuit="mixto" data-measure="v_r2"> V | <input type="text" class="difference" readonly> V |
| V_R3 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="v_r3_theo"> V | <input type="text" class="measurement" data-circuit="mixto" data-measure="v_r3"> V | <input type="text" class="difference" readonly> V |
| V_R4 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="v_r4_theo"> V | <input type="text" class="measurement" data-circuit="mixto" data-measure="v_r4"> V | <input type="text" class="difference" readonly> V |
| I Total | <input type="text" class="theoretical" data-circuit="mixto" data-measure="i_total_theo"> A | <input type="text" class="measurement" data-circuit="mixto" data-measure="i_total"> A | <input type="text" class="difference" readonly> A |
| I_R1 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="i_r1_theo"> A | <input type="text" class="measurement" data-circuit="mixto" data-measure="i_r1"> A | <input type="text" class="difference" readonly> A |
| I_R2 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="i_r2_theo"> A | <input type="text" class="measurement" data-circuit="mixto" data-measure="i_r2"> A | <input type="text" class="difference" readonly> A |
| I_R3 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="i_r3_theo"> A | <input type="text" class="measurement" data-circuit="mixto" data-measure="i_r3"> A | <input type="text" class="difference" readonly> A |
| I_R4 | <input type="text" class="theoretical" data-circuit="mixto" data-measure="i_r4_theo"> A | <input type="text" class="measurement" data-circuit="mixto" data-measure="i_r4"> A | <input type="text" class="difference" readonly> A |

### 6.5. Cálculos    
- R_paralelo = (R3 × R4) / (R3 + R4) = <input type="text" class="calculation" data-circuit="mixto" data-calc="r_parallel"> Ω
- R_total = R1 + R_paralelo + R2 = <span id="r_total_mixto"></span> Ω
- I_total = 9V / R_total = <input type="text" class="calculation" data-circuit="mixto" data-calc="i_total_theo"> A
- V_R1 = I_total × R1 = <input type="text" class="calculation" data-circuit="mixto" data-calc="v_r1_theo"> V
- V_paralelo = I_total × R_paralelo = <input type="text" class="calculation" data-circuit="mixto" data-calc="v_parallel_theo"> V
- V_R2 = I_total × R2 = <input type="text" class="calculation" data-circuit="mixto" data-calc="v_r2_theo"> V

### 6.6. Captura circuito combinado (serie-paralelo)

   <div class="screenshot-upload">
        <label>Insertar captura del circuito mixto:</label>
        <input type="file" id="screenshotSerie" accept="image/*" class="screenshot-input">
        <div id="screenshotPreviewSerie" class="screenshot-preview"><pre>circuito-mixto.jpg</pre></div>
    </div>
</div>

---

## 7. ACTIVIDAD OPCIONAL: CIRCUITO CON DIODOS LED
_Duración estimada: 25 minutos_

### 7.1. Diseño con led (diodo emisor de luz)
┌─────────────────────────────────────────────────────────────┐
│ CIRCUITO LED - ESQUEMA │
├─────────────────────────────────────────────────────────────┤
│ + 9V ---[R1 220Ω]---[LED Rojo]--- 0 V │
│ [R2 330 Ω]---[LED Verde]--- │
│ [R3 470 Ω]---[LED Azul]---- │
└─────────────────────────────────────────────────────────────┘

### 7.2. Consideraciones Leds  
- [ ] Los LEDs requieren resistencia limitadora de corriente
- [ ] Verificar polaridad (ánodo +, cátodo -)
- [ ] Observar intensidad luminosa según resistencia

### 7.3. Mediciones  
- [ ] Corriente en LED rojo: <input type="text" class="measurement" data-circuit="leds" data-measure="i_led_rojo"> A
- [ ] Corriente en LED verde: <input type="text" class="measurement" data-circuit="leds" data-measure="i_led_verde"> A
- [ ] Corriente en LED azul: <input type="text" class="measurement" data-circuit="leds" data-measure="i_led_azul"> A
- [ ] Voltaje en cada LED: <input type="text" class="measurement" data-circuit="leds" data-measure="v_led"> V

### 7.4. Captura circuito con leds  

<div class="screenshot-section">
    <div class="screenshot-upload">
        <label>Insertar captura del circuito con LEDs:</label>
        <input type="file" id="screenshotLEDs" accept="image/*" class="screenshot-input">
        <div id="screenshotPreviewLEDs" class="screenshot-preview"><pre>circuito-leds.jpg</pre></div>
    </div>
</div>

---

## 8. FICHA DE TRABAJO DEL ALUMNO

<div class="student-info">
    <div class="info-field">
        <label>Nombre completo:</label>
        <input type="text" id="studentName" placeholder="Escribe tu nombre completo">
    </div>
    <div class="info-field">
        <label>Grupo:</label>
        <input type="text" id="studentGroup" placeholder="Ej: SMR1W">
    </div>
    <div class="info-field">
        <label>Fecha de realización:</label>
        <input type="date" id="practiceDate">
    </div>
</div>

---


### 8.1. Checklist de realización
| Circuito | Montaje | Mediciones | Cálculos | Capturas |
|----------|---------|------------|----------|----------|
| Serie | ☐ | ☐ | ☐ | ☐ |
| Paralelo | ☐ | ☐ | ☐ | ☐ |
| Mixto | ☐ | ☐ | ☐ | ☐ |
| LEDs (opc) | ☐ | ☐ | ☐ | ☐ |

### 8.2. Verificación leyes fundamentales
| Ley | Circuito Serie | Circuito Paralelo | Circuito Mixto |
|-----|----------------|-------------------|----------------|
| **Ley de Ohm** (V = I × R) | ☐ Correcta | ☐ Correcta | ☐ Correcta |
| **Kirchhoff Voltajes** (ΣV = 0) | ☐ Verificada | ☐ Verificada | ☐ Verificada |
| **Kirchhoff Corrientes** (ΣI = 0) | ☐ Verificada | ☐ Verificada | ☐ Verificada |

### 8.3. Incidencias y observaciones  
Describe aquí las dificultades encontradas, diferencias entre valores teóricos y medidos, y comportamientos observados en los circuitos:  

<pre>   ...   </pre>

<!--<textarea id="observations" placeholder="" rows="4" style="width: 100%; padding: 10px; border: 1px solid #ddd; border-radius: 5px; margin: 10px 0;"><pre>Describe aquí las dificultades encontradas, diferencias entre valores teóricos y medidos, y comportamientos observados en los circuitos...</pre></textarea>-->

---

## 9. Recursos de apoyo

### 9.1. Documentación técnica
- [Guía oficial Tinkercad circuits](https://www.tinkercad.com/learn/circuits)
- [Tutorial mediciones con polímetro virtual](https://www.tinkercad.com/things/0xqL1dF2d7F)
- [Tabla código colores resistencias](https://www.allaboutcircuits.com/tools/resistor-color-code-calculator/)

### 9.2. Videotutoriales
- [Introducción a Tinkercad circuits](https://youtube.com/watch?v=yaS7m84YeD8)
- [Mediciones con polímetro virtual](https://youtube.com/watch?v=2-4L0gTjXsQ)
- [Circuitos serie, paralelo y mixto](https://youtube.com/watch?v=7vfd)


##  
_&copy; 2025 - Fundamentos de Programación - Ezequiel Llarena Borges_
