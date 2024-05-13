# Mini Laboratorio 1: Configuración Básica y Clonación de Repositorio

**Objetivos:**

- Configurar Git (nombre de usuario y correo).
- Clonar un repositorio existente.

**Instrucciones:**

1. Instala Git si aún no está instalado. (Checar si no lo tienes con Soporte Tecnico de FEMSA)
2. Configura tu nombre de usuario y correo electrónico con los comandos:
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu.email@example.com"
```
3. [Forkea repositorio](https://github.com/gigabyte-codespace/laboratorios-git.git)

4. Clona el repositorio que se FORKeo en el punto 3 
```bash
git clone https://github.com/tu-nombre-de-usuario/laboratorios-git.git
```
5. Abrir la carpeta donde clonaste el repositorio y crear un archivo llamado **tu-nombre-usuario.info**
6. Agregarlo usado el comando git add
7. Usar el comando git commit para agregarlo a la area de staging
8. Usar el comando git push para que sea agregado a tu repositorio forkeado del punto 3
