# ep1dp24_Eden_Aquino
Parte práctica, Parcial 1
from Programa import Representante
objeto=Representante()
objeto.ingresoDatos()
objeto.mostrarDatos()


class Continente:
    codigoContinente=0
    nombreContinente=""
    def ingresoDatos(self):
        self.codigoContinente=input("Ingrese el código del Continente\t")
        self.nombreContinente=input("Ingrese el nombre del Continente\t")

    def mostrarDatos(self):
        print("El código es: ", self.codigoContinente)
        print("El Contiente es: ", self.nombreContinente)

class Pais(Continente):
    codigoPais=0
    nombrePais=""
    def ingresoDatos(self):
        super().ingresoDatos()
        self.codigoPais=input("Ingrese el código del País\t")
        self.nombrePais=input("Ingrese el nombre del País\t")

    def mostrarDatos(self):
        super().mostrarDatos()
        print("El código es: ", self.codigoPais)
        print("El País es: ", self.nombrePais)

class Empresa(Pais):
    codigoEmpresa=0
    nombreEmpresa=""
    telefonoEmpresa=0
    def ingresoDatos(self):
        super().ingresoDatos()
        self.codigoEmpresa=input("Ingrese el código de la Empresa\t")
        self.nombreEmpresa=input("Ingrese el nombre de la Empresa\t")
        self.telefonoEmpresa=input("Ingrese el teléfono de la Empresa\t")

    def mostrarDatos(self):
        super().mostrarDatos()
        print("El código es: ", self.codigoEmpresa)
        print("La empresa es: ", self.nombreEmpresa)
        print("El teléfono es: ", self.telefonoEmpresa)

class Representante(Empresa):
    codigoRepresentante=0
    nombreRepresentante=""
    def ingresoDatos(self):
        super().ingresoDatos()
        self.codigoRepresentante=input("Ingrese el código del Representante\t")
        self.nombreRepresentante=input("Ingrese el nombre del Representante\t")
        
    def mostrarDatos(self):
        super().mostrarDatos()
        print("El código es: ", self.codigoRepresentante)
        print("El representante es: ", self.nombreRepresentante)
