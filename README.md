Sistema operativo para OSINT, ciberinteligencia, análisis forense e inteligencia artificial local.

Alcázar-OS es una distribución especializada basada en Debian GNU/Linux 13 “Trixie”. Reúne herramientas de investigación, análisis y elaboración de informes en un entorno ligero, modular y organizado.

El proyecto incorpora Alcaza-IA, un asistente de inteligencia artificial ejecutado localmente mediante Jan, llama.cpp y Qwen2.5-3B-Instruct Q4_K_M.

Alcázar-OS nació como parte de un Trabajo Fin de Máster, pero no es un proyecto abandonado ni cerrado. Continuará manteniéndose, ampliándose y mejorándose hasta alcanzar una versión definitiva, estable y preparada para su distribución.

Estado del proyecto

Versión actual: Alcázar-OS v0.1Estado: prototipo funcional en desarrollo activoBase: Debian GNU/Linux 13 “Trixie”Distribución pública: pendiente de validación

La máquina virtual en formato OVA y los enlaces de descarga se publicarán cuando hayan sido revisados y validados. Actualmente no existe una descarga pública oficial.

Objetivos

Reunir herramientas de ciberinteligencia en una única plataforma.

Organizar las aplicaciones según el flujo de trabajo del analista.

Mantener un consumo moderado de recursos.

Ejecutar inteligencia artificial de forma local.

Activar los servicios de anonimato únicamente cuando sean necesarios.

Facilitar la investigación, el análisis y la creación de informes.

Construir una plataforma modular que pueda mantenerse y ampliarse.

Categorías

Las aplicaciones y recursos se organizan en ocho áreas:

Número

Categoría

Finalidad

01

OSINT

Investigación de fuentes abiertas

02

CTI

Inteligencia de amenazas

03

GEOINT

Análisis geoespacial

04

IMINT

Análisis de imágenes y metadatos

05

FORENSE

Informática forense y recuperación de evidencias

06

IA

Asistencia mediante inteligencia artificial local

07

ANONIMATO

Privacidad y anonimato bajo demanda

08

REPORTES

Elaboración y revisión de informes

Alcaza-IA

Alcaza-IA proporciona asistencia local para organizar investigaciones, plantear metodologías, analizar información y preparar documentación.

Su arquitectura está compuesta por:

Jan como interfaz gráfica.

llama.cpp como motor de inferencia.

Qwen2.5-3B-Instruct Q4_K_M como modelo seleccionado.

También se evaluó Qwen2.5 de 1,5B parámetros, pero el modelo de 3B ofreció un equilibrio más adecuado entre calidad de respuesta y consumo de recursos.

La IA sirve como herramienta de apoyo. Sus resultados deben ser revisados y contrastados por el analista.

Arquitectura

Alcázar-OS utiliza:

Debian GNU/Linux 13 “Trixie”.

LXQt como entorno de escritorio.

XFWM4 como gestor de ventanas.

X11 como sistema gráfico.

SDDM como gestor de acceso.

Thunar como gestor de archivos.

La interfaz, el menú de aplicaciones, GRUB y la pantalla de acceso cuentan con una identidad visual propia.

Métricas

Las pruebas se realizaron en una máquina virtual con 6 vCPU y aproximadamente 8 GiB de RAM.

Medición

Antes

Después

Memoria utilizada en reposo

985 MiB

764 MiB

Servicios activos

17

16

Tiempo de arranque

11,003 s

8,223 s

Con Jan y Qwen2.5-3B activos:

Aproximadamente 3,0 GiB de RAM utilizada.

Aproximadamente 4,7 GiB disponibles.

0 B de memoria swap utilizada.

La optimización principal consistió en impedir que Tor y Privoxy se ejecutaran automáticamente, manteniéndolos disponibles bajo demanda.

Capturas

Las capturas definitivas del sistema se incorporarán progresivamente.

<!-- Ejemplo:
![Escritorio de Alcázar-OS](assets/capturas/escritorio.webp)
-->

Hoja de ruta

Las siguientes líneas de trabajo están previstas para futuras versiones:

Validación definitiva de la máquina virtual OVA.

Ampliación y actualización del catálogo de herramientas.

Mayor integración entre Alcaza-IA y las aplicaciones del sistema.

Incorporación de mecanismos RAG.

Automatización de tareas de investigación.

Mejora del sistema de actualización y mantenimiento.

Realización de nuevas pruebas de estabilidad y rendimiento.

Revisión de seguridad, privacidad y eliminación de datos personales.

Publicación de documentación técnica y manuales de uso.

Preparación de una versión definitiva para su distribución.

Blog del proyecto

Este repositorio contiene el sitio web estático de Alcázar-OS. Está desarrollado con HTML y CSS, sin frameworks ni dependencias externas.

Publicación con GitHub Pages

Accede a Settings → Pages dentro del repositorio.

Selecciona Deploy from a branch.

Elige la rama main.

Selecciona la carpeta / (root).

Guarda la configuración.
