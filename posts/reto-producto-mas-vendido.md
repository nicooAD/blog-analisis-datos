# 🧩 Reto SQL: ¿Cuál es el producto más vendido?

> Fecha: 28 de abril de 2025  
> Autora: Nicolle Explora Datos 🦋

---

## 🎯 Enunciado del reto

Imagina que tienes una tabla llamada `ventas` que guarda la información de los productos vendidos.

La estructura de la tabla es:

| id_venta | producto   | cantidad |
|----------|------------|----------|
| 1        | Laptop     | 2        |
| 2        | Smartphone | 5        |
| 3        | Laptop     | 1        |
| 4        | Tablet     | 3        |
| 5        | Smartphone | 2        |

Tu misión es:  
**Encontrar el producto que ha vendido la mayor cantidad de unidades en total.**

---

## 🔍 ¿Qué debes usar?

- `SELECT`
- `SUM()`
- `GROUP BY`
- `ORDER BY`
- `LIMIT` (opcional)

---

## 💡 Pistas

- Usa `GROUP BY` para agrupar las ventas por producto.
- Usa `SUM(cantidad)` para obtener la cantidad total vendida de cada producto.
- Usa `ORDER BY` para ordenar de mayor a menor.
- Usa `LIMIT 1` si quieres obtener solo el más vendido.

---

## 📝 Solución esperada

Aquí tienes una posible consulta:

```sql
SELECT producto, SUM(cantidad) AS total_vendido
FROM ventas
GROUP BY producto
ORDER BY total_vendido DESC
LIMIT 1;
