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

