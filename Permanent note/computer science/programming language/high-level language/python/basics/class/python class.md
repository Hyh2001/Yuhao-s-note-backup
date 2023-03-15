我们根据现实生活中的事物和情景编写类（class），并用它们去创建**对象（[[python object]]）**。这个过程叫作 **实例化（instantiation)**。([“python编程：从入门到实践”, p. 80](zotero://select/library/items/G9UNSS38)) ([pdf](zotero://open-pdf/library/items/WD5FAGAK?page=80&annotation=XGB3YMV3)) By convention, **capitalized names** refer to classes in Python. ([Matthes, p. 158](zotero://select/library/items/SSLQAI3E)) ([pdf](zotero://open-pdf/library/items/D9X5UPWD?page=196&annotation=MV275UCZ))
# python 类基本构造
```python
class Dog():
	def __init__(self,name):
		self.name = name
		
```
1. 类中的函数称为方法 ([[python method]])
2. Any variable prefixed with self is available to **every method** in the class, and we’ll also be able to access these variables through **any instance created from the class**. ([Matthes, p. 159](zotero://select/library/items/SSLQAI3E)) ([pdf](zotero://open-pdf/library/items/D9X5UPWD?page=197&annotation=JIXVW7SU)) <!--SR:!2023-03-15,3,250!2023-03-17,4,270-->
# naming rules 
Class names should be written in "CamelCase". To do this, capitalize the **first letter** of each word in the name, and don’t use underscores. ([Matthes, p. 181](zotero://select/library/items/SSLQAI3E)) ([pdf](zotero://open-pdf/library/items/D9X5UPWD?page=219&annotation=GSVNZUC9))
