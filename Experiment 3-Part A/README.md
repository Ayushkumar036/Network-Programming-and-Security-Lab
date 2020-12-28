# Experiment 5 - Checksum and Hamming code

## Checksum

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


## Hamming code

## steps

1.Hamming code uses redundant bits (extra bits) which are calculated according to the below formula:-  

  2r ≥ m+r+1  

2.Where r is the number of redundant bits required and m is the number of data bits.  

3.R is calculated by putting r = 1, 2, 3 … until the above equation becomes true.  
 
4.R1 bit is appended at position 20   

5.R2 bit is appended at position 21  

6.R3 bit is appended at position 22 and so on.  

7.These redundant bits are then added to the original data for the calculation of error at receiver’s end.  

8.At receiver’s end with the help of even parity (generally) the erroneous bit position is identified and since data is in binary we take complement of the erroneous bit position to correct received data.   

9.Respective index parity is calculated for r1, r2, r3, r4 and so on.  


## Output  

![2 diffrent inputs for the checksum](https://github.com/Ayushkumar036/Network-Programming-and-Security-Lab/blob/main/Experiment%203-Part%20A/Hamming-op1.PNG?raw=true)
![Output2](https://github.com/Ayushkumar036/Network-Programming-and-Security-Lab/blob/main/Experiment%203-Part%20A/Hamming-op2.PNG?raw=true)
