# Modelo de Datos

El modelo está diseñado utilizando un **esquema tipo estrella (Star Schema)**, una de las arquitecturas más utilizadas en sistemas de Business Intelligence por su eficiencia y claridad analítica.

### 🔹 Tabla de Hechos
**FactVentas**  
Contiene las transacciones del negocio e incluye métricas como ventas, costos, márgenes y tiempos de proceso.

### 🔹 Tablas Dimensión
Las dimensiones describen el contexto de cada transacción:

- Cliente  
- Producto  
- Vendedor  
- Territorio  
- Método de Pago  

Estas tablas permiten segmentar y analizar la información desde distintas perspectivas de negocio.

### 🔹 Tabla de Fechas
- Calendario  
Tabla dedicada para análisis temporal, que permite realizar comparaciones por año, mes, trimestre y otros periodos de tiempo.

### 🔹 Tabla de Medidas
- Medidas  
Tabla auxiliar utilizada para organizar y centralizar las métricas creadas con **DAX**, facilitando el mantenimiento del modelo y mejorando la claridad del proyecto.

---

## Beneficios del Diseño

Este enfoque permite:

- **Escalabilidad** del modelo  
- **Mejores tiempos de cálculo**  
- **Análisis temporal consistente**  
- **Mayor claridad estructural**  
- **Separación lógica entre datos y métricas**