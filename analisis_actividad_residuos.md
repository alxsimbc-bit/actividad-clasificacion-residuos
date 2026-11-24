# Taller individual · Recursos multimedia educativa

## Análisis de requerimientos para una actividad de clasificación de residuos

**Estudiante:** Erick Custodio  
**Carrera y nivel:** Informática, octavo semestre  
**Herramienta elegida:** H5P Course Presentation  
**Público destinatario:** estudiantes de 12 a 14 años  
**Uso previsto:** computadoras y celulares; actividad comprensible con el sonido desactivado.

## 1. Análisis del caso: respuestas individuales

### 1. ¿Quién utilizará el recurso y en qué condiciones?

Lo utilizarán estudiantes de 12 a 14 años como actividad individual de aprendizaje. Accederán desde una computadora o un celular, posiblemente con distintos tamaños de pantalla y sin audio. Por eso las instrucciones, ejemplos y respuestas deben estar escritos, ser directos y poder leerse en una pantalla pequeña. Las categorías exactas de recolección pueden variar por localidad, así que el recurso no debe presentar como universal un color de contenedor.

### 2. ¿Qué deberá ser capaz de hacer el estudiante al terminar la actividad?

Deberá clasificar un residuo orgánico (la cáscara de mandarina, siguiendo la guía local), reconocer una botella plástica vacía y limpia como envase potencialmente reciclable, y distinguir un pañuelo usado del papel limpio reciclable. También deberá interpretar la explicación que recibe después de elegir una respuesta.

### 3. ¿Qué información de la ficha conservarás y qué parte convertirás en una actividad interactiva?

Conservaré los tres objetos de la ficha —cáscara de mandarina, botella plástica limpia y pañuelo usado— y el propósito de practicar su clasificación. La cáscara será un ejemplo guiado con explicación en la segunda diapositiva. Convertiré la botella y el pañuelo en dos preguntas de opción múltiple en la tercera diapositiva, con tres opciones y retroalimentación inmediata escrita para cada respuesta. La primera diapositiva presentará el objetivo e instrucciones breves.

### 4. ¿Qué imágenes, textos o animaciones utilizarás y qué aportará cada elemento?

Incluiré una ilustración vectorial sencilla de una cáscara de mandarina, dibujada dentro del HTML para no depender de archivos o servicios externos; su función es asociar visualmente el ejemplo con el concepto de residuo orgánico. Usaré títulos cortos, instrucciones, nombres de categorías y explicaciones para que el contenido se comprenda sin audio. En la práctica, el texto nombra cada objeto y las opciones de respuesta. No añadiré animaciones decorativas: podrían distraer y no aportan información necesaria; la navegación entre diapositivas será suficiente para mostrar la secuencia.

### 5. ¿Qué acciones podrá realizar el usuario desde que abre el recurso hasta que finaliza?

Podrá leer el objetivo, iniciar la actividad, avanzar y volver entre las diapositivas con los controles de navegación, leer el ejemplo de la cáscara, seleccionar una opción para la botella y otra para el pañuelo y consultar la retroalimentación escrita de cada selección. Los controles serán botones y opciones nativos, utilizables con toque y teclado. No se recopilarán datos personales ni se enviarán resultados a un servicio externo.

### 6. ¿Qué mensaje mostrarás si el estudiante clasifica la botella plástica como residuo orgánico?

Mostraré: **“No: una botella plástica limpia no es un residuo orgánico. Sepárala como envase reciclable si tu localidad la acepta; sigue las instrucciones locales.”** El mensaje identifica el error, explica la distinción y evita asegurar que todas las localidades reciben los mismos envases.

### 7. ¿Qué características tendrá el recurso para que sea fácil de usar desde un celular y con el sonido desactivado?

Usará diseño adaptable, texto legible, bloques breves, botones amplios y opciones separadas con etiquetas claras. Las respuestas tendrán texto de retroalimentación además de una diferencia visual, y los controles mostrarán el foco de teclado. No habrá información esencial transmitida solo por sonido, animación o color. La demostración HTML incluirá su estilo e interacción dentro de un único archivo, sin dependencias de red.

### 8. ¿Qué requerimientos son indispensables para tu prototipo y cómo comprobarás que se cumplen?

