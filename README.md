## Automatización de Pruebas:
La automatización de pruebas es una técnica de pruebas donde se utilizan scripts y herramientas para controlar la ejecución de las pruebas y la comparación de los resultados reales con los resultados pronosticados, dichas herramientas pueden automatizar algunas tareas repetitivas. Hoy en día existen algunas herramientas de automatización de pruebas, tales como: Selenium, Testim, HeadSpin, etc.

## Descripción:

El presente proyecto trata de un demo configurado para trabajar localmente con [Selenium WebDriver](https://www.npmjs.com/package/selenium-webdriver) y Javascript integrado adicionalmente con [Mocha](https://mochajs.org/) y [mochawesome](https://www.npmjs.com/package/mochawesome) para generar informes de pruebas.

En el ejemplo se han automatizado 2 simples casos de pruebas para testear el aplicativo [TODO](https://lambdatest.github.io/sample-todo-app/).


## Requerimientos:
- Tener instalado NodeJS.
- Configurar localmente el controlador del navegador desde donde vamos a correr nuestros test. En nuestro caso utilizamos el controlador de [Firefox](https://github.com/mozilla/geckodriver/releases/) para el sistema operativo MacOS. Lo descargamos y lo colocamos en un directorio de su elección. Luego actualizamos el sistema con esta ruta, modificando el siguietente archivo:

```
sudo nano /etc/paths/

Agregamos una nueva línea con la ruta del controlador.
```

- Modificar el archivo: "package.json" y cambiar los valores de las banderas: << reportDir>> y << reportFilename >> colocar el nombre del directorio donde se va a almacenar los reportes generados de la ejecución de las pruebas y el nombre del archivo del reporte en formato HTML respectivamente.


### Instalamos las dependencias:
```
npm install
```

### Ejecutamos los tests:
```
npm test
```
