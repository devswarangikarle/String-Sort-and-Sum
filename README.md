# String-Sort-and-Sum
Given a string containing lowercase alphabets and integer digits (from 0 to 9), the task is to print the alphabets in the lexicographical order followed by the sum of digits.

def string_and_nums(s):
    
    alphabets = ''.join(char for char in s if char.isalpha())
    digits_sum = sum(int(char) for char in s if char.isdigit())

    sorted_alphabets = ''.join(sorted(alphabets))

    result = sorted_alphabets + str(digits_sum)
    return result

input_string = input().strip()  
output_result = string_and_nums(input_string)
print(output_result)
