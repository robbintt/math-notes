# Sage Basics

Collecting some code patterns for representing problems in sage.


## I think I would like to use sage for investigating problem sets for my Differential Equations book.

> You can use Sage to investigate ordinary differential equations.

It uses Sage's interface to [Maxima](http://maxima.sourceforge.net/) a Computer Algebra System.

- [Sage Maxima Docs](http://doc.sagemath.org/html/en/tutorial/interfaces.html#section-maxima)
- [Tutorial: How to Investigate Ordinary Differential Equations](http://doc.sagemath.org/html/en/tutorial/tour_algebra.html#solving-differential-equations)
- [Sage Constructions: Ordinary Differential Equtions](http://doc.sagemath.org/html/en/constructions/calculus.html#ordinary-differential-equations)


## Sage Constructions

* [Sage Constructions Documentation](http://doc.sagemath.org/html/en/constructions/)

> This document collects the answers to some questions along the line “How do I construct … in Sage?” Though much of this material can be found in the manual or tutorial or string documentation of the Python code, it is hoped that this will provide the casual user with some basic examples on how to start using Sage in a useful way.


## TUTORIAL: Basic Algebra & Calculus

I converted most of this to a jupyter notebook. It might not be worth keeping most of the below documentation. Figure it out over time.

- TODO: Convert into Jupyter notebook...
- Summarized from: [Sage Tutorial - A Guided Tour: Basic Algebra & Calculus](http://doc.sagemath.org/html/en/tutorial/tour_algebra.html)

- var()
- solve()
- diff()
- function assignment & usage

### Solving


#### Systems of Equations

```
x = var('x') # define your terms
solve((x+2)*(x-2), x)  # solve in terms of x

x, y, z = var('x y z') # define many terms
solve(10 == x+y+z, x)  # solve for x
solve([10==x+y+z, 5==y, 4==z], x,y,z) # solve for x given y and z
solve([10==x+y+z, 5==y], x,y) # solve for x given y (z is a free variable)
```

#### Differentiation

```
x, y, z = var('x y z')
diff(sin(x), x)  # derivative is cos(x)
diff(x^2+x+1, x, 2)  # second derivative is 2
f = x^2+17*y^2 # assignment: used here for partial derivative
f.diff(x) # partial derivative wrt x, 2x
f.diff(y) # partial derivative wrt y, 34y
```

####
