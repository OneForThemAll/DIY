## Square Star Pattern
```
Expectation: * * * *
             * * * *
             * * * *
             * * * *
```
```python
h = int(input("What is the square's height? -> "))
for i in range(h):
    print('* ' * h)
```

## Hollow Square Star Pattern
```
Expectation: * * * *
             *     *
             *     *
             * * * *
```
```python
h = int(input("What is the square's height? -> "))
for i in range(h):
    if i == 0 or i == h-1:
        print('* ' * h)
    else:
        print('* ' + '  ' * (h-2) + '*')
```
#### Without 'if' statement

```python
h = int(input("What is the square's height? -> "))
print('* ' * h)
for i in range(h-2):
    print('* ' + '  ' * (h-2) + '*')
print('* ' * h)
```

## Rectangle Star Pattern
```
Expectation: * * * * * *
             * * * * * *
             * * * * * *
             * * * * * *
```
```python
x, y = input("What is the rectangle's height and width? (separate by a comma and space) -> ").split(",")
for i in range(int(x)):
    print('* ' * int(y))
```    
    
## Hollow Rectangle Star Pattern
```
Expectation: * * * * * *
             *         *
             *         *
             * * * * * *
```            
```python
x, y = input("What is the rectangle's height and width? (separate by a comma) -> ").split(",")
x, y = int(x), int(y)
for i in range(x):
    if i == 0 or i == x-1:
        print('* ' * y)
    else:
        print('* ' + '  ' * (y-2) + '*')
```

## Right Triangle Star Pattern
```
Expectation: *
             * *
             * * *
             * * * *
```
```python
h = int(input('How tall would you like your triangle to be? -> '))
for i in range(h):
    print('* ' * (i+1))
```

## Hollow Right Triangle Star pattern
```
Expectation: *
             * *
             *   *
             *     *
             * * * * *
```
```python
h = int(input('How tall would you like your triangle to be? -> '))
for i in range(h):
    if i == 0 or i == h-1:
        print('* ' * (i+1))
    else:
        print('* ' + '  ' * (i-1) + '*')
```
## Pyramid Star Pattern
```
Expectation:      * 
                * * * 
              * * * * * 
            * * * * * * * 
```
```python
h = int(input('How tall would you like your pyramid to be? -> '))
for i in range(h):
    print('  ' * (h-i-1) + '* ' * (2*i+1))
```

## Hollow Pyramid Star Pattern
```
Expectation:      * 
                *   * 
              *       * 
            * * * * * * * 
```
```python
h = int(input('How tall would you like your pyramid to be? -> '))
print('  ' * (h-1) + '*')
for i in range(h-2):
    print('  ' * (h-i-2) + '* ' + '  ' * (2*i+1) + '*')
print('* ' * (2*h-1))
```
## Inverted Pyramid Star Pattern
```
Expectation: * * * * * * *
               * * * * *
                 * * *
                   * 
```
```python
h = int(input('How tall would you like your inverted pyramid to be? '))
for i in range(h):
    print('  ' * i + '* ' * (2*h-2*i-1))
``` 
## Inverted Hollow Pyramid Star Pattern
```
Expectation: * * * * * * *
               *       *
                 *   *
                   *
```
```python
h = int(input('How tall would you like your inverted pyramid to be? -> '))
print('* ' * (2*h-1))
for i in range(h-2):
    print('  ' * (i+1) + '* ' + '  ' * (2*h-2*i-5) + '*' )
print('  ' * (h-1) + '*')
```
