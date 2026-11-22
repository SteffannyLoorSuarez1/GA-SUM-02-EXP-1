
# GA-SUM-02 / EXP-1 — Computación paralela y RabbitMQ

**Universidad:** Universidad Técnica Estatal de Quevedo (UTEQ)  
**Asignatura:** Aplicaciones Distribuidas  
**Actividad:** GA-SUM-02 / EXP-1  
**Tema asignado:** Computación paralela (sincronía, asincronía e hilos)  
**Sistema de análisis propuesto:** RabbitMQ  
**Integrantes:** LOOR SUAREZ STEFFANNY DEL ROCIO, SANCHEZ VERA DARWIN JOEL y ZAMBRANO YONG ANGEL DANIEL
**Fecha:** 21 de Noviembre de 2026

## Objetivo

Explicar los fundamentos de la computación paralela y analizar
RabbitMQ como sistema distribuido real, aplicando los conceptos
de arquitectura, transparencias, CAP/PACELC, comunicación,
tolerancia a fallos y análisis crítico.

## Distribución del trabajo

| Integrante | Responsabilidades | Rama |
|---|---|---|
| Sánchez Darwin | Fundamentos, arquitectura y transparencias | `sanchez/arquitectura` |
| Loor Steffanny| Sincronía, asincronía, hilos, CAP/PACELC y comunicación | `loor/comunicacion` |
| Zambrano Ángel| Fallos, comparación y conclusiones | `zambrano/fallos` |

Cada integrante trabaja en sus propios archivos, y luego se une.

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
## Video del ensayo

**Enlace:**
https://drive.google.com/drive/folders/19zjzoN_4WMlsvBQsWxvj4CusjlUrZKGT?usp=drive_link
