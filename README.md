# basic_calculator
def again():
    calculation_again = input('''
Do you calculate again?
Please type Y for yes or N for no
''')
    if calculation_again.upper() == 'Y':
        calculate()
    elif calculation_again.upper() == 'N':
        print('Good Bye')
    else:
        again()
def calculate():
    operation = input('''
Please select the Math operation symbol you would like to complete :
+ for Addition
- for Subtraction
* for Multiplication
/ for Division
''')
    number_1 = float(input('Enter the 1st number: '))
    number_2 = float(input('Enter the 2nd number: '))

    if operation == '+':
        print('{} + {} ='.format(number_1, number_2))
        print(number_1 + number_2)

    elif operation == '-':
        print('{} - {} ='.format(number_1, number_2))
        print(number_1 - number_2)

    elif operation == '*':
        print('{} * {} ='.format(number_1, number_2))
        print(number_1 * number_2)

    elif operation == '/':
        print('{} / {} ='.format(number_1, number_2))
        print(number_1 / number_2)

    else:
        print('You have entered a wrong math symbol')
    again()

calculate()
