# D-ML-DATOS
Datos para curso de ML

## Archivo publicado

[04-Fichero_para_EJERCICIO_3.json](04-Fichero_para_EJERCICIO_3.json) contiene los datos facilitados para el ejercicio 3 de lectura
de JSON del módulo 3:

- Competición: **English Premier League 2010/11**.
- Partidos: **380**.
- Equipos diferentes: **20**.
- Estructura: un campo `name` y una lista `matches`; los equipos de cada partido
  aparecen en `team1` y `team2`.

## Enlace directo

[Descargar o abrir el JSON](https://raw.githubusercontent.com/mleyvalamas/D-ML-DATOS/main/04-Fichero_para_EJERCICIO_3.json).

```text
https://raw.githubusercontent.com/mleyvalamas/D-ML-DATOS/main/04-Fichero_para_EJERCICIO_3.json
```

Es el enlace al contenido del archivo, adecuado para leerlo desde Pandas:

```python
import pandas as pd

origen = "https://raw.githubusercontent.com/mleyvalamas/D-ML-DATOS/main/04-Fichero_para_EJERCICIO_3.json"
datos = pd.read_json(origen)
```

Para la variante local, descarga el archivo y sustituye `origen` por su ruta.
El procesamiento posterior de los datos será el mismo para ambas variantes.

## Integridad

SHA-256 del archivo original y publicado:

```text
a94631cc82fd4034d4da5f5594d32cb191942f0b594e3a9cd9dcf29fe7dfa707
```

Este repositorio público contiene los datos de ejemplo y su descripción.

## Módulo 6 · Ejercicio 1 · Datos de GOOG

[04-Fichero_para_EJERCICIO_1_MODULO_6.csv](04-Fichero_para_EJERCICIO_1_MODULO_6.csv)
es una copia íntegra del CSV entregado para el examen del módulo 6. Contiene
1.346 registros, desde 2016-01-04 hasta 2021-05-07, con las columnas `Date`,
`Open`, `High`, `Low`, `Adj Close` y `Volume`. La variable objetivo del ejercicio
es `Adj Close`, el cierre ajustado.

### Lectura remota del CSV

Este enlace devuelve el contenido CSV, sin la página de presentación de GitHub:

```text
https://raw.githubusercontent.com/mleyvalamas/D-ML-DATOS/main/04-Fichero_para_EJERCICIO_1_MODULO_6.csv
```

Ejemplo básico de lectura con Pandas:

```python
import pandas as pd

origen = "https://raw.githubusercontent.com/mleyvalamas/D-ML-DATOS/main/04-Fichero_para_EJERCICIO_1_MODULO_6.csv"
datos = pd.read_csv(origen, parse_dates=["Date"])
print(datos.head())
```

### Procedencia e integridad del CSV

La copia procede de
[D-ML · módulo 6](https://github.com/mleyvalamas/D-ML/blob/e3e64df/modulos/modulo_06/tareas/examen/datos/04-Fichero_para_EJERCICIO_1_MODULO_6.csv).
Las indicaciones del curso identifican los datos como históricos de GOOG y citan
Yahoo Finance como fuente. Esta URL sirve el archivo proporcionado por el curso
desde GitHub; no realiza una consulta en directo a Yahoo ni actualiza sus precios.

El original y la copia publicada tienen 70.794 bytes y la misma huella SHA-256:

```text
89eb059f63e759959f8b85a4c9da64d90df750e7ed99eec2711d481ebfc9b4c8
```

El archivo JSON del módulo 3 se conserva sin cambios.

## Módulo 7 · Ejercicio 1 · Calidad del vino

[winequality-red.csv](winequality-red.csv) conserva íntegro el CSV adjuntado por
el alumno el 24 de noviembre de 2026 para el examen del módulo 7.

- 1.599 filas, once características fisicoquímicas y el objetivo `quality`.
- Campos separados por punto y coma (`;`).
- Se conservan las 240 filas repetidas adicionales, sin limpiar ni transformar.

### Lectura remota y copia local

[Descargar el CSV](https://raw.githubusercontent.com/mleyvalamas/D-ML-DATOS/main/winequality-red.csv).
Para leerlo con Pandas se debe indicar `sep=";"`. El examen prevé un único
programa con lectura remota por defecto y una opción local explícita, siguiendo
el criterio del módulo 6.

### Procedencia e integridad

Fuente de referencia: [Wine Quality de UCI](https://archive.ics.uci.edu/dataset/186/wine+quality),
Cortez, P., Cerdeira, A., Almeida, F., Matos, T. y Reis, J. (2009),
[DOI 10.24432/C56S3T](https://doi.org/10.24432/C56S3T), licencia CC BY 4.0.

La copia publicada procede del archivo aportado por el alumno. No se presenta
como una descarga directa de UCI realizada desde el entorno de trabajo.

Tamaño: 84.199 bytes. SHA-256:

```text
4a402cf041b025d4566d954c3b9ba8635a3a8a01e039005d97d6a710278cf05e
```
