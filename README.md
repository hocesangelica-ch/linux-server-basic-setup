# linux-server-basic-setup

## Objetivo:
Simular un servidor para una pequeña empresa que necesita estabilidad y respaldo de información.

## Tecnologías:
- Ubuntu (WSL)
- Bash
- APT

## Paso 1: Actualización del sistema.

Se realizó la actualización inicial del sistema operativo para asegurar estabilidad y seguridad antes de configurar servicios.

Comandos utilizados:
- apt update
- apt upgrade

## Paso 2: Creación de usuarios y grupos.

Se creó un usuario estándar para simular un empleado del sistema, siguiendo buenas prácticas de seguridad.

Comando utilizado:
- sudo adduser empleado1

Se creó un grupo para simular un departamento de una empresa y asignarlo al usuario. Por último, se comprueba que se creó y asignó correctamente el usuario y grupo:

Comandos utilizados:
- sudo addgroup departamento_contabilidad
- sudo gpasswd -a empleado1 departamento_contabilidad
- sudo cat /etc/group
 
