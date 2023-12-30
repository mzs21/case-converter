This project is part of Freecodecamp's [Scientific Computing with Python](https://www.freecodecamp.org/learn/scientific-computing-with-python/) curriculum

```py
def convert_to_snake_case(pascal_or_camel_cased_string):

    snake_cased_char_list = [
        '_' + char.lower() if char.isupper()  # This will append '_' + lowercase char if char is uppercase 
        else char # Otherwise char will be appended
        for char in pascal_or_camel_cased_string # Loopoing through the input string
    ]

    return ''.join(snake_cased_char_list).strip('_') # Joining the list and returing as a list

def main():
    print(convert_to_snake_case('FreecodeCampPython'))

if __name__ == '__main__':
    main()
```