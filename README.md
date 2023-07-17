# Maximum-number-of-handshakes-in-java

Maximum number of handshakes in Java
Here, we will discuss the maximum number of handshakes in java. The given program will find the maximum number of handshakes in a room. Suppose there are N persons in a room. We have to find the maximum number of Handshakes possible. Given the fact that any two persons shake hand only once.

MAximum number of handshakes in Java
Approach :
For the number of handshakes to be maximum, every person should hand-shake with every other person in the room

i.e. all persons present should shake hands.

For the first person, there will be N-1 people to shake hands with
For second person, there will be N -1 people available but as he has already shaken hands with the first person, there will be N-1-1 = N-2 shake-hands
For third person, there will be N-1-1-1 = N-3, and So On…
Therefore the total number of handshake   =   ( N – 1 + N – 2 +….+ 1 + 0 )   =   ( (N-1) * N ) / 2.

Algorithm
For N = 8
handshakes  =  ( (N-1) * N ) / 2  =  ( 8 x 7 )/2  =  28
Print Result
Related Pages
Quadrants in which a given coordinate lies
 
Permutations in which n people can occupy r seats in a classroom
 
Addition of two fractions

Replace all 0’s with 1 in a given integer

Can a number be expressed as a sum of two prime numbers

java program for finding the maximum number of handshakes
Java Code
Run
public class Main
{
	public static void main(String[] args) {
	     //fill the code
    int num = 10;

    int total = num * (num-1) / 2; // Combination nC2

		System.out.println("For "+ num +" people there will be " +total+" handshakes");
	}
}
Output
Maximum number of handshakes for 30 people are 435
