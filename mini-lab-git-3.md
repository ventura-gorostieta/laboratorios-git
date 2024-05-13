# Mini Laboratorio: Resolución de Conflictos en Git

## Objetivos
- Aprender a resolver conflictos que surgen al fusionar ramas.
- Comprender la importancia de la comunicación y la coordinación en un entorno de equipo.

## Pre-requisitos
- Tener Git instalado.
- Acceso a una terminal o línea de comandos.
- Un repositorio Git con al menos una rama adicional a la principal.

## Ejercicios

### Ejercicio 1: Crear un Conflicto
**Instrucciones:**
1. Asegúrate de estar en la rama principal (por ejemplo, `main`):
   ```bash
   git checkout main
   ```
2. Crea y cambia a una nueva rama llamada conflict-branch:
```bash
git checkout -b conflict-branch
```

3. En la nueva rama, abre un archivo que también existe en la rama principal y realiza algunos cambios significativos.

4. Añade y confirma los cambios

```bash
git add .
git commit -m "Cambios en conflict-branch que causarán conflicto"
```

5. Cambia de regreso a la rama principal
```bash
git checkout main
```

6. Modifica el mismo archivo que antes, pero cambia diferentes partes del contenido o el mismo contenido de manera diferente.
7. Añade y confirma estos cambios:
```bash
git add .
git commit -m "Cambios en main que causarán conflicto"
```

### Ejercicio 2: Resolver el Conflicto
**INSTRUCCIONES**

1. Asegúrate de estar en la rama principal (main). Es esencial estar en esta rama antes de intentar fusionar y resolver cualquier conflicto:
```bash
git checkout main
```
2. Intenta fusionar conflict-branch en la rama principal:
```bash
git merge conflict-branch
```
3. Git debería indicar que hay un conflicto. Abre el archivo conflictivo y verás las secciones marcadas donde Git no puede resolver automáticamente el conflicto.
4. Edita el archivo para resolver el conflicto. Esto puede involucrar elegir una versión de las modificaciones, combinar ambas, o reescribir la sección conflictiva.
5. Una vez resuelto el conflicto, añade el archivo al área de preparación para indicar que el conflicto ha sido resuelto:
```bash
git add <nombre-del-archivo>
```
6. Completa la fusión con un commit de fusión, que Git te pedirá que hagas:
```bash
git commit
```
Esto abrirá un editor para que ingreses un mensaje de commit para el merge. Guarda y cierra el editor para completar el commit.
7. Verifica que la fusión se haya completado correctamente y que no haya más conflictos:
```bash
git log
```

## Conclusion
En este laboratorio, aprendiste cómo manejar conflictos en Git, una habilidad esencial cuando se trabaja con más personas en el mismo conjunto de archivos. Recordar siempre estar en la rama correcta al resolver conflictos es crucial para mantener un flujo de trabajo eficiente y claro.