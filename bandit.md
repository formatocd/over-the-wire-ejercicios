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

