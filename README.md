# PROGprotfolio
## Семестр 1
[Ссылка на рпеозиторий](https://github.com/RandiSPB/PROG3)
## Семестр 2
[Ссылка на рпеозиторий](https://github.com/RandiSPB/PROG4)
## Семестр 3
[Ссылка на рпеозиторий](https://github.com/RandiSPB/PROG5semestr)
## Семестр 4
[Ссылка на рпеозиторий](https://github.com/RandiSPB/Theme4PROG6)
## Дополнительное задание
```python
def return_number(n):
  def return_sequence(n):
    cur_number = 1
    for _ in range(n):
      number_of_square = cur_number * cur_number
      split_number = []
      while number_of_square > 0:
        split_number.append(number_of_square % 10)
        number_of_square = number_of_square // 10
        split_number = split_number[::-1]
      for number in split_number:
        yield number
      cur_number = cur_number + 1
  if int(n) == 0:
    return 0
  return tuple(return_sequence(n))[n-1]

print(return_number(1))
print(return_number(7))
print(return_number(12))
```
