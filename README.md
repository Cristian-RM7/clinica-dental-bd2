# Sistema de Gestión para Clínica Dental

## Descripción del Proyecto

Sistema de base de datos relacional diseñado para gestionar las operaciones de una clínica dental pequeña. El sistema permitirá registrar pacientes, odontólogos, citas, tratamientos realizados y facturación, automatizando procesos críticos mediante procedimientos almacenados, triggers de auditoría y transacciones para garantizar la integridad de los datos.

## Problema a Resolver

Una clínica dental necesita digitalizar su gestión de citas y tratamientos para:
- Evitar la pérdida de información de pacientes y su historial clínico
- Controlar el inventario de insumos dentales utilizados en cada tratamiento
- Generar facturación automática basada en los servicios prestados
- Registrar auditoría de cambios críticos (cancelaciones, modificaciones de precios)
- Garantizar que operaciones complejas (como registrar una atención completa) se ejecuten de forma atómica (todo o nada)

## Reglas de Negocio Iniciales

1. Un paciente puede tener múltiples citas a lo largo del tiempo
2. Una cita puede incluir varios tratamientos
3. Cada tratamiento tiene un precio base, pero puede variar según el odontólogo
4. Al atender una cita, se debe:
   - Marcar la cita como atendida
   - Registrar los tratamientos aplicados
   - Generar la factura correspondiente
   - Descontar los insumos utilizados del inventario
5. Si alguna parte del proceso falla, toda la operación debe revertirse (transacción)
6. Las cancelaciones de citas deben quedar registradas con fecha, hora y responsable
7. Un odontólogo tiene una especialidad y horario de atención específico

## ️ Tecnologías

- Motor de Base de Datos: MySQL 8.x
- Herramienta de Desarrollo: MySQL Workbench
- Control de Versiones: Git / GitHub
- Lenguaje de Consulta: SQL (DDL, DML, DCL)

## Información del Estudiante

- Nombre: Cristian Ramos Mendoza
- Usuario GitHub: Cristian-RM7
- Materia: Base de Datos II
- Docente: Ing. Nagib Luis Vallejos Mamani
- Semestre: VI Semestre - Ingeniería de Sistemas
- Fecha de inicio: Octubre 2026

## Estado del Proyecto

### Fase 1: Diseño y Modelado
- [x] Definición del tema y reglas de negocio
- [ ] Modelo Entidad-Relación (ERD) Conceptual
- [ ] Modelo Entidad-Relación (ERD) Lógico
- [ ] Modelo Entidad-Relación (ERD) Físico

### Fase 2: Implementación de Base de Datos
- [ ] Scripts DDL (Creación de tablas)
- [ ] Scripts DML (Datos de prueba)
- [ ] Restricciones y validaciones (CHECK, UNIQUE, FOREIGN KEY)

### Fase 3: Consultas Avanzadas
- [ ] Consultas con JOIN (INNER, LEFT)
- [ ] Agregaciones (GROUP BY, HAVING)
- [ ] Subconsultas y expresiones CASE
- [ ] Vistas (VIEW)

### Fase 4: Programación Almacenada
- [ ] Procedimientos almacenados (PROCEDURE)
- [ ] Funciones almacenadas (FUNCTION)
- [ ] Disparadores de auditoría (TRIGGER)

### Fase 5: Transacciones y Seguridad
- [ ] Transacciones (COMMIT/ROLLBACK)
- [ ] Índices y optimización (EXPLAIN)
- [ ] Permisos de usuarios (GRANT/REVOKE)
- [ ] Respaldo y restauración

### Fase 6: Documentación Final
- [ ] README completo con instrucciones
- [ ] Evidencias de pruebas
- [ ] Entrega final en repositorio

## Estructura del Repositorio 

