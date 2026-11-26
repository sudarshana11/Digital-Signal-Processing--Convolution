# Digital-Signal-Processing--Convolution
## Aim:
                  To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 
```
%Name: Sudarshana   Reg No:212223050054
clear all;
close all;
clc;

% INPUT SEQUENCE
a = input('enter the starting of x(n): ');
x = input('enter the x(n) sequence: ');

n_a = a : length(x)+a-1;

figure(1);
stem(n_a,x);
xlabel('time');

ylabel('amplitude');
title('input sequence');

% IMPULSE SEQUENCE
b = input('enter the starting of h(n): ');
y = input('enter the h(n) sequence: ');

m = b : length(y)+b-1;

figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response');
% {2,-1,4,9,-3}*{3,-4,1,1,-2.3,5}
% LINEAR CONVOLUTION
z = conv(x,y);

n1 = a+b : length(z)+a+b-1;

figure(3); 
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
```

## OUTPUT:
<img width="1292" height="597" alt="image" src="https://github.com/user-attachments/assets/1bb36ae5-e9f2-4aad-aae1-1146c1278d3d" />
<img width="1202" height="557" alt="image" src="https://github.com/user-attachments/assets/ea939421-edb9-4112-bd53-8f3f60af651f" />
<img width="1191" height="538" alt="image" src="https://github.com/user-attachments/assets/d765772d-4d22-40f9-adf7-d671947afa40" />

## RESULT:

<img width="1599" height="505" alt="image" src="https://github.com/user-attachments/assets/c6b4bbba-a58c-4d40-a933-e24b0ba6d328" />
