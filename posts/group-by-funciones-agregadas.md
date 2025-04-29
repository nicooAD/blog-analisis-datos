# GROUP BY y funciones agregadas en SQL

> Fecha: 28 de abril de 2025  
> Autora: Nicolle Explora Datos 🦋

---

## 🔍 Introducción

Cuando trabajamos con bases de datos, a menudo queremos **agrupar datos** y **realizar cálculos** como sumas, promedios o conteos.  
Para eso usamos **GROUP BY** junto con **funciones agregadas** como `SUM()`, `AVG()`, `COUNT()`, `MIN()` y `MAX()`.

---

## 📘 Conceptos clave

- **GROUP BY**: Agrupa los datos que tienen los mismos valores en columnas específicas.
- **Funciones agregadas**:
  - `SUM()`: Suma los valores de una columna.
  - `AVG()`: Calcula el promedio.
  - `COUNT()`: Cuenta el número de filas.
  - `MIN()`: Devuelve el valor mínimo.
  - `MAX()`: Devuelve el valor máximo.

---

## 💻 Ejemplo práctico

Sigamos con la tabla `empleados`:

| id_empleado | nombre | departamento | salario |
|-------------|--------|--------------|---------|
| 1           | Ana    | Ventas       | 2500    |
| 2           | Luis   | TI           | 3200    |
| 3           | María  | Marketing    | 2800    |
| 4           | José   | Ventas       | 2600    |

---

### 🔹 Consulta 1: ¿Cuánto ganan en total por departamento?

```sql
SELECT departamento, SUM(salario) AS salario_total
FROM empleados
GROUP BY departamento;
