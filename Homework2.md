# CSC0056 Data Communication, Homework 2

Submit your work before 9AM, Oct 26th. Clearly label your answer.

#### 1. Layered Networked Architecture (10%)

1a. (10%) Explain two benefits of designing a network architecture in layers. Five points each. Explain your answer in no more than 200 words per benefit. 

 

#### 2. Error Detection using Parity Checks (40%)

2a. (5%) Explain why using the single parity check we may detect any odd number of errors.



2b. (5%) Using the single parity check, the probability that a random bit string will be accepted as error-free is 50%. Explain why it is 50%.



2c. (5%) Consider the horizontal and vertical parity checks, and suppose we have seven data bits per row. Draw an example where the data bits contain six errors as a whole and that these errors *cannot* be detected by the horizontal and vertical parity checks. You should draw your answer in a way similar to that of Figure 2.14 on page 59 in the textbook.



2d. (5%) Using CRC, if the generator polynomial is of degree 4, what would be the resulting number of parity checks? Explain your answer.



2e. (10%) Using CRC with generator polynomial $g(D)=D^2+1$, what is the minimum distance of the code, if the number of data bits is three?



2f. (10%) Using CRC with generator polynomial $g(D)=D^2+1$, what is the code word with respect to data bits $(11101)_2$ ?



#### 3. Hamming Code (25%)

3a. (5%) When determining the Hamming weight of a linear code, why can we ignore the all-zero code word?

3b. (20%) Consider the following standard generator matrix: $\begin{pmatrix}100110\\010001\\001101\end{pmatrix}$

   3b1. (5%) What is the Hamming weight of this linear code? Explain your answer.

   3b2. (10%) Suppose the received bit vector is $(101110)_2$. Use the nearest-neighbor rule to determine the original data.

   3b3. (5%) Give an example showing that in this case we cannot correctly correct a two-bit error using the nearest-neighbor rule. Explain your example.



#### 4. Data Retransmission Strategies (25%)

4a. (15%) The caption of Figure 2.19 on page 67 in the textbook says that Node A cannot tell whether the second Ack is for packet 0 or 1. The figure illustrates the first case, where the second Ack is for packet 0. Now, answer the following three questions:

  4a1. (5%) Draw an example to illustrate the second case, where the second Ack from Node B is lost and the second Ack that Node A received is for packet 1.

  4a2. (5%) In the case illustrated in the original figure, can Node A tell whether that *Nak* is for packet 1 or 2? Explain your answer.

  4a3. (5%) In the case illustrated in the original figure, could it be possible that that *Nak* is actually for the *second* packet 0? If you think the answer is no, explain; if you think the answer is yes, modify the figure to illustrate that case.



4b. (5%) For the working version of the stop-and-wait ARQ, assuming that Node A sends packets to Node B in sequence, draw a scenario where (1) the first packet 0 was lost, (2) the acknowledgement for the first packet 1 was lost, and (3) the first packet 2 was corrupted. Include all of the three troubles in your scenario.



4c. (5%) Refer to slides 10-12 in Lecture04. Suppose that $q=80\%$. To make $T_2\leq 1.1T_1$, what is the maximum value of $T_{to}$? Represent $T_{to}$ as a function of $T_1$.



#### 5. Tracing Code in Mosquitto

I think the first four sections are enough for Homework 2. We will work on code tracing sometime later.