---
title: Google en Hamina, Finlandia
date: Centro de Procesamiento de Datos - UGR
author: David Charte
theme: m
colortheme: metropolis
lang: spanish
polyglossia-lang.name: spanish
mainfont: "Fira Sans"
monofont: "Fira Mono"
graphics: true
classoption:
  - compress
header-includes:
- "%\\metroset[sectionpage=none]"
- \newcommand{\columnsbegin}{\begin{columns}}
- \newcommand{\columnsend}{\end{columns}}
- \definecolor{headbg}{RGB}{61, 96, 103}
- \definecolor{headfg}{RGB}{232, 239, 241}
- \setbeamercolor{headtitle}{fg=headfg,bg=headbg}
- \setbeamercolor{headnav}{fg=headfg,bg=headbg}
- \setbeamercolor{section in head/foot}{fg=headfg,bg=headbg}
- "\\defbeamertemplate*{headline}{miniframes theme no subsection}{
    \\begin{beamercolorbox}[ht=2.5ex,dp=1.125ex,
      leftskip=.3cm,rightskip=.3cm plus1fil]{headtitle}
      {\\usebeamerfont{title in head/foot}\\insertshorttitle}
      \\hfill
      \\leavevmode{\\usebeamerfont{author in head/foot}\\insertshortauthor}
    \\end{beamercolorbox}
    \\begin{beamercolorbox}[colsep=1.5pt]{upper separation line head}
    \\end{beamercolorbox}
    \\begin{beamercolorbox}{headnav}
      \\vskip2pt\\textsc{\\insertnavigation{\\paperwidth}}\\vskip2pt
    \\end{beamercolorbox}
    \\begin{beamercolorbox}[colsep=1.5pt]{lower separation line head}
    \\end{beamercolorbox}
  }"
- "\\makeatletter\\renewcommand{\\@metropolis@frametitlestrut}{
    \\vphantom{ÁÉÍÓÚABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz}
  }\\makeatother"
- "\\defbeamertemplate*{footline}{miniframes theme no subsection}{}"
- \beamertemplatenavigationsymbolsempty
---

# Hamina

## Localización

\columnsbegin
\column{0.5\textwidth}

* Sur de Finlandia
* 20800 habitantes

\column{0.5\textwidth}
\includegraphics{hamina_location.png}

\columnsend

## Clima

\includegraphics{hamina_weather.png}

# Data center

## CPD

* Construido en el lugar de una **antigua fábrica** de papel
* Mantenida estructura de túneles submarinos
* Objetivo: **100% energía renovable**

\columnsbegin
\column{0.5\textwidth}

\includegraphics{google-hamina-out.jpg}

\column{0.5\textwidth}

\includegraphics{google-hamina-in.jpg}

\columnsend

\scriptsize\centering

`https://www.google.com/about/datacenters/inside/locations/hamina/`

## Infraestructura

* Software: versiones propias de Linux (Google Web Server)
    * Almacenamiento: Google Filesystem, BigTable
    * MapReduce, Sawzall
    * Tolerancia a fallos de hardware
* Hardware: Google no proporciona detalles concretos
    * Fuentes de alimentación no estándares tamaño ATX
    * Cada servidor tiene una batería de 12V
* Redes con topologías propias
* Tier III?

\scriptsize\centering

`https://en.wikipedia.org/wiki/Google_Data_Centers`

# Eficiencia

## Técnicas de refrigeración

* Oportunidad: aprovechar antigua red de conducciones de agua submarinas
* Se utiliza en **intercambiadores de calor**
* No es necesaria refrigeración adicional

\columnsbegin
\column{0.5\textwidth}

\includegraphics{cpd-sea.png}

\column{0.5\textwidth}

\includegraphics{cpd-pipes.png}

\columnsend

\scriptsize\centering

`https://www.google.com/about/datacenters/inside/locations/hamina/`

## Técnicas de refrigeración

* El agua caliente se hace enfriar antes de devolver al mar

\columnsbegin
\column{0.5\textwidth}

\includegraphics{cooldown.png}

\column{0.5\textwidth}

\includegraphics{google-sauna.jpg}

\columnsend

\scriptsize\centering

`https://www.wired.com/2012/10/google-finland-data-center-2/`

## Medición del PUE

\centering
\includegraphics[width=0.65\textwidth]{pueexplained.png}
\flushleft
\scriptsize

*  **ESIS** Energy consumption for supporting infrastructure power substations feeding the cooling plant, lighting, office space, and some network equipment

* **EITS** Energy consumption for IT power substations feeding servers, network, storage, and computer room air conditioners (CRACs)

* **ETX** Medium and high voltage transformer losses

* **EHV** High voltage cable losses

* **ELV** Low voltage cable losses

* **EF** Energy consumption from on-site fuels including natural gas & fuel oils

* **ECRAC** CRAC energy consumption

* **EUPS** Energy loss at uninterruptible power supplies (UPSes) which feed servers, network, and storage equipment

* **ENet1** Network room energy fed from type 1 unit substitution

\normalsize

\scriptsize\centering

`https://www.google.com/about/datacenters/efficiency/internal/`

## PUE

* Último trimestre: **1.12**

* \huge Últimos 12 meses: **1.11**


\scriptsize\centering

`https://www.google.com/about/datacenters/efficiency/internal/`

# Gracias!

## Gracias!

\includegraphics{hamina-cpd.jpg}
