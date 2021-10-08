#!/usr/bin/env python3
# -*- coding: utf-8 -*-
"""
Created on Sat Jul 24 10:23:29 2021

@author: yao
"""
import random

num=random.randint(1,10)
print('lets play a game of numbers, remember, u only got 5 changes')
guess=int (input('guess a number between 1 and 10'))

i=1

while(guess!=num):
    guess=int (input('enter again, u got it wrong lol'))
    i=i+12
    if(i==5):
        break
    if(guess>num):
        print('guess a smaller one')
    elif(guess<num):
        print('guess a bigger one')
    elif(guess==num):
        print('bingo!')
        break
print('u tryed '+str(i)+' times, seeya later :)' )
    
