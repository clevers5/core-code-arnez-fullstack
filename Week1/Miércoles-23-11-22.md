# Desafío - *Miércoles 23-11-22*

## *1. Entero más pequeño en matriz*

**Descripción:** Dada una matriz de enteros, su solución debe encontrar el entero más pequeño. 

  - Por ejemplo:
      - Dado [34, 15, 88, 2] su solución devolverá 2 
      - Dado [34, -345, -1, 100] su solución devolverá -345
  - Puede suponer, a los efectos de este kata, que la matriz proporcionada no estará vacía.

**Solución:**

```Javascript
class SmallestIntegerFinder {
  findSmallestInt(args) {
    args.sort(function (a, b) {
      return a - b;
    });
    return args[0];
  }
}
```
