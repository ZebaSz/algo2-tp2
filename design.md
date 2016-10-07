# Sistema

## contadorTotalPoke

- Nat

## Vector(jugador)

- arreglo REdimensionable

| operación | complejidad |
|:---------:|:-----------:|
| insertar  | O(n)*       |
| obtener   | O(1)        |
| borrar    | O(n)*       |

_*O(1) amortizado_

## DiccString(nat)

- multiconjunto trie de pokemones

- definición = cant total del pokemon

| operación | complejidad |
|:---------:|:-----------:|
| insertar  | O(\|clave\|)|
| obtener   | O(\|clave\|)|
| borrar    | O(\|clave\|)|

## Grilla(tupla(bool, dataPos))

- mapa

- arreglo de arreglos (dimensionables)

- bool = pos valida

### dataPos: tupla(nat, PQ(jugador))

- contador de movsLejosDePos

- minPQ para jugadores esperando captura


|       operación        | complejidad |
|:----------------------:|:-----------:|
| ver contador           | O(1)        |
| modificar contador     | O(1)        |
| obtener capturante     | O(1)        |
| agregar/quitar jugador*| O(log(n))   |
| borrar PQ              | O(n)        |
_* ya sea por conexion o movimiento_

# Jugador

## DiccString(nat)

- multiconjunto trie de pokemones

- definición = cant de ese pokemon capturados por el jugador

| operación | complejidad |
|:---------:|:-----------:|
| insertar  | O(\|clave\|)|
| obtener   | O(\|clave\|)|
| borrar    | O(\|clave\|)|

------------

# Pendiente

guardar también los pokemons en esta grilla? no debería ser un módulo aparte esto?

    Ignacio Tarrio: **cualquier conjunto piola** para guardar las posiciones con pokemons

conj(tupla) o dicc? complejidad? hace falta que el mismo conjunto guarde que pokemon está en esa pos? podemos guardar el pokemon en la grilla?
