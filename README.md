# Infra_project
The final project for big data infrastructure course by **Hamid Reza Taremian**

# Setting up google cloud platform
### 1. First we need to set up a **bucket** to have a storgae for our proejct
![bucket for our project](images/bucket.jpg)
### 2. Then we need to make a cluster for our project using command shell which will allow jupyter notebook using the followinf command:
      gcloud beta dataproc clusters create infra_projcet \
    --optional-components=ANACONDA,JUPYTER \
    --image-version=1.3 \
    --enable-component-gateway \
    --bucket infra_project \
    --project big-data-infrastructure-pro

![running jupyter notebook on a cluster](images/shell_commad_cluster.jpg)

### 3. Now we can have access to jupyter notebook to write our code

![jupyter note book in cluster webservices](images/jupyter.jpg)


# The python+spark code
..* our data consists of one CSV file for the information related to the each station and CSV files for monthly rides. so first we upload our files into the bucket that we made before.

![bucket with CSV files](images/file_saved_uploaded_bucket.jpg)
