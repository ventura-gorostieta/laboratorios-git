# Mini Laboratorio 2: Ramas y Fusiones (Merge)

**Objetivos:**

- Manejo de ramas.
- Fusionar cambios de una rama a otra.

### Ejercicio 1: Crear y Listar Ramas
**Instrucciones:**
1. Abre tu terminal y navega al directorio de un repositorio Git existente.
2. Lista las ramas existentes en tu repositorio con:
   ```bash
   git branch
   ```
3. Crea una nueva rama llamada `feature-x usando`
```bash
git branch feature-x
```
4. Verifica que la rama se ha creado correctamente listando nuevamente las ramas:
```bash
git branch
```

### Ejercicio 2: Cambia entre ramas
1. Cambia a la nueva rama
```bash
git checkout feature-x
```
3. Confirma que estás ahora en la nueva rama con:
```bash
git branch
```
Deberías ver un asterisco (*) al lado de feature-x, indicando que es la rama activa.

### Ejercicio 3: Modificar y Confirmar Cambios en la Rama
**instrucciones**
1. Mientras estés en la rama feature-x, crea un nuevo archivo llamado test.txt y añade algún contenido.
2. Añade el archivo al área de preparación con
```bash
git add test.txt
```
5. Usa el comando commit para confirmar el cambio
```bash
git commit -m "Añadiendo test.txt a feature-x"
```

### Ejercicio 4: Fusionar Ramas (merge)
1. Cambia de regreso a la rama principal (generalmente main o master):
```bash
git checkout main
```

2. Fusiona (merge) la rama feature-x en la rama principal con:
```bash
git merge feature-x
```

3. Verifica que los cambios se han integrado viendo el historial de commits:
```bash
git log
```

4. Usa el comando push para enviar tus cambios a tu remote/origin en la rama main
```bash
git push origin main
```

### Ejercicio 5: Eliminar Ramas (branches)
**instrucciones**
1. Una vez fusionada la rama y confirmado que todo está correcto, puedes eliminar la rama feature-x con:
```bash
git branch -d feature-x
```

## Conclusion
```text
Este mini laboratorio proporciona una forma estructurada y clara de aprender sobre el manejo de ramas en Git.
```