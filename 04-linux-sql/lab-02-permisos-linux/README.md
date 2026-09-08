# LAB-02 · Gestión de Permisos en Linux

## Módulo

**Módulo 4:** Tools of the Trade: Linux y SQL

## Objetivo

Aplicar permisos sobre archivos y directorios utilizando `chmod` para proteger información sensible mediante el principio de mínimo privilegio.

## Escenario

Como analista de ciberseguridad, debo restringir el acceso a un archivo que contiene credenciales y proteger un directorio donde se almacenan documentos sensibles.

## Herramientas utilizadas

- Linux
- Terminal Bash

---

## Procedimiento y evidencia

### Paso 1. Crear el entorno de trabajo

#### Comandos ejecutados

```bash
mkdir permisos_lab
cd permisos_lab
touch credenciales.txt
ls -l
```

#### Evidencia

<img width="665" height="608" alt="01-permisos-iniciales png" src="https://github.com/user-attachments/assets/165d1267-d59e-41e8-9a0f-b3d98896880f" />

---

### Paso 2. Restringir el acceso al archivo

#### Comandos ejecutados

```bash
chmod 600 credenciales.txt
ls -l
```

#### Evidencia

<img width="653" height="546" alt="02-permisos-600 png" src="https://github.com/user-attachments/assets/f4475e82-6d45-4f14-897a-9d0356b0c5b3" />

---

### Paso 3. Proteger un directorio

#### Comandos ejecutados

```bash
mkdir documentos
chmod 700 documentos
ls -ld documentos
```

#### Evidencia

<img width="727" height="711" alt="03-directorio-protegido" src="https://github.com/user-attachments/assets/cb7eb9a3-143e-46f5-9d77-8ebd8890569b" />

---

## Análisis

Los permisos en Linux controlan qué usuarios pueden leer, escribir o ejecutar archivos y directorios. Durante este laboratorio se aplicó el principio de mínimo privilegio, limitando el acceso al propietario mediante permisos `600` para archivos y `700` para directorios.

## Conceptos aplicados

| Permiso | Significado |
|---------|-------------|
| 700 | Acceso total para el propietario |
| 600 | Lectura y escritura únicamente para el propietario |
| 755 | Acceso público de lectura y ejecución |
| 644 | Lectura para otros usuarios y escritura solo para el propietario |

## Conclusión

La correcta configuración de permisos constituye uno de los controles de seguridad más importantes en sistemas Linux, ya que reduce la posibilidad de accesos no autorizados a información sensible.
