We can define a function in Matlab using the phrase below: 
```matlab 
function [output argument1,output argument2,...] = name(input argument 1,input argument 1,...) 
	function body 
end 
```
 ([Driscoll, 2009, p. 30](zotero://select/library/items/DVHEC49B)) ([pdf](zotero://open-pdf/library/items/E33BQLVG?page=44&annotation=X43SNQVL))  
Usually the name of the function should match the name of the file that contains it. ([Driscoll, 2009, p. 30](zotero://select/library/items/DVHEC49B)) ([pdf](zotero://open-pdf/library/items/E33BQLVG?page=44&annotation=6XNHGL8C))

# properties and features of Matlab functions 
## [[Matlab local workspace]]
## Ignore some outputs 
If we only need some specific outputs of a function then we can use ~ 
```matlab
[~,ivMax] = max(v2) % then it will only return a number denoted the index of the biggest number
```


# [[Matlab inline function]]
```matlab 
a = inline('ax+b')
a(x)
```





# Matlab standard function list 
[[Matlab format]]
[[Matlab input]]
