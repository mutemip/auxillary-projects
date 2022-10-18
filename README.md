# auxillary-projects

This project automates the process of onboarding several users in a server and adding them to a group "developers"

To set up the project follow these steps:
  - mkdir shell && cd shell
  - vi names.csv

Then enter the name of users to be added to the server

create a group "developers"
  - sudo groupadd developers
  
create these files:
  - touch id_rsa id_rsa.pub onboading-users.sh
  
enter the keys in their respective files

Make sure the script is executable by running:
  - sudo chmod +x onboarding-users.sh
  
  Changes From:
  
 ![before](https://user-images.githubusercontent.com/64135078/196560868-c5625dd7-e493-43fc-afce-ad78a9bdfae8.png)
  
  To:
  
![af2](https://user-images.githubusercontent.com/64135078/196562042-06ecfea6-7c67-42b5-aa0a-d0794f3924f7.png)


Then use 
  - sudo su - To switch to root user
 
 and execute the script using:
 - ./onboarding-users.sh
 
 
Name in "names.csv" file:
![names](https://user-images.githubusercontent.com/64135078/196562286-8d0e8c73-74e0-4d38-90d2-cc698458b56f.png)

After executing the script, check available users in the server
  - ls -l /home
![users](https://user-images.githubusercontent.com/64135078/196562654-5ce844c4-8c26-45de-ba2b-27b0a17ea0ea.png)

Now checking if we can login to the server using any newly added user:
  - vi aux-project.pem and paste the private key provided in it... remember we've already configured public key
 Then change the aux-project.pem using:
  - sudo chmod 600 aux-project.pem 
 
 Trying to log in as timo,  the logging goes successful:
 ![timo](https://user-images.githubusercontent.com/64135078/196564060-441a0ea0-d577-46c6-baf7-48d3d4f8e9ea.png)


 Checking in .ssh dir:
 ![ssh](https://user-images.githubusercontent.com/64135078/196564267-a55ae1ea-880c-462e-b03d-8109365a0371.png)

 checking if he has sudo previleges:
 ![sudo](https://user-images.githubusercontent.com/64135078/196564452-7935c0b8-034c-48f5-95be-ead0c0274985.png)

 
 
 
 

 
 
 





