*Consider a mechanism consisting of ​*​*$N$*​*​ links, where ground is also regarded as a link. Let ​*​*$J$*​*​ be the number of joints, ​*​*$m$*​*​ be the number of degrees of freedom of a rigid body (*​*$m =3$*​*​ for planar mechanisms and ​*​*$m =6$*​*​ for spatial mechanisms),*​*$f_i$*​*​ be the number of freedoms provided by joint ​*​*$i$*​*,and ​*​*$c_i$*​*​ be the number of constraints provided by joint ​*​*$i$*​*(the constraints should be independent between each joints), where ​*​*$f_i + c_i = m$*​*​ for all ​*​*$i$*​*. Then,*​*dof = ​*​*$m(N-1) - \sum_{i = 1}^J c_i = m(N-1-J) + \sum_{i=1}^J f_i$*

# overlap joints

This formula is true only when all joint constraints are independent, if not, then Grubler's formula only provides a lower bound on the [[degree of freedom]]s. Therefore for overlapping joints: joints that connect more than two [[link]]s, we need to treat it as several joints overlaps each other



1. “Grubler’s formula” ([Lynch 和 Park, 2017, p. 21](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=21&annotation=3G8C25Y8)) 
