# auxillary-projects

This project automates the process of onboarding several users in a server and adding them to a group "developers"

To set up the project follow these steps:
- mkdir shell && cd shell
- vi names.csv

Then enter the name of users to be added to the server

create a group "developers"
  sudo groupadd developers
  
create these files:
  touch id_rsa id_rsa.pub onboading-users.sh
  
enter the keys in their respective files

Make sure the script is executable by running:
  sudo chmod +x onboarding-users.sh
  
  Changes From:
  
 ![before](https://user-images.githubusercontent.com/64135078/196560868-c5625dd7-e493-43fc-afce-ad78a9bdfae8.png)
  
  To:
  
![after](https://user-images.githubusercontent.com/64135078/196561092-51f7c486-12cb-4093-94b8-dcac4e876ace.png)

Then use 
  sudo su - To switch to root user
 
 and execute the script using:
  ./onboarding-users.sh
 
