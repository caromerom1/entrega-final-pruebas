# Entrega final pruebas

## Validación de datos

Para ejecutar las pruebas de validación de datos, correr el siguiente comando:

```console
npm run dataValidationTests
```

## VRT

Para ejecutar las pruebas VRT, correr el siguiente comando: 

```console
npm run vrtTests
```

Seguido de esto, renombrar los archivos obtenidos en la carpeta `vrt/cypress/screenshots` para que coincidan entre las versiones de ghost para la posterior ejecución de resemblejs.

Luego, mover estos archivos renombrados en la carpeta `vrt/cypress/resembleJS/scenarios` en las carpetas `v3` y `v5` correspondiente a la versión de los pantallazos.

Finalmente, para ejecutar resemblejs, correr el siguiente comando:

```console
npm run resemble:run
```

Abrir el archivo `report.html` ubicado en la carpeta `reports/<fecha_del_reporte>`

## Recognition

Para ejecutar las pruebas de reconocimiento, es necesario crear una cuenta en ghost para la versión 5.47.1

Credenciales esperadas de la cuenta

> test@test.com
> Sec.ure@Pas.sw0rd*158

Seguido de esto, es necesario cambiar a los directorios de cada herramienta `(monkey-cypress/RIPuppetCoursera)` y ejecutar el siguiente comando para ambas herramientas

```console
npm install
```

### monkey-cypress

Estando en la carpeta `monkey-cypress`, ejecutar el comando

```console
npm run monkey
```

### RIPuppetCoursera

Estando en la carpeta `RIPuppetCoursera`, ejecutar el comando
***Nota: es importante tener instalados previamente los navegadores Chromium y Firefox***

```console
node index.js
```

Seguido de esto, para ver el informe de resultados, correr el siguiente comando:

```console
npx http-server results
```

Con el comando anterior se ejecutará un servidor desde el que se puede acceder mediante la hora de ejecución a los reportes ingresando a la carpeta. Seguido de esto, se selecciona el navegador del cual se quiera observar el reporte `Chromium/Firefox` y se abre el arcivo `report.html`.

Para ver el informe, se selecciona uno de los puntos del grafo que se observa y puede observarse a detalle cada punto del grafo

