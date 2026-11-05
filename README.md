# cola
class Cliente:
 """Nodo de la cola. Representa
un cliente del banco."""

def __init__(self,numero):
   self.numero = numero
   self.siguiente=None 

   class Colaclientes:
    def __init__(self):
      self.frente= None
      self.final=None

   def encolar(self,  numero) :
     Nuevo = Cliente(numero)  
     if self.frente is None:
        self.frente= Nuevo
        self.final=Nuevo

     else:
      self.Final.siguiente = Nuevo
      self.final=Nuevo

      def desencolar(self):
        if self.frente is None:
          print("La cola esta vacia, no hay clientes para atender")
          return None
        cliente_atendido =self.frente
        self.frente.siguiente
        if self.frente is None: self.final= None
        cliente_atendido.siguiente= None
        return None
      return self.frente.numero

     def mostrar(self):
       actual=self.frente 
       texto = " "
       while actual is not None: texto += f"{actual.numero}" > "" 
       actual =actual.siguiente 
       texto += "None"
       print(texto)

       # prueba principal 
       cola = Colaclientes()
       cola.encolar(1)
       cola.encolar(2)
       cola.encolar(3)
       cola.enolar(4)

       print ("contenido de la cola:")
       cola.mostrar()
       print(f" nproximo cliente a ser atendido:[cola.peak()]")
       print(f"ncliente atendido: [cola.desencolar()]")
       print("ncontenidode la cola despues de desencolar:")
       cola.mostrar()
            







  



