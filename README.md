# Digital-Signal-Processing--Correlation
## AIM:
To generate discrete auto correlation and cross correlation of signals using MATLAB.
## APPARATUS REQUIRED:
MATLAB R2012.
## ALGORITHM:
Step 1: Open matlab. Write the program.

Step 2: Read the input sequence 1 and input sequence 2 sequence.

Step 3: Perform auto correlation and cross correlation for both the sequences. 

Step 4: Plot the output sequence with x-label and y-label with suitable title.

Step 5: Terminate the program.


## PROGRAM: 
```
clc;%clear screen
clear all;
close all;
a=input('enter the starting x(n)');
x=input('enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');
b=input('enter the starting h(n)');
y=input('enter the h(n) sequence');
m=b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response');
z=conv2(x,y);
n1=a+b:1:length(z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
```

## OUTPUT:
<img width="829" height="747" alt="DSPEXP2 INPUT1" src="https://github.com/user-attachments/assets/bcee6416-57d5-44fd-b657-22fd21ca5d89" />
<img width="834" height="749" alt="DSPEXP2 INPUT2" src="https://github.com/user-attachments/assets/1af37dd4-3844-43e6-b9ad-84202f78012f" />
<img width="842" height="745" alt="DSPEXP2 D1" src="https://github.com/user-attachments/assets/39da46c8-9627-491b-91a8-f7fe5759b2d4" />
<img width="834" height="742" alt="DSPEXP2 D2" src="https://github.com/user-attachments/assets/abdf5f0f-9a3f-49d4-a0cc-49650bf11f20" />

## RESULT:
![WhatsApp Image 2026-03-30 at 11 50 37 AM](https://github.com/user-attachments/assets/add650c7-044d-4197-ae5c-d286bd8f07ec)


