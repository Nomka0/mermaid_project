# Diseño de una novela visual

## Plantilla de informe técnico del proyecto de curso

Este documento registra cómo el equipo define, construye, prueba y mejora una micronovela visual navegable.  
Su propósito es justificar las decisiones de contenido y conservar evidencia de la evolución del prototipo.

### Nombre del juego

[Título del equipo]

### Autores y curso

- Juan José Bolaños Delgado
- Daniel
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

[En 150 a 200 palabras: problema, público, propósito, solución, estado del prototipo y resultados disponibles. En la entrega 1 no anticipen resultados de pruebas.]

### Problema y propósito

[¿Qué necesita comprender o hacer la persona? ¿Qué dificultad de comunicación aborda el juego? Formulen el propósito y un criterio observable de éxito.]

### Alcance del curso

Experiencia de 8 a 12 minutos; máximo tres personajes principales; tres decisiones significativas con dos o tres opciones cada una; dos o tres desenlaces; 12 a 18 pantallas o pasajes principales. Documenten las variantes de estado aparte y reconecten ramas cuando sea pertinente.

Incluyan un formulario breve o interacción equivalente, error y recuperación, confirmación, éxito o cierre, dos estados críticos y una decisión explícita de accesibilidad. El resultado es un prototipo navegable por enlace; la programación y la alta fidelidad visual no son obligatorias.

| Versión y fecha | Cambio relevante           | Autoría       |
| :-------------- | :------------------------- | :------------ |
| [v1/fecha]      | [Creación o actualización] | [Responsable] |
| [v2/fecha]      | [Cambio y motivo]          | [Responsable] |

---

## 2 Público contexto y referentes

_Entrega 1_

### Público y contexto de uso

[Describan experiencia previa, necesidades de lectura, dispositivo y entorno. Justifiquen el perfil con evidencia; señalen lo que todavía es un supuesto.]

### Necesidades y riesgos comunicativos

[¿Qué información necesita la persona antes de actuar? ¿Qué confusiones, barreras o riesgos de exclusión deben prevenir?]

### Análisis de referentes

Seleccionen obras o interfaces pertinentes. Comparen decisiones de narrativa y contenido; no se limiten a describir su apariencia. Incluyan la fuente y la fecha de consulta.

| Referente y fuente      | Qué se analiza                               | Aplicación al proyecto                    |
| :---------------------- | :------------------------------------------- | :---------------------------------------- |
| [Obra o interfaz / URL] | [Elecciones, etiquetas, tono o recuperación] | [Qué adoptar, adaptar o evitar y por qué] |
| [Obra o interfaz / URL] | [Elemento y evidencia]                       | [Decisión del equipo]                     |

### Conclusión del análisis

[Qué aprendieron de los referentes y cómo orienta su propuesta. Diferencien hallazgos de las fuentes y decisiones propias.]

### Criterios para evaluar la experiencia

[Definan indicadores observables: anticipar una acción, distinguir opciones, recuperar un error o completar una ruta. Indiquen cómo los comprobarán.]

---

## 3 Arquitectura narrativa y reglas de interacción

_Entrega 1_

### Premisa y dilema central

[Resuman la situación inicial, el conflicto y lo que está en juego. Identifiquen al protagonista, su objetivo y el papel del jugador.]

| Personaje          | Función narrativa      | Motivación y relación           |
| :----------------- | :--------------------- | :------------------------------ |
| [Nombre]           | [Protagonista o apoyo] | [Qué busca y cómo se relaciona] |
| [Nombre]           | [Función]              | [Motivación]                    |
| [Nombre si aplica] | [Función]              | [Motivación]                    |

### Mapa narrativo

[Insertar un diagrama legible con inicio, escenas, D01 a D03, opciones, reconexiones y F01 a F03. Usar los mismos códigos que en el prototipo. Añadir una descripción textual equivalente.]

### Reglas y memoria de las decisiones

[Qué información se conserva: elecciones, relaciones o datos. Cómo condiciona escenas y finales. Si la herramienta solo simula esa lógica, expliquen cómo y sus límites.]

### Ficha de decisión repetible

_Dupliquen esta ficha para D01, D02 y D03. Cada opción debe expresar una acción distinguible y tener una consecuencia verificable._

| Opción y texto visible  | Consecuencia narrativa      | Estado y destino         |
| :---------------------- | :-------------------------- | :----------------------- |
| [D01 A/etiqueta exacta] | [Qué cambia en la historia] | [Cambio funcional / Sxx] |
| [D01 B/etiqueta exacta] | [Qué cambia en la historia] | [Cambio funcional / Sxx] |
| [D01 C si aplica]       | [Qué cambia en la historia] | [Cambio funcional / Sxx] |

### Condiciones de los desenlaces

[F01 a F03: qué decisiones conducen a cada final y cómo se comunica su relación con lo ocurrido.]

---

## 4 Guion y ficha de pantalla

_Entrega 1 y actualización en la entrega 3_

_Dupliquen la ficha por pantalla o pasaje principal. Separen el texto de la historia del contenido que permite operar la interfaz. Las etiquetas deben describir la acción real._

### Identificación y propósito

