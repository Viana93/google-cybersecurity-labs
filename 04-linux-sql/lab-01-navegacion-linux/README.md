# LAB-01 · Navegación y Administración Básica en Linux

## Módulo

**Módulo 4:** Tools of the Trade: Linux y SQL

## Objetivo

Utilizar la terminal de Linux para navegar por el sistema de archivos, identificar directorios y administrar archivos mediante comandos básicos.

## Escenario

Como analista de ciberseguridad, recibes acceso a un servidor Linux para revisar archivos de configuración y registros del sistema. Antes de realizar cualquier análisis, debes localizar directorios, verificar la ubicación actual y listar el contenido disponible.

## Comandos utilizados

| Comando | Función |
|----------|---------|
| `pwd` | Muestra el directorio actual. |
| `ls` | Lista el contenido de un directorio. |
| `ls -la` | Muestra archivos ocultos y permisos. |
| `cd` | Cambia de directorio. |
| `mkdir` | Crea un directorio. |
| `touch` | Crea un archivo vacío. |
| `cp` | Copia archivos. |
| `mv` | Mueve o renombra archivos. |
| `rm` | Elimina archivos. |

## Procedimiento

1. Verificar la ubicación actual con `pwd`.
2. Listar el contenido del directorio utilizando `ls -la`.
3. Crear una carpeta llamada `evidencias`.
4. Crear un archivo de prueba dentro de la carpeta.
5. Renombrar el archivo y verificar el resultado.

## Evidencia esperada

```bash
pwd
ls -la
mkdir evidencias
cd evidencias
touch reporte.txt
mv reporte.txt evidencia.txt
ls -la
```

## Análisis

La navegación eficiente dentro de Linux permite localizar rápidamente archivos de configuración, registros y evidencias digitales. El uso de `ls -la` facilita identificar permisos, propietarios y archivos ocultos, información esencial durante actividades de análisis forense y administración de servidores.

## Conclusión

Los comandos básicos de navegación constituyen la base del trabajo diario de un analista de ciberseguridad en entornos Linux y permiten administrar de forma segura la información del sistema.
