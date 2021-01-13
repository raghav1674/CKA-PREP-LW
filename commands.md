## KUBERNETES COMMANDS:

	1. TO CREATE POD:
	>  kubectl run POD_NAME --image=IMAGE_NAME
	2. TO EXPOSE POD:
	> kubectl expose pod POD_NAME --type=SERVICE_TYPE(NodePort|External|ClusterIP) --port=TARGET_PORT [--nodePort=NODE_PORT]
	3. TO DESCRIBE POD:
	> kubectl describe pod POD_NAME 
	4. TO LIST ALL THE PODS IN DEFAULT NAMESPACE:
	> kubectl get pods [-o : OUTPUT_FORMAT] [wide |json |yaml| text]
	5. TO LIST ALL THE PODS IN DEFAULT NAMESPACE ALONG WITH THE LABELS:
	> kubectl get pods --show-labels
	6. TO LIST THE PODS WITH SPECIFIC LABEL:
	> kubectl get pods -L LABEL(KEY=VALUE)
	7. TO DELETE THE SPECIFIC POD:
	> kubectl delete pod POD_NAME
	8. TO DELETE ALL THE PODS:
	> kubectl delete pod --all
        
	






### TO CREATE A RESOURCE FROM THE YAML FILE:
> kubectl create|apply  -f FILENAME.(yml|yaml)


	
