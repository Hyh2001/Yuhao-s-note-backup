#ros

It specifies the datatype and data that going through the [[ROS topic]] s. The type of message transferred through a topic should match type defined in [[publisher node]] and [[subscriber node]]. To see the message type, use [[ROS topic]],

```shell
	rostopic type
```

command at first. Then use the result of it as

```shell
	rosmsg show name
```

# build own message type

We can also build our own message types. The implementation is as follow:

1. write a [[msg file]]




1. ROS message ([pdf](zotero://open-pdf/library/items/AZFGEHEQ?page=8&annotation=CLGKQITY))