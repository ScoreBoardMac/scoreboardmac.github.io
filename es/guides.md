---
lang: es
ref: guides
layout: page
title: Guía de usuario
description: >
  Tutoriales paso a paso para añadir un marcador de ScoreBoard en OBS, Streamlabs, Wirecast
  o Meld: cronómetros de texto, fondo del marcador, cronómetro con décimas de segundo y alineaciones.
image: /img/scoreboard_for_mac_light.png
permalink: /es/guides/
---

Tutoriales para añadir un marcador en OBS: las mismas fuentes de archivos TXT e imagen funcionan igual en Streamlabs, Wirecast y Meld.

_Los nombres de los menús de OBS corresponden a la interfaz en español; entre paréntesis, a la interfaz en inglés._

- [Preguntas frecuentes](#faq)
- [Primeros pasos](#getting-started)
- [Archivos de texto e imagen de salida](#output-text-and-image-files)
- [Cómo añadir un cronómetro/contador en OBS](#how-to-add-a-text-timer-or-counter-in-obs)
- [Cómo añadir un fondo de marcador](#how-to-add-a-scorebug-background-image-in-obs)
- [Cómo mostrar correctamente las décimas](#how-to-display-tenths-of-a-second-in-obs)
- [Cómo mostrar las alineaciones](#how-to-show-team-rosters-in-an-obs-broadcast)

---

## Preguntas frecuentes {#faq}

**¿Cómo añado un marcador deportivo en vivo a OBS en Mac?**  
Instala ScoreBoard para Mac y, después, añade sus archivos TXT de salida como fuentes *Texto (FreeType 2)* y sus imágenes de promo/logotipo como fuentes *Imagen* en OBS. Consulta [Primeros pasos](#getting-started) más abajo.

**¿Por qué mi fuente de texto de OBS no se actualiza al instante?**  
Por defecto, OBS vuelve a leer los archivos de texto aproximadamente una vez por segundo. Para actualizaciones más rápidas (por ejemplo, las décimas de segundo de un cronómetro), usa el plugin Advanced Scene Switcher. Consulta [Cómo mostrar las décimas de segundo](#how-to-display-tenths-of-a-second-in-obs).

**¿Puedo mostrar las alineaciones de los equipos en mi transmisión?**  
Sí: añade la alineación como texto en el campo Estado de un equipo y/o como imagen mediante los botones de promo, y muéstrala con fuentes de Texto e Imagen en OBS. Consulta [Cómo mostrar las alineaciones](#how-to-show-team-rosters-in-an-obs-broadcast).

**¿Funciona en Streamlabs, Wirecast o Meld en lugar de OBS?**  
Sí. ScoreBoard genera archivos TXT e imágenes simples que cualquier software de streaming con fuentes de archivos de texto o de imagen puede leer igual que OBS.

**¿Necesito una imagen de fondo para el marcador o basta con las fuentes de texto?**  
Ambas opciones sirven. Las fuentes de texto por sí solas muestran los valores en vivo; una imagen de fondo detrás (consulta [Cómo añadir un fondo de marcador](#how-to-add-a-scorebug-background-image-in-obs)) le da un aspecto más cuidado.

---

## Primeros pasos {#getting-started}

**Scoreboard para OBS en macOS** es una app fácil de usar pensada para aficionados al deporte, narradores y streamers que quieren mostrar el marcador en vivo de dos equipos o jugadores en sus escenas de OBS Studio. Esta app ligera simplifica la gestión e integración del marcador para que puedas centrarte en el partido y en tu audiencia.

**Mejora tus retransmisiones deportivas con Scoreboard para OBS en macOS: sencillo, eficaz y pensado para el directo.**

## Casos de uso ideales {#ideal-use-cases}

- Eventos deportivos (fútbol, baloncesto, voleibol, etc.)  
- Torneos de eSports y videojuegos  
- Transmisiones de comentarios y análisis en directo  

## Funciones {#features}

- **Actualización del marcador en vivo:** cambia el marcador fácilmente en tiempo real durante un partido.  
- **Integración mediante archivos de texto:** genera y actualiza automáticamente archivos `.txt` con los datos del marcador, compatibles con la fuente *Texto (FreeType 2)* de OBS Studio.  
- **Consumo mínimo de recursos:** la app está optimizada para macOS y funciona con fluidez incluso en equipos modestos.  
- **Interfaz intuitiva:** una interfaz sencilla y clara para gestionar equipos, marcador y otros detalles del partido.
- **Diseño personalizable:** adapta el aspecto del marcador al estilo de tu transmisión, incluidos tamaño de fuente, color y posición. Esto se hace en el programa de streaming, por ejemplo en OBS.  

## Cómo funciona {#how-it-works}

1. **Instala la app**  
   - Instala ScoreBoard para Mac en tu ordenador:  
      - [Comprar en el Mac App Store](https://apps.apple.com/app/id1579159150)  
      - [Descargar la versión gratuita](/free-apps/ScoreBoard-free.zip) y descomprimirla: está notarizada por Apple y es segura  
   - Abre la app y configura los nombres de los equipos/jugadores y otros ajustes iniciales.  

2. **Actualiza el marcador en tiempo real**  
   - Ajusta el marcador de los equipos con los controles sencillos de la app.  
   - La app guarda automáticamente los valores actualizados en archivos `.txt`. Carpeta por defecto: `Descargas/ScoreBoard Outputs`.

3. **Intégrala con OBS Studio**  
   - En OBS, crea una nueva fuente *Texto (FreeType 2)* o simplemente arrastra el archivo de texto deseado a la ventana de OBS.  
   - Activa la opción «Leer desde archivo» (*Read from File*) y selecciona el archivo `.txt` generado por la app.  
   - Personaliza la fuente de texto en OBS: posición, tamaño, tipo de letra, color, etc.  

4. **Transmite o graba**  
   - Al cambiar el marcador en ScoreBoard, los cambios se reflejan en OBS en tiempo real. OBS lee automáticamente los archivos del disco (aproximadamente una vez por segundo) y muestra el resultado.  

---

## Archivos de texto e imagen de salida {#output-text-and-image-files}

Por defecto, ScoreBoard escribe estos archivos en `Descargas/ScoreBoard Outputs` (puedes elegir otra carpeta en Preferencias). Cada archivo `.txt` se actualiza en vivo mientras controlas el partido y se añade en OBS como fuente **Texto (FreeType 2)**; cada archivo `.png` se añade como fuente **Imagen**. Consulta [Primeros pasos](#getting-started) más arriba.

### Archivos de texto {#text-files}

| Archivo | Contenido | Ejemplo |
|---|---|---|
| `Timer.txt` | Cronómetro/temporizador principal del partido | `12:45` |
| `Timer_Extra.txt` | Temporizador adicional con dos ajustes predefinidos (p. ej., reloj de posesión) | `14` |
| `Home_Name.txt` / `Away_Name.txt` | Nombres de los equipos | `Eagles` |
| `Match_Name.txt` | Nombre del partido/evento | `Semifinal` |
| `Period.txt` | Periodo/cuarto/tiempo actual (también OT, 2OT, 3OT…) | `2nd` |
| `Home_Goal.txt` / `Away_Goal.txt` | Marcador principal (goles/puntos) de cada equipo | `3` |
| `Home_Shots.txt` / `Away_Shots.txt` | Contador extra de tiros de cada equipo | `18` |
| `Home_Points.txt` / `Away_Points.txt` | Contador extra de puntos de cada equipo | `2` |
| `Home_Status.txt` / `Away_Status.txt` | Descripción/estado del equipo; también se usa para las [alineaciones](#how-to-show-team-rosters-in-an-obs-broadcast) | `#9 J. Smith` |
| `Match_Status.txt` | Descripción/estado del partido | `Final` |
| `Home_Penalties_Numbers.txt` / `Away_Penalties_Numbers.txt` | Dorsales de los jugadores sancionados, uno por línea | `12` |
| `Home_Penalties_Timers.txt` / `Away_Penalties_Timers.txt` | Tiempo restante de cada sanción activa, uno por línea | `1:32` |
| `NHL_Penalties_Title.txt` | Etiqueta de superioridad numérica para la sanción activa más corta | `5 ON 4` |
| `NHL_Penalties_Time.txt` | Tiempo restante de la sanción activa más corta | `1:32` |

### Archivos de imagen {#image-files}

| Archivo | Contenido |
|---|---|
| `Home_Logo.png` / `Away_Logo.png` / `Match_Logo.png` | Logotipo del equipo/partido |
| `Home_Promo.png` / `Away_Promo.png` / `Match_Promo.png` | Gráfico promocional, p. ej., una imagen de la alineación |
| `Home_Penalty_Card.png` / `Away_Penalty_Card.png` | Gráfico de tarjeta amarilla/roja |

No todos los archivos sirven para todos los deportes: los tiros y los puntos son contadores independientes que puedes renombrar según tu deporte, y los dos archivos de sanciones NHL solo se actualizan mientras hay una sanción activa.

---

## Cómo añadir un cronómetro o contador de texto en OBS {#how-to-add-a-text-timer-or-counter-in-obs}

![Añadir en OBS una fuente de texto de cronómetro vinculada a un archivo TXT de ScoreBoard](/tutorial-img/how_add_text_to_obs.gif)

### 1. Abre OBS Studio  
Inicia OBS Studio en tu ordenador.

### 2. Crea una nueva escena (opcional)  
Si quieres organizar tu configuración, crea una nueva escena:  
- Haz clic en el botón **+** de la sección **Escenas** (*Scenes*).  
- Ponle un nombre a la escena y guárdala.

### 3. Añade una fuente de texto  
- En la sección **Fuentes** (*Sources*), haz clic en el botón **+**.  
- Selecciona **Texto (FreeType 2)** (*Text (FreeType 2)*) en la lista.  
*O simplemente arrastra el archivo de texto deseado desde el Finder a la ventana de OBS.*

### 4. Pon nombre a la fuente de texto  
- Escribe un nombre descriptivo para la fuente (p. ej., `Main Timer`).  
- Haz clic en **Aceptar** (*OK*) para crear la fuente.

### 5. Activa la lectura desde archivo  
- En la ventana de propiedades de la fuente de texto, marca la casilla **Leer desde archivo** (*Read from File*).  
- Así el texto se actualizará automáticamente desde un archivo TXT.

### 6. Selecciona el archivo TXT  
- Haz clic en **Examinar** (*Browse*) junto al campo de la ruta del archivo.  
- Busca tu archivo TXT local, selecciónalo y haz clic en **Abrir** (*Open*).

### 7. Coloca el texto en el lienzo  
- Arrastra el cuadro de texto en la vista previa para situarlo en la escena.  
- Cambia su tamaño si es necesario.

### 8. Personaliza el aspecto  
- Usa las opciones **Fuente**, **Tamaño** y **Color** (*Font*, *Size*, *Color*) para ajustar el estilo del texto.  
- Prueba la alineación, el degradado y el fondo para que encaje con tu diseño.

### 9. Comprueba la actualización del archivo  
- Cambia el valor del contador en ScoreBoard, por ejemplo, inicia un cronómetro.  
- Comprueba que los cambios aparecen en OBS en tiempo real.

**Añade y configura del mismo modo todos los cronómetros/contadores que necesites para la transmisión de tu deporte.**

---

## Cómo añadir una imagen de fondo del marcador en OBS {#how-to-add-a-scorebug-background-image-in-obs}

![Añadir en OBS una fuente de imagen con el fondo del marcador](/tutorial-img/how_add_scoreboard_background_to_obs.gif)

### 1. Añade una fuente de Imagen  
- En la sección **Fuentes** (*Sources*), haz clic en el botón **+**.  
- Selecciona **Imagen** (*Image*) en la lista.  
*O simplemente arrastra la imagen deseada desde el Finder a la ventana de OBS.*

### 2. Pon nombre a la fuente de imagen  
- Escribe un nombre descriptivo para la fuente (p. ej., `Background`) y haz clic en **Aceptar** (*OK*).  

### 3. Selecciona el archivo de imagen  
- Haz clic en **Examinar** (*Browse*) junto al campo de la ruta del archivo.  
- Busca tu archivo de imagen local, selecciónalo y haz clic en **Abrir** (*Open*).
- Después haz clic en **Aceptar** (*OK*) para guardar la fuente.

### 4. Coloca la imagen debajo de las capas de texto  
- Arrastra la imagen en la vista previa para situarla en la escena.  
- Cambia su tamaño si es necesario.
- En la lista de fuentes, mueve el fondo al final del todo.

*Ejemplo de fondo para el marcador:*
![Ejemplo de plantilla de fondo para un marcador deportivo](/tutorial-img/DefaultScoreBoard.png)

---

## Cómo mostrar las décimas de segundo en OBS {#how-to-display-tenths-of-a-second-in-obs}

*Por defecto, OBS lee los archivos de texto aproximadamente una vez por segundo. Para mostrar correctamente las décimas, hay que reducir ese retardo.*

![Cronómetro con décimas de segundo en OBS usando Advanced Scene Switcher](/tutorial-img/AdvancedSceneSwitcher/Show_tenths_timer.gif)

### 1. Instala el plugin [Advanced Scene Switcher](https://obsproject.com/forum/resources/advanced-scene-switcher.395/)
  
### 2. Abre el plugin 
- Menú principal de OBS – **Herramientas** (*Tools*) – **Advanced Scene Switcher**  
- En la pestaña **General**, ajusta **Check conditions every** a **100ms**

![Pestaña General de Advanced Scene Switcher con el intervalo de comprobación en 100 ms](/tutorial-img/AdvancedSceneSwitcher/Advanced_Scene_Switcher_General.png)

### 3. Añade una nueva macro  
- Haz clic en el botón **+** de la esquina inferior izquierda y cambia el nombre de la macro (p. ej., «Timer Delay»)  
- Desmarca **Perform actions only on condition change**  

### 4. Añade una nueva condición  
- Haz clic en el botón **+** de la sección de condiciones  
- Selecciona **If**  
- Elige **File**  
- Haz clic en **Browse**  
- Selecciona el archivo «Timer.txt» (u otro) en la carpeta de salida de ScoreBoard  
- Ajusta la condición a **content changed**  

### 5. Añade una nueva acción  
- Haz clic en el botón **+** de la sección de acciones  
- Selecciona **Source**  
- Elige **Set Settings**  
- Selecciona tu fuente FreeType 2 (p. ej., «Main Timer»)  
- Ajusta **Text(Text)**  
- Elige **Set to macro property**  
- Selecciona **File content**

![Condición y acción de una macro de Advanced Scene Switcher para actualizar la fuente de texto de OBS](/tutorial-img/AdvancedSceneSwitcher/Advanced_Scene_Switcher_Macro.png)

### 6. Cambia el modo de entrada de texto de la fuente del cronómetro  
- En OBS, haz doble clic en tu fuente FreeType 2 en la lista de fuentes (p. ej., «Main Timer»)  
- Cambia el modo de entrada de texto (*Text input mode*) a manual (*Manual*)  
- Escribe cualquier texto provisional (p. ej., un espacio) en el campo **Texto** (*Text*)  
- Haz clic en **Aceptar** (*OK*)

![Propiedades de una fuente de texto FreeType 2 en OBS con el modo de entrada manual](/tutorial-img/AdvancedSceneSwitcher/OBS_Property_FreeType2_manual.png) 

### 7. Inicia el cronómetro principal en ScoreBoard y compruébalo  
- En los ajustes de ScoreBoard, elige un estilo para el cronómetro principal (p. ej., [:5.3] o [5.3])
- Para probar, ajusta el cronómetro de ScoreBoard a 1 minuto (1:00)
- Inicia el cronómetro y comprueba el resultado en OBS

---

## Cómo mostrar las alineaciones en una transmisión de OBS {#how-to-show-team-rosters-in-an-obs-broadcast}
![Alineación de un equipo junto a un marcador de ScoreBoard en OBS](/tutorial-img/RostersScoreBoard.png)

### Fuente de imagen {#image-source}
1. Crea un archivo gráfico (PDF o imagen) con la alineación del equipo en el programa que prefieras.

2. Añade el archivo al botón de promo del equipo local (home promo) o visitante (away promo) en ScoreBoard y hazlo visible.

3. Añade en OBS una fuente de Imagen para el archivo Home_Promo.png o Away_Promo.png.

### Fuente de texto {#text-source}
1. Añade en OBS una fuente de texto para los archivos Home_Status.txt y Away_Status.txt.

2. Escribe la alineación en el campo Estado (Status) de cada equipo en ScoreBoard. Por ejemplo:
>#4   Erik Lindqvist  
>#7   Marco Bianchi  
>#9   Connor MacLeod  
>#11  Lukas Weber  
>#13  Tomas Novak  
>#16  Henrik Andersson  
>#19  Diego Fernandez  
>#21  Kai Nakamura  
>#23  Owen Fitzgerald  
>#27  Niklas Berg  
>#29  Marek Kowalski  
>#33  Jesse Virtanen  
>#44  Liam O'Brien  
>#61  Pavel Dvorak  
>#71  Anders Holm  
>#88  Zach Whitfield  
>#91  Miroslav Klimek  

3. Añade una imagen de fondo o una fuente de color sólido (*Color Source*).

4. Agrupa las capas de texto y de fondo en un solo grupo para controlar su visibilidad con un solo clic.

---

Volver a la [presentación de ScoreBoard para Mac](/es/) o [descargar la versión de prueba gratuita](/free-apps/ScoreBoard-free.zip).

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "inLanguage": "es",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "¿Cómo añado un marcador deportivo en vivo a OBS en Mac?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Instala ScoreBoard para Mac y, después, añade sus archivos TXT de salida como fuentes Texto (FreeType 2) y sus imágenes de promo/logotipo como fuentes Imagen en OBS."
      }
    },
    {
      "@type": "Question",
      "name": "¿Por qué mi fuente de texto de OBS no se actualiza al instante?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Por defecto, OBS vuelve a leer los archivos de texto aproximadamente una vez por segundo. Para actualizaciones más rápidas, como las décimas de segundo de un cronómetro, usa el plugin Advanced Scene Switcher: reduce el intervalo de comprobación y pasa el contenido del archivo a la fuente de texto."
      }
    },
    {
      "@type": "Question",
      "name": "¿Puedo mostrar las alineaciones de los equipos en mi transmisión?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Sí. Añade la alineación como texto en el campo Estado de un equipo y/o como imagen mediante los botones de promo de ScoreBoard, y muéstrala con fuentes de Texto e Imagen en OBS."
      }
    },
    {
      "@type": "Question",
      "name": "¿Funciona en Streamlabs, Wirecast o Meld en lugar de OBS?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Sí. ScoreBoard genera archivos TXT e imágenes simples que cualquier software de streaming con fuentes de archivos de texto o de imagen puede leer igual que OBS."
      }
    },
    {
      "@type": "Question",
      "name": "¿Necesito una imagen de fondo para el marcador o basta con las fuentes de texto?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Ambas opciones sirven. Las fuentes de texto por sí solas muestran los valores en vivo; una imagen de fondo detrás le da a la superposición un aspecto más cuidado."
      }
    }
  ]
}
</script>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "HowTo",
  "inLanguage": "es",
  "name": "Cómo añadir un cronómetro o contador de texto en OBS",
  "step": [
    { "@type": "HowToStep", "position": 1, "name": "Abre OBS Studio", "text": "Inicia OBS Studio en tu ordenador." },
    { "@type": "HowToStep", "position": 2, "name": "Crea una nueva escena (opcional)", "text": "Haz clic en el botón + de la sección Escenas, ponle un nombre a la escena y guárdala." },
    { "@type": "HowToStep", "position": 3, "name": "Añade una fuente de texto", "text": "En la sección Fuentes, haz clic en el botón + y selecciona Texto (FreeType 2), o arrastra el archivo de texto deseado desde el Finder a la ventana de OBS." },
    { "@type": "HowToStep", "position": 4, "name": "Pon nombre a la fuente de texto", "text": "Escribe un nombre descriptivo para la fuente y haz clic en Aceptar para crearla." },
    { "@type": "HowToStep", "position": 5, "name": "Activa la lectura desde archivo", "text": "En la ventana de propiedades de la fuente de texto, marca la casilla Leer desde archivo." },
    { "@type": "HowToStep", "position": 6, "name": "Selecciona el archivo TXT", "text": "Haz clic en Examinar junto al campo de la ruta del archivo, busca tu archivo TXT local, selecciónalo y haz clic en Abrir." },
    { "@type": "HowToStep", "position": 7, "name": "Coloca el texto en el lienzo", "text": "Arrastra el cuadro de texto en la vista previa para situarlo en la escena y cambia su tamaño si es necesario." },
    { "@type": "HowToStep", "position": 8, "name": "Personaliza el aspecto", "text": "Usa las opciones Fuente, Tamaño y Color para ajustar el estilo del texto." },
    { "@type": "HowToStep", "position": 9, "name": "Comprueba la actualización del archivo", "text": "Cambia el valor del contador en ScoreBoard y comprueba que los cambios aparecen en OBS en tiempo real." }
  ]
}
</script>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "HowTo",
  "inLanguage": "es",
  "name": "Cómo añadir una imagen de fondo del marcador en OBS",
  "step": [
    { "@type": "HowToStep", "position": 1, "name": "Añade una fuente de Imagen", "text": "En la sección Fuentes, haz clic en el botón + y selecciona Imagen, o arrastra la imagen deseada desde el Finder a la ventana de OBS." },
    { "@type": "HowToStep", "position": 2, "name": "Pon nombre a la fuente de imagen", "text": "Escribe un nombre descriptivo para la fuente y haz clic en Aceptar." },
    { "@type": "HowToStep", "position": 3, "name": "Selecciona el archivo de imagen", "text": "Haz clic en Examinar junto al campo de la ruta del archivo, selecciona tu imagen local, haz clic en Abrir y después en Aceptar para guardar la fuente." },
    { "@type": "HowToStep", "position": 4, "name": "Coloca la imagen debajo de las capas de texto", "text": "Arrastra la imagen en la vista previa para situarla, cambia su tamaño si es necesario y muévela al final de la lista de fuentes." }
  ]
}
</script>
