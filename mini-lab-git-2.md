# Mini Laboratorio 2: Ramas y Fusiones (Merge)

**Objetivos:**

- Crear y cambiar entre ramas.
- Fusionar cambios de una rama a otra.

**Instrucciones:**

1. Crear una nueva rama
```bash
git branch mi-nueva-rama
```
2. Cambia a la nueva rama
```bash
git checkout mi-nueva-rama
```
3. Realiza cambios y agregalos con el comando add.

4. Cambia de regreso a la rama principal (main/master):
```bash
git checkout main
```
5. Fusiona (merge) la nueva rama con la principal
```bash
git merge mi-nueva-rama
```