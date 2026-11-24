# Guía de Moodle y estado del paquete H5P

## Estado de entrega

**No se incluye un archivo `.h5p` importable.** Se comprobó el código fuente público de Course Presentation y de sus dependencias; los repositorios consultados exponen fuentes y manifiestos, pero no los archivos de ejecución compilados que sus manifiestos requieren. Un `.h5p` sin esos archivos no sería un paquete funcional. Por eso se entrega una demostración HTML autocontenida y una guía de preparación/importación, sin afirmar que el HTML o un JSON descriptivo puedan importarse como H5P.

La demostración `prototipo_residuos.html` es interactiva en un navegador, pero **no es un H5P**. Para convertirla en contenido H5P, hay que recrear las tres diapositivas en el editor Course Presentation de Moodle (o empaquetarla con las bibliotecas completas y compatibles).

## Preparar el tipo de contenido en Moodle

1. Ingrese con una cuenta administradora y abra la administración de tipos de contenido H5P. Según la versión, suele encontrarse en **Administración del sitio → Plugins → Módulos de actividad → H5P → Administrar tipos de contenido** (o en el área H5P/Content bank).
2. Actualice/instale los tipos de contenido disponibles desde H5P Hub. Confirme que aparecen **Course Presentation** y **Multiple Choice**, junto con las dependencias que Moodle solicite. Las dependencias runtime que se observaron en los manifiestos consultados incluyen `H5P.CoursePresentation`, `H5P.MultiChoice`, `H5P.Question`, `H5P.JoubelUI`, `H5P.FontIcons`, `FontAwesome`, `H5P.Transition`, `H5P.Components`, `jQuery.ui` y `H5P.Text`; las versiones ofrecidas por Moodle/H5P Hub pueden variar.
3. Si la instancia no tiene acceso al Hub, solicite a la persona administradora del Moodle que instale las bibliotecas desde paquetes oficiales compatibles con esa versión. No copie solo los manifiestos ni fuentes sin compilar: Course Presentation espera sus recursos de ejecución.
4. En el Banco de contenido, cree contenido **Course Presentation** y reproduzca la secuencia de tres diapositivas —inicio, ejemplo guiado de cáscara de mandarina y práctica— y las dos preguntas según `analisis_actividad_residuos.md` y `prototipo_residuos.html`.
5. Guarde el contenido como archivo `.h5p` desde el editor de Moodle. Si Moodle presenta dependencias faltantes, instale/actualice las bibliotecas indicadas y vuelva a guardar/exportar.
6. Importe el `.h5p` resultante en el Banco de contenido o agréguelo a un curso con la actividad H5P. Pruebe el paquete en la misma versión de Moodle donde se utilizará.

## Comprobaciones antes de entregar

- El archivo exportado debe incluir `h5p.json`, `content/content.json` y todas las dependencias de ejecución declaradas, con sus carpetas y recursos reales.
- Reabra/importa el paquete en Moodle de destino; que sea un ZIP con extensión `.h5p` no basta para demostrar compatibilidad.
- Compruebe exactamente tres diapositivas, dos preguntas de tres opciones, retroalimentación correcta/incorrecta y visualización móvil.
- Revise las normas locales de separación de residuos y sustituya las categorías si la localidad usa otra clasificación.

## Limitación concreta de esta entrega

No se construyó ni validó un `.h5p` en Moodle. La disponibilidad de bibliotecas depende del Moodle de destino y de sus versiones instaladas. La guía no presupone permisos de administración ni publicación; no se publicó contenido ni se creó una URL pública.

## Publicación y enlace

La consigna también solicita publicar el recurso y enviar el enlace. Ese paso queda pendiente: no se proporcionó una instancia, cuenta ni permiso de publicación. Para completarlo, una persona con acceso debe crear/exportar el Course Presentation en el Moodle del curso, agregarlo a la actividad o al Banco de contenido, verificar los permisos de acceso del curso y compartir el enlace que Moodle genere con su audiencia. Un enlace de Moodle puede requerir inicio de sesión; no se debe tratar como público sin comprobar los permisos.
