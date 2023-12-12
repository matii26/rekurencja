# rekurencja

def silnia_i(n):
    s=1
    for i in range(2,n+1):
        s = s * i
        return s


print(silnia_i(5))

def silnia_r(n):
    if n<2:
        return 1
    else:
        return silnia_r(n-1)*n

print(silnia_r(5))

print(silnia_r(100))
print(silnia_i(100))


def fib_r(n):
    if n<2:
        return n
    else:
        return fib_r(n-1) + fib_r(n-2)

print(fib_r(15))

def fib_i(n):
    a = 0
    b = 1
    for i in range(2,n+1):
        c = a+b
        a = b
        b = c
    return c

print(fib_i(15))


def pot_r(n):
    if n == 0:
        return 1
    else:
        return pot_r(n-1)*2

print(pot_r(5))
