Q. 리터럴 표기법(literal)의 잇점은?   
A. 생성자를 사용하지 않아 객체를 직관적으로 짧게 만들기 쉽다.

Q. 리스트, 튜플의 차이점?   
A. 리스트 : mutable, 튜플 : immutable

Q. 유니버셜 함수의 종류?   
```python
import numpy as np

a = dir(np)

count = 0
for i in a :
  if i == "Tester":
    continue
  if type(np.__dict__[i]) == np.ufunc :
    print(i, end=", ")
    count += 1
    if count % 10 == 0 :
      print()
```
A.   
abs, absolute, add, arccos, arccosh, arcsin, arcsinh, arctan, arctan2, arctanh,
bitwise_and, bitwise_not, bitwise_or, bitwise_xor, cbrt, ceil, conj, conjugate, copysign, cos,
cosh, deg2rad, degrees, divide, divmod, equal, exp, exp2, expm1, fabs,
float_power, floor, floor_divide, fmax, fmin, fmod, frexp, gcd, greater, greater_equal,
heaviside, hypot, invert, isfinite, isinf, isnan, isnat, lcm, ldexp, left_shift,
less, less_equal, log, log10, log1p, log2, logaddexp, logaddexp2, logical_and, logical_not,
logical_or, logical_xor, matmul, maximum, minimum, mod, modf, multiply, negative, nextafter,
not_equal, positive, power, rad2deg, radians, reciprocal, remainder, right_shift, rint, sign,
signbit, sin, sinh, spacing, sqrt, square, subtract, tan, tanh, true_divide,
trunc,