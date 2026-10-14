# Diseño de una novela visual

## Plantilla de informe técnico del proyecto de curso

Este documento registra cómo el equipo define, construye, prueba y mejora una micronovela visual navegable.  
Su propósito es justificar las decisiones de contenido y conservar evidencia de la evolución del prototipo.

### Nombre del juego

Unspoken Words

### Autores y curso

- Juan José Bolaños Delgado
- Daniel Arias Castrillón
- Alejandra Ospina

### Datos de esta entrega

Entregable 1

### Acceso al prototipo

[Enlace, versión y punto de inicio]

---

### Cómo completar la plantilla

Reemplacen los textos entre corchetes por información del proyecto. Dupliquen las fichas y filas necesarias. Identifiquen capturas y anexos mediante códigos y expliquen qué evidencia aporta cada uno. Las orientaciones pueden retirarse de la versión final.

Mantengan un único informe acumulativo. En la primera entrega, marquen las secciones de pruebas e iteración como pendientes. En las siguientes, actualicen la síntesis y registren los cambios. No presenten supuestos como resultados ni inventen pruebas, participantes o fuentes.

---

## 1 Síntesis y delimitación del proyecto

_Completar en la entrega 1 y actualizar en las entregas 2 y 3_

### Resumen técnico

Esta micronovela visual aborda la dificultad de representar dilemas morales interactivos donde las decisiones del jugador impactan genuinamente en el desarrollo ético y psicológico del protagonista, superando las ramificaciones cosméticas tradicionales. Diseñada para un público joven adulto y universitario (18 a 30 años) con interés en ficciones interactivas y narrativa de fantasía oscura, la obra sitúa al usuario en el rol de Dominick, un caballero cuyas determinaciones frente a situaciones límite van moldeando progresivamente los rasgos de su personalidad (honor, pragmatismo o desapego). El propósito es propiciar una experiencia inmersiva y reflexiva, pero a la vez intensa donde cada elección dialógica desencadene consecuencias éticas tangibles, bifurcando el relato hacia tres desenlaces contrastantes a través de distintos escenarios. La solución se materializa en un prototipo interactivo navegable desarrollado en Figma, que incorpora microcopy contextual, decisiones de bifurcación con memoria narrativa y estados de validación funcional. El prototipo se encuentra en fase inicial de diseño y especificación técnica para la Entrega 1; los resultados empíricos y pruebas con usuarios quedan marcados como pendientes para iteraciones posteriores.

### Problema y propósito

**Problema:** En el diseño de narrativas interactivas, las decisiones morales suelen reducirse a elecciones binarias superficiales («bueno» vs. «malo») que generan disonancia ludo-narrativa, provocando que el usuario no sienta el peso real de sus acciones ni perciba cómo forjan el carácter del personaje.

**Propósito:** Brindar una experiencia donde el jugador deba navegar dilemas éticos sin respuestas fáciles, comprendiendo que cada línea de diálogo y acción asumida moldea internamente la brújula moral de Dominick (orientándolo hacia el honor inflexible, el pragmatismo despiadado o el desapego nihilista) y determina directamente su destino final.

**Criterio observable de éxito:**
1. Al menos el 80% de los evaluadores identifica con claridad en cuál de las facetas éticas concluyó Dominick tras su partida.
2. El usuario reconoce la relación causal directa entre sus elecciones de diálogo y el desenlace obtenido (`F01`, `F02` o `F03`).
3. El recorrido completo de 8 a 12 minutos se efectúa sin abandonos ni bloqueos por ambigüedad en las etiquetas de decisión.

### Alcance del curso

Experiencia de 8 a 12 minutos; máximo tres personajes principales; tres decisiones significativas con dos o tres opciones cada una; dos o tres desenlaces; 12 a 18 pantallas o pasajes principales. Documenten las variantes de estado aparte y reconecten ramas cuando sea pertinente.

Incluyan un formulario breve o interacción equivalente, error y recuperación, confirmación, éxito o cierre, dos estados críticos y una decisión explícita de accesibilidad. El resultado es un prototipo navegable por enlace; la programación y la alta fidelidad visual no son obligatorias.

| Versión y fecha | Cambio relevante  | Autoría            |
| :-------------- | :---------------- | :----------------- |
| v1 13/10/2026   | Creación          | Juan José y Daniel |
| [v2/fecha]      | [Cambio y motivo] | [Responsable]      |

---

## 2 Público contexto y referentes

_Entrega 1_

### Público y contexto de uso

- **Perfil del público:** Jóvenes adultos y estudiantes universitarios (18 a 30 años) con interés en géneros de fantasía oscura, rol (RPG) y novelas visuales narrativas.
- **Experiencia previa:** Familiaridad media con mecánicas de diálogo de elección múltiple y lectura interactiva en pantalla.
- **Necesidades de lectura:** Requieren textos fragmentados y concisos (máximo 3 a 4 líneas por bloque narrativo), microcopy funcional que evidencie la intención de la respuesta antes de pulsar y ritmo pausado con control manual de avance.
- **Dispositivo y entorno:** Acceso mediante enlace de Figma en navegadores de escritorio (resolución 1920×1080 o laptops) y adaptable a dispositivos móviles. El uso se sitúa en sesiones cortas y concentradas de 8 a 12 minutos en entornos cotidianos (hogar o estudio).
- **Sustento y supuestos:**
  - `[Evidencia]`: Hábitos consolidados de consumo de medios interactivos y narrativas ramificadas en el rango del curso.
  
  - `[Supuesto]`: Preferencia por opciones dialógicas con intención explícita frente a las elecciones del jugador. disposición a rejugar para explorar los 3 desenlaces (pendiente de validación empírica en la Entrega 2).

### Necesidades y riesgos comunicativos

