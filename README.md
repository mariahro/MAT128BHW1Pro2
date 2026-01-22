# MAT128BHW1Pro2
def f(x):
    return x**3 - 7*x**2 + 14*x - 6

a = 3.2
b = 4.0
tol = 1e-2

while (b - a) / 2 > tol:
    p = (a + b) / 2
    if f(a) * f(p) < 0:
        b = p
    else:
        a = p

p_approx = (a + b) / 2
print("Approximate root:", p_approx)
