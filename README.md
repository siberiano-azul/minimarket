# Proyecto minimarket
Proyecto hecho en colab

## Solución interfaz carrito
Bibliotecas utilizadas: *pandas* y *ipywidgets*

El archivo está divido en 5 celdas. 

 Celda 1. Base de datos de productos
 Celda 2. Funciones básicas del carrito
 Celda 3. Componentes de la interfaz
 Celda 4. Conexión de botones con las funciones
 Celda 5. Organización y visualización

Ejemplo de función principal:
`
def buscar_productos(inventario, texto, categoria):

    if texto != '':
        nombres = inventario['nombre'].str.lower()
        inventario = inventario[nombres.str.contains(texto.lower())]

    if categoria != 'Todas':
        inventario = inventario[inventario['categoria'] == categoria]

    return inventario
 `
 
https://colab.research.google.com/drive/1CTkl2UfKUM98G_SHy6SkqeCkH0WVE3st

## Interfaz carrito minimarket



