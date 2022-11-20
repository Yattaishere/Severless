# serverless-hpc



**Serverless FaaS (Function as a Service)** 
Zero wait time, fault tolerant execution of scientific workloads that include popular data processing, classification and computer vision libraries. Both opensource and commercial clouds have been leveraging FaaS capabilities to power microservices and distributed application deployments on cloud. 

With the experimental analysis performed in this project through cloud deployments on Apache Openwhisk and Amazon Web Services (AWS), we gain an insight into real time performance of scientific workloads and their white box behavior in serverless environments. We also simulate a traditional parallel computing architecture that is used in containerized deployments on classical high-performance applications. 

In the current configuration, we have implemented tensorflow image classification for 1000 images in MNIST library. 

Requirements: 

AWS account	N/A \
aws-cli	2.8.4  \ 
Apache openwhisk	1.0.0 \
wsk cli 	1.0.0 \
docker	20.10.17 \
funcx	1.0.4 \
python	3.8 \
TensorFlow 	2.0

Before running the application, make sure: 

Apache Openwhisk Endpoint is available on your computer. 
https://github.com/apache/openwhisk#readme

AWS / WSK cli installation and configuration is complete. 
aws-cli: https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
wsk-cli: https://github.com/apache/openwhisk-cli

AWS credentials are setup.

Docker Daemon is logged in and running. 
https://docs.docker.com/get-started/overview/#:~:text=The%20Docker%20daemon%20(%20dockerd%20)%20listens,daemons%20to%20manage%20Docker%20services.

Funcx is installed: 
https://github.com/funcx-faas/funcX


<img width="1057" alt="image" src="https://user-images.githubusercontent.com/38281651/202928806-98f26947-8efd-4ed7-beb7-7134f53f5663.png">


```
cd ../serverless-hpc 
npm install body-parser express 
node index.js
```
## Results

<img width="717" alt="image" src="https://user-images.githubusercontent.com/38281651/202928716-c30a769f-ed09-4d49-bdab-a4fe72a3d158.png">

