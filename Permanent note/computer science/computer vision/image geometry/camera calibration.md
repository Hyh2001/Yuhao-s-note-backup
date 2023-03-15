#robotics #computer_vision #review 
A few points in 3-D with known coordinates and their corresponding image coordinates are used to calibrate the camera.

![[Pasted image 20211001205641.png]]
we need to calculate A matrix. Matrix A convert world homogeneous coordinates into camera one's.

### solve

by assuming $a_{44} =1$  
![[Pasted image 20211001210712.png|300]]

![[Pasted image 20211001210827.png]]
