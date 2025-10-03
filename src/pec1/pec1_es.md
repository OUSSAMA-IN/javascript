# Respuestas a las preguntas teóricas

## Ejercicio T1
**T.1.1
--dev1
git add .
git commit -m "Cambios de Dev1"
git push
--dev2
git pull         # importante
git add .
git commit -m "Cambios de Dev2"
git push
--dev3
git clone <url-del-repo>     #porque todavia no tiene repo local
git add .
git commit -m "Cambios de Dev3"
git push

**T.1.2
Ejemplo de conflicto (misma parte del archivo):si Dev1 y Dev2 modifican la misma línea del archivo styles.css .
dev1
git add .
git commit -m "  color red para  el backgroud"
git push
dev2(sin haber hecho git pull)   #el problema 
git add .
git commit -m "  color azul para el backgroud"
git push
asi git no puede decidir que modificacion tiene que conservar :
---SOLUCION: 
div2  debe hacer :
1:git pull Para traer los cambios del repositorio y ver el conflicto.
2:edita el archivo styles.cs
3:git add .
git commit -m "  color Azul por el back groud"
git push

## Ejercicio T2
*** El commit C6 contiene el contenido combinado de los commits C1, C2 y C5.y también lo que se registre en C6 al momento del merge.
*** El commit C7 contiene el contenido  de los commits C1, C2, C3, C4 y C7.
*** El conflicto puede ocurrir en el commit C8:si se modifica la misma línea de un mismo archivo en los commits C6 y C7.
 ***la solucion:Editas archivos con conflicto manualmente 
