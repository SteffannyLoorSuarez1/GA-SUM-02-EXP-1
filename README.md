
# GA-SUM-02 / EXP-1 — Computación paralela y RabbitMQ

**Universidad:** Universidad Técnica Estatal de Quevedo (UTEQ)  
**Asignatura:** Aplicaciones Distribuidas  
**Actividad:** GA-SUM-02 / EXP-1  
**Tema asignado:** Computación paralela (sincronía, asincronía e hilos)  
**Sistema de análisis propuesto:** RabbitMQ  
**Integrantes:** Sánchez, Loor y Zambrano  
**Fecha:** Noviembre de 2026

## Objetivo

Explicar los fundamentos de la computación paralela y analizar
RabbitMQ como sistema distribuido real, aplicando los conceptos
de arquitectura, transparencias, CAP/PACELC, comunicación,
tolerancia a fallos y análisis crítico.

> Pendiente: confirmar que el docente autorice RabbitMQ como
> sistema de análisis para GA-SUM-02.

## Distribución del trabajo

| Integrante | Responsabilidades | Rama |
|---|---|---|
| Sánchez | Fundamentos, arquitectura y transparencias | `sanchez/arquitectura` |
| Loor | Sincronía, asincronía, hilos, CAP/PACELC y comunicación | `loor/comunicacion` |
| Zambrano | Fallos, comparación y conclusiones | `zambrano/fallos` |

Cada integrante trabaja en sus propios archivos y presenta
sus cambios mediante un Pull Request hacia `main`.

## Estructura

- `main.tex`: presentación Beamer.
- `notas.tex`: notas de exposición y declaración de IA.
- `secciones/`: diapositivas de cada apartado.
- `notas/`: notas individuales.
- `referencias/`: bibliografía de cada integrante.
- `diagramas/`: diagramas editables y exportaciones.
- `evidencias/`: bosquejo, capturas y ensayo.
- `BITACORA.md`: registro de trabajo del equipo.
- `entrega/`: PDF de identificación para el SGA.

## Compilación

### Requisitos

- Distribución LaTeX (MiKTeX o TeX Live).
- PDFLaTeX.
- Biber.
- Paquetes Beamer, biblatex, babel, graphicx,
  booktabs, tabularx, geometry y float.

### Diapositivas

```powershell
pdflatex -interaction=nonstopmode -halt-on-error main.tex
biber main
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
```

### Notas

```powershell
pdflatex -interaction=nonstopmode -halt-on-error notas.tex
biber notas
pdflatex -interaction=nonstopmode -halt-on-error notas.tex
pdflatex -interaction=nonstopmode -halt-on-error notas.tex
```

## Evidencias obligatorias

- Historial de trabajo en al menos tres días distintos.
- Tres commits significativos por integrante.
- Bosquejo de arquitectura a mano con nombres y fecha.
- Tres capturas anotadas de artículos con páginas.
- Ejemplo del entorno propio.
- Ensayo grabado con todos los integrantes.
- Bitácora de trabajo.
- Declaración de uso de IA.

## Video del ensayo

**Enlace:** Pendiente.

## Referencias

Se requieren al menos seis referencias publicadas en los
últimos cinco años, incluyendo tres artículos de revistas
indexadas con DOI verificable.

## Entrega

El repositorio debe ser público y contener los archivos
fuente, diagramas editables, evidencias y PDF compilados.

En el SGA se entrega únicamente un PDF de una página con
los datos del equipo y la URL completa del repositorio.
