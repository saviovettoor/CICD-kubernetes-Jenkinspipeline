CICD-Kuberenetes+Jenkinspipeline
================================
```
Jenkins Plugins: git,Kubernetes Continuous Deploy, Multibranch pipeline
Setup Credentials for Github (kind: username and password),Dockerhub(kind: username and password) and Kubernetes (kind: Kubernetes configuration(kubeconfig))
	Credentials ->Global credentials -> Add Credentials
	Kubernetes configuration(kubeconfig): ID - <kubeconfig> #this will be refered in our jenkinsfile
	  Kubeconfig [x] Enter Directly # get the entire kubeconfig file from kube master node ~/.kube/config and paste here.
```

The following pipeline will deploy the sample javaapp to the kuberntes cluster.<br>
The application will be accessible on port 8080.
