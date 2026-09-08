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

![Permisos iniciales](01-permisos-iniciales.png)

---

### Paso 2. Restringir el acceso al archivo

#### Comandos ejecutados

```bash
chmod 600 credenciales.txt
ls -l
```

#### Evidencia

![Permisos 600](02-permisos-600.png)

---

### Paso 3. Proteger un directorio

#### Comandos ejecutados

```bash
mkdir documentos
chmod 700 documentos
ls -ld documentos
```

#### Evidencia

![Directorio protegido](03-directorio-protegido.png)

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
