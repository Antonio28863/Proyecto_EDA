# Proyecto_EDA
Análisis exploratorio de los datos bancarios con Python

# Descripción

# Estructura

# Análisis descriptivo de los datos

- Clientes estudiados:
  
| Clientes estudiados  |       |
|----------------------|-------|
|    No contrataron    | 38156 |
|      Contrataron     |  4844 |

De los 43000 clientes estudiados 4844 contrataron el producto, lo que supone algo más del 11%.

- Comparativa de variable entre clientes que contratan y no.
  
|     Suscripción producto    | No contratan | Contratan |
|:---------------------------:|:------------:|:---------:|
|             Edad            |     39.8     |    40.8   |
|     Préstamo Hipotecario    |     0.54     |    0.56   |
|        Otro préstamo        |     0.17     |    0.17   |
| Duración última interacción |      220     |    551    |
|     Contactos en campaña    |       3      |     2     |
|     Días último contacto    |       6      |     6     |
|      Contactos previos      |     0.13     |    0.49   |
|    Tasa variación empleo    |     0.24     |   -1.24   |
|       Ingresos anuales      |     93324    |   92584   |
|           Nº niños          |       1      |     1     |
|       Nº adolescentes       |       1      |     1     |
|    Visitas web mensuales    |      17      |     17    |
|           Nº hijos          |       2      |     2     |

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
