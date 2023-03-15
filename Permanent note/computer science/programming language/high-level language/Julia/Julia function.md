There are two ways to define a function for Julia. 

## 1 
```julia
function f(x,y)
	x + y
end
```

## 2
```julia
f(x,y) = x + y
```

# Julia find solutions to functions

‍
# Julia function plotting

1. Before plotting, first we need to invoke packages

    ```julia
    import Pkg
    Pkg.add("Plots")
    using Plots 

    gr()
    ```

2. Then we can plot functions by

    ```julia
    plot(f,x,y) #f is the function, x and y are arguments
    ```

3. If we want to change elements of the graph.

    1. add lables

        ```julia
        plot!(aspect_ratio = 1, xlabel = "x", ylabel = "y")
        ```
    2. add plots

        ```julia
        # add a plot in the exsisting plot
        g(x) = 0
        plot!(g, -15,15)
        ```
    3. we can plot multiple figures are once

        ```julia
        f(x) = ax + b
        g(x) = cx + d

        plot([f,g],x1,x2)  #x1 is for f and x2 is for g
        ```

‍

‍
