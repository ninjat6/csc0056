# CSC0056 Data Communication, Homework 3

* **IMPORTANT**:
  * Submit your answer of "Part 1" before 9PM, Nov 6th (Friday). Clearly label your answer.
  * Submit your answer of "Part 2" before 9PM, Nov 12th (Wednesday).
  * We will have the midterm exam on Nov 9th, in class.



#### Part 1: Writing Tasks (60%)

1. (20%) Basics of the discrete-time Markov chain (DTMC):

   A networking server is either busy or idle. If it is currently busy, with 80% probability it will be busy at the next time step; if it is currently idle, with 60% probability it will be idle at the next time step; but after the server remains idle for three consecutive time steps, at the next time step it will perform some  garbage collection and thus will be busy.

   1. (5%) Draw the DTMC diagram. There are four states in total.
   2. (5%) State the transition probability matrix (please use the format introduced in this course).
   3. (10%) Compute the limiting probability for each state.

2. (15%) The exponential distribution and its memoryless property:

   1. (10%) Suppose that a system has three servers, and that packet $P$ arrived at the system when all the servers were processing some other packets. Assume that (1A) all packets have independent, identical, exponential distribution of service time, (1B) packet $P$ is the only one waiting in the system (the other three packets are being processed), and (1C) packet $P$ will start being processed right after any of the servers is available. Among this four packets, what is the probability that packet $P$ will be the last to complete the process? 
   2. (5%) Following the above question, what is the average time packet $P$ will spend in the system, assuming that the average service time is 30 milliseconds?

3. (25%) M/M/1 system, with arrival rate $\lambda$ and service rate $\mu$:

   1. (5%) Explain in your own word, conceptually, why we have $p_n\cdot\lambda=p_{n+1}\cdot\mu$ for the corresponding continuous-time Markov chain.
   2. (10%) Suppose $\lambda=44$ packets/second and $\mu=50$ packets/second. What would be the steady-state probability that there are 10 packets in the system?
   3. (10%) Now let's consider the end-to-end delay in delivering a packet, where this M/M/1 queue sit on the end-to-end delivery path. Suppose a networking application's service-level agreement (SLA) demands an end-to-end delay of no more than 100 milliseconds. If we know that each packet will take no more than 35 milliseconds to reach this M/M/1 system from the sender, and it will take no more than 40 milliseconds for the network to forward a packet from the output of the system to the destination. Suppose service rate $\mu=0.25$ packets/millisecond for this system. Determine the range of admissible arrival rate to this system so that such a configuration can meet the SLA of 100 milliseconds. 



 

#### Part 2: Programming Tasks (40%)

This part will be available on the evening of Nov 1st (Saturday) and the submission deadline is 9PM, Nov 12th.

To download and manage the content, we recommend to use `git` the fast version-control tool: https://git-scm.com/about 

Tutorial: https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

In short, to install git:

`$ sudo apt-get update`

`$ sudo apt-get install git`

To download Part 2 of this homework (Do this after Nov 1st):

`$ git clone https://github.com/wangc86/mosquitto.git`

Then follow the README_hw3.md in the cloned repository to complete Homework 3.