# Q1 :

fib(0) = fib(1) = 1
fib(n) = fib(n- 1) + fib(n -2) pour tout n >= 2
def fib(n) :
cache = {
0 : 1 ,
1 : 1
} # key : n , value : fib(n)
prec , curr = 1 , 1

    def _fib(n) :
        if n in cache :
            return cache[n]
        res = _fib(n -1 ) +  _fib(n-2)
        cache[n] = res
        return res
    retrun _fib(n)

# V2 :

def fib(n) :
if n == 0 or n == 1 :
return 1

    prec , curr = 1 , 1

    for _ in rane(n-1) :
        temp = curr # fib(n-1)
        curr = prec + curr # fib(n) = fib(n-1) + fib(n-2)
        prec = temp
    retrun curr

fib(4) : - boucles 2 fois : - 1 ere fois :
fib(2) = 1 + 1 = 2
curr = 2 # fib(2)
prec = 1 # fib(1) - 2 eme fois :
fib(3) = fib(2) + fib(1) = 2 + 1 = 3 - 3 eme fois :
fib(4) = fib(3) + fib(2) = 3 + 2 = 5 - return 5

################# Q2 :

-   f(x : double) -> double : f POly de deg q
-   def g(f , i :int)

# f(x) = ax^2 + bx + c

# f(0) = c

# f'(x) = 2ax + b

# f'(0) = b

# c = a_0

# f^(i)(0) / i! = a_i

# f(x) = ax^3 + bx^2 + cx + d

# f(0) = d

# f'(0) = c

# f''(0) / 2! = b

# f'''(0) / 3! = a

def approx*derive(f , eps : 1e-9) :
def f*(x)
retrun (f(x + eps) - f(x - eps)) / 2\*eps
return f\_

def get*coeff(f : Callback[double ,double] , i : int) -> double :
f* = f
for _ in range(i) :
f_ = approx*derive(f*)
return f\_(0) / factr(i)

#########################
