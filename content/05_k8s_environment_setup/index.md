## Kubernetes Environment Set up

### Before we jump into K8s, we want to generate some events​

1. Login to your Bastion Host through Dynatrace University​
2. Run the following command:

    
        kubectl get pods –n easytrade​
        

3. Copy the full name of the "frontend pod" and paste it into the next command​
4. Run the following command: 


        kubectl delete pod frontend-xxxxxxxx-xxxx -n easytrade​


5. Re-run the following command: 


        kubectl get pods –n easytrade  ​

    
* Make sure the pod has been recycled, by re-running step 2. Check the timestamp of the new pod. 

6. Exit the Bastion Host 

