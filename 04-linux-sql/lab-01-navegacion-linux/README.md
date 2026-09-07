# LAB-01 · Navegación y Administración Básica en Linux

## Módulo

**Módulo 4:** Tools of the Trade: Linux y SQL

## Objetivo

Aplicar comandos fundamentales de Linux para navegar por el sistema de archivos, crear directorios, administrar archivos y organizar evidencias utilizando la terminal.

## Escenario

Como analista de ciberseguridad, recibí acceso a un entorno Linux para crear una estructura de trabajo destinada al almacenamiento de evidencias digitales. Todo el procedimiento fue realizado desde la terminal Bash.

## Herramientas utilizadas

- Linux
- Terminal Bash

---

## Procedimiento y evidencia

### Paso 1. Verificación del entorno

Se verificó el directorio de trabajo y se inspeccionó el contenido del sistema antes de iniciar el laboratorio.

#### Comandos ejecutados

```bash
pwd
ls -la
mkdir laboratorio_linux
cd laboratorio_linux
pwd
mkdir evidencias
touch evidencias_01.txt
touch evidencias_02.txt
ls -la
```

#### Evidencia

<img width="980" height="797" alt="Captura de pantalla 2026-09-07 155749" src="https://github.com/user-attachments/assets/34169e9a-7374-4e94-8574-5aaa56540126" />


---

### Paso 2. Organización de evidencias

Se movió un archivo al directorio de evidencias y posteriormente se creó una copia para simular la preservación de información durante una investigación.

#### Comandos ejecutados

```bash
mv evidencias_01.txt evidencias/
cp evidencias_02.txt evidencias/copia_evidencia.txt
ls -R
```

#### Evidencia

<img width="815" height="252" alt="Captura de pantalla 2026-09-07 160141" src="https://github.com/user-attachments/assets/5cc5870a-183f-4c57-a2cd-2b34f300058c" />


---

## Estructura obtenida

```text
laboratorio_linux
├── evidencias
│   ├── copia_evidencia.txt
│   └── evidencias_01.txt
└── evidencias_02.txt
```

---

## Análisis

Durante el laboratorio se comprobó la importancia de la navegación y administración de archivos en Linux para organizar información de manera estructurada. La utilización de los comandos `mkdir`, `touch`, `mv`, `cp` y `ls -R` permitió crear un entorno de trabajo reproducible, organizar evidencias digitales y verificar la integridad de la estructura creada desde la terminal.

---

## Competencias desarrolladas

- Navegación en Linux
- Gestión de directorios y archivos
- Bash básico
- Organización de evidencias digitales
- Documentación técnica

---

## Conclusión

La administración de archivos desde la terminal constituye una habilidad esencial para analistas SOC y profesionales de ciberseguridad, ya que permite gestionar información y evidencias de forma eficiente en entornos Linux sin depender de interfaces gráficas.
