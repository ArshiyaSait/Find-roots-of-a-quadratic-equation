# Find-roots-of-a-quadratic-equation
import math
a = float(input("Enter the first coefficient (a): "))
b = float(input("Enter the second coefficient (b): "))
c = float(input("Enter the third coefficient (c): "))
if a != 0.0:
    d = b**2 - 4*a*c  # discriminant
    if d == 0.0:
        print("The roots are real and equal.")
        r = -b / (2*a)
        print("The roots are:", r, "and", r)
    elif d > 0.0:
        print("The roots are real and distinct.")
        r1 = (-b + math.sqrt(d)) / (2*a)
        r2 = (-b - math.sqrt(d)) / (2*a)
        print("Root1 is:", r1)
        print("Root2 is:", r2)
    else:
        print("The roots are imaginary.")
        rp = -b / (2*a)
        ip = math.sqrt(-d) / (2*a)
        print("Root1 is: {} + i{}".format(rp, ip))
        print("Root2 is: {} - i{}".format(rp, ip))
else:
    print("Not a quadratic equation.")

OUTPUT:
Enter a: 1
Enter b: -3
Enter c: 2
The roots are real and distinct.
Root1 is: 2.0
Root2 is: 1.0

