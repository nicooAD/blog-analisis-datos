# SELECT - FROM - WHERE

> Fecha: 22 de abril de 2025  
> Autora: Nicolle Explora Datos 🦋

---

## 🔍 Introducción

En esta entrada exploraremos tres comandos esenciales en SQL: **SELECT**, **FROM** y **WHERE**.  
Son la base de cualquier consulta de bases de datos, permitiéndonos seleccionar datos específicos según nuestras necesidades.

---

## 📘 Conceptos clave

- **SELECT**: Indica las columnas que queremos ver.
- **FROM**: Indica de qué tabla(s) queremos extraer los datos.
- **WHERE**: Permite aplicar condiciones para filtrar los resultados.

---

## 💻 Ejemplo práctico

Supongamos que tenemos una tabla llamada `empleados` con esta estructura:

| id_empleado | nombre   | departamento | salario |
|-------------|----------|--------------|---------|
| 1           | Ana      | Ventas       | 2500    |
| 2           | Luis     | TI           | 3200    |
| 3           | María    | Marketing    | 2800    |
| 4           | José     | Ventas       | 2600    |

---

### 🔹 Consulta 1: Seleccionar todas las columnas

```sql
SELECT * 
FROM empleados;
