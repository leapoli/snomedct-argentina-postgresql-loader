# snomedct-argentina-postgresql-loader

Conjunto de scripts para cargar los archivos de la distribución para Argentina de SNOMED-CT:

* create-database-postgres.sql
* environment-postgresql.sql
* load_release-postgresql.sh

Para poder crear el entorno y el esquema, e insertar los datos en la base; es necesario bajar el archivo comprimido de distribución en la misma carpeta que los scripts.
Luego ejecutar el siguiente comando (ejemplo para la distribución FULL):

`bash load_release-postgresql.sh SnomedCT_Argentina-EditionRelease_PRODUCTION_20191130T120000Z_v2.zip snomedct FULL`

El programa pedirá nombre de usuario de base de datos (por default **postgres**) y puerto (por default **5432**) 