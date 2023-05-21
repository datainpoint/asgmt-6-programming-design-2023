# Assignment 6

> Programming Design 2023

## 01. Define a function `double_odd_args` which doubles the odd args then return as a `list`.

```python
def double_odd_args(*args) -> list:
    """
    >>> double_odd_args(55)
    [110]
    >>> double_odd_args(55, 66)
    [110]
    >>> double_odd_args(55, 66, 77, 88)
    [110, 154]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 02. Define a function `filter_str_args()` which filters the `str` type args and return as a `list`.

```python
def filter_str_args(*args) -> list:
    """
    >>> filter_str_args("5566")
    ['5566']
    >>> filter_str_args("5566", 5566, False)
    ['5566']
    >>> filter_str_args("5566", 5566, False, True, "Luke Skywalker")
    ['5566', 'Luke Skywalker']
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 03. Define a class `ReduceArgs()` which instantiates objects with two methods `summation()` and `product()` that take flexible args and return aggregated result.

```python
class ReduceArgs:
    """
    >>> reduce_args = ReduceArgs(1, 2, 3, 4)
    >>> type(reduce_args)
    '__main__.ReduceArgs'
    >>> reduce_args.summation()
    10
    >>> reduce_args.product()
    24
    >>> reduce_args = ReduceArgs(1, 2, 3, 4, 5)
    >>> reduce_args.summation()
    15
    >>> reduce_args.product()
    120
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 04. Define a class `SortArgs` which instantiates objects with two methods `sort_asc()` and `sort_desc()` that take flexible integers and return a sorted `list`.

```python
class SortArgs:
    """
    >>> sort_args = SortArgs()
    >>> type(sort_args)
    '__main__.SortArgs'
    >>> sort_args.sort_asc(1, 2, 0)
    [0, 1, 2]
    >>> sort_args.sort_desc(1, 2, 0)
    [2, 1, 0]
    >>> sort_args.sort_asc(4, 3, 5)
    [3, 4, 5]
    >>> sort_args.sort_desc(4, 3, 5)
    [5, 4, 3]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 05. Define a class `ReverseKeyValues` which instantiates objects with 2 attributes `keys` and `values`, 1 method `reverse()`.

```python
class ReverseKeyValues:
    """
    >>> reverse_key_values = ReverseKeyValues(twn='Taiwan')
    >>> type(reverse_key_values)
    '__main__.ReverseKeyValues'
    >>> reverse_key_values.keys
    ['twn']
    >>> reverse_key_values.values
    ['Taiwan']
    >>> reverse_key_values.reverse()
    {'Taiwan': 'twn'}
    >>> reverse_key_values = ReverseKeyValues(twn='Taiwan', jpn='Japan')
    >>> type(reverse_key_values)
    '__main__.ReverseKeyValues'
    >>> reverse_key_values.keys
    ['twn', 'jpn']
    >>> reverse_key_values.values
    ['Taiwan', 'Japan']
    >>> reverse_key_values.reverse()
    {'Taiwan': 'twn', 'Japan': 'jpn'}
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 06. Define a class `FizzBuzz` which instantiates objects with 2 methods `nth_element()` and `generate_sequence()`.

Source: <https://en.wikipedia.org/wiki/Fizz_buzz>

```python
class FizzBuzz:
    """
    >>> fizz_buzz = FizzBuzz()
    >>> type(fizz_buzz)
    '__main__.FizzBuzz'
    >>> fizz_buzz.nth_element(1)
    1
    >>> fizz_buzz.nth_element(3)
    'Fizz'
    >>> fizz_buzz.nth_element(5)
    'Buzz'
    >>> fizz_buzz.nth_element(15)
    'Fizz Buzz'
    >>> fizz_buzz.generate_sequence(5)
    [1, 2, 'Fizz', 4, 'Buzz']
    >>> fizz_buzz.generate_sequence(15)
    [1, 2, 'Fizz', 4, 'Buzz', 'Fizz', 7, 8, 'Fizz', 'Buzz', 11, 'Fizz', 13, 14, 'Fizz Buzz']
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 07. Define a class `MonthName` instantiates objects with 2 methods `get_name()` and `get_abb()`.

```python
months = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"]
```

```python
class MonthName:
    """
    >>> month_name = MonthName()
    >>> type(month_name)
    '__main__.MonthName'
    >>> month_name.get_name(1)
    'January'
    >>> month_name.get_abb(2)
    'Feb.'
    >>> month_name.get_name(11)
    'November'
    >>> month_name.get_abb(12)
    'Dec.'
    """
    ### BEGIN SOLUTION

    ### END SOLUTION
```

## 07. Define a function `import_zip_codes_json()` which imports the `zip_codes.json` as a `list` in working directory.

```python
def import_zip_codes_json() -> list:
    """
    >>> zip_codes_json = import_zip_codes_json()
    >>> type(zip_codes_json)
    list
    >>> len(zip_codes_json)
    378
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 08. Define a function `import_teams_json` which imports the `teams.json` as a `dict` in working directory.

```python
def import_teams_json() -> dict:
    """
    >>> teams_json = import_teams_json()
    >>> type(teams_json)
    dict
    >>> len(teams_json["data"])
    30
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 09. Define a function `find_teams_conference_division` which returns a team's conference and division in a `tuple` given team's abbreviation, based on `teams.json` in working directory.

```python
def find_teams_conference_division(team_abb: str) -> tuple:
    """
    >>> find_teams_conference_division("BOS")
    ('East', 'Atlantic')
    >>> find_teams_conference_division("MIA")
    ('East', 'Southeast')
    >>> find_teams_conference_division("LAL")
    ('West', 'Pacific')
    >>> find_teams_conference_division("DEN")
    ('West', 'Northwest')
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 10. Define a function `find_teams_city` which returns a team's city given team's name, based on `teams.json` in working directory.

```python
def find_teams_city(team_name: str) -> str:
    """
    >>> find_teams_city("Celtics")
    'Boston'
    >>> find_teams_city("Heat")
    'Miami'
    >>> find_teams_city("Lakers")
    'Los Angeles'
    >>> find_teams_city("Nuggets")
    'Denver'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```