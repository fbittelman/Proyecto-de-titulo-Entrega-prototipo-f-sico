# Desafío 3: Fabricación y evaluación experimental del sistema

Repositorio del Grupo 7 para el curso **ICM3390 - Taller de Diseño de Productos Mecánicos**, Pontificia Universidad Católica de Chile.

Este repositorio contiene la documentación técnica, archivos CAD, planos de fabricación y antecedentes de manufactura asociados al prototipo final en su versión **As Built**.

## Descripción del proyecto

El proyecto consiste en el diseño, fabricación y evaluación experimental de un prototipo dispensador con sistema de enfriamiento mediante recirculación e intercambio de calor.

La versión documentada corresponde al diseño **As Built**, es decir, la configuración real fabricada y ensamblada para la evaluación experimental. Esta versión incorpora modificaciones realizadas durante la etapa de manufactura, principalmente por compatibilidad con componentes comerciales, disponibilidad de fittings, adaptación de mangueras y mejoras estructurales.

El sistema está compuesto por una estructura principal fabricada mayoritariamente mediante impresión 3D, un circuito hidráulico con mangueras y flexibles, bombas, fittings comerciales, una válvula de servicio, un growler, un tanque de recirculación y un intercambiador de calor de cobre.

## Estructura del repositorio

```text
.
├── CAD/
│   ├── Ensamble_general/
│   ├── Componentes/
│   └── Exportados_STEP_STL/
│
├── Planos/
│   ├── Ensamble_general.pdf
│   └── Planos_fabricacion/
│
├── Informe/
│   └── Informe_3_PDT_GRUPO_7.pdf
│
├── Simulaciones/
│   ├── Perdidas_de_carga/
│   ├── Monte_Carlo/
│   └── Graficos/
│
├── Imagenes/
│   ├── Prototipo_final/
│   └── Registro_fabricacion/
│
└── README.md
```

## Archivos CAD

La carpeta `CAD/` contiene el modelo tridimensional del prototipo final. Se incluyen archivos del ensamble general y de los componentes individuales utilizados en la versión **As Built**.

Entre los componentes modelados se encuentran la estructura inferior, estructura intermedia, estructura superior, base de soporte, tapas, soportes internos, adaptador del growler, soportes para bomba, soportes para growler, riel estructural e intercambiador de calor.

## Planos de fabricación

La carpeta `Planos/` contiene la documentación técnica utilizada para fabricar y ensamblar el prototipo. Los planos corresponden a la versión final del sistema y permiten identificar dimensiones, geometría, materiales y relaciones de ensamble.

## Materiales principales

| Componente                | Material |
| ------------------------- | -------- |
| Estructura principal      | PETG     |
| Tapa trasera              | MDF      |
| Intercambiador de calor   | Cobre    |
| Adaptador growler-bomba   | TPU      |
| Riel estructural interior | Aluminio |
| Growler                   | Vidrio   |
| Tanque de recirculación   | Vidrio   |

## Manufactura

La estructura principal fue fabricada mediante impresión 3D. La tapa trasera fue fabricada en MDF mediante corte con herramienta rotativa, mientras que el intercambiador de calor fue ensamblado mediante soldadura con estaño.

Los componentes hidráulicos, bombas, válvula, termocupla, fittings y mangueras fueron seleccionados a partir de disponibilidad comercial. Durante la fabricación se realizaron ajustes geométricos y de conexión para asegurar compatibilidad mecánica entre los distintos elementos del sistema y reducir el riesgo de fugas.

## Cambios principales respecto a la versión anterior

El diseño final aumentó su tamaño general debido a la necesidad de adaptar el sistema a mangueras y fittings disponibles en el mercado. Para facilitar la manufactura y el ensamble, la estructura se dividió en tres secciones principales.

También se incorporaron rieles de aluminio para aumentar la rigidez estructural, se modificó la zona de anclaje de la válvula dispensadora, se aumentó el espacio para el paso de tuberías, se agregaron tapas exteriores, se incorporó una termocupla y se añadieron patas en la base para mejorar la estabilidad del prototipo.

## Recálculos y simulaciones

Debido a las modificaciones del circuito hidráulico, se actualizaron los cálculos de pérdida de carga, caudal de operación y tiempo de enfriamiento.

El caudal actualizado de la bomba 2 fue de aproximadamente **1.37 L/min** tanto para agua con gas como para agua sin gas. Además, se realizaron simulaciones de Monte Carlo para estimar la variabilidad del tiempo de enfriamiento.

## Especificaciones finales

| Variable                            | Valor actualizado P50 |
| ----------------------------------- | --------------------: |
| Temperatura de salida objetivo      |                  8 °C |
| Caudal bomba 2, agua con gas        |            1.37 L/min |
| Caudal bomba 2, agua sin gas        |            1.37 L/min |
| Tiempo de enfriamiento agua con gas |               71.05 s |
| Tiempo de enfriamiento agua sin gas |               67.95 s |

## Integrantes

| Nombre             |
| ------------------ |
| Fernando Bittelman |
| Alonso Espinoza    |
| Enrique Rojas      |
| Martín Salinas     |

## Uso del repositorio

Para revisar o replicar el diseño, se recomienda comenzar por el informe técnico, luego revisar el ensamble general en CAD y finalmente consultar los planos individuales de fabricación.

El informe incluido en la carpeta `Informe/` documenta la descripción del sistema, los cambios respecto a la entrega anterior, el proceso de manufactura, los recálculos, las simulaciones y las especificaciones finales del prototipo.

## Licencia

Repositorio desarrollado con fines académicos para el curso **ICM3390 - Taller de Diseño de Productos Mecánicos**.
