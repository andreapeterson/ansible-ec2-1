# ansible-ec2-1
Using Ansible to create key pair and EC2 instance. 

By running Ansible, it will create a key pair then subsequently create an EC2 instance using the same key pair it just generated. I set 'wait' equal to true and 'state' equal to running so Ansible will wait until the instance is running to finish the output. In addition, I set 'exact_count' equal to 1, so Ansible will maintain the state of just 1 instance, and not creating one everytime the playbook is ran. 

Before running the playbook, I created an IAM user for Ansible and stored key credentials in the control machines .bashrc file.
Additionally, I installed pip then used pip to install boto3 so my playbook could run smoothly.

<img width="1487" alt="Screenshot 2024-01-25 at 3 53 19 PM" src="https://github.com/andreapeterson/ansible-ec2-1/assets/134665743/40da2808-c2de-4cab-b04a-36e95aee6415">
