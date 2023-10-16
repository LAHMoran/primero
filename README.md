# primero T

#Caso de Ventas
# Instala el paquete "readr" si aún no está instalado
install.packages("readr")

# Carga la biblioteca "readr" una vez instalada
library(readr)
# Carga los datos desde el archivo CSV (reemplaza la ruta con la ubicación de tu archivo)

venta <- read.csv("C:\\Users\\Luis Angel Hernandez\\Desktop\\Resumen V.csv")

#primero vemos la ruta seleccionando el archivo
file.choose()
#Ya generada la ruta delacras la variable con esa ruta con un nombre
venta <- "C:\\Users\\Luis Angel Hernandez\\Desktop\\Resumen V.csv"

df <- read.csv(venta)
# Leer el archivo y crear el data frame
str(df)
# Ver la estructura del data frame
summary(df)
df
#Ver el data frame
venta
#Tambien se muestra el data frame ya que se guardaron con ambos nombres

# Ajustar el modelo de regresión lineal
modelo <- lm(Venta ~ Mes, data = venta)

# Resumen del modelo
summary(modelo)
