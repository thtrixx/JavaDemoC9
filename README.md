         ___        ______     ____ _                 _  ___  
        / \ \      / / ___|   / ___| | ___  _   _  __| |/ _ \ 
       / _ \ \ /\ / /\___ \  | |   | |/ _ \| | | |/ _` | (_) |
      / ___ \ V  V /  ___) | | |___| | (_) | |_| | (_| |\__, |
     /_/   \_\_/\_/  |____/   \____|_|\___/ \__,_|\__,_|  /_/ 
 ----------------------------------------------------------------- 


Hi there! Welcome to AWS Cloud9!

To get started, create some files, play with the terminal,
or visit https://docs.aws.amazon.com/console/cloud9/ for our documentation.

Happy coding!

Để chạy code trên Cloud9
Install java 8 on cloud 9:
+ Update công cụ: sudo yum -y update
+ Cài đặt OpenJDK 8: sudo yum -y install java-1.8.0-openjdk-devel
-Chuyển hoặc nâng cấp bộ công cụ phát triển Java mặc định lên OpenJDK 
sudo update-alternatives --config java
sudo update-alternatives --config javac
Kiểm tra lại cài đặt với lệnh java –version và javac –version
Install Maven 3 on cloud 9:
Sử dụng cách lệnh sau :
+ sudo wget http://repos.fedorapeople.org/repos/dchen/apache-maven/epel-apache-maven.repo -O /etc/yum.repos.d/epel-apache-maven.repo
+ sudo sed -i s/\$releasever/6/g /etc/yum.repos.d/epel-apache-maven.repo
+ sudo yum install -y apache-maven

Để chạy Maven Project Console ta làm như sau:
cd my-app
mvn compile
java -cp target/classes com.mycompany.app.App

Đối với Springboot JSP ta thực hiện như sau:
cd springboot-jsp
mvn spring-boot:run