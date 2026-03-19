# Task 

Реализуйте функцию count_vowels(), которая принимает строку, считает и возвращает количество гласных букв в ней.

Для проверки, является ли буква гласной, импортируйте и используйте функцию is_vowel() из модуля symbols.py.

is_vowel('a')  # True
is_vowel('n')  # False

count_vowels('One')  # 2
count_vowels('London is the capital of Great Britain')  # 13

# Solutions

Ваше решение

from symbols import is_vowel
def count_vowels(text: str)-> int:
    count=0
    for i in text:
        if is_vowel(i):
            count+=1
    return count
Решение учителя

from symbols import is_vowel


def count_vowels(text):
    result = 0
    for char in text:
        if is_vowel(char):
            result += 1
    return result
