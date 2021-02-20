# Keeping Up With the Javascript: ES6

## www.pirple.com

## Homework Assignment #12: OOP

## Author: Guadalupe Tienda López

## Country: México

## Language: Spanish / Español

</br>

**my github:** [<https://github.com/gtienda/OOP.git>)

### What is object oriented programming, and why would you use it? As you may already know, many javascript projects are written using a functional, or event-driven design pattern. In which cases would an OOP pattern be a better choice?

</br>

La idea principal de la programación orientada a objetos (OOP) es la de usar "objetos" para representar cosas del mundo real.
</br>

Como en el mundo real a los objetos (cosas) les damos características (properties) y usos (functions) que al mismo tiempo nos pueden arrojar datos (data) que representan la información de lo que estamos modelando (structure).
</br>

Estas estructuras de datos como objetos pueden incluir funciones y datos. Se pueden crear relaciones entre un objeto y otro. Es decir, objtos pueden heredar (inherit) características de otros objetos.
</br>

Una de las principales ventajas de la programación orientada a objetos (OOP) sobre los patrones de usar procedimientos es que permite a los desarrolladores crear módulos que no necesitan cambiarse cuando un tipo nuevo de obejto es agregado. Esto es, el desarrollador simplemente crea un nuevo objeto que hereda muchas de las características que contiene el objeto original, por lo tanto, esto nos permite más facilmente modificar nuestra programación orientada a objetos.
</br>

## Projecto: Candidatos favoritos

</br>

### Descripción

El propósito de este sistema es que el usuario (ciudadano) en edad de votar, conozca la lista de candidatos de los 13 estados con elección a gobernador de este 2021, que el ciudadano pueda ver algunas características de ellos, que los elija como favoritos, o los borre y que pueda visualizar su lista de candidatos favoritos por cada uno de los estados en elección.

### Historias de los usuarios (ciudadanos)

</br>

* Como usuario quiero revisar la lista de candidatos a gobernador con su respectivo estado y partido político al que pertenecen.

* Como usuario quiero ver las características de los candidatos.

* Como usuario quiero ver los cargos públicos que ha ocupado el candidato en los últimos tres años.

* Como usuario quiero agregar al candidato a mi lista de favoritos.

* Como usuario quiero remover al candidato a mi lista de favoritos.

* Como usuario quiero ver mi lista de candidatos favoritos por estado.

### Pseudocódigo

### Usuario = Ciudadano (En edad de votar)

```
class Ciudadano {
    first name,
    last name,
    email,
    password,
    favorite list of candidates by State
    ---
    addFavoriteCandidate()
    removeFavoriteCandidate()
    getListOfFavoritesCandidatesByState()
}

class Candidato {
   full name,
   state name,
   politic party,
   genre,
   age,
   image,
   voters ranking,
   list of public positions
   ---
   addPublicPosition()
   removePublicPosition()
   getListOfPublicPositions() 
}

user = create Ciudadano("John","Smith","john@email.com","1234")

candidato1 = create Candidato("Adrián de la Garza","Nuevo León","PRI","Male",50,"adrian_url",8)

candidato2 = create Candidato("Maru Campos","Sonora","PAN","Female",49,"maru_url",7)

list of candidates = [candidato1, candidato2]

position1 = create Position("Alcalde","Monterrey, NL",2015,2018,"3 años")

position2 = create Position("Alcaldeza","Hermosillo, SON",2016,2019,"3 años")

candidato1.addPublicPosition(position1)
candidato2.addPublicPosition(position2)

Ciudadano.addFavoriteCandidate(candidato1)
Ciudadano.addFavoriteCandidate(candidato2)
Ciudadano.removeFavoriteCandidate(candidato2)
Ciudadano.getListOfFavoritesCandidatesByState()
```
