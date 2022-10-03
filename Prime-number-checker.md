### Shehu Ibrahim
- Python
- Location: Nigeria
- Github: https://github.com/Ns-SheF

#Prime Number Checker program

number = None
#set a flag variable
notp = False
#User interaction/input
print('Hello, my dude')
name = input('What do i call you, my dude? ')

print('Nice to mee you ' +name +', My name is Prime.')
print('I can help you determine if a number is prime or not -just like me *)')

number = int(input('Enter a number '))
#Check prime
if number > 1:
    #factor check
    for i in range(2, number):
        if (number % i) == 0:
            #set flag True if factor found
            notp = True
            break
#Output
if notp:
    print(name + ', {} is not prime.' .format(number))
    print('>>>',i,'times',(number//i),'is',number)
else:
    print(name + ', {} is a prime.' .format(number))