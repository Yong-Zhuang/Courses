The Homework 1 of CS752 - Yong Zhuang Student ID : 01431919. 

The queue system implemented by these files:

1- main.c: This is the main program that run the threads.
2- queue.h: The code for the queue is iin this file. The queue implemented using the linked list. 

You can compile the code using this command: make queuePThread
With using the help option in the run, the user can find out about the command line options:

The following is the output of M/M/1

******************Results******************
The Queue System has 3 threads, 0 is customer, 1 is statistic, the others for server
Producer generate 1005 customers
Servers process 1001 customers
The mean and standard deviation of the inter-arrival time are: 0.337780 secs, 0.342634 
The mean and standard deviation of customer waiting time time are: 0.747253 secs, 1.001026 
The mean and standard deviation of service time are: 0.252095 secs, 0.246223 
The mean and standard deviation of the queue length are: 2.252038 , 3.347778 
The utilization of the server: Busty time(secs): 252.347209 / Total time(secs): 340.000000 = Utilization: 0.742198 
*******************************************


The following is the output of -N 3 -L 5.1 -M 1.8 :

[user8@gpu1 Homework1]$ make
gcc -Wall -O3 -lm -pthread main.c
[user8@gpu1 Homework1]$ ./a.out
Welcome to the Pthread System, please enter the factors:
-N NumberOfServers(default 1)
3
-L arraival rate: lamda(default 3.0)
5.1
-M service rate: mu(default 4.0)
1.8
-C NumberOfCustomers(default 1000)
1000

******************Results******************
The Queue System has 5 threads, 0 is customer, 1 is statistic, the others for server
Producer generate 1018 customers
Servers process 1003 customers
The mean and standard deviation of the inter-arrival time are: 0.194293 secs, 0.195348 
The mean and standard deviation of customer waiting time time are: 1.417747 secs, 1.384994 
The mean and standard deviation of service time are: 0.534609 secs, 0.520478 
The mean and standard deviation of the queue length are: 7.191420 , 7.193329 
The utilization of the server: Busty time(secs): 536.212984 / Total time(secs): 604.000000 = Utilization: 0.887770 
*******************************************
