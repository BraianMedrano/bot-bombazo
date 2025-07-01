
# Tipo de herramienta: consumir planilla de Excel o sheet de Google

# Nombre de la herramienta 
- Lista de Piscinas

# Utilidad de la integración
- Sirve para cuando el cliente pregunta sobre alguna piscina, oferta de piscina que vió, o quiere saber las piscinas disponibles. Responde a las preguntas: - Que piscinas tenes?, Me das informacion sobre la piscina malvina?

# Subir Archivo
- Link: https://docs.google.com/spreadsheets/d/1rJCVOPpxbfWfASAjHezmlBZNqatFOqY671rqloPPBB0

# Prompt personalizado para la Ia: Henko utiliza una IA independiente para realizar búsquedas en la base de datos de esta integración. Puedes editar las instrucciones que le darás a esta IA para que realice las búsquedas. Recuerda que esta IA no tiene contexto de las instrucciones que escribiste por fuera de esta integración. Si no estás seguro, puedes dejar el prompt vacío y Henko usará un prompt por defecto.

## tipo de búsqueda:
- **Modelo**  
  - Si recibís el nombre del modelo de la piscina como input, buscá coincidencias  en **columna A: Modelo**.  
- **Línea**  
  - Si recibís el nombre de la línea, buscá en **columna B: Línea** y devolvé todos los modelos pertenecientes a esa línea.  
- **Medidas (largo, ancho, profundidad)**  
  - Si recibís *largo* y *ancho*, filtrá por **columna C: Largo** y **columna D: Ancho**.  
  - Si recibís solo *profundidad*, filtrá por **columna E: Profundidad**.  
  - Si recibís *largo*, *ancho* y *profundidad*, filtrá por las tres columnas; si no hay coincidencia exacta, devolvé el/los modelo(s) cuyas medidas más se aproximen.  
- **Estilo**  
  - Si recibís el estilo (diseño/configuración), buscá coincidencias en **columna F: Estilo**.  
- **Uso recomendado**  
  - Si recibís un tipo de uso (p.ej. “familia”, “espacios reducidos”), filtrá por **columna G: Uso**.  
- **Notas u observaciones**  
  - Si el input coincide con palabras clave de notas, buscá en **columna H: Notas** y mostrales los modelos relacionados.   
- **Precio (lista)**  
  - Si recibís un precio preciso, filtrá por **columna J: Precio** y devolvé los modelos coincidentes.  
  - Si no hay coincidencias exactas, devolvé el/los modelo(s) con precio más cercano.

## Descripción de columnas:
- **Columna A: Modelo** – Nombre del modelo de la piscina.  
- **Columna B: Línea** – Línea a la que pertenece la piscina.  
- **Columna C: Largo** – Largo del modelo (m).  
- **Columna D: Ancho** – Ancho del modelo (m).  
- **Columna E: Profundidad** – Profundidad fija (m).  
- **Columna F: Estilo** – Tipo de diseño o configuración (ej. con solárium, con escalera tribuna).  
- **Columna G: Uso** – Uso recomendado o usuario ideal.  
- **Columna H: Notas** – Observaciones o características destacadas.  
- **Columna I: Promoción** – Detalle de promociones vigentes.  
- **Columna J: Precio** – Precio de lista de la piscina.  
- **Columna K: Forma de pago** – Condiciones y plan de pagos ofrecidos.

## Siempre debes devolver toda la información que encuentres en cada modelo.
