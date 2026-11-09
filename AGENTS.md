# text-analytics-notes

Material de un curso de análisis de textos: apuntes, notebooks, ejemplos en Python/Scala y recursos en español e inglés.

## Visibilidad y rama

- Público. Es un fork de `Toletum/text-analytics-notes` (remoto `origin`). Rama por defecto: `master`.

## Stack

- Contenido, no hay código de producción: Jupyter notebooks (`.ipynb`), Python (NLTK), Scala (Spark MLlib, exportaciones de Databricks) y Markdown.
- Librerías mencionadas en los apuntes: NLTK (con datos de `nltk.download`), Elasticsearch, Solr, Spark MLlib, Meaningcloud, BeautifulSoup. No hay `requirements.txt` ni `pom.xml`.

## Estructura

- `README.md`: título y descripción del repo.
- `programa.md`: temario del curso y distribución en sesiones.
- `install-notes.md`: instalación de NLTK y de sus datos.
- `NLTK-notes.md`, `recursos.md`, `awesome-*.md`: apuntes y listas de recursos.
- `chunking/`, `tagging/`, `text-classification/`, `text-representation/`: notebooks por tema; `text-representation/tokenization.py` es un script.
- `search/`: notebooks de Elasticsearch, Solr y motores de búsqueda (`index.txt` es el índice).
- `spark/`: ejemplos Scala de Spark (`.scala`) con su exportación `.html`.
- `meaningcloud/`: notebook de análisis con Meaningcloud.
- `img/`: imágenes usadas en los apuntes.
- `.gitignore`: `*.ipynb_checkpoints`, `*.sublime-project`, `*.sublime-workspace`.

## Comandos

- No hay comandos de build, lint ni tests.
- Instalar NLTK y sus datos: ver `install-notes.md` (no verificado en este entorno).
- Ejecutar notebooks: Jupyter (no documentado en el repo).

## Configuración

- No hay variables de entorno ni ficheros de configuración.
- Los notebooks de Spark/Databricks usan rutas tipo `/databricks-datasets/...` que solo existen en Databricks.

## Convenciones para agentes

- El contenido está en español; mantener el idioma de cada fichero.
- No versionar `.ipynb_checkpoints`.
- Al cambiar un notebook, conservar las salidas que sirven de ejemplo y no añadir credenciales (ej. APIs de Meaningcloud).
- Si se toca el temario, mantener `programa.md` y `README.md` sincronizados.

## Estado

- Es un fork: no se ha comparado con el upstream (no verificado).
- `text-representation/tokenization.py` usa sintaxis de Python 2 (`print tokens`) y tiene un TODO sobre un ejemplo en español: no ejecutable en Python 3 tal cual.
- Los `.scala` son exportaciones de Databricks de 2016 (`sqlContext`); no se han probado fuera de Databricks.
- El último commit "Prueba a commitear desde RStudio" no aporta contenido.
- Sin tests ni CI.
