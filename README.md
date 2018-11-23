# Hello-World
A simple script for introductory to programing 

# Python tutorial
published Nov 10, 2014 by Derek Banas https://www.youtube.com/watch?v=N4mEzFDjqtA&t=0s&list=WL&index=34

import random
import sys
import os

# Print command, Variables, Expressions

print("Hello World!")

name = "Radiovox"
print(name)

name = 15
print(name)

print("5 + 2", 5+2)
print("5 = 2", 5-2)
print("5 * 2", 5*2)
print("5 / 2", 5/2)
print("5 % 2", 5%2)
print("5 ** 2", 5**2)
print("5 // 2", 5//2)

quote = "\"Always remember you are unique"

multi_line_quote = '''Just
like everyone else...'''

new_string = quote + multi_line_quote
print("%s %s %s" % ('I like quote',quote, multi_line_quote))

print("I don't like ",end="")
print('\n' * 5)
print("newlines")


# Lists 

grocery_list = ['Juice', 'Tomatoes', 'Potatoes', 'Bananas']

print('First Item', grocery_list[0])
grocery_list[0] = "Green Juice"

print('First Item', grocery_list[0])

print(grocery_list[1:3])

other_events = ['Wash Car', 'Pick Up Kids', 'Cash Check']

to_do_list = [other_events, grocery_list]

print(to_do_list)

print((to_do_list[1][1]))

grocery_list.append('Onions')

print(to_do_list)

grocery_list.insert(1, "Pickle")

print(to_do_list)

grocery_list.remove('Pickle')

print(to_do_list)

grocery_list.sort()

print(to_do_list)

grocery_list.reverse()

del grocery_list[4]

print(to_do_list)

to_do_list2 = other_events + grocery_list

print(len(to_do_list2))
print(max(to_do_list2))
print(min(to_do_list2))

# Tuples

pi_tuple = (3,1,4,1,5,9)

print(pi_tuple)

new_list = list(pi_tuple)

print(new_list)

new_tuple = tuple(new_list)
print(pi_tuple)
print(new_tuple)

print(len(new_tuple))
print(min(new_tuple))
print(max(new_tuple))
new_list.sort()
print(new_tuple)
print(new_list)


# Dictionairies


super_villains = {'Fiddler' : 'Isaac Bowin',
                  'Captain Cold' : 'Leonard Snart',
                  'Weather Wizard' : 'Mark Mardin',
                  'Mirror Master' : 'Sam Scudder',
                  'Pied Piper' : 'Thomas Peterson'}

print(super_villains['Captain Cold'])

print(super_villains.get('Pied Piper'))

print(super_villains.keys())

print(len(super_villains))

del super_villains['Fiddler']

print(super_villains.keys())

print(len(super_villains))

print(super_villains.values())


# Conditionals

# if else elif "" !" > >" <=


age = 21

if age > 16 :
    print('You are old enough to drive')
else :
    print('You are not old enough to drive')

if age >= 21 :
    print('You are old enough to drive a tractor trailer')
elif age >= 16:
    print('You are old enough to drive a car')
else :
    print("You are not old enough to drive")


#Logical Operators

#and or not


if ((age >=1) and (age <= 18)):
    print("You get a birthday")
elif (age == 21) or (age >= 65):
    print("You get a birthday")
elif not(age == 30):
    print("You don't get a birthday")
else:
    print('You get a birthday party yeah')
