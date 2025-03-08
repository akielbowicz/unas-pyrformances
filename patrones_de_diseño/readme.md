# Patrones de Diseño

Formas o maneras de estructurar el código que ayudan a que sea más sencillo trabajar.
Tratan de resolver distintos problemas.

### Factory

Ejemplo de la Pizza, existe solo una abstracción de "pizza", pero la podemos
construir de muchas maneras. Pero no nos interesa crear cualquier pizza posible,
solo tenemos un menú limitado de las que podemos preparar. 

```python
class Pizza:

    def __init__(self, masa, salsa, toppings):
        self.masa = masa
        self.salsa = salsa
        self.toppings = toppings

def muzza():
    return Pizza(molde(), None, {"queso":"200g"})

def fugazzeta():
    return Pizza(molde(), None, {"cebolla":1, "queso":"200g"})

def fugazzeta_rellena():
    return Pizza(molde(relleno={"jamón":"200g","queso":"100g"}), None, {"cebolla":1, "queso":"200g"})

def new_york_style():
    return Pizza(fina(), "tomate", {"queso":"5g"})
```

### Decorator

Tenemos un objeto al cual queremos agregarle comportamiento.
De manera que mantenga el mismo protocolo que el objeto original, pero realice más cosas.


```python
class Ayudante:

    def __init__(self, nombre):
        self.nombre = nombre

    def saludar(self, otro):
        return f"Hola {otro.nombre}"


class DecoradorAyudanteRegistrador:

    def __init__(self, ayudante, lista_participantes):
        self.ayudante = ayudante 
        self.lista_participantes = lista_participantes 

    def saludar(self, otro):
        self.lista_participantes.anotar(otro)
        self.ayudante.saludar(otro)

class DecoradorAyudanteCebadorDeMate:

    def __init__(self, ayudante, set_de_mate):
        self.ayudante =  ayudante
        self.ayudante = set_de_mate

    def saludar(self, otro):
        self.ayudante.saludar(otro)
        self.set_de_mate.cebar(otro)
```
