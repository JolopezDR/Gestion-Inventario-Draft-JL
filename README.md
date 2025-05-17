# Gestion-Inventario-Draft-JL
Caso Propuesto.  La Empresa XX necesita la creacion de un sistema de inventario que permita registrar, analizar y reportar indicadores logisticos diarios que ofrezcan a los analistas y gerentes la oportunidad de de monitorear el desempeño operativo y reducir el impacto economico del inventario

📦 Proyecto: Sistema de Gestión de Inventarios - Empresa XX
1. ✅ Objetivos del Sistema
   
•	Automatizar el control de entradas y salidas de productos en el almacén.

•	Mantener información actualizada sobre niveles de stock.

•	Mejorar la trazabilidad y reducción de pérdidas por vencimiento, obsolescencia o errores.

•	Generar alertas por bajo inventario o vencimiento próximo.

•	Facilitar reportes e indicadores clave para la toma de decisiones logísticas.
________________________________________
2. 🔑 Entidades Clave a Proponer
   
Entidad	Descripción

Producto	Representa los ítems almacenados.
ID
Nombre
Descripcion
Precio

Categoría	Clasificación de los productos (Ej. electrónicos, alimentos).
ID
Nombre

Proveedor	Datos del proveedor del producto.
ID
Nombre
Contacto
Telefono
Localizacion

Entrada	Registro de ingreso de productos al almacén.
ID
Producto ID
Ubicacion Temporal
Fecha de Registro
Fecha de Expiracion Producto 
Cantidad

Salida	Registro de salida de productos (ventas, traspasos).
ID
Producto ID
Tipo de Salida (Ventas,Traspaso)
Ubicacion de Salida
Usuario 

Ubicación	Espacio físico dentro del almacén (estantería, zona, etc.).
ID
Almacen
Localidad
Estanteria

Usuario	Persona que opera el sistema.
ID
Nombre
Responsabilidad
Correo Electronico
Numero de Telefono

Inventario	Estado actual de existencias por producto.
________________________________________
3. 📜 Reglas del Almacén
   
•	Todo producto debe tener una categoría y un proveedor asignado.

•	No se puede registrar una salida si no hay stock suficiente.

•	Se deben registrar las fechas de entrada y vencimiento si aplica.

•	Cada movimiento (entrada/salida) debe tener un responsable (usuario).

•	Se debe asignar una ubicación física a cada producto.

•	Se genera una alerta automática cuando el stock llega al nivel mínimo configurado.
________________________________________
4. 📈 Ejemplos de Indicadores (KPIs)
   
Indicador	Fórmula / Fuente de Datos

Nivel de Stock Promedio	Promedio de unidades por producto

Tasa de Rotación de Inventario	Salidas ÷ Stock promedio

Días de Inventario Disponible	Stock actual ÷ Salida diaria promedio

Porcentaje de Productos Vencidos	(Productos vencidos ÷ Total productos) × 100

Alertas de Bajo Inventario	Número de productos por debajo del mínimo
________________________________________
5. 🔍 Consultas Comunes
   
•	¿Cuáles productos están por debajo del nivel mínimo?

•	¿Qué productos vencen en los próximos 30 días?

•	¿Cuántas entradas/salidas hubo en el último mes?

•	¿Cuál es el historial de movimiento de un producto específico?

•	¿Cuáles son los productos con mayor/menor rotación?
  
