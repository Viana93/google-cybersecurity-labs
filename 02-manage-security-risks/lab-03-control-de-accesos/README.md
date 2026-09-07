# LAB-03 · Principio de Mínimo Privilegio y Control de Accesos

## Módulo

**Módulo 2:** Play It Safe: Gestionar los riesgos de seguridad

## Objetivo

Aplicar el principio de mínimo privilegio mediante la asignación de permisos según las responsabilidades de cada usuario dentro de una organización.

## Escenario

Una empresa cuenta con cuatro tipos de usuarios: Administrador de TI, Analista de Recursos Humanos, Asesor Comercial y Cliente. El objetivo es definir el nivel de acceso adecuado para proteger la información y reducir el riesgo de accesos no autorizados.

## Matriz de accesos

| Usuario | Base de datos | Nómina | CRM | Configuración del sistema |
|----------|---------------|---------|-----|---------------------------|
| Administrador de TI | Lectura y escritura | No | No | Completo |
| Recursos Humanos | Lectura | Lectura y escritura | No | No |
| Asesor Comercial | Lectura | No | Lectura y escritura | No |
| Cliente | No | No | Lectura limitada | No |

## Análisis

Cada usuario recibe únicamente los permisos necesarios para desempeñar sus funciones, evitando el acceso innecesario a información sensible.

## Controles implementados

- Control de acceso basado en roles (RBAC).
- Principio de mínimo privilegio.
- Revisión periódica de permisos.
- Registro de actividades de los usuarios.

## Conclusión

Limitar los privilegios de acceso disminuye la superficie de ataque, protege la información crítica y fortalece la seguridad de la organización.