[Código Sxx, nombre, función, requisito de entrada y vínculo con la decisión Dxx o final Fxx.]

### Contenido narrativo

[Texto definitivo de narración, diálogo y pensamientos. Identifiquen quién habla; indiquen variantes según decisiones previas.]

### Representación visual y sonora

[Escenario, personajes, expresiones y sonido si aplica. Expliquen su función y el equivalente textual de información indispensable.]

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

[Propósito comunicativo, relación con el público y principios que deben reconocerse en la interfaz.]

### Atributos de voz

Definan rasgos verificables con ejemplos propios. La voz de la interfaz puede diferenciarse de las voces de los personajes; indiquen cómo mantienen esa distinción.

| Somos      | No somos              | Regla y ejemplo aplicado   |
| :--------- | :-------------------- | :------------------------- |
| [Atributo] | [Límite del atributo] | [Regla / texto real / Sxx] |
| [Atributo] | [Límite]              | [Regla / texto real / Sxx] |
| [Atributo] | [Límite]              | [Regla / texto real / Sxx] |

### Matriz de tono

| Situación y pantalla   | Emoción y riesgo           | Tono y texto aplicado       |
| :--------------------- | :------------------------- | :-------------------------- |
| [Inicio / Sxx]         | [Estado esperado y riesgo] | [Adaptación / texto exacto] |
| [Decisión / Sxx]       | [Emoción y riesgo]         | [Adaptación / texto]        |
| [Error / Sxx]          | [Emoción y riesgo]         | [Adaptación / texto]        |
| [Estado crítico / Sxx] | [Emoción y riesgo]         | [Adaptación / texto]        |
| [Éxito o cierre / Sxx] | [Emoción y riesgo]         | [Adaptación / texto]        |

### Convenciones editoriales

[Tratamiento al público, términos consistentes, longitud y estructura de instrucciones, nombres de controles y criterios de lenguaje inclusivo. Incluyan ejemplos del proyecto.]

---

## 6 Navegación formularios y mensajes

_Entrega 1 y revisión en la entrega 3_

### Inventario de contenido funcional

_Dupliquen filas para cubrir los controles y mensajes. Indiquen propósito y acción real, no solo ubicación. El texto definitivo debe coincidir con el prototipo._

| ID y pantalla | Tipo y texto exacto   | Función y justificación          |
| :------------ | :-------------------- | :------------------------------- |
| [C01 / Sxx]   | [Etiqueta / texto]    | [Acción y razón de la redacción] |
| [C02 / Sxx]   | [Instrucción / texto] | [Qué permite comprender]         |
| [C03 / Sxx]   | [Ayuda / texto]       | [Confusión que previene]         |

### Navegación y control

[Cómo se reconoce inicio, ubicación, avance, regreso, reinicio y cierre. Indiquen si volver conserva una decisión o permite cambiarla, y cómo se informa.]

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
| Error E01           | [Entrada inválida o acción imposible] | [Sxx / captura]      |
| Confirmación CF01   | [Acción relevante que se revisa]      | [Sxx / captura]      |
| Éxito o cierre EX01 | [Resultado que se completó]           | [Sxx / captura]      |
| Crítico CR01        | [Riesgo, urgencia o impacto]          | [Sxx / captura]      |
| Crítico CR02        | [Situación diferente]                 | [Sxx / captura]      |

### Ficha de estado repetible

_Dupliquen esta ficha para cada estado de la tabla anterior._

#### Código condición y consecuencia

[ID, pantalla, condición de aparición, riesgo y lo que realmente ocurrió o está por ocurrir.]

#### Mensaje definitivo

[Título si corresponde y texto exacto. Qué debe entender la persona; tono elegido y su justificación.]

| Acción disponible                 | Etiqueta exacta     | Resultado y destino |
| :-------------------------------- | :------------------ | :------------------ |
| [Corregir, continuar o confirmar] | [Texto del control] | [Respuesta / Sxx]   |
| [Cancelar, volver o pedir ayuda]  | [Texto del control] | [Respuesta / Sxx]   |

#### Verificación del estado

[Cómo se activa en el prototipo, cómo se recorre su recuperación y qué evidencia demuestra que la acción funciona.]

---

## 8 Accesibilidad y especificación del prototipo

_Entrega 1 y actualización en la entrega 3_

### Decisiones de accesibilidad e inclusión

Distingan diseño previsto, simulación y verificación real. Un prototipo visual no demuestra por sí mismo compatibilidad con tecnologías de asistencia. Registren la barrera y el alcance de cada comprobación.

| Barrera y pantalla                     | Ajuste aplicado                     | Evidencia y estado               |
| :------------------------------------- | :---------------------------------- | :------------------------------- |
| [Lectura o contraste / Sxx]            | [Medida concreta]                   | [Método / resultado o pendiente] |
| [Dependencia de color, imagen o audio] | [Equivalente o ajuste]              | [Evidencia]                      |
| [Lenguaje o representación]            | [Revisión y cambio]                 | [Fragmento / justificación]      |
| [Interacción o navegación]             | [Ajuste y límite de la herramienta] | [Comprobación]                   |

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
