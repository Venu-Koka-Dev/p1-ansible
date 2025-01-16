# Steps
1. To create an AWS EC2 instance
ansible-playbook -v create_ec2_instance_playbook.yml

2. Grant permissions
chmod 400 ansible-ch2.key

3. To configure the EC2 server to run Node app
ansible-playbook -v -i inventory.aws_ec2.yml configure_sample_app_playbook.yml

4. To test:
http://<PUBLIC_IP>:8080
