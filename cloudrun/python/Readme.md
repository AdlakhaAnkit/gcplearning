Build your container image using Cloud Build, by running the following command from the directory containing the Dockerfile:

gcloud builds submit --tag gcr.io/PROJECT-ID/helloworld

where PROJECT-ID is your GCP project ID. You can get it by running gcloud config get-value project

To deploy the container image:

Deploy using the following command:

gcloud beta run deploy --image gcr.io/PROJECT-ID/helloworld --platform managed
