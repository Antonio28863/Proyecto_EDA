# Proyecto_EDA
Análisis exploratorio de los datos bancarios con Python

# Descripción:
Para realizar el análisis se parte de un archivo csv que contiene datos relacionados con campañas de marketing directo y un archivo excel con datos demográficos de los clientes.  
Lo primero que hacemos es concatenar las hojas de excel en un dataframe. Traducimos los encabezados de las columnas para tener más claro con los datos que estamos trabajando.  
Comprobamos que los id de cliente sean únicos, si coinciden en los dos dataframes y cuales solo están en un dataframe. Unimos en un solo dataframe descartando los id de los que solo tenemos los datos demograficos.  
Colocamos el id de cliente como indice y borramos un par de columnas con indices que no usaremos.  
Hacemos una primera exploración de los datos. En la columna historial_incumplimiento vemos que solo hay tres valores positivos que no nos valen para el análisis al ser un numero muy pequeño, eliminamos la columna. Cambiamos el tipo de dato a booleano de las columnas prestamo_hipotecario y otro_prestamo. En dias_ultimo_contacto cambiamos el valor 999 por NaN para poder trabajar con números. La columna resultado_campaña_previa se cambia a booleano. Se cambian las columnas de datos macroeconomicos de str a float. La de fecha interacción de str a fecha. Se eliminan las columnas de latitud y longitud porque no vamos a trabajar con ellas.  
Creamos la columna num_hijos a partir de las de número de niños y adolescentes. Creamos la columna tiempo_cliente con el tiempo que llevan siendo clientes y antiguedad_cliente segmentando los clientes en nuevos (menos de 6 meses), recientes(menos de 2 años) y antiguos (los que llevan más de 2 años). También creamos las columnas día_interacción y mes_interacción.  
Se guardan los datos en un nuevo archivo csv y un archivo pkl.  
En otro archivo se realiza el anális exhaustivo de los datos. Se comprueba el exito total de la campaña, se calculan las medias de las variables numericas y se comparan con los de la campaña anterior. Calculamos las medias para suscripcion_producto con las demas categorias.  

# Análisis:
El éxito total de la campaña es ligeramente superior al 11% con un total de 4844 suscripciones de producto.  
El dato que más llama la atención es el de la duración de la llamada, muy superior de los que suscriben, dato que no hay que tener muy en cuenta ya que parece más una consecuencia de tener interés que una condición para suscribirse.  
Los contactos en campaña son ligeramente superiores en los que no suscriben lo cual puede suponer que el llamar de más puede ser una causa de no suscribir.  
Los contactos previos son superiores en los que suscriben, la fidelización de clientes es importante fuera de campañas para que funcionen mejor.  
La tasa de variación de empleo, la tasa de interes a tres meses y los demas datos macroeconomicos nos dicen que cuanto mayor es la incertidumbre economica hay mas predisposición a suscribir productos. Se pueden aprovechar esos momentos par lanzar campañas.  
Los clientes que ya suscribieron en una campaña previa tiene un 65% de posibilidades de repetir. Se pueden plantear campañas para clientes que ya suscribieron con anterioridad.  
Por ocupación los estudiantes con un 31% y jubilados con un 25% son los targets a tener en cuenta. Aunque son menos de 3000 clientes.  
Hay una ligera suscripción superior de solteros.  
Por nivel educativo los datos son bastante estables, detaca el de analfabetos pero al haber solo 18 casos no es reseñable.  
Por método de contacto el teléfono móvil triplica a los suscritos por teléfono fijo.  
El mes de interacción con mayor éxito es ligeramente octubre y el día los jueves.  
La tasa de suscripción de clientes con menos de dos años de antigüedad llega casi al 20% por el 10% de los antiguos. Se deberia fidelizar a los clientes antiguos y lanzar campañas para clientes nuevos.  
De los 247 clientes recientes jubilados contrataron el 40%. Se deben hacer campañas especificas para atraer más clientes con este perfil.  
En conclusión, el análisis muestra que los clientes más propensos a suscribir son los que ya suscribieron antes, los nuevos clientes y los estudiantes y jubilados. La mejor forma de contactar con ellos es el teléfono móvil.

# Archivos adjuntos:
- En la carpeta datos_brutos: Los datos brutos recibidos
- En la carpeta datos_limpios: Los datos preparados para el análisis.
- En la caperta notebook: El archivo Datos con la limpieza y preparación de los datos y el archivo análisis con el análisis de los datos.

# Autor:
Antonio Fernández
@antonio28863
