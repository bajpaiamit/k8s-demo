# k8s-demo
Setup a flask application
file added app.py
*******
Create a DockerFile
Added DockerFile
************
Updated and added requirmentent.txt
*************
Generate a self-signed SSL certificate with below command

openssl req -x509 -newkey rsa:4096 -nodes -out cert.pem -keyout key.pem -days 365

**************
Build and Run Docker conatiner with Below command (Make sure all the above files in same Directory)

docker build -t my-app .
docker run -p 5000:5000 my-app

********************************
Adeed Yaml file 
myapp.yml

kubectl apply -f myapp.yml

Application will be deployed with two replicas for high availability and exposed via a LoadBalancer service on port 80.
