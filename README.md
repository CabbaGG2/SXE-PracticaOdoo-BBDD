# Instalación del servico Odoo, PgAdmin y respaldo de base de datos de Odoo.

Realizamos los pasos de instalación y puesta en marcha vistos en prácticas anteriores.

 <br><br>
  ![PyCharm_plugins](imagenes/1.png)

 <br><br>
  ![PyCharm_plugins](imagenes/2.png)

 <br><br>
  ![PyCharm_plugins](imagenes/3.png)

## Realización de los apartados:

<details><summary><h3>Apartado 1</h3></summary>
  
  - Hacemos click derecho en las tablas ➡ Create ➡ Table.. 
  <br><br>
  ![PyCharm_plugins](imagenes/4.png)
  <br><br>
  - Nombramos la tabla en el espacio "Name" como "EmpresasFCT"
  <br><br>
  ![PyCharm_plugins](imagenes/5.png)
  - Vamos agregando las tablas de una en una con su nombre y los parametros solicitados para ellas y pinchamos "Save".
  <br><br>
  ![PyCharm_plugins](imagenes/6.png)
  - En la pestaña "SQL" podemos ver como se genera la sentencia SQL para insertar la tabla con sus respectivas columnas.
  <br><br>
  ![PyCharm_plugins](imagenes/7.png)
  <br><br>
  - Sentencia SQL:
     ```bash
    CREATE TABLE IF NOT EXISTS public."EmpresasFCT"
    (
    "idEmpresa" integer NOT NULL DEFAULT nextval('"EmpresasFCT_idEmpresa_seq"'::regclass),
    nombre character varying(40) COLLATE pg_catalog."default" NOT NULL,
    "quiereAlumnos" boolean,
    "numAlumnos" integer,
    "fechaContacto" date,
    CONSTRAINT "EmpresasFCT_pkey" PRIMARY KEY ("idEmpresa")
    )
    ```
  
</details>