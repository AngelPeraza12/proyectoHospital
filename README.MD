Como se hizo el proyecto paso a paso.


- se crearon las carpetas src y db
- Se crearon las subcarpetas
    SCR
    Folder principal del aplicativo el cual contiene la lógica pertienente de los componentes y sus respectivas conexiones.

    API
    Api contendrá los componentes propios del aplicativo REST de Node 

    config
    Es un directorio que contiene todos los proceso que se encargan de configurar la aplicación a nivel transversal.  

    test
    Son test que pemiten correr los test de cada uno de los componentes.

    app.js
    En este archivo se realiza la inicialización del servicio.

- Se hizo el package.json como punto de inicio se indica que se haga desde "main": "src/app.ts",

-Instalar typescript npm install typescript

-Instalar dependencias tales como:

    express npm install express
    ts-node npm install ts-node --save-dev
    types/express npm install @types/express
    Para desintallar se corre le comando npm uninstall

- Crear un tsconfig por defecto con el comando npx tsc --init, y luego activamos la opción de outDir dentro del archivo y definimos la carpeta que contiene el archivo main (index.ts o app.ts)

Para correr el proyecto desde el main se hace uso del comando npx ts-node src/app.ts.

Para la migraciones se debe instalar la dependecia del ORM llamado knex, donde haremos uso del comando npm install knex knex-cli pg --save-dev

Para leer variables de entorno instalamos la libreria de dotenv npm install dotenv

POSTGRES_URI=postgresql://<usuario_db>:<password_db>@<host_db>:<port_db>/