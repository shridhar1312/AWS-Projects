* Project II: How to Bootstrap Web Server Creation

In this lecture we are going to learn about

1.Bootstrapping

2.What is Bootstrapping

3.How to write Bootstrapping script

4.Convert Project I Step into Bootstrap Script



ubantu-18.06 ami -->working

#!/bin/bash
 sudo apt update -y && sudo apt install -y nginx
 sudo systemctl start nginx

 amazon linux 2 ami

 #!/bin/bash
 sudo yum update -y
 sudo amazon-linux-extras install -y lamp-mariadb10.2-php7.2 php7.2
 sudo yum install -y httpd
 sudo systemctl start httpd


 amazon linux 2 ami--->Working

 #!/bin/bash
yum update -y
yum install -y httpd
echo '<h1>Hello World</h1>' > /var/www/html/index.html
systemctl start httpd
systemctl enable httpd


Document link on Bootstrap:-

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/user-data.html

Document laink on Instance-metadata

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-metadata.html
