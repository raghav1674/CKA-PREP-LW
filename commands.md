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


### PV has three types of RECLAIM POLICY:
   -------------------------------------
	1. RECYCLE:
	   	>if pvc is deleted then pv is released and the data from actual storage is deleted to be used with another pvc.
	2. RETAIN: 
	   	>if pvc is deleted then pv is released but not available to be used any other pvc as the storage is still persistent in the device.
	3. DELETE: 
 	   	>if pvc is deleted the pv will automatically released and then deleted.	
