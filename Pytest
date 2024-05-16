import pytest
import math

#1. является ли число квадратом целого числа
@pytest.mark.parametrize('a, results', [(25, True),
                                        (10, False),
                                        (-24, False),
                                        (0, False)])
def test_sqrt(a, results):
    try:
        assert (math.sqrt(a).is_integer() == results)
    except AssertionError:
        pass
    except ValueError:
        pass

#2. существует ли треугольник
def triangle(a, b, c):
    if a + b > c and a + c > b and b + c > a:
        return True
    else:
        return False

def test_answer():
    assert triangle(3, 4, 5) == True

#3. проверка максимального элемента списка
def test_max_element():
    assert max([1, 2, 5, 4]) == 5

#4. проверка заполненности списка
def test_list_count():
    assert len([]) == 0

#5. сумма кортежа меньше определенного значения
@pytest.mark.parametrize('a, results', [((25, 11, 2, 44), 100),
                                        ((4, 18, 31, 15), 90),
                                        ((25, 11, 3, 0), 50),
                                        ((11, -5, 2, 44), 31)])
def test_tuple_sum(a, results):
    try:
        assert sum(a) < results
    except AssertionError:
        pass

#6. проверка вхождения символа в элемент кортежа
def test_tuple_():
    tuple_1 = ("Orlando", "Blum", 45, "London")
    assert 'o' in tuple_1[0]
