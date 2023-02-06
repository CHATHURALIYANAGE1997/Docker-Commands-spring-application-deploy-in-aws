# Commands to deploy spring boot using docker in aws EC2-instance

## 1st step
First you have to create a ec2-instance with required security group acoding to your requirement. 

## 2nd step
On the location where Key Pair is saved, open terminal and type the following command.</br>
> cd ~/my-aws-key-pairs</br>
  chmod 400 my-ec2-key-pair.pem</br>
  ssh -i my-ec2-key-pair.pem ec2-user@EC2-INSTANCE-PUBLIC-IP-ADDRESS</br>

## 3rd step
Now, go ahead and install Docker</br>
> [ec2-user]$ sudo yum update -y</br>
  [ec2-user]$ sudo yum install -y docker</br>
  [ec2-user]$ sudo service docker start</br>
  
## 4th step
> [ec2-user]$ sudo usermod -a -G docker ec2-user</br>
  [ec2-user]$ exit</br>
> ssh -i my-ec2-key-pair.pem ec2-user@EC2-INSTANCE-PUBLIC-IP-ADDRESS</br>
[ec2-user]$ docker info
