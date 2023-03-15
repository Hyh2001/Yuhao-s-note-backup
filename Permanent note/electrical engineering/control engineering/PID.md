#control/PID

PID is a control algorithm. Its mathematical form is as follow: 

$u(t) = K_pe(t)+K_i\int_0^te(t^{'})dt^{'} + K_d\frac{de(t)}{dt}$ where $e$ denotes error, $u$ denotes output and $t$ denotes time.

It consists of three parts:

## Proportional part (present)

$K_pe(t)$, this part is proportional to the error. This means that this part changes linearly comparing with $e(t)$. 

### problems

The system will be oscillating at last which is called [[overshooting]] because the error will not be able to approach 0 and there is always residue errors.

## Integral part (past)

$K_i\int_0^te(t^{'})dt^{'}$, this part is proportional to the total error during the operating time. 

### why we need it

Considering that if the system stays at some points where error is really small and the Proportional part (present)[^1] will not drawn little feedbacks.   

## Derivative part (future)

$K_d\frac{de(t)}{dt}$, this part is proportional to the rate of change of the error. It will act like prevent overshooting. 

‍

[^1]: ## Proportional part (present)
