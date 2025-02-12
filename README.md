# PARADIGMAS-DE-PROGRAMACION
"NUMEROS: N= numero 1 ,  "
n = 18
m = 2      
"N debe ser mayor que M o igual"
def S(n):
    return n + 1

def suma(n, m):
    result = n
    for _ in range(m):
        result = S(result)
    return result

def multiplicacion(n, m):
    if m == 0:
        return 0
    elif m == 1:
        return n
    else:
        return suma(n, multiplicacion(n, A(m)))  

print(f"Suma: {suma(n, m)}")
print(f"Multiplicación: {multiplicacion(n, m)}")


def A(n):
    if n <= 0:
        raise ValueError("deben ser mayores que cero (0).")
    return n - 1
    
def resta(n, m):
    result = n
    for _ in range(m):
        if result <= 0: 
            break  
        result = A(result)  
    return result

def division(n, m):
    if m == 0:
        raise ZeroDivisionError("la division en 0 es compleja.")
  quotient = 0
    remainder = n
    while remainder >= m:
        remainder = resta(remainder, m)  
        quotient = S(quotient)

  if remainder != 0:
        return f"{quotient} (inexacta)"
    else:
        return quotient
print(f"Resta: {resta(n, m)}")
print(f"División: {division(n, m)}")

Suma: 20
Multiplicación: 36
Resta: 16
División: 9

"NUMEROS: N= numero 1 ,  "
n = 2
m = 18      
"N debe ser mayor que M o igual"
def S(n):
    return n + 1

def suma(n, m):
    result = n
    for _ in range(m):
        result = S(result)
    return result

def multiplicacion(n, m):
    if m == 0:
        return 0
    elif m == 1:
        return n
    else:
        return suma(n, multiplicacion(n, A(m)))  

print(f"Suma: {suma(n, m)}")
print(f"Multiplicación: {multiplicacion(n, m)}")


def A(n):
    if n <= 0:
        raise ValueError("deben ser mayores que cero (0).")
    return n - 1
    
def resta(n, m):
    result = n
    for _ in range(m):
        if result <= 0: 
            break  
        result = A(result)  
    return result

def division(n, m):
    if m == 0:
        raise ZeroDivisionError("la division en 0 es compleja.")

  quotient = 0
    remainder = n
    while remainder >= m:
        remainder = resta(remainder, m)  
        quotient = S(quotient)

  if remainder != 0:
        return f"{quotient} (inexacta)"
    else:
        return quotient
print(f"Resta: {resta(n, m)}")
print(f"División: {division(n, m)}")

Suma: 20
Multiplicación: 36
Resta: 0
División: 0 (inexacta)
