# aws-glue-kaggle-etl-s3-data-engineering-project

the project analyses the dataset of trending videos on utube, builds aws glue data catalog, stores metadata on the dataset, and shows some data in athena


![youtube-data-egn](https://github.com/erjan/aws-glue-kaggle-etl-s3-data-engineering-project/assets/4441068/9ab42b9a-cc18-488e-96d2-c5f0de0d3a04)

the dataset is here: https://www.kaggle.com/datasets/datasnaek/youtube-new

1. start ec2, install kaggle api ctl, get kaggle token, upload kaggle.json to ec2 using 'scp - key.pem ubuntu@my_ip.com'; download dataset via kaggle cli using cmd "kaggle datasets download -d datasnaek/youtube-new"

2. create lambda function, include aws wrangler layer (outdated - so use arn from serverless repo com)
3. create s3 buckets, upload the kaggle dataset
4. create data catalog using aws glue - create database, then table - point the crawler to s3 bucket with raw dataset
5. 

