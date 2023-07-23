# Cellular-Network-Congestion-Control-Evaluation-with-Pantheon


Install pantheon following the link - https://github.com/StanfordSNR/pantheon

sudo sysctl -w net.ipv4.ip_forward=1

Here in our use case, we have installed pantheon in our local machine and in Ec2 instance remote server.




`cd pantheon`

`python src/experiments/test.py remote --schemes "cubic"  ubuntu@{ec2_ip_address}:/home/ubuntu/pantheon --data-dir /home/{your_username}/pantheon/ -f 1 --interval 10 --run-times 2`

`src/analysis/analyze.py --data-dir /home/{your_username}/pantheon/`


