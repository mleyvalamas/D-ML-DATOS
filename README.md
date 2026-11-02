# D-ML-DATOS
Datos para curso de ML

## Archivo publicado

[04-Fichero_para_EJERCICIO_3.json](04-Fichero_para_EJERCICIO_3.json) contiene los datos facilitados para el ejercicio de lectura
de JSON del módulo 3:

- Competición: **English Premier League 2010/11**.
- Partidos: **380**.
- Equipos diferentes: **20**.
- Estructura: un campo `name` y una lista `matches`; los equipos de cada partido
  aparecen en `team1` y `team2`.

La copia se conserva sin modificaciones respecto al archivo proporcionado.

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
