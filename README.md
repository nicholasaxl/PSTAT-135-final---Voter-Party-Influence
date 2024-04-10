# PSTAT-135-final---Voter-Party-Influence
UCSB PSTAT 135 - Big Data Analytics final project on the oregon focused US voter dataset 

Created by: Aapthi Nagesh, Alex Roginski, Yuchen Wu, Nicholas Axl Andrian

The folders contain the pdf reports alongside a jupyter notebook.
The dataset used is renamed to "state name" data for ease of access on local machines, make sure to edit the pyspark readdataframe inputs when doing so locally.

Acessing voter files in GCP

gsutil -u ##PROJECT-ID## ls gs://winter-2024-voter-file/

First, create a bucket with an appropriate name under your project. To copy files to your storage bucket, use the following command in the google cloud shell:
gsutil -u ##PROJECT-ID## \
-m cp -r \
gs://winter-2024-voter-file/VM2Uniform/VM2Uniform--WY--2021-01-13 \
gs://##BUCKET-NAME##/

A word of caution, some state’s directory are quite large. For example, the state of California is over 3 GB. (CSV would have been over 30GB)
