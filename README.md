# Jenkins_Project
I am practicing the devops. In this project I'm gonna use AWS ubuntu instance for installing jenkins.  Going to do the below steps-  Install Jenkins on ec2 , Configure Jenkins and expose to outside world , Use Docker as Agents against the VM approach  , Advantages of using Docker as Agents, GitOps appraoch to deploy applications on to k8s.
1) After succesfully creation on AWS EC2 instance we need to  install java vesion which is compatible with the jenkins. I we install java older version jenkins will give error. We can check the error in below directory mostly- /var/log/jenkins/jenkins.log.
2) After sucessfully running when we try to connect in browser it will give error. For the solution we need to set inboud rule. follow below steps- Click on instance which is running. Go to Security - click on Security Groups- Edit inbound rules - Add rule select Custom TCP in type - enter port 8080 Select ipv4 and save it. After this you will be able to access jenkins through browser. To view password use the given path enter in cmd of instance cmd- sudo cat (path).
3) On browser page click on Install suggested plugins. Enter the details and save continue.
4) Next step is installing docker on EC2- sudo apt install docker.io
5) 
