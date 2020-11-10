# Equality
2 == (1 + 1)
"intermediate" != "python"
True != False
"Python" != "python"
```

# Comparison of booleans

"True" == "False"

# Comparison of integers
(- 5 * 15 )!= 75

# Comparison of strings

"pyscript" == "PyScript"

# Compare a boolean with an integer
True == 1
```

# Greater and less than
```
# Comparison of integers
x = -3 * 6
print(x >= -10)

# Comparison of strings
y = "test"
print( "test"<= y)

# Comparison of booleans
print(True > False)
```
# Compare arrays
```
# Create arrays
import numpy as np
my_house = np.array([18.0, 20.0, 10.75, 9.50])
your_house = np.array([14.0, 24.0, 14.25, 9.0])

# my_house greater than or equal to 18
print(my_house >= 18)

# my_house less than your_house
print(my_house< your_house)
```

# and, or, not (1)

```
# Define variables
my_kitchen = 18.0
your_kitchen = 14.0

# my_kitchen bigger than 10 and smaller than 18?
print(my_kitchen >10 and  my_kitchen<18)

# my_kitchen smaller than 14 or bigger than 17?
print(my_kitchen >14 or  my_kitchen<17)


# Double my_kitchen smaller than triple your_kitchen?
print(my_kitchen * 2 <  your_kitchen* 3)
```
# Boolean operators with Numpy
```
To use these operators with Numpy, you will need np.logical_and(), np.logical_or() and np.logical_not(). Here's an example on the my_house and your_house arrays from before to give you an idea:

np.logical_and(my_house > 13, 
               your_house < 15)
               
  ## script 
  
  # Create arrays
import numpy as np
my_house = np.array([18.0, 20.0, 10.75, 9.50])
your_house = np.array([14.0, 24.0, 14.25, 9.0])

# my_house greater than 18.5 or smaller than 10
print(np.logical_or(my_house> 18.5, my_house< 10))

# Both my_house and your_house smaller than 11
print(np.logical_and(my_house<11 , your_house<11))

```

# Driving right (1)

```
# Import cars data
import pandas as pd
cars = pd.read_csv('cars.csv', index_col = 0)

# Extract drives_right column as Series: dr
dr = cars.drives_right

# Use dr to subset cars: sel
sel = cars[dr]

# Print sel
print(sel)

```
# Driving right (2)
```
# Import cars data
import pandas as pd
cars = pd.read_csv('cars.csv', index_col = 0)

# Convert code to a one-liner
sel = cars[cars['drives_right']]

# Print sel
print(sel)

```

# Cars per capita (1)
```
# Import cars data
import pandas as pd
cars = pd.read_csv('cars.csv', index_col = 0)

# Create car_maniac: observations that have a cars_per_cap over 500

cpc = cars.cars_per_cap
many_cars = cars['cars_per_cap'] > 500
car_maniac =     cars[many_cars]    


# Print car_maniac
print(car_maniac)
```
# Cars per capita (2)

```
Remember about np.logical_and(), np.logical_or() and np.logical_not(), the Numpy variants of the and, or and not operators? You can also use them on Pandas Series to do more advanced filtering operations.

Take this example that selects the observations that have a cars_per_cap between 10 and 80. Try out these lines of code step by step to see what's happening.

cpc = cars['cars_per_cap']
between = np.logical_and(cpc > 10, cpc < 80)
medium = cars[between]


### script

# Import cars data
import pandas as pd
cars = pd.read_csv('cars.csv', index_col = 0)

# Import numpy, you'll need this
import numpy as np

# Create medium: observations with cars_per_cap between 100 and 500

cpc = cars['cars_per_cap']
between = np.logical_and(cpc > 100, cpc < 500)
medium = cars[between]


# Print medium
print(medium)

````
