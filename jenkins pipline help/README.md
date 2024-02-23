# Deployment to Kubernetes in GCP through CLI 
### ✍🏻👨🏻‍💻 you can use it inside jenkins pipelines

#### ❄️ To deploy a Kubernetes deployment (`deployment.yaml`) to a Google Cloud Platform (GCP) Kubernetes cluster :

 ### ✅ **Activate Service Account**: Activate the service account using the following command. 
 ❗️ Replace `/path/to/service-account-key.json` with the actual path to your service account key file:
 
         gcloud auth activate-service-account --key-file=/path/to/service-account-key.json
 
  
### ✅ **Authenticate with the Cluster**: Authenticate with the Kubernetes cluster using the following command. 
❗️ Replace CLUSTER_NAME, REGION, and PROJECT_ID with your cluster name, region, and project ID:

      gcloud container clusters get-credentials CLUSTER_NAME --region REGION --project PROJECT_ID

### ✅ Apply Deployment: Apply your deployment.yaml file to the Kubernetes cluster using the following command. 
❗️ Replace deployment.yaml with the actual path to your deployment file:

      kubectl apply -f deployment.yaml
