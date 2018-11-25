# Phase Color From A Circuit Number

In Canada our 3-phase system's color code is *Red, Black and Blue*. With White as the identified conductor, the shared neutral between the set of 3 line conductors.

Therefore it becomes necessary to be able to determine quickly what color of wire to pull for a give circuit shown on the print. There could be receptacles are circuit #12 with lights(from the same panel) as circuit #79 and you have to figure out what color of wires to pull.

> Luckily I have made an web app that can do just that! And it can be found here.

However for those more interested in how to do this on their own, I will tell you how I was taught, as well as how the application does the calculation.

**How I was taught**
1. Know your multiples of 6, or the 6 times table; 6, 12, 18, 24, etc.
2. Multiples of 6 are **Blue**, as well as the number below them; 6 & 5, 12 & 11, etc.
3. Adding 1 or 2 to the multiple of 6 gives **Red** circuits; 6 + 1 = 7(red), 12 + 2 = 14(red)
4. Adding 3 and 4 to the multiple of 6 gives **Black** circuits; 72 + 3 = 75(black)

So if I was asked to pull wire for circuit #79 I would think of the closest multiple of 6, 78, and by adding 1 I know that 79 is a Red.

**How the Application Works**
1. Divides the given circuit number by 6 and cares only for the remainder.
2. Remainders of 1 or 2 are **Red** circuits
3. Remainders of 3 or 4 are **Black** circuits and,
4. Remainders of 5 or 0 are **Blue** circuits.
5. Display this for the user.

*Example.*
```
  Find circuit #75.
  75 / 6 = 12.5
  .5 * 6 = 3 <-- Remainder
  Therefore #75 is a Black circuit.
  ```
