# CMPE-272_HW1_Ansible - Team AlphaGo

Steps:-

1. Create two VM instances

2. Install Ansible on your local machine and set up password less authentication for the two VMs

3. Try to do SSH from your local machine without Key pair authentication

4. Create inventory file on your local machine to make it control node and the two VMs as manged node

5. Create a yaml file on your local machine which will be the playbook containing the two plays to deploy or undeploy webserver

6. Run the below command with correct tag(to deploy or undeploy):-

     ansible-playbook -i inventory.ini webserver.yml --tags deploy
   

7. Run the curl command or browse to http://VM1_ip:8080 and http://VM2_ip:8080 to verify the expected html content.

8. Run the below command to undeploy the web server :-

     nsible-playbook -i inventory.ini webserver.yml --tags undeploy

