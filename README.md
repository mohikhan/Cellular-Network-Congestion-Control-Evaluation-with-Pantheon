# Cellular-Network-Congestion-Control-Evaluation-with-Pantheon

Pantheon is a platform that is open to the public and created to aid in the study and creation of Internet congestion control schemes. 
With a variety of network settings and scenarios, Pantheon offers a platform for evaluating congestion management methods under controlled circumstances. 
It includes a suite of realistic network conditions that emulate a variety of Internet paths, as well as a set of metrics for evaluating the performance of congestion control algorithms. 
By providing a standardized platform for evaluating congestion control algorithms, Pantheon enables researchers and developers to compare the effectiveness of different approaches and improve the overall quality of Internet congestion control.


> Install pantheon following the link - https://github.com/StanfordSNR/pantheon

> **Note**
> Pantheon only runs in Ubuntu 18.04



> In our specific scenario, we've implemented Pantheon both on our local computer and on a remote EC2 server.


Scripts below to run the Pantheon

`cd pantheon`

`python src/experiments/test.py remote --schemes "cubic"  ubuntu@{ec2_ip_address}:/home/ubuntu/pantheon --data-dir /home/{your_username}/pantheon/ -f 1 --interval 10 --run-times 2`

`src/analysis/analyze.py --data-dir /home/{your_username}/pantheon/`


