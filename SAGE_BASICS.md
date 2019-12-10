# Sage Basics

Collecting some code patterns for representing problems in sage.


## Basic Algebra & Calculus

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
