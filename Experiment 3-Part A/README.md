# Experiment 5 - Checksum

## Steps

At sender side,

1.If m bit checksum is used, the data unit to be transmitted is divided into segments of m bits.  
2.All the m bit segments are added.  
3.The result of the sum is then complemented using 1’s complement arithmetic.  
4.The value so obtained is called as checksum.  

5.The data along with the checksum value is transmitted to the receiver.  

6.If m bit checksum is being used, the received data unit is divided into segments of m bits.  
7.All the m bit segments are added along with the checksum value.  
8.The value so obtained is complemented and the result is checked.  



## Output

![2 diffrent inputs for the checksum](https://github.com/Ayushkumar036/Network-Programming-and-Security-Lab/blob/main/Experiment%203-Part%20A/op1.PNG?raw=true)
![Output2](https://github.com/Ayushkumar036/Network-Programming-and-Security-Lab/blob/main/Experiment%203-Part%20A/op2.PNG?raw=true)


