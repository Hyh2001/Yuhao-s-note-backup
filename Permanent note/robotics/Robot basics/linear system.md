#robotics/robot_motion #differential_equation 

The linear system has the form $\dot{x}(t) = Ax(t)$ where $A \in \mathbb{R}^{n \times n}$ is constant and $x(t) \in \mathbb{R}^n$. The solution of this equation can be expressed as:
# solution of linear system 
$x(t) = e^{At}x_0$  where $e^{At} = I + tA + \frac{t^2}{2!}A^2 + \frac{t^3}{3!}A^3...$  is called the [[matrix exponential]].

