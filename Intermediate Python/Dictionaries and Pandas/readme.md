
# Create dictionary
```
my_dict = {
   "key1":"value1",
   "key2":"value2",
}
```

# Access dictionary
```
example :
# Definition of dictionary
europe = {'spain':'madrid', 'france':'paris', 'germany':'berlin', 'norway':'oslo' }

# Print out the keys in europe
print(europe.keys())

# Print out value that belongs to key 'norway'
print(europe['norway'])
```

# Dictionary Manipulation (1)
```
# Definition of dictionary
europe = {'spain':'madrid', 'france':'paris', 'germany':'berlin', 'norway':'oslo' }

# Add italy to europe
europe['italy'] = 'rome'
# Print out italy in europe
print('italy' in europe) 

# Add poland to europe

europe['poland'] = 'warsaw'

# Print europe
print(europe)
```

# Dictionary Manipulation (2)
```
# Definition of dictionary
europe = {'spain':'madrid', 'france':'paris', 'germany':'bonn',
          'norway':'oslo', 'italy':'rome', 'poland':'warsaw',
          'australia':'vienna' }

# Update capital of germany
europe['germany']='berlin'

# Remove australia
del(europe['australia'])

# Print europe
print(europe)
```
# Dictionariception
```
# Dictionary of dictionaries
europe = { 'spain': { 'capital':'madrid', 'population':46.77 },
           'france': { 'capital':'paris', 'population':66.03 },
           'germany': { 'capital':'berlin', 'population':80.62 },
           'norway': { 'capital':'oslo', 'population':5.084 } }


# Print out the capital of France
print(europe['france']['capital'])

# Create sub-dictionary data
data = { 'capital': 'rome','population': 59.83}

# Add data to europe under key 'italy'
europe['italy']= data

# Print europe
print(europe)
```
# Dictionary to DataFrame (1)
```


```
