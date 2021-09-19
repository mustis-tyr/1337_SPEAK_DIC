# 1337_SPEAK_DIC

Este script es una herramienta para creación de diccionarios con leet_speak.

Para poder usar este proyecto es necesario tener instalado y compilado el siguiente software.

 1. **git clone https://github.com/hashcat/maskprocessor.git**
 2. **cd maskprocessor/src && make**
 3. **./mp64.bin**

Una vez instalado el mp64.bin se debe configurar el path del mp64.bin dentro de la variable del script  $path_mp64.

 **path_mp64=~/Tools/maskprocessor/src/mp64.bin**

Ejemplos:

**./1337_SPEAK.sh  [palabra]**

**./1337_SPEAK.sh  banco**

La salida de este script les dará algo como lo siguiente:

**~/Tools/maskprocessor/src/mp64.bin  -1 cCnN  -2 08bBoO  -3 @4aA  ?2?3?1?1?2 | egrep "^[b,B,8][a,A,@,4][N,n][C,c][o,O,0]"**

El cual nos generará la regla para poder crear un diccionario con la herramienta mp64.bin junto con la expresión regular que se necesita para poder traer solo lo que requerimos.

