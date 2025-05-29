# Analisis_datos
Este es el repositorio oficial de la asignatura "ANALISIS DE DATOS" del Master Universitario de Ingeniería de la Energía MUIE

# Hechos Relevantes. 
Extrae automa ticamente los Hechos Relevantes del ultimo mes que pueden afectar al mercado ele ctrico en https://umm.omie.es/electricity-list

# Mercado diario “Day ahead “incluyendo ofertas”
Ficheros mensuales con curvas agregadas de oferta y demanda del mercado diario “Day ahead “incluyendo ofertas” para mercado electrico contenidas en los archivos “curva_pbc_uof”  https://www.omie.es/en/file-accesslist#Mercado%20DiarioCurvas?parent=Mercado%20Diario 

# Mercado diario “intra-day“ incluyendo ofertas
Ficheros mensuales con curvas agregadas de oferta y demanda del mercado diario “intra-day“ incluyendo ofertas para mercado electrico contenidas en los archivos  “curva_pibc_uof”

# Indisponibilidades del u ltimo mes. “indisp2024_0X”

## Overview

This repository contains two Python scripts: `extract_data_grupo_4.py`, `clean_data_grupo_4.py` and `visualize_data_grupo_4.py`. These scripts are designed to extract data related to the unavailability declarations of Spanish bid units from a specified website and then visualize the data using bar charts.

### `extract_data_grupo_4.py`

This script downloads the latest unavailability declarations from the OMIE website, extracts any zip files, and saves the data in a local directory.

### `clean_data_grupo_4.py`

This script clean the wrong data contained in the files

### `visualize_data_grupo_4.py`

This script reads the downloaded data files, analyzes them to find the most common values in a specific column, and visualizes these values using bar charts.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/joseluissanchezr/analisis_datos.git
   ```
   ```bash
   cd analisis_datos
   ```
   
2. Move to source code : 
   ```bash
   cd grupo_4
   ```

## Usage

### Extract Data

To download and extract the unavailability data, run the following command:

```bash
python extract_data_grupo_4.py
```

This will create a data directory (if it does not already exist) and download the latest unavailability data files from the OMIE website.

### Visualize Data

To analyze and visualize the data, run the following command:

```bash
python visualize_data_grupo_4.py <top_n>
```

Replace <top_n> with the number of top occurrences you want to visualize. For example:

```bash
python visualize_data_grupo_4.py 30
```

![Exemple_of_usage](exemple_of_visualisation_30.png)

Please wait for the others programs ! 
