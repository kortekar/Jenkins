# Deploying Kubernetes Deployment in GCP

To deploy a Kubernetes deployment (`deployment.yaml`) to a Google Cloud Platform (GCP) Kubernetes cluster, you can use the following steps:

 **Activate Service Account**: Activate the service account using the following command. Replace `/path/to/service-account-key.json` with the actual path to your service account key file:

   gcloud auth activate-service-account --key-file=/path/to/service-account-key.json
