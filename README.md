# Commands to deploy spring boot using docker in aws EC2-instance

## 1st step
First you have to create a ec2-instance with required security group acoding to your requirement. 

## 2nd step
On the location where Key Pair is saved, open terminal and type the following command.
  cd ~/my-aws-key-pairs</br>
  chmod 400 my-ec2-key-pair.pem</br>
  ssh -i my-ec2-key-pair.pem ec2-user@<EC2-INSTANCE-PUBLIC-IP-ADDRESS></br>

