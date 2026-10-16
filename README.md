# PDF Catalog

Aplicacion FastAPI que muestra un catalogo de productos y permite descargarlo
como PDF mediante xhtml2pdf.

## Rutas

- `/`: pagina inicial.
- `/report`: vista previa del catalogo.
- `/report/pdf`: descarga del catalogo en PDF.

## Despliegue en Vercel

Importa este repositorio en Vercel o despliegalo con la CLI de Vercel. El runtime
detecta la aplicacion FastAPI en `main.py`, usa Python 3.14, indicado en
`.python-version`, y las tres dependencias fijadas en `requirements.txt` y
sincronizadas con `pyproject.toml` y `uv.lock`.
`vercel.json` incluye las plantillas HTML necesarias para atender las rutas y
generar el PDF.

Las dependencias de ejecucion se mantienen limitadas a las tres bibliotecas
declaradas en `requirements.txt`.
