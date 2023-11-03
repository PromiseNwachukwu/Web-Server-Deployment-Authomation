Step 1: Provision an EC2 instance running ubuntu 20.04. You can refer to the course Implementing load balancer with Nginx for a refresher
Step 2: Open port 8000 to allow traffic from anyhere using the security group. Again refer to the course mentioned above in step one for a refresher.
Step 3: Connect to the webserver via the terminal using SSH cleint
Step 4: Open a file, paste the script above and close the file using the command below:
    sudo vi install.sh

To close the file type the esc key then Shift + :wqa!
Step 5: Change the permissions on the file to make an executable using the command below:
    sudo chmod +x install.sh

Step 6: Run the shell script using the command below. Make sure you read the instructions in the shell script to learn how to use it.
    ./install.sh PUBLIC_IP
