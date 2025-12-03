# FDS-2025-2-CC52

## Objetivo del proyecto
Desarrollar un modelo de *scoring* que estime la **probabilidad de que un cliente compre una bicicleta** en la empresa Peru_bike, utilizando técnicas de minería de datos (regresión logística) sobre información demográfica y de comportamiento. El modelo sirve como herramienta para **priorizar clientes** en campañas comerciales y de marketing.

## Nombre de los alumnos participantes
- Renzo Gabriel Gutierrez Fernandez

*(Proyecto desarrollado de forma individual, asumiendo los roles de Business Sponsor, Data Scientist, Data Engineer y Data Analyst.)*

## Breve descripción del conjunto de datos
Se utiliza el archivo `bike_buyers.csv`, que contiene información de **1 000 clientes** de Peru_bike, incluyendo:

- Datos demográficos: edad, género, estado civil, nivel educativo, región.
- Datos socioeconómicos: ingreso anual, número de hijos, número de vehículos, propiedad de vivienda.
- Datos de contexto: distancia de viaje al trabajo.
- Variable objetivo: `Purchased Bike` (indica si el cliente compró o no una bicicleta).

En el repositorio también se puede adjuntar o referenciar el **PDF de enunciado/objetivos** del proyecto para mayor contexto.

## Conclusiones
- Los clientes que compran bicicleta presentan, en promedio, **ingresos ligeramente mayores** y suelen estar asociados a **ocupaciones profesionales o de gestión**, con cierta estabilidad (propiedad de vivienda, más vehículos).
- La **regresión logística** construida ofrece un desempeño **moderado** (accuracy ≈ 63 %, F1 ≈ 0.60, AUC ≈ 0.68), suficiente como **primer modelo de scoring** para priorizar clientes.
- Ajustando el **umbral de decisión** (por ejemplo, a 0.4) se consigue **aumentar el recall de la clase “compra”**, lo que permite identificar más compradores potenciales a costa de algunos falsos positivos, alineado con un uso de marketing.
- El modelo no es perfecto, pero entrega una **ventaja clara frente a seleccionar clientes al azar**, y sienta la base para futuras mejoras (nuevas variables, modelos más complejos, reentrenamiento periódico).

## Licencia de uso
Este proyecto se distribuye bajo la licencia **MIT**.  