Son indispensables: las tres pantallas en el orden pedido; el ejemplo guiado de la cáscara; dos preguntas (botella limpia y pañuelo usado), con tres opciones cada una; retroalimentación escrita que responda a aciertos y errores; legibilidad en celular; y comprensión sin audio. La matriz de la sección 2 asigna una prueba comprobable y un resultado esperado a cada requisito. Esos resultados son criterios de prueba, no observaciones inventadas de una prueba individual.

## 2. Matriz de requerimientos

| Código | Tipo | Requerimiento | ¿Cómo se comprobará? | Resultado esperado |
|---|---|---|---|---|
| RF-01 | Funcional | El prototipo presenta exactamente tres pantallas: inicio, ejemplo guiado de cáscara de mandarina y práctica. | Abrir la demostración y avanzar en orden; contar las pantallas y verificar el contenido. | Se muestran las tres pantallas requeridas, sin una cuarta. |
| RF-02 | Funcional | En práctica, el estudiante puede elegir una categoría para la botella plástica limpia y otra para el pañuelo usado; cada pregunta ofrece tres opciones. | Contar las opciones de ambas preguntas y seleccionar una opción en cada una. | Hay dos preguntas y cada una permite seleccionar exactamente una de tres opciones. |
| RF-03 | Funcional | El recurso explica cada respuesta correcta e incorrecta, incluyendo el caso de botella limpia clasificada como residuo orgánico. | Probar las respuestas correcta e incorrecta en ambas preguntas; comprobar en particular la opción “Residuos orgánicos” de la botella. | Cada elección produce retroalimentación escrita; la botella orgánica recibe el mensaje definido en la respuesta 6. |
| RNF-01 | No funcional | La actividad se entiende y se completa con el sonido desactivado. | Completar las tres pantallas sin activar audio. | Objetivo, instrucciones, ejemplo, opciones y explicaciones se entienden por escrito. |
| RNF-02 | No funcional | La interfaz conserva legibilidad y controles utilizables en computadora y en un celular de 360 px de ancho. | Abrir la demostración a 360 px; inspeccionar texto, botones y desplazamiento horizontal. | No hay contenido cortado ni desplazamiento horizontal de la página; los controles se pueden accionar. |
| RNF-03 | No funcional | El estado de respuesta no se comunica únicamente mediante color y los controles pueden usarse con teclado. | Navegar con Tab/Shift+Tab y seleccionar opciones; revisar el texto de retroalimentación. | El foco es visible y correcto/incorrecto se expresa por escrito. |

## 3. Registro de prueba y ajuste

**Estado: PENDIENTE DE VALIDACIÓN INDIVIDUAL.** No se realizó una prueba individual con un estudiante ni se afirma que se haya observado a un usuario. La verificación técnica del archivo en un navegador no sustituye la prueba individual solicitada en el taller.

| Campo | Estado y registro |
|---|---|
| Fecha, dispositivo y condiciones de audio | Pendiente de completar durante la prueba individual |
| Persona que realiza la prueba | Pendiente; registrar solo la información necesaria |
| Tarea | Completar las tres pantallas y responder ambas preguntas sin ayuda |
| Observación real | Pendiente; anotar conducta o comentario efectivamente observado, sin inventar citas |
| Ajuste propuesto, todavía no validado | Si la persona clasifica la botella como orgánica, comprobar si el mensaje explícito de la respuesta 6 aclara el error. Si persiste la confusión, hacer más visible la diferencia entre material orgánico y envase limpio. |
| Ajuste realizado como consecuencia de una prueba | Pendiente: solo se completará después de una prueba real y de aplicar un cambio comprobable |

## Alcance y limitaciones de entrega

La demostración HTML es un prototipo interactivo publicado en GitHub Pages: [abrir el sitio](https://alxsimbc-bit.github.io/actividad-clasificacion-residuos/). El repositorio público, que contiene el análisis y los archivos del prototipo, está en [GitHub](https://github.com/alxsimbc-bit/actividad-clasificacion-residuos/).

**Limitación:** la demostración HTML no es un paquete H5P ni se puede importar como tal en Moodle. La asignación requiere Course Presentation, pero no se pudo generar un archivo `.h5p` válido con las bibliotecas de ejecución completas en este entorno. Para entregar un H5P nativo, hay que recrear/exportar la actividad desde una instancia Moodle compatible. La prueba individual indicada en la sección 3 también está pendiente de realizar.
