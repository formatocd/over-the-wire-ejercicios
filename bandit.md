# Over The Wire - Niveles Bandit
## Level 1 -> Level 2
**Ficheros con guión (Dashed filenames)**

Son ficheros cuyo primer carácter es un guión (`-`). Para realizar una operación sobre él hay incluir dos guiones (`--`) inmediatamente después del comando.

**Ejemplos**

- Crear: `touch -- -file.txt`
- Leer: `cat -- -file.txt` o `cat < -file.txt`
- Eliminar: `rm -- -file.txt`
- List: `ls -l -- -file.txt`
- Edit: `vim -- -file.txt`

## Level 2 -> Level 3

Los espacios en los comandos de consola representan la separación de opciones del mismo. De modo que no puedes accederse al fichero de este modo:

```bash
vim fichero con espacios.txt
```
El comando del ejemplo no considera un solo fichero para el comando `vim` sino que son `fichero`, `con` y `espacios.txt`. Para que los comandos tomen los espacios como carácter de cadena, existen dos alternativas:

- Escapando los espacios: `vim fichero\ con\ espacios.txt`
- Con comillas: `vim "fichero con espacios.txt"`

En el caso de que el fichero empiece con guión, se combina con el caso anterior:
```bash
cat -- "-fichero con espacios.txt"
```
