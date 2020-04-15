# learnmath
# finding the greatest common divisor using euclidean algorithm


def gcd(a, b):
    q = int(a/b)
    r = a - b*q
    if r == 0:
        print(f'highest common factor is: {b}')
    elif r != 0:
        q1 = int(b/r)
        r1 = b - r*q1
        if r1 == 0:
            print(f'highest common factor is: {r}')
        else:
            gcd(r, r1)


gcd(a, b)