- **Información requerida antes de actuar:**
  - El usuario debe conocer el contexto del dilema ético inmediato, las partes en conflicto y las consecuencias potenciales que están en juego antes de que se le exija decidir.
  - Las opciones de diálogo deben comunicar con claridad la intención y carga emocional de Dominick (si responde con templanza, agresión o evasión) para evitar desajustes entre la intención del jugador y la reacción del personaje.
  - Se debe informar cuándo una acción es crítica o irreversible mediante avisos previos o pantallas de confirmación (`CF01`).

- **Confusiones, barreras y riesgos de exclusión a prevenir:**
  - *Disonancia de intención (falsa expectativa dialógica):* Prevenir que una etiqueta resumida haga decir a Dominick algo inesperado para el jugador. **Ajuste:** Diseñar etiquetas con verbos de acción e intención explícita (ej. «Cuestionar con frialdad» en lugar de un ambiguo «Hablar»).
  - *Sobrecarga cognitiva:* Evitar párrafos largos de prosa descriptiva que saturen al lector y diluyan la tensión del dilema. **Ajuste:** Jerarquía visual estricta y separación nítida entre texto narrativo y microcopy funcional.
  - *Barreras visuales y contraste:* Evitar tipografías demasiado ornamentales e ilegibles o bajo contraste sobre fondos oscuros. **Ajuste:** Cumplimiento de ratio de contraste WCAG AA (mínimo 4.5:1) y tipografía sans-serif legible en botones y diálogos.

### Análisis de referentes

Seleccionen obras o interfaces pertinentes. Comparen decisiones de narrativa y contenido; no se limiten a describir su apariencia. Incluyan la fuente y la fecha de consulta.

