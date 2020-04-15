#chasunny/food_service:v1

FROM centos
RUN yum install epel-release -y
RUN yum install java-1.8.0-openjdk -y
RUN yum install wget -y
RUN yum install vim -y
RUN yum install git -y
RUN yum install maven -y
RUN git clone https://github.com/chasunny/allServices.git
WORKDIR allServices/food
RUN mvn clean install
WORKDIR target
EXPOSE 8081
ENTRYPOINT ["java", "-jar", "food-0.0.1-SNAPSHOT.jar"]

