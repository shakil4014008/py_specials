# yield
```py
class yie: 
  def __init__(self): 
    pass

  def next(self):
    i = 1
    while True: 
      yield i * i
      i += 1
       
# if __main__ == '__main__': 
if __name__ == '__main__':
  y = yie()
  
  for num in y.next(): 
    if num > 100: 
      break 
    print(num, end=' ')
 ```
     