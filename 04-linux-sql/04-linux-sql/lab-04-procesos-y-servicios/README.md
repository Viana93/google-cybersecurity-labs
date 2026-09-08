# LAB-04 · Inspección de Procesos y Servicios en Linux

## Módulo

**Módulo 4:** Tools of the Trade: Linux y SQL

## Objetivo

Inspeccionar los procesos activos del sistema e identificar servicios en ejecución utilizando herramientas nativas de Linux.

## Escenario

Como analista de ciberseguridad, debo revisar qué procesos se encuentran ejecutándose en un servidor Linux para detectar actividades inusuales y verificar el estado de los servicios del sistema.

## Herramientas utilizadas

- Linux
- Terminal Bash

---

## Procedimiento y evidencia

### Paso 1. Visualizar procesos activos

#### Comandos ejecutados

```bash
ps aux
```

#### Evidencia

<img width="860" height="877" alt="01-ps-aux" src="https://github.com/user-attachments/assets/4533fac7-72e1-4381-a29b-ddd92aeea521" />

---

### Paso 2. Identificar un proceso específico

#### Comandos ejecutados

```bash
pgrep bash
ps -fp $(pgrep bash)
```

#### Evidencia

<img width="905" height="445" alt="02-pgrep-bash" src="https://github.com/user-attachments/assets/00489e15-1589-4e49-a176-c428deafd110" />

---

### Paso 3. Verificar servicios del sistema

#### Comandos ejecutados

```bash
systemctl list-units --type=service --state=running
```

#### Evidencia

<img width="932" height="546" alt="03-servicios-running" src="https://github.com/user-attachments/assets/74cf61d8-bfde-4bd9-ab81-e8326c338c4e" />

---

## Análisis

El comando `ps aux` permite visualizar todos los procesos activos del sistema, mientras que `pgrep` facilita localizar procesos específicos por nombre. Finalmente, `systemctl` permite verificar qué servicios se encuentran en ejecución, información esencial durante actividades de monitoreo y respuesta a incidentes.

## Competencias desarrolladas

- Monitoreo de procesos
- Identificación de servicios
- Uso de `ps`
- Uso de `pgrep`
- Administración básica con `systemctl`

## Conclusión

La inspección de procesos y servicios permite identificar comportamientos anómalos y constituye una habilidad fundamental para el análisis de sistemas Linux en entornos SOC.
