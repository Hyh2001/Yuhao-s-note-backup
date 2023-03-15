

# import one class 
```python
from car import Car # car is the file named car.py which is a python module and Car is the class named Car 
```
The import statement tells Python to open the car module and import the class Car. ([Matthes, p. 175](zotero://select/library/items/SSLQAI3E)) ([pdf](zotero://open-pdf/library/items/D9X5UPWD?page=213&annotation=SXI3TPHL))

# import multiple classes 
As [[python module]] can store as many as classes. ([Matthes, p. 175](zotero://select/library/items/SSLQAI3E)) ([pdf](zotero://open-pdf/library/items/D9X5UPWD?page=213&annotation=ECIB5WGN))
?
```python 
from car import Car, ElectricCar #car is the file named car.py which is a python module, Car and ElectricCar are the classes contained in the module  
```

# import all classes 
```
from car import * 
```
## drawbacks 
1. It is unclear which **classes** we are using 
2. Lead to **confusion of name** 
# import entire module 
```python 
import car # car is a module stored in car.py 
```
We can access the classes we need through the module_name.ClassName syntax ([Matthes, p. 177](zotero://select/library/items/SSLQAI3E)) ([pdf](zotero://open-pdf/library/items/D9X5UPWD?page=215&annotation=KPW7KM96))
?
```python 
car.Car( ... )
```

# aliases 
To avoid tedious names:
?
```python
from electric_car import ElectricCar as EC #alases for classes 
import electric_car as ec # aliases for modules 
```
([Matthes, p. 178](zotero://select/library/items/SSLQAI3E)) ([pdf](zotero://open-pdf/library/items/D9X5UPWD?page=216&annotation=Z838FMHM))