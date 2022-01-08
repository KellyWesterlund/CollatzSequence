# CollatzSequence
# A short practice program to test the Collatz conjecture for any positive integer

def collatz(number):
    while number <=0:
        print('Please enter a positive integer')
        number = int(input())
    while number > 1:
        print(number, end=' ')
        if (number % 2 == 0):
            number = number // 2
        else:
            number = 3 * number + 1  
    
print('Enter Number:')
try:
    number = int(input())
    print(collatz(number))
    
except ValueError:
    print('Please enter a positive integer')
