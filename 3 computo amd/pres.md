---
title: "Cómputo AMD: Bulldozer, Piledriver"
date: Actividad 3 - Centro de Procesamiento de Datos - UGR
author: David Charte
theme: metropolis
colortheme: metropolis
lang: spanish
polyglossia-lang.name: spanish
graphics: true
classoption:
  - compress
header-includes:
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
- "\\defbeamertemplate*{footline}{miniframes theme no subsection}{}"
- \beamertemplatenavigationsymbolsempty
---

# Introducción

## Sobre AMD

* Fundada por Jerry Sanders en 1969
* Establecida en Sunnyvale, California
* Microcódigos: Acuerdo con Intel hasta 486
* Diseñó x86-64 en 2000 (K8 series)
* Compra ATI en 2006

![](amdhq.jpg)

# Bulldozer

## Bulldozer

* Lanzada en octubre de 2011
* Predecesor: K10
* 32 nm
* Soporte para AVX: AES, SSE4.1, SSE4.2; instrucciones SSE5 compatibles con AVX
* Soporte para DDR3

## Clustered Multithreading

\columnsbegin
\column{0.5\textwidth}

* Alternativa simple a SMT (*Hyperthreading*)
* Desarrollado por DEC en 1996
* En Bulldozer: equivalente a 2 cores para enteros/1 core SMT para coma flotante
* Desventaja: 1 hebra sola desaprovecha unidades de ejecución

\column{0.5\textwidth}
\includegraphics[width=\textwidth]{bulldozer_cpu.PNG}
\columnsend

## Rendimiento

* Rendimiento menor de lo esperado en Linux
* Resultados de benchmarks heterogéneos (FX-8150)
* Poco eficiente bajo carga

\centering\scriptsize
`https://www.phoronix.com/scan.php?page=article&item=amd_fx8150_bulldozer&num=1`

# Piledriver

## Piledriver

* Segunda generación de Bulldozer

# Siguientes generaciones

## Steamroller

## Excavator
