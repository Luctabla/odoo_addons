### Como crear una base de datos en odoo local y levantar el backup un una base de datos managed en Digital Ocean

dentro del contenedor de postgres de odoo correr
/usr/bin/pg_dump --file "/backups" --host "localhost" --port "5432" --username "odoo" --no-password --verbose --format=c --blobs --section=data "local"
/usr/bin/pg_dump --file "/backups/postgres_bak" --host "localhost" --port "5432" --username "odoo" --no-password --verbose --format=c --blobs "postgres"