| Referente y fuente                                            | Qué se analiza                                                                                                                     | Aplicación al proyecto                                      |
| :------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------- |
| [Arte de alew.scrawl](https://www.instagram.com/alew.scrawl/) | Estilo visual/artistico para los personajes y la interfaz                                                                          | Uso de personajes con permiso y participación del artista   |
| De lo espiritual en el arte - Vasili Kandinski                | Sobre los colores y cómo pueden influir en la personalidad de ciertos personajes (Lirio y Alba)                                    | Conceptos de teoría de color                                |
| Narciso y Goldmundo - Herman Hesse                            | Se analizan a los personajes, porque tienen similitud con el concepto inicial de personalidad de ciertos personajes (Lirio y Alba) | Inspiración y referente para personajes y sus interacciones |
|                                                               |                                                                                                                                    |                                                             |

### Conclusión del análisis

[Qué aprendieron de los referentes y cómo orienta su propuesta. Diferencien hallazgos de las fuentes y decisiones propias.]

### Criterios para evaluar la experiencia

Para evaluar la interacción y la recepción narrativa del prototipo durante las pruebas con usuarios (programadas para la Entrega 2), se establecen cuatro criterios con indicadores observables y métodos de verificación concretos:

1. **Anticipación de la acción e intención dialógica:**
   - *Indicador observable:* La persona comprende la actitud y carga moral que adoptará Dominick antes de presionar un botón de opción en el diálogo.
   - *Método de comprobación:* Protocolo de pensamiento en voz alta (*Think Aloud*) en las tres decisiones clave (`D01`, `D02`, `D03`); meta: al menos el 85% de los participantes anticipa correctamente la postura que asumirá el personaje.

2. **Diferenciación y peso de las opciones morales:**
   - *Indicador observable:* La persona distingue con claridad el contraste ético entre las alternativas de cada decisión, sin percibir que conducen al mismo resultado por mero artificio estético.
   - *Método de comprobación:* Pregunta cualitativa post-decisión («¿Sentiste que las opciones representaban caminos morales distintos?»); umbral esperado: calificación promedio ≥ 4/5 en escala Likert de diferenciación.

3. **Recuperación autónoma del estado de error (`E01`):**
   - *Indicador observable:* Al interactuar con la pantalla de error del formulario o mecanismo, el usuario comprende la causa del fallo y localiza la salida navegable sin abandonar la experiencia ni reiniciar el prototipo.
   - *Método de comprobación:* Observación de navegación sin intervención del equipo; meta: 100% de los usuarios retorna exitosamente a la pantalla de corrección en menos de 15 segundos.

4. **Completitud de ruta y atribución causal del desenlace:**
   - *Indicador observable:* La persona completa una sesión de lectura de 8 a 12 minutos hasta uno de los tres desenlaces (`F01`, `F02` o `F03`) y atribuye el destino final de Dominick a las decisiones tomadas a lo largo de los diálogos.
   - *Método de comprobación:* Cuestionario de cierre con la pregunta: «¿El final obtenido se sintió consecuente con la personalidad que construiste para Dominick?»; meta esperada: ≥ 80% de respuestas afirmativas fundamentadas en elecciones previas.

---

## 3 Arquitectura narrativa y reglas de interacción

_Entrega 1_

### Premisa y dilema central

Dominick cometió un acto atroz en la guerra y busca expiación o un milagro para su pueblo. Viaja al santuario  prohibido de Alba y Lirio, quienes actúan como juezas oraculares (Alba juzga la intención/emoción; Lirio juzga el hecho/consecuencia).

| Personaje | Función narrativa                        | Motivación y relación                                        |
| :-------- | :--------------------------------------- | :----------------------------------------------------------- |
| Dominick  | Protagonista                             | [Qué busca y cómo se relaciona]                              |
| Alba      | Reto a superar/ jueza moral (emocional)  | Definir el destino de Dominick de acuerdo a lo que él siente |
| Lirio     | Reto a superar/ jueza moral (pragmatico) | Definir el destino de Dominick                               |

### Mapa narrativo

```mermaid
flowchart TD
    S01["S01: Umbral del Santuario<br>(Llegada de Dominick)"] --> S02["S02: Antesala del Juicio<br>(Apertura mística)"]
    S02 --> S03["S03: Altar de la Confesión<br>(Formulario de ofrenda / C01)"]
    S03 --> S04["S04: Aparición del Oráculo Dual<br>(Manifestación de Alba y Lirio)"]
    
    S04 --> S05["S05: Primera Prueba<br>(Decisión D01: Confesión del pasado)"]
    
    S05 -->|D01 A: Asumir culpa con dolor| S06["S06: El Eco del Veredicto Inicial<br>(Reconexión de ramas)"]
    S05 -->|D01 B: Justificar necesidad militar| S06
    S05 -->|D01 C: Silencio desafiante| S06
    
    S06 --> S07["S07: Segunda Prueba<br>(Decisión D02: El enemigo herido)"]
    
    S07 -->|D02 A: Perdonar y soltar armas| S08["S08: El Espejo de las Almas<br>(CR01: Crisis de lucidez moral)"]
    S07 -->|D02 B: Ejecutar por justicia implacable| S08
    
    S08 --> S09["S09: Tercera Prueba<br>(Decisión D03: Petición en el núcleo)"]
    
    S09 -->|D03 A: Entrega humilde de la espada| CF01["CF01: Confirmación de Voto<br>(Acción irreversible)"]
    S09 -->|D03 B: Exigir gracia por derecho| CF01
    
    CF01 -->|Confirmar veredicto| S10["S10: Deliberación de las Siamesas<br>(CR02: Tensión oracular)"]
    CF01 -->|Reconsiderar| S09
    
    S10 -->|Consenso a favor: Alba y Lirio aprueban| S11["S11: Despertar Iluminado<br>(F01: Redención Obtenida)"]
    S10 -->|Desacuerdo: Alba y Lirio en conflicto| S12["S12: Juicio Inconcluso<br>(F02: Atrapado en el Limbo)"]
    S10 -->|Consenso en contra: Alba y Lirio rechazan| S13["S13: Destierro Eterno<br>(F03: Redención Denegada)"]
    
    S11 --> S14["S14: Epílogo y Registro Moral<br>(EX01: Cierre de la Experiencia)"]
    S12 --> S14
    S13 --> S14
```

#### Descripción textual equivalente del mapa narrativo

1. **Ruta inicial y rito de ofrenda (S01 a S04):**
   - El recorrido inicia en **S01** (Umbral del Santuario) y avanza a **S02** (Antesala).
   - En **S03** se despliega el formulario breve de inscripción/ofrenda (`C01`) para registrar el voto del peregrino, coneictando directamente con **S04**, donde se manifiestan Alba y Lirio.
1. **Primera bifurcación y reconexión (S05 a S06):**
   - En **S05** se presenta la primera decisión significativa (**D01** sobre el pasado en la guerra) con tres opciones: asumir la culpa con dolor (**D01 A**), justificar la necesidad militar (**D01 B**) o guardar silencio desafiante (**D01 C**).
   - Todas las opciones reconectan en **S06** (Eco del Veredicto Inicial), alterando el diálogo de las siamesas y el balance de juicio moral acumulado.
3. **Segunda bifurcación y estado crítico 1 (S07 a S08):**
   - En **S07** se plantea la segunda decisión (**D02** ante el enemigo derrotado): perdonar (**D02 A**) o ejecutar (**D02 B**).
   - Ambas ramas conducen a **S08**, donde se detona el estado crítico **CR01** (Crisis de lucidez moral / temblor del santuario) que confronta a Dominick con el peso acumulado de sus actos.
4. **Tercera bifurcación, confirmación y deliberación (S09 a S10):**
   - En **S09** se ejecuta la decisión clímax (**D03** en el Núcleo): entregar la espada con humildad (**D03 A**) o exigir la gracia por la fuerza de sus méritos (**D03 B**).
   - Previo al paso irreversible, se despliega la pantalla de confirmación **CF01**. Si el usuario confirma, avanza a **S10**; si cancela, regresa a **S09**.
   - En **S10** se vive el estado crítico **CR02** durante la deliberación de las siamesas, evaluando el balance ético acumulado.
5. **Bifurcación de desenlaces y cierre (S11 a S14):**
   - **Desenlace F01 (S11):** Alba y Lirio coinciden a favor; Dominick obtiene la redención y la paz interior.
   - **Desenlace F02 (S12):** Alba y Lirio entran en contradicción moral no resuelta; el juicio queda congelado y Dominick queda atrapado indefinidamente en el santuario.
   - **Desenlace F03 (S13):** Alba y Lirio coinciden en contra; rechazan sus justificaciones y Dominick es expulsado con su culpa intacta.
   - Los tres desenlaces convergen en **S14** (**EX01**), pantalla final que resume la personalidad forjada por el jugador, tiempo de lectura y control para reiniciar el recorrido.

### Reglas y memoria de las decisiones

- **Variables conservadas en memoria:**
  - `Afinidad_Alba` (entero): Mide la validación moral emocional (arrepentimiento, empatía, renuncia al ego).
  - `Afinidad_Lirio` (entero): Mide la validación moral pragmática (coherencia de hechos, asunción de responsabilidad, justicia objetiva).
  - `Rasgo_Dominick` (texto): Registra el perfil ético predominante del protagonista (*Caballero Íntegro*, *Pragmático Marcial* o *Tiránico Impenitente*).
- **Cómo condiciona escenas y finales:**
  - En `S06`, el diálogo de las siamesas varía sutilmente según la opción elegida en `D01`.
  - En `S10` (`CR02`), se evalúa el balance combinado de ambas variables para determinar el veredicto unánime a favor (`F01`), el conflicto entre ellas (`F02`), o la condena unánime (`F03`).
- **Simulación en Figma y límites técnicos:** Al ser un prototipo en Figma, la lógica de variables condicionales se simula mediante ramificación de componentes interactivos y variables locales de prototipo (Figma Variables). En rutas donde la herramienta no soporta cálculo aritmético complejo, se mapean conexiones directas representativas por ruta crítica.

### Ficha de decisión repetible

#### Decisión D01: La Confesión del Pasado (Pantalla S05)
*Frente al estanque del santuario, Alba y Lirio interrogan a Dominick sobre la aldea destruida bajo su mando durante la guerra.*

| Opción y texto visible | Consecuencia narrativa | Estado y destino |
| :---------------------- | :--------------------- | :--------------- |
| **D01 A:** «Reconocer la culpa con pesar: "Seguí órdenes crueles y la sangre mancha mis manos"» | Dominick asume la responsabilidad con dolor y arrepentimiento sincero. Conmueve la empatía de Alba y demuestra franqueza ante Lirio. | `Afinidad_Alba += 1`<br>`Afinidad_Lirio += 1`<br>Destino: `S06` |
| **D01 B:** «Justificar el acto por estrategia militar: "Era la guerra; vacilar habría costado la vida de mi pelotón"» | Dominick apela a la dura lógica castrense. Lirio valida el razonamiento táctico, pero Alba resiente la falta de remordimiento humano. | `Afinidad_Alba -= 1`<br>`Afinidad_Lirio += 1`<br>Destino: `S06` |
| **D01 C:** «Responder con frialdad desafiante: "La piedad en el campo de batalla solo engendra más tumbas"» | Dominick muestra un corazón endurecido y cínico. Ambas siamesas perciben soberbia e incapacidad de redención. | `Afinidad_Alba -= 1`<br>`Afinidad_Lirio -= 1`<br>Destino: `S06` |

#### Decisión D02: El Juicio del Enemigo Herido (Pantalla S07)
*El oráculo proyecta la visión espectral del general enemigo derrotado, desarmado y suplicando clemencia.*

| Opción y texto visible | Consecuencia narrativa | Estado y destino |
| :---------------------- | :--------------------- | :--------------- |
| **D02 A:** «Bajar la espada y perdonar la vida: "El ciclo de sangre se detiene aquí"» | Dominick renuncia a la venganza. Alba exalta la pureza de la compasión y Lirio constata el autocontrol sobre los instintos destructivos. | `Afinidad_Alba += 1`<br>`Afinidad_Lirio += 1`<br>Destino: `S08` (`CR01`) |
| **D02 B:** «Ejecutarlo en nombre de la justicia marcial: "Tus crímenes exigen retribución, no misericordia"» | Dominick aplica la ley marcial con severidad. Lirio acepta la equidad del castigo, pero Alba lamenta la ausencia de compasión. | `Afinidad_Alba -= 1`<br>`Afinidad_Lirio += 1`<br>Destino: `S08` (`CR01`) |
| **D02 C:** «Burlarse de su derrota antes de ultimarlo: "Suplicas ahora la piedad que jamás concediste"» | Dominick manifiesta crueldad y deleite en la humillación ajena. Ambas juezas reprueban unánimemente su degradación ética. | `Afinidad_Alba -= 1`<br>`Afinidad_Lirio -= 1`<br>Destino: `S08` (`CR01`) |

#### Decisión D03: La Consagración en el Núcleo (Pantalla S09)
*Ante la llama viva del Núcleo de las Almas, Dominick debe formalizar su petición de redención.*

| Opción y texto visible                                                                                            | Consecuencia narrativa                                                                                                                           | Estado y destino                                                                |
| :---------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| **D03 A:** «Rendir la espada y jurar penitencia: "Renuncio a las armas; consagraré mi vida a reparar el daño"»    | Dominick renuncia al poder y abraza la humildad reparadora. Consolida la aprobación unánime de las siamesas.                                     | `Afinidad_Alba += 1`<br>`Afinidad_Lirio += 1`<br>Destino: `CF01` (Confirmación) |
| **D03 B:** «Exigir la absolución como mérito de honor: "He servido con lealtad a la corona y purgado mi culpa"»   | Dominick intenta negociar su redención como un título ganado. Lirio evalúa sus servicios objetivos, pero Alba rechaza la soberbia transaccional. | `Afinidad_Alba -= 1`<br>`Afinidad_Lirio += 1`<br>Destino: `CF01` (Confirmación) |
| **D03 C:** «Rechazar la autoridad del santuario: "No mendigaré el perdón de ningún oráculo para seguir adelante"» | Dominick rompe el rito con desprecio altivo, consumando la total corrupción de su propósito inicial.                                             | `Afinidad_Alba -= 2`<br>`Afinidad_Lirio -= 2`<br>Destino: `CF01` (Confirmación) |

### Condiciones de los desenlaces

| Código y Nombre | Condición de activación | Relación causal y comunicación con el jugador |
| :-------------- | :---------------------- | :-------------------------------------------- |
| **F01: Despertar Iluminado (Redención Obtenida)** | **Consenso a favor de ambas siamesas:** `Afinidad_Alba ≥ +2` y `Afinidad_Lirio ≥ +2`. Ocurre al acumular opciones A (arrepentimiento sincero, perdón y humildad). | **Comunicación:** Alba baña el estanque con luz dorada en señal de perdón moral, mientras Lirio entrega la gema purificada del santuario como reconocimiento de un juicio justo. Dominick despierta en el plano terrenal libre del peso del pasado, renacido como un caballero protector y compasivo. |
| **F02: Juicio Inconcluso (Atrapado en el Limbo)** | **Desacuerdo entre las siamesas:** Asimetría moral en las respuestas (`Afinidad_Lirio` positivo pero `Afinidad_Alba` negativo, o contradicción entre opciones de culpa y de venganza). | **Comunicación:** Alba defiende que hay dolor en su alma y pide piedad, pero Lirio argumenta con severidad que sus actos no demuestran una transformación ética real. Al no existir consenso armónico, el santuario se envuelve en una niebla espectral perpetua; Dominick queda suspendido en un limbo meditativo sin poder despertar. |
| **F03: Destierro Eterno (Redención Denegada)** | **Consenso en contra de ambas siamesas:** `Afinidad_Alba ≤ -1` y `Afinidad_Lirio ≤ -1`. Ocurre al acumular opciones B y C (soberbia militar, crueldad o desprecio del rito). | **Comunicación:** Alba aparta el rostro con tristeza y repulsión, mientras Lirio proclama con voz atronadora la sentencia de expulsión. El santuario colapsa en sombras y expulsa a Dominick con violencia. El caballero despierta solo en las ruinas físicas, portando una armadura corroída y condenado a arrastrar su culpa sin redención posible. |

---

## 4 Guion y ficha de pantalla

_Entrega 1 y actualización en la entrega 3_

_Dupliquen la ficha por pantalla o pasaje principal. Separen el texto de la historia del contenido que permite operar la interfaz. Las etiquetas deben describir la acción real._

Principio, final, y retos (pueden ser no todos por ahora)

### Identificación y propósito

[Código Sxx, nombre, función, requisito de entrada y vínculo con la decisión Dxx o final Fxx.]

### Contenido narrativo

[Texto definitivo de narración, diálogo y pensamientos. Identifiquen quién habla; indiquen variantes según decisiones previas.]

### Representación visual y sonora

[Escenario, personajes, expresiones y sonido si aplica. Expliquen su función y el equivalente textual de información indispensable.]

|                                        Figura 1: Dominick                                         |                                         Figura 2: Lirio y Alba                                         |                                            Figura 3: Dominick                                             |
| :-----------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: |
| <img src="imgs/Pasted%20image%2020261013185746.png" alt="Figura 1: Dominick" width="260" /> | <img src="imgs/Pasted%20image%2020261013185814.png" alt="Figura 2: Lirio y Alba" width="260" /> | <img src="imgs/Pasted%20image%2020261013185824.png" alt="Figura 3: Dominick" width="260" /> |


### Contenido funcional de la pantalla

| Elemento              | Texto exacto       | Comportamiento y destino         |
| :-------------------- | :----------------- | :------------------------------- |
| [Botón o elección]    | [Etiqueta visible] | [Qué ocurre / Sxx]               |
| [Instrucción o ayuda] | [Texto visible]    | [Cuándo se muestra]              |
| [Navegación o estado] | [Texto visible]    | [Acción, recuperación o destino] |

### Boceto o captura

[Insertar captura legible y su identificación: Figura xx, pantalla Sxx, versión y fecha. Añadir una breve explicación de su función.]

### Justificación y comprobación

[Por qué el contenido orienta al público; qué riesgo previene; cómo se comprobará su comprensión. Indiquen el ajuste de accesibilidad de esta pantalla.]

---

## 5 Identidad voz y tono

_Entrega 1 y revisión en la entrega 3_

### Identidad del juego

- **Propósito comunicativo:** Confrontar al jugador con la naturaleza de sus decisiones morales a través del juicio oracular de Dominick ante Alba y Lirio, evidenciando que toda elección ética tiene costo, consecuencias y define la psique de quien la toma.
- **Relación con el público:** Trato respetuoso y reflexivo. La interfaz no juzga prematuramente al usuario ni lo premia con condescendencia; actúa como un testigo sobrio e imparcial de sus elecciones.
- **Principios reconocibles en la interfaz:**
  1. *Sobriedad mística:* Interfaz despojada de adornos superfluos; protagonismo del texto, las voces y la tensión ética.
  2. *Claridad intencional:* Toda opción dialógica comunica su postura moral antes del clic para evitar disonancia.
  3. *Inmutabilidad solemne:* El avance narrativo transmite el peso de lo irreversible sin trampas de reinicio arbitrario.

### Atributos de voz

La voz de la interfaz (sistema) se mantiene neutra, orientadora y solemne en tercera persona, diferenciándose claramente de las voces dramáticas de los personajes (Dominick: introspectivo y marcial; Alba: empática y compasiva; Lirio: analítica y justa).

| Somos                       | No somos                                   | Regla y ejemplo aplicado                                                                                                                                                                                 |
| :-------------------------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Éticamente transparente** | No somos engañosos, ambiguos ni moralistas | Transparentar la postura del personaje en cada botón; no sermonear al usuario sobre lo que "debe" hacer.<br>*Ejemplo (S07):* «Bajar la espada y perdonar la vida: "El ciclo de sangre se detiene aquí"». |
| **Funcionalmente preciso**  | No somos crípticos ni confusos             | Las instrucciones y etiquetas del sistema indican la acción real con verbos concretos.<br>*Ejemplo (CF01):* «Consagrar voto irrevocable» (en vez de «Aceptar» o «Continuar»).                            |

### Matriz de tono

| Situación y pantalla            | Emoción y riesgo                                                            | Tono y texto aplicado                                                                                                                                       |
| :------------------------------ | :-------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Inicio / S01**                | Cautela y misterio. Riesgo: desinterés o falta de inmersión inicial.        | **Solemne y sugerente:** «El Santuario Olvidado aguarda en silencio; solo quienes cargan con una culpa verdadera cruzan su umbral».                         |
| **Decisión / S05**              | Tensión ética e introspección. Riesgo: desconexión entre intención y botón. | **Firme y comprometido:** «Reconocer la culpa con pesar: "Seguí órdenes crueles y la sangre mancha mis manos"».                                             |
| **Confirmación / CF01**         | Gravedad e incertidumbre. Riesgo: clic impulsivo no advertido.              | **Advertencia serena y transparente:** «Una vez consagrado este voto, las juezas deliberarán de forma irrevocable. ¿Confirmas tu resolución?».              |
| **Estado crítico / S08 (CR01)** | Asfixia moral y urgencia. Riesgo: frustración o confusión visual.           | **Tensión psicológica contenida:** «El estanque se agita con violencia. La memoria de tus caídos pesa sobre la espada; sostén la templanza para continuar». |
| **Éxito o cierre / S14 (EX01)** | Catarsis, serenidad y reflexión. Riesgo: sensación de cierre abrupto.       | **Conclusivo y reflexivo:** «El juicio ha concluido. Has forjado el alma de Dominick como un Caballero Íntegro. El oráculo guarda silencio».                |

### Convenciones editoriales

- **Tratamiento al público:** Segunda persona sobria («tú / contemplas / eliges») en descripciones ambientales e instrucciones funcionales del sistema; primera persona directa («yo / reconozco / renuncio») en las elecciones dialógicas de Dominick.
- **Términos consistentes:** Vocabulario canónico fijado en el proyecto: *Oráculo*, *Juicio*, *Santuario*, *Núcleo de las Almas*, *Consagración*, *Voto*, *Redención*.
- **Estructura y longitud:** Párrafos narrativos breves (máximo 3 líneas en desktop). Microcopy en botones con formato: `[Verbo de acción] + [Carga moral explícita entre comillas]`.
- **Criterios de lenguaje:** Español neutro culto sin arcaísmos artificiales; inclusión mediante sustantivos colectivos y formulaciones universales («quien cruce el umbral», «la persona frente al oráculo»).

---

## 6 Navegación formularios y mensajes

_Entrega 1 y revisión en la entrega 3_

### Inventario de contenido funcional

| ID y pantalla  | Tipo y texto exacto                                                                     | Función y justificación                                                                                        |
| :------------- | :-------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------- |
| **C01 / S01**  | Botón de avance: «Cruzar el umbral del santuario»                                       | Inicia el recorrido activo del jugador; la redacción enfatiza el compromiso del caballero de entrar al juicio. |
| **C02 / S03**  | Instrucción de campo: «Inscribe el nombre de la culpa que vienes a purgar»              | Guía la interacción del formulario breve ficticio sin pedir datos personales reales.                           |
| **C03 / S03**  | Botón de acción: «Depositar ofrenda y abrir juicio»                                     | Envía el voto inicial para hacer aparecer al oráculo dual en S04.                                              |
| **C04 / S05**  | Botón de elección D01 A: «Reconocer la culpa con pesar: "Seguí órdenes crueles..."»     | Acción dialógica reflexiva; suma afinidad con Alba (+1) y Lirio (+1).                                          |
| **C05 / S05**  | Botón de elección D01 B: «Justificar el acto por estrategia: "Era la guerra..."»        | Acción dialógica marcial; suma afinidad con Lirio (+1) y resta a Alba (-1).                                    |
| **C06 / S05**  | Botón de elección D01 C: «Responder con frialdad: "La piedad solo engendra más tumbas"» | Acción dialógica cínica; resta afinidad a ambas siamesas (-1 cada una).                                        |
| **C07 / S07**  | Botón de elección D02 A: «Bajar la espada y perdonar la vida: "El ciclo termina aquí"»  | Acción ética de clemencia; suma afinidad con Alba (+1) y Lirio (+1).                                           |
| **C08 / S07**  | Botón de elección D02 B: «Ejecutarlo en nombre de la justicia marcial»                  | Acción punitiva rigurosa; suma afinidad con Lirio (+1) y resta a Alba (-1).                                    |
| **C09 / S09**  | Botón de consagración D03 A: «Rendir la espada y jurar penitencia»                      | Selecciona la renuncia y abre el modal de confirmación CF01.                                                   |
| **C10 / CF01** | Botón de confirmación irreversible: «Consagrar voto irrevocable»                        | Ejecuta el paso crítico definitivo hacia la deliberación S10.                                                  |
| **C11 / CF01** | Botón de retorno: «Reconsiderar respuesta»                                              | Permite regresar a S09 para cambiar la elección de D03 sin penalización.                                       |
| **C12 / S14**  | Botón de reinicio: «Reiniciar experiencia»                                              | Restablece las variables éticas y devuelve al usuario a S01.                                                   |

### Navegación y control

- **Reconocimiento de inicio, ubicación y avance:**
  - En la parte superior de la interfaz se muestra un indicador sutil de etapa («Etapa I: Umbral», «Etapa II: Juicio», «Etapa III: Veredicto») que orienta sobre el progreso sin invadir el arte.
  - El avance se realiza pulsando botones con texto explícito de acción; no existen transiciones automáticas forzadas.
- **Regreso y memoria de decisiones:**
  - Durante los textos de narración pura se permite releer diálogos mediante el historial de lectura (*Log*).
  - Al tomar una decisión moral significativa (`D01`, `D02`, `D03`), la elección queda fijada inmediatamente en las variables de afinidad y el retroceso queda restringido para mantener el peso y la gravedad de las consecuencias. La interfaz informa esto mediante la microleyenda: *"Tus palabras han sido escuchadas por el santuario"*.
  - En el punto crítico irreversible (`S09`), se implementa una confirmación explícita (`CF01`) donde el jugador sí puede pulsar «Reconsiderar respuesta» para cambiar su opción antes de que se compute el veredicto final.
- **Reinicio y cierre:**
  - Al alcanzar cualquiera de los desenlaces y la pantalla de cierre `S14` (`EX01`), se habilita el botón «Reiniciar experiencia», que limpia las variables de sesión y permite explorar las demás ramas éticas.

### Formulario breve o interacción equivalente

#### Propósito y pertinencia

[Qué dato se solicita, por qué es necesario para esta historia, qué ocurre con él y cómo se evita pedir datos personales reales.]

| Campo o control    | Etiqueta e instrucción   | Regla y respuesta                    |
| :----------------- | :----------------------- | :----------------------------------- |
| [Nombre]           | [Texto exacto y ejemplo] | [Obligatorio / formato / validación] |
| [Nombre si aplica] | [Texto exacto]           | [Regla / respuesta]                  |

#### Prevención y confianza

[Qué debe saber la persona antes de actuar, qué consecuencias se explican y cómo se comunican las limitaciones del prototipo sin prometer funciones inexistentes.]

---

## 7 Estados y recuperación

_Entrega 1 y revisión en la entrega 3_

Completen todos los estados exigidos. La recuperación debe tener una salida navegable. Una confirmación ocurre antes de la acción relevante; el éxito comunica un resultado ya ocurrido.

| Estado e ID         | Situación que lo activa               | Pantalla y evidencia |
| :------------------ | :------------------------------------ | :------------------- |
| **Error E01**           | Envío de formulario de ofrenda con campo de texto en blanco o inválido | `S03` / Modal de advertencia `[Captura E01]` |
| **Confirmación CF01**   | Intento de sellar la decisión final irreversible D03 | `S09` / Modal de confirmación `[Captura CF01]` |
| **Éxito o cierre EX01** | Conclusión del recorrido y despliegue del balance ético final | `S14` / Pantalla de epílogo `[Captura EX01]` |
| **Crítico CR01**        | Tensión psicológica extrema tras D02; asfixia moral y temblor del estanque | `S08` / Pantalla de crisis `[Captura CR01]` |
| **Crítico CR02**        | Deliberación contradictoria del oráculo dual en el clímax | `S10` / Pantalla de deliberación `[Captura CR02]` |

### Ficha de estado repetible

#### Estado CF01: Confirmación de Voto Irrevocable (Pantalla S09 / Modal CF01)

##### Código condición y consecuencia
- **ID:** `CF01`
- **Pantalla:** `S09` (Modal superpuesto).
- **Condición de aparición:** Se activa cuando el jugador pulsa cualquiera de las opciones de consagración final en `D03`.
- **Riesgo:** Pulsación accidental de una elección que define de forma definitiva e irreversible el final del juego.
- **Consecuencia:** Detiene el avance inmediato, advierte de la gravedad del acto y exige ratificar o reconsiderar la resolución.

##### Mensaje definitivo
- **Título:** *Consagración de Voto Irrevocable*
- **Texto exacto:** «Estás a punto de sellar tu postura definitiva ante el Núcleo de las Almas. Una vez depositada tu respuesta, las juezas deliberarán de manera irrevocable y no habrá retorno. ¿Deseas consagrar este voto ante el oráculo?»
- **Qué debe entender la persona:** Que el juego entra en su resolución final y que su respuesta actual sellará el veredicto sin posibilidad de cambio posterior.
- **Tono elegido y justificación:** Tono solemne, transparente y sin apremios, permitiendo una pausa reflexiva antes de la culminación dramática.

| Acción disponible | Etiqueta exacta | Resultado y destino |
| :---------------- | :-------------- | :------------------ |
| Confirmar acción | «Consagrar voto irrevocable» | Fija la variable de decisión y transiciona a la deliberación de las siamesas en `S10`. |
| Cancelar o corregir | «Reconsiderar respuesta» | Cierra el modal y devuelve el control a `S09` para modificar la opción seleccionada. |

##### Verificación del estado
- **Activación en el prototipo:** Configurado como interacción *On click* en las opciones de `D03` que abre una superposición (*Open overlay*) centrada con fondo oscurecido al 60%.
- **Recorrido de recuperación:** Al hacer clic en «Reconsiderar respuesta», se activa *Close overlay*, restableciendo la selección en `S09` sin alterar las variables previas. Al pulsar «Consagrar voto», se ejecuta la navegación a `S10`.
- **Evidencia:** Flujo probado en el modo de presentación de Figma verificando navegación bidireccional limpia.

---

#### Estado CR01: Crisis de Lucidez Moral (Pantalla S08)

##### Código condición y consecuencia
- **ID:** `CR01`
- **Pantalla:** `S08`.
- **Condición de aparición:** Ocurre inmediatamente después de resolver el dilema del enemigo herido en `D02`.
- **Riesgo:** Desorientación del jugador ante el cambio abrupto de atmósfera mística.
- **Consecuencia:** Dominick experimenta el peso acumulado de sus culpas; el entorno se vuelve opresivo antes de acceder al Núcleo.

##### Mensaje definitivo
- **Título:** *La Fractura de la Memoria*
- **Texto exacto:** «El estanque sagrado hierve en sombras. El peso de tus determinaciones amenaza con doblegar tu espíritu, pero el umbral del Núcleo exige un alma resuelta. Sostén la respiración y da un paso al frente.»
- **Qué debe entender la persona:** Que el juicio está llegando a su fase más crítica y que sus decisiones previas ya han dejado una huella indeleble en el ambiente.
- **Tono elegido y justificación:** Tono de urgencia psicológica y gravedad épica para enfatizar el clímax narrativo.

| Acción disponible | Etiqueta exacta | Resultado y destino |
| :---------------- | :-------------- | :------------------ |
| Avanzar con templanza | «Avanzar hacia el Núcleo» | Transiciona a la prueba final en `S09`. |

##### Verificación del estado
- **Activación en el prototipo:** Navegación lineal encadenada desde `S07` tras pulsar cualquier opción de `D02`.
- **Recorrido:** El usuario lee la crisis ambiental y pulsa el botón único de avance para estabilizar el trance.
- **Evidencia:** Componente de pantalla `S08` enlazado con animación de disolución suave (*Dissolve 300ms*) hacia `S09`.

---

#### Estado EX01: Veredicto y Cierre de la Experiencia (Pantalla S14)

##### Código condición y consecuencia
- **ID:** `EX01`
- **Pantalla:** `S14`.
- **Condición de aparición:** Se activa tras la conclusión narrativa de cualquiera de los tres desenlaces (`S11`, `S12` o `S13`).
- **Riesgo:** Finalización sin feedback sobre las decisiones tomadas o sensación de callejón sin salida.
- **Consecuencia:** Muestra el balance ético forjado para Dominick, resume el arquetipo de personalidad alcanzado y permite reiniciar.

##### Mensaje definitivo
- **Título:** *El Juicio ha Concluido*
- **Texto exacto:** «Las aguas del santuario han dictado sentencia. Tus elecciones a lo largo de este viaje forjaron el destino de Dominick. Puedes contemplar las consecuencias de tus actos o reiniciar la travesía para explorar otros senderos morales.»
- **Qué debe entender la persona:** Que la experiencia concluyó satisfactoriamente, cuál fue el perfil ético final de su protagonista y cómo recomenzar si desea explorar otras rutas.
- **Tono elegido y justificación:** Tono catártico, reflexivo y conclusivo.

| Acción disponible | Etiqueta exacta | Resultado y destino |
| :---------------- | :-------------- | :------------------ |
| Reiniciar recorrido | «Reiniciar experiencia» | Restablece las variables de afinidad a 0 y navega a `S01`. |

##### Verificación del estado
- **Activación en el prototipo:** Conexión interactiva desde los botones de cierre de `S11`, `S12` y `S13` hacia `S14`.
- **Recorrido:** Al hacer clic en «Reiniciar experiencia», el prototipo vuelve al estado inicial en `S01`.
- **Evidencia:** Flujo circular comprobado en Figma (*On click -> Navigate to S01* con reseteo de componentes).

---

## 8 Accesibilidad y especificación del prototipo

_Entrega 1 y actualización en la entrega 3_

### Decisiones de accesibilidad e inclusión

Distingan diseño previsto, simulación y verificación real. Un prototipo visual no demuestra por sí mismo compatibilidad con tecnologías de asistencia. Registren la barrera y el alcance de cada comprobación.

| Barrera y pantalla                                   | Ajuste aplicado                                                                                                                                                                                                | Evidencia y estado                                                                              |
| :--------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------- |
| **Lectura y contraste / S01 a S14**                  | Contraste de texto mínimo de 4.8:1 sobre fondos oscuros (texto principal `#F3F4F6` sobre caja contenedora `#111827` al 85% de opacidad), cumpliendo estándar WCAG 2.1 AA.                                      | Verificado con plugin de contraste en Figma. `[Aprobado / Relación 5.2:1 media]`                |
| **Doble codificación en decisiones / S05, S07, S09** | Las opciones de diálogo no dependen exclusivamente de color; se acompañan de texto con intención explícita e iconografía distintiva (balanza para justicia, corazón/olivo para compasión, espada para fuerza). | Verificado en biblioteca de componentes de Figma. `[Evidencia: Componentes duales]`             |
| **Ritmo de lectura y motricidad / S01 a S14**        | Ausencia absoluta de temporizadores que fuercen el avance automático. Todo avance y decisión depende de la pulsación manual voluntaria del usuario.                                                            | Verificado en configuración de prototipo (*On click* exclusivo). `[Aprobado]`                   |
| **Sensibilidad fotosensible / S08, S10**             | Los estados críticos prescinden de parpadeos rápidos, luces estroboscópicas o temblores bruscos de pantalla. La tensión se transmite mediante variaciones tonales suaves y texto.                              | Verificado en diseño de transiciones (*Dissolve 300ms* sin animaciones agresivas). `[Aprobado]` |

### Especificación técnica del prototipo

#### Herramienta y organización

[Herramienta y versión si está disponible; organización de pantallas, componentes, archivos y recursos; motivos de elección. Documenten implementación adicional solo si existe.]

#### Acceso y entorno de prueba

[Enlaces inicial y actual, punto de inicio, permisos, dispositivo o tamaño previsto, navegador si aplica y fecha de verificación.]

#### Lógica simulada y limitaciones

[Qué está conectado, qué se simula y qué no está implementado. Cómo se activan los estados para probarlos. No describan una base de datos o servicio que no exista.]

#### Comprobación antes de las pruebas

[Registrar evidencia de enlaces accesibles, controles visibles, rutas y finales completos, coherencia entre opción y destino, estados activables, recuperación, legibilidad y uso sin explicación del equipo.]

---

## 13 Fuentes recursos IA y anexos

_Sección transversal a las tres entregas_

### Referencias

[Incluir las fuentes realmente consultadas con un estilo consistente: autor o entidad, fecha, título y URL o DOI. Citar en el cuerpo las afirmaciones que se apoyan en ellas. Incorporar la guía docente del proyecto como documento de curso cuando corresponda.]

### Procedencia y permisos de los recursos

| Recurso y uso                      | Autor y fuente           | Licencia o permiso         |
| :--------------------------------- | :----------------------- | :------------------------- |
| [Imagen, audio o tipografía / Sxx] | [Autor / enlace / fecha] | [Condiciones y atribución] |
| [Recurso]                          | [Procedencia]            | [Permiso y evidencia]      |

### Declaración de uso de IA

[Indicar si se utilizó IA. Si no se usó, declararlo. Si se usó, duplicar el registro siguiente para cada uso relevante y conservar los prompts y resultados como anexo.]

#### Herramienta propósito y material

[Herramienta o modelo y fecha, tarea, prompt o referencia al anexo, resultado que se consideró y alcance del uso en el prototipo.]

#### Revisión y decisión humana

[Qué se aceptó, modificó o rechazó y por qué. Qué fuentes, comprobaciones o pruebas se usaron. Documentar al menos una recomendación corregida o descartada si se utilizó IA, y quién tomó la decisión final.]

> _No introduzcan datos personales de participantes en herramientas de IA. La IA no sustituye participantes, pruebas ni evidencia; los resultados deben verificarse y declararse._

### Índice de anexos y evidencias

| Código       | Contenido y versión                   | Ubicación y acceso          |
| :----------- | :------------------------------------ | :-------------------------- |
| [A01 / EV01] | [Mapa, captura, protocolo o registro] | [Enlace o anexo / permisos] |
| [A02 / EV02] | [Contenido / versión / fecha]         | [Ubicación]                 |

---

_Antes de entregar: comprobar enlaces y permisos; mantener los mismos códigos en texto, tablas y prototipo; retirar orientaciones que ya no se necesiten; conservar pendientes explícitos; anonimizar evidencias y revisar que cada conclusión tenga sustento._
