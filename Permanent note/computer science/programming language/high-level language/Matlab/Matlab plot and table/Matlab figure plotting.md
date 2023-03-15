	# plot figures

```matlab
plot(x,y,"r--o*")  % more arguments can be used inside "  "
% x and y are ordered lists 
% r specify the color 
% -- specify the line type, if no line needed then we will not put in arguments
% o specify the type of dots
% * also specify the type of dots 

plot(y) % x-axis data will be set to the range of 1 to n

% add titles
title("name of the plot")
% add labels 
ylabel("name of the y-axis")
xlabel("name of the x-axis")
% add legend
legend("a","b") 
```
## Plot separate plot in one figure 
```matlab
plot(x1,y1)
hold on
plot(x2,y2) 
% if we to exit this mode  
hold off
```
## close figures

```matlab
close
```

## plot a picture

```matlab
a = imread(‘name’)
image(a)
truesize     %each color in the array to be displayed by exactly one pixel
```
## plot inline functions 
```matlab 
a = inline('ax+b')
plot(x,a(x))
```