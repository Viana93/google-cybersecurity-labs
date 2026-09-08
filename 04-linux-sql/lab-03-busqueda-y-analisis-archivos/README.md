# LAB-03 · Búsqueda y Análisis de Archivos en Linux

## Módulo

**Módulo 4:** Tools of the Trade: Linux y SQL

## Objetivo

Utilizar comandos de Linux para localizar archivos, buscar contenido y analizar información desde la terminal.

## Escenario

Como analista de ciberseguridad, debo localizar archivos de interés y buscar información específica dentro de ellos durante una revisión inicial de un servidor Linux.

## Herramientas utilizadas

- Linux
- Terminal Bash

---

## Procedimiento y evidencia

### Paso 1. Crear archivos de prueba

#### Comandos ejecutados

```bash
mkdir analisis_archivos
cd analisis_archivos

echo "usuario: paola" > usuarios.txt
echo "rol: administrador" >> usuarios.txt
echo "estado: activo" >> usuarios.txt

ls -l
```

#### Evidencia

<img width="707" height="621" alt="01-archivos-creados" src="https://github.com/user-attachments/assets/dace62b1-897c-49dd-bd82-f46f41fda27e" />

---

### Paso 2. Buscar información dentro del archivo

#### Comandos ejecutados

```bash
cat usuarios.txt
grep "administrador" usuarios.txt
```

#### Evidencia

<img width="637" height="738" alt="02-grep-administrador" src="https://github.com/user-attachments/assets/bb7b6454-54bf-43e4-bfba-8bcc5c54474a" />

---

### Paso 3. Localizar el archivo

#### Comandos ejecutados

```bash
find ~ -name usuarios.txt
```

#### Evidencia

<img width="667" height="807" alt="03-find-usuarios" src="https://github.com/user-attachments/assets/a607a28f-c279-424c-8603-4a9b79464adb" />

---

## Análisis

Los comandos `cat`, `grep` y `find` permiten inspeccionar rápidamente información dentro de un sistema Linux. Durante investigaciones de seguridad son fundamentales para localizar evidencias, identificar configuraciones y buscar indicadores de compromiso.

## Competencias desarrolladas

- Búsqueda de archivos
- Análisis de contenido
- Uso de `grep`
- Uso de `find`
- Investigación en Linux

## Conclusión

La capacidad de localizar y analizar archivos desde la terminal optimiza los procesos de investigación y constituye una habilidad esencial para analistas de ciberseguridad y SOC.
