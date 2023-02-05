# lambda
```py
 
       
# if __main__ == '__main__': 
if __name__ == '__main__':

  # lambda arguments : expression
  # lambda can be used inside map, filter, sorted and other functions

  calc = lambda num: 'Even' if num % 2 == 0 else 'Odd'
  print(calc(20))

  filter_nums = lambda s: ''.join([ch for ch in s if ch.isdigit()])
  print(filter_nums("Geeks123John"))

  find_sum = lambda n: sum([int(x) for x in str(n)])
  print(find_sum(5))

  cube_30 = lambda n: n ** 3
  print(cube_30(5))

  list_data  = ['2','3', '-1','-100', '20']
  # the right x can be int(x) if not formatted
  # key contains the lambda function, where sorted use that as input info
  # meaning: sort use input x and output is int converted value 
  # which used in sorted method
  sorted_list_data = sorted(list_data, key = lambda x: int(x)) 
  print(sorted_list_data)

  # sorted(iterable, key=key, reverse=reverse)
  sorted_list_data_reverse = sorted(list_data, key = lambda x: -int(x))
  print(sorted_list_data_reverse)

  #filter positive even number from a list
  # filter(function, sequence)
  filter_list_data = list(filter(lambda x: (int(x) % 2 == 0 and int(x) > 0), list_data))
  print(filter_list_data)

# map(fun, iter)
  map_list_data = list(map(lambda x: str(int(x) + 10), list_data))
  print(map_list_data)
  
  def addition(n): 
    return n+n
  numbers  = (1,2,3,4)
  result = map(addition, numbers)
  print(list(result))

  
 ```
     