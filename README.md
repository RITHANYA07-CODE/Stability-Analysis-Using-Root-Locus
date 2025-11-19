# Stability Analysis using Root Locus
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=K/(S(S+5)(S+10)) using root locus and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:
<img width="573" height="895" alt="image" src="https://github.com/user-attachments/assets/c68203eb-7075-40b5-bb7a-4de5ba5aecb7" />

<img width="472" height="872" alt="image" src="https://github.com/user-attachments/assets/c02364d9-a298-42e1-a100-3b8fc33a5c80" />

<img width="652" height="876" alt="image" src="https://github.com/user-attachments/assets/44a6f498-7e8a-4433-bef8-19397ad9e2e7" />

## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Click on the crossing point of the root locus to find the value of K and poles at the crossing point.
	From the value of K, analyse the stability.

## Program: 
```
num = [1];
den = [1 15 50 0];
sys = tf(num, den);       
rlocus(sys);              
[k poles] = rlocfind(sys); 
```

## Output: 
<img width="1641" height="991" alt="image" src="https://github.com/user-attachments/assets/13b9dc05-f8ca-4362-b634-953e683dbac3" />


## Result:

Thus the root locus for the given transfer function was drawn and verified using MATLAB. The conditions for stability is 753.
