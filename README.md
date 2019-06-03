# wordpress-GCP

To create the Cloud Filestore instance with the fileshare used in the code use something like this:

$ gcloud filestore instances create nfs-server-2 \
      --project=myproject \
      --zone=myzone \
      --file-share=name="NFSvol",capacity=2TB \
      --network=name="default"

See https://cloud.google.com/filestore/docs/creating-instances#create-instance-gcloud for more inforrmation about how to create a Cloud Filestore instance.

