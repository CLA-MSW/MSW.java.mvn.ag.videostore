# Proyecto - Java VideoStore con Pruebas para Autograding - Maven

**VideoStore** es una App Java desarrollada para gestionar el Punto de Venta de una tienda de renta de Videos.

La tienda ofrece a sus clientes tres tipos de películas:

* REGULAR
* NEW_RELEASE
* CHILDREN

Su equipo ha recibido la última versión de la App, la cual posee varios defectos. 

Se les ha encomendado la tarea de detectar y corregir los mismos y verificar su eliminación mediante un conjunto pruebas unitarias (incluidas). 
Utilice las herramientas y técnicas estudiadas para dar mantenimiento a esta aplicación

## Uso del proyecto con Maven

### Compilar
```
mvn -f app compile
```
### Probar N tests
```
mvn -f app test
```
### Probar 1 test
```
mvn -f app test -Dtest="AppTest#testSingleNewReleaseStatement"
mvn -f app test -Dtest="AppTest#testDualNewReleaseStatement"
mvn -f app test -Dtest="AppTest#testSingleChildrensStatement"
mvn -f app test -Dtest="AppTest#testMultipleRegularStatement"
mvn -f app test -Dtest="AppTest#testRentalStatementFormat"

```
### Ejecutar App
```
java -cp app/target/classes miPrincipal.App
```
### Empacar App
```
mvn -f app package
```
### Limpiar binarios
```
mvn -f app clean
```
## Comandos Git-Cambios y envío a Autograding

### Por cada cambio importante que haga, actualice su historia usando los comandos:
```
git add .
git commit -m "Descripción del cambio"
```
### Envíe sus actualizaciones a GitHub para Autograding con el comando:
```
git push origin main
```
Los comandos anteriores están considerados para un ambiente Linux. [Referencia.](https://www.baeldung.com/junit-run-from-command-line)
