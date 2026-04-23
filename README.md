# cloud-run-cicd
Deploy a simple flask application to Cloud Run using CICD pipeline.

GCP Services used
Source Code Repository — To store the source code of the application.
Cloud Build — Build a CI/CD pipeline.
Container Registry — To store the container images.
Cloud Run — To deploy containers.

LAB OVERVIEW
Add Github repository to Source code repository
write a sample python flask application 
Create a cloudbuild.yaml file.
Create a Cloud Build Trigger using Console.
Run the Trigger.

Add **permissions**
gcloud run services add-iam-policy-binding flask-service \
  --region asia-south1 \
  --member="allUsers" \
  --role="roles/run.invoker"
