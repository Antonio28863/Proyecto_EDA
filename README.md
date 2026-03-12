# Proyecto_EDA
Análisis exploratorio de los datos bancarios con Python

# Descripción

# Estructura

# Análisis descriptivo de los datos

- Clientes estudiados:
+------------------------------+
|   Suscripción de producto    |
+----------------------+-------+
|          No          | 38156 |
+----------------------+-------+
|          Si          |  4844 |
+----------------------+-------+

De los 43000 clientes estudiados 4844 contrataron el producto, lo que supone algo más del 11%.

- Comparativa de variable entre clientes que contratan y no.
+-----------------------------+--------------+--------------+
|        suscripcion_producto | No contratan |  Contratan   |  
+-----------------------------+--------------+--------------+
|                        edad |    39.861724 |    40.886310 |  
+-----------------------------+--------------+--------------+
|        prestamo_hipotecario |     0.544973 |     0.563584 |  
+-----------------------------+--------------+--------------+
|               otro_prestamo |     0.176407 |     0.170727 |  
+-----------------------------+--------------+--------------+
| duracion_ultima_interaccion |   220.430208 |   551.621387 |  
+-----------------------------+--------------+--------------+
|        contactos_en_campaña |     2.632797 |     2.050784 |  
+-----------------------------+--------------+--------------+
|        dias_ultimo_contacto |     6.246935 |     5.974435 |  
+-----------------------------+--------------+--------------+
|           contactos_previos |     0.132771 |     0.498968 | 
+-----------------------------+--------------+--------------+
|       tasa_variacion_empleo |     0.244499 |    -1.241247 | 
+-----------------------------+--------------+--------------+
|               ingreso_anual | 93324.595031 | 92584.301197 |  
+-----------------------------+--------------+--------------+
|                   num_niños |     1.004744 |     1.005161 |
+-----------------------------+--------------+--------------+
|            num_adolescentes |     0.998821 |     0.996903 | 
+-----------------------------+--------------+--------------+
|       visitas_web_mensuales |    16.587850 |    16.604253 |  
+-----------------------------+--------------+--------------+
|                   num_hijos |     2.003564 |     2.002064 |
+-----------------------------+--------------+--------------+

Con esto se ve que los datos más decisivos para la contaratación o no son: 
- La duración de la ultima interacción:
  Es mayor en los que contratan. Esto es lógico, cuando un cliente esta interesado, la conversación se alarga. No es algo que se deba tener en cuenta ya que es      una consecuencia de la decisión ya tomada, no un factor que decida si contratar o no.
- Contactos en campaña:
  Son ligeramente mayores en los que no contratan, lo que puede indicar que llamar mucho a un cliente puede causar rechazo.
- Contactos previos:
  Los clientes con los que hubo contactos previos tienden a contratar más. Lo que señala que una fidelización de clientes aumenta las contrataciones
- Tasa de variación de empleo:
  La tasa de variación del empleo también afecta a la contratación. En contextos laborales más estables hay mayor indice de contratación. Se puede aprovechar para   hacer campañas en esos momentos.

# Informe explicativo del análisis
