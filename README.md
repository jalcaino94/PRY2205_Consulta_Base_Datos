# PRY2205 - Consulta de Bases de Datos | Experiencia 2 - Semana 5
## Actividad Formativa: Utilizando Subconsultas para Resolver Requerimientos

Repositorio correspondiente al encargo semanal de la asignatura **Consulta de Bases de Datos**, enfocado en el caso de estudio **FinanCorp** sobre gestión de cobranzas y productos financieros.

### Integrantes (Dupla)
* **Integrante 1:** Oscar Fuente R.
* **Integrante 2:** Juan Sereño A.

---

### Contenido del Repositorio
* `PRY2205_Exp2_S5_Actividad.sql`: Script SQL ejecutado en Oracle SQL Developer / Oracle Cloud que contiene la solución completa a los requerimientos solicitados.

---

### Resumen de Casos Resueltos
1. **Caso 1 – Listado de Clientes:**
   * Identificación de clientes trabajadores dependientes con profesión `CONTADOR` o `VENDEDOR`.
   * Filtrado mediante **subconsulta de una fila** comparando el año de inscripción contra el promedio redondeado (`ROUND(AVG(...))`) de inscripción de todos los clientes.
   * Formateo de salida con `TO_CHAR`, `INITCAP`, `UPPER`, `TRIM` y ordenamiento ascendente por RUT.

2. **Caso 2 – Aumento de Crédito:**
   * Creación dinámica de la tabla `CLIENTES_CUPOS_COMPRA` mediante `CREATE TABLE ... AS SELECT`.
   * Cálculo paramétrico de edad actual (`SYSDATE`) y filtrado de cupos disponibles de compra iguales o superiores al máximo cupo registrado el año anterior mediante subconsulta.
   * Ordenamiento ascendente por edad.
