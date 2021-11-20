<p align="center">
  <h1 align="center">Seven-segment-printer</h1>
  <p align="center"> print Like 7-seg LED display  </p>
</p> 

## Simple Knowledge

A seven-segment display is a form of electronic display device for displaying decimal numerals that is an alternative to the more complex dot matrix displays. Seven-segment displays are widely used in digital clocks, electronic meters, basic calculators, and other electronic devices that display numerical information.

In this code we can learn How to Print like 7-seg display on python

## Python Code 

Enter a number (max 10 digits) to convert into led digits

Copy code and test on Any Editor



```cpp

try:
    s = int(input().strip())
    assert 0 <= s <= 9999999999
except (ValueError, AssertionError):
    s = 1234567890

p_num = {
0: ' _ | ||_|',
1: '     |  |',
2: ' _  _||_ ',
3: ' _  _| _|',
4: '   |_|  |',
5: ' _ |_  _|',
6: ' _ |_ |_|',
7: ' _   |  |',
8: ' _ |_||_|',
9: ' _ |_| _|',
}

for i in range(3):
    for n in str(s):
        print(p_num[int(n)][i*3:i*3+3], end = '')
    print()
```


## Demo 
Input 145

output

```python
       _ 
  ||_||_ 
  |  | _|
```

## Contributing

Contributions are always welcome!
