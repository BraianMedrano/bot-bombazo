# Prompt personalizado para la IA:  
Henko utiliza una IA independiente para realizar búsquedas en la base de datos de esta integración. Podés editar las instrucciones que le darás a esta IA para que realice las búsquedas. Recordá que esta IA no tiene contexto de las instrucciones que escribiste por fuera de esta integración. Si no estás seguro, podés dejar el prompt vacío y Henko usará un prompt por defecto.

## Tipo de búsqueda:
- Si el input es el nombre de una bomba de calor, buscá en la columna A: **Nombre** y devolvé toda la información correspondiente a ese producto.
- Si el input incluye las medidas de la piscina (por ejemplo { "largo": "7" }), buscá en la columna B: **Largo_piscinas** y devolvé la bomba que coincida con esase medidas, tene en cuenta que una bomba puede ser apta para varias medidas de piscina.
- Si se menciona financiación, entrega inicial o formas de pago, devolvé el contenido de la columna D: **forma_de_pago** correspondiente a cada bomba.

## Descripción de columnas:
- **Columna A: Nombre** — Nombre del modelo de bomba de calor.
- **Columna B: Largo_piscinas** — Rango de largo de piscinas para las que está recomendada la bomba.
- **Columna C: Precio** — Precio total estimado en pesos argentinos.
- **Columna D: forma_de_pago** — Detalles de pago: anticipos, cuotas, y otras condiciones de compra.