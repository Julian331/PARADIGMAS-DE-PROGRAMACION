RECURSIVO

#include <stdio.h>

unsigned long long factorial_recursivo(int n) {
    if (n == 0 || n == 1) {
        return 1;
    }
    return n * factorial_recursivo(n - 1);
}
----------------------------------------------------------------------------------------------------------------------------------
ITERATIVO

#include <stdio.h>

unsigned long long factorial_iterativo(int n) {
    unsigned long long resultado = 1;
    for (int i = 1; i <= n; i++) {
        resultado *= i;
    }
    return resultado;
}
-------------------------------------------------------------------------------------------------------------------------------------

1) TIEMPO DE EJECUCION
   - ITERATIVO
       - Es mas rapido ya que no es necesario que tenga que usar las llamadas recursivas
       - Cada iteracion representa una operacion basica por lo que hace que sea mas eficiente en cuanto a tiempo
       - si es un numero pequeño, el tiempo de ejecucion es corto
    - RECURSIVO
        - En comparacion al iterativo, aca se presenta una saturacion en cuanto a las llamadas recursivas
        - En cada llamada recursiva es necesario guardar los elementos del dato. lo que hace que su tiempo de ejecucion sea lento
        - en caso de que sea un numero pequeño tardara mas comparandolo con el iterativo.
        - Funciona mejor cuando no se necesita efectividad sino mas bien un codigo el cual sea claro.
----------------------------------------------------------------------------------------------------------------------------------------
2) CANTIDAD DE MEMORIA USADA
   - ITERATIVO
       - 
   - RECURSIVO
       -
        
