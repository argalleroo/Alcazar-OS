<div align="center">

# 🏰 Alcázar-OS

### Ciberinteligencia, investigación e inteligencia artificial local

![Versión](https://img.shields.io/badge/versión-v0.1-e52b2f?style=for-the-badge)
![Estado](https://img.shields.io/badge/estado-desarrollo_activo-e52b2f?style=for-the-badge)
![Base](https://img.shields.io/badge/base-Debian_13-111111?style=for-the-badge&logo=debian&logoColor=white)
![Licencia](https://img.shields.io/badge/licencia-pendiente-555555?style=for-the-badge)

**Alcázar-OS** es una distribución basada en Debian para OSINT, ciberinteligencia,
análisis forense e inteligencia artificial local mediante **Alcaza-IA**.

Nace como parte de un Trabajo Fin de Máster, pero es un proyecto activo y con
futuro: continuará manteniéndose, ampliándose y mejorándose hasta alcanzar una
versión definitiva, estable y preparada para su distribución.

[Explorar el proyecto](#-el-proyecto) · [Capacidades](#-capacidades) · [Resultados](#-resultados) · [Hoja de ruta](#-hoja-de-ruta)

</div>

---

## 🔴 El proyecto

Alcázar-OS reúne herramientas que normalmente se utilizan de forma independiente
en una estación ligera, modular y organizada alrededor del flujo de trabajo del
analista.

Su objetivo no es competir por cantidad de aplicaciones, sino ofrecer un entorno
coherente para investigar, analizar, proteger la información y elaborar resultados.

> [!IMPORTANT]
> **Alcázar-OS no es un proyecto terminado ni abandonado.** La versión v0.1 es el
> punto de partida de un desarrollo que seguirá recibiendo mantenimiento, mejoras
> y nuevas funciones hasta alcanzar una versión definitiva.

## 🧱 Arquitectura

| Capa | Componentes |
|:--|:--|
| **Base** | Debian GNU/Linux 13 “Trixie” |
| **Escritorio** | LXQt, XFWM4, X11, SDDM y Thunar |
| **Capacidades** | OSINT, CTI, GEOINT, IMINT, forense, IA, anonimato y reportes |
| **Inteligencia artificial** | Jan, llama.cpp y Qwen2.5-3B-Instruct Q4_K_M |
| **Interacción** | Menú organizado, aplicaciones locales, terminal y recursos web |

## 🧭 Capacidades

| | Categoría | Función | Algunas herramientas |
|:--:|:--|:--|:--|
| **01** | **OSINT** | Investigación de fuentes abiertas | Sherlock, Maigret, Holehe, theHarvester |
| **02** | **CTI** | Inteligencia de amenazas | YARA, Sigma, VirusTotal CLI |
| **03** | **GEOINT** | Análisis geoespacial | QGIS y recursos especializados |
| **04** | **IMINT** | Imágenes y metadatos | ExifTool, GIMP, ImageMagick, Steghide |
| **05** | **FORENSE** | Evidencias, discos y memoria | Autopsy, Sleuth Kit, Volatility, Binwalk |
| **06** | **IA** | Asistencia local al analista | Jan, llama.cpp, Qwen2.5 |
| **07** | **ANONIMATO** | Privacidad bajo demanda | Tor Browser, Torsocks, ProxyChains, Privoxy |
| **08** | **REPORTES** | Elaboración de entregables | LibreOffice Writer, Pandoc, Okular |

## 🧠 Alcaza-IA

Alcaza-IA incorpora asistencia de inteligencia artificial ejecutada localmente.
Las consultas no necesitan enviarse obligatoriamente a un servicio externo.

```text
┌──────────────┐      ┌──────────────┐      ┌─────────────────────┐
│     Jan      │ ───▶ │  llama.cpp   │ ───▶ │ Qwen2.5-3B Q4_K_M │
│  Interfaz    │      │    Motor     │      │       Modelo        │
└──────────────┘      └──────────────┘      └─────────────────────┘
```

Durante el proyecto se compararon modelos Qwen2.5 Instruct de **1,5B** y **3B**
parámetros. El modelo de 3B fue seleccionado por ofrecer un equilibrio más adecuado
entre calidad de respuesta y consumo de recursos.

> [!NOTE]
> Alcaza-IA funciona como herramienta de apoyo. La información generada debe ser
> revisada, contrastada y validada por el analista.

## 📊 Resultados

Las mediciones se realizaron en una máquina virtual con **6 vCPU** y aproximadamente
**8 GiB de RAM**.

| Métrica | Antes | Después | Mejora |
|:--|--:|--:|--:|
| RAM utilizada en reposo | 985 MiB | **764 MiB** | **−22,4 %** |
| Tiempo de arranque | 11,003 s | **8,223 s** | **−25,3 %** |
| Servicios activos | 17 | **16** | **−1** |

### Con Alcaza-IA activa

| RAM utilizada | RAM disponible | Swap utilizada |
|:--:|:--:|:--:|
| **≈ 3,0 GiB** | **≈ 4,7 GiB** | **0 B** |

La mejora se obtuvo al desactivar el inicio automático de Tor y mantener Tor y
Privoxy disponibles únicamente cuando son necesarios.

## 🖼️ Capturas

Las capturas definitivas del escritorio, el menú, Alcaza-IA y los flujos de
investigación se incorporarán progresivamente en `assets/capturas/`.

<!--
<p align="center">
  <img src="assets/capturas/escritorio.webp" alt="Escritorio principal de Alcázar-OS" width="800">
</p>
-->

## 🚧 Estado actual

| Elemento | Estado |
|:--|:--:|
| Prototipo funcional | ✅ Completado |
| Organización por categorías | ✅ Completado |
| Integración de Alcaza-IA | ✅ Completado |
| Optimización inicial | ✅ Completado |
| Capturas definitivas | 🔄 En preparación |
| Documentación pública | 🔄 En preparación |
| Validación de la OVA | ⏳ Pendiente |
| Versión definitiva | 🚧 En desarrollo |

## 🗺️ Hoja de ruta

- [x] Construir la base sobre Debian 13.
- [x] Crear la identidad visual de Alcázar-OS.
- [x] Organizar las aplicaciones en ocho categorías.
- [x] Integrar Alcaza-IA con Jan, llama.cpp y Qwen2.5.
- [x] Optimizar los servicios y el consumo en reposo.
- [ ] Validar definitivamente la máquina virtual OVA.
- [ ] Publicar la documentación de usuario y técnica.
- [ ] Ampliar y actualizar el catálogo de herramientas.
- [ ] Mejorar la integración entre Alcaza-IA y el sistema.
- [ ] Investigar mecanismos RAG y nuevas automatizaciones.
- [ ] Realizar nuevas pruebas de estabilidad y rendimiento.
- [ ] Preparar una versión definitiva para distribución.

## 🌐 Blog del proyecto

Este repositorio contiene el blog estático de Alcázar-OS. Está desarrollado con
HTML y CSS, sin frameworks ni dependencias externas.

### Publicación mediante GitHub Pages

1. Abre **Settings → Pages** dentro del repositorio.
2. En **Build and deployment**, selecciona **Deploy from a branch**.
3. Elige la rama `main` y la carpeta `/ (root)`.
4. Guarda la configuración.

GitHub Pages publicará el sitio directamente desde `index.html`.

```text
.
├── .nojekyll
├── README.md
├── index.html
├── styles.css
└── assets/
    └── capturas/
```

## 📦 Documentación y descarga

> [!WARNING]
> La OVA todavía no cuenta con una descarga pública oficial. Los enlaces de
> documentación y distribución se añadirán únicamente después de completar su
> revisión y validación.

## ⚖️ Uso responsable

Alcázar-OS es un proyecto académico y experimental en desarrollo. Sus herramientas
deben utilizarse exclusivamente con fines legítimos, educativos y de investigación,
respetando la legislación aplicable y las autorizaciones correspondientes.

---

<div align="center">

**Alcázar-OS v0.1** · Construyendo una estación abierta, privada y modular para la ciberinteligencia.

</div>
