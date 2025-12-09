Esta es una lista de cosas a tomar en cuenta para el correcto funcionamiento de la app

- los ingredientes en las recetas al momento de mostrarse al usuario se harán así:
  Cantidades Estándar [Cantidad] [Unidad] de [Nombre]
  Opcionales ([Opcional]) al final del nombre o de la línea.
  Especias [Cantidad] [Unidad] de [Nombre] (Ej: "1 pizca de Pimienta Negra").

- cuando las recetas son de tipo unidad aparecerán en la db como 1, 0.5, 0.25 y similares, en caso de que sea un numero menor a un entero en el frontend se mostrará como 1/2, 1/4, etc
