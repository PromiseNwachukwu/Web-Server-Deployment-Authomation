
# Automation of the Deployment of Webservers
## Deploying and Configuring the Webservers
#### Step 1: Provisioning 2 EC2 instance running ubuntu 20.04. 
![Screenshot from 2023-11-09 22-59-56](https://github.com/PromiseNwachukwu/Web-Server-Deployment-Authomation/assets/109115304/c9083e88-7187-49f4-b873-57af6f57a2a0)

#### Step 2: Open port 8000 to allow traffic from anyhere using the security group.
![Screenshot from 2023-11-09 23-36-51](https://github.com/PromiseNwachukwu/Web-Server-Deployment-Authomation/assets/109115304/35cf84fd-82ba-4be8-ba03-e97c191a2be2)
![Screenshot from 2023-11-09 23-37-52](https://github.com/PromiseNwachukwu/Web-Server-Deployment-Authomation/assets/109115304/6a517374-bf17-4a02-a231-227065f51d48)

#### Step 3: Connect to the webserver via the terminal using SSH cleint
![Screenshot from 2023-11-09 21-57-15](https://github.com/PromiseNwachukwu/Web-Server-Deployment-Authomation/assets/109115304/6ecba3df-94d5-414a-81e2-5be593a29697)

#### Step 4: Open a file, paste the script above and close the file using the command below:
    sudo vi install.sh
To close the file type the esc key then Shift + :wqa!
![Screenshot from 2023-11-09 22-48-22](https://github.com/PromiseNwachukwu/Web-Server-Deployment-Authomation/assets/109115304/ec017b4b-e1db-4499-8042-57e03299340e)

#### Step 5: Change the permissions on the file to make an executable using the command below:
    sudo chmod +x install.sh
![Screenshot from 2023-11-09 22-12-41](https://github.com/PromiseNwachukwu/Web-Server-Deployment-Authomation/assets/109115304/11b70e4c-0f5e-4da5-86a6-611040f31d28)

#### Step 6: Run the shell script using the command below. Make sure you read the instructions in the shell script to learn how to use it.
    ./install.sh PUBLIC_IP
![Screenshot from 2023-11-09 22-53-20](https://github.com/PromiseNwachukwu/Web-Server-Deployment-Authomation/assets/109115304/744a3c21-f058-4420-be5a-0564142a1e68)

# Deployment of Nginx as a Load Balancer using Shell script
## Automate the Deployment of Nginx as a Load Balancer using Shell script
## Deploying and Configuring Nginx Load Balancer

### Steps to Run the Shell Script
#### Step 1: Provision an EC2 instance running ubuntu 22.04, open port 80 and connect to terminal.
![Screenshot from 2023-11-09 22-59-04](https://github.com/PromiseNwachukwu/Web-Server-Deployment-Authomation/assets/109115304/e1e9300c-dc1c-4cfa-af64-2f6cf1986437)
![Screenshot from 2023-11-09 22-59-56](https://github.com/PromiseNwachukwu/Web-Server-Deployment-Authomation/assets/109115304/c4b7046f-6b6a-426b-ad22-f53e147b1415)
![Screenshot from 2023-11-09 23-03-16](https://github.com/PromiseNwachukwu/Web-Server-Deployment-Authomation/assets/109115304/79b341ef-feab-493b-b45c-0e4b74acca56)

#### Open a file nginx.sh using the command below:
sudo vi nginx.sh

#### Step 2: Copy and Paste the script inside the file
#### Step 3: Close the file using the command below:
type esc the shift + :wqa!
#### Step 4: Change the file permission to make it an executable using the command below:
sudo chmod +x nginx.sh
#### Step 5: Run the script with the command below:
./nginx.sh PUBLIC_IP Webserver-1 Webserver-2

