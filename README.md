# Serverless Registration Form : AWS LAMBDA PROJECT
===================================================

## Step 1: Create DynamoDB Table

```sh
Table Name: registration-table
Partition key: email
create table

```

add email value :- 1 (any value)

create Item :- name , phone , password ( all string )
## Step 2: Create IAM Role for Lambda Function
```sh
IAM Role Name: RegistrationFormRole

Permissions:
1. CloudWatch Full Access
2. DynamoDB Full Access

```

## Step 3: Create Lambda Function

```sh
Function Name: registration-form-function
Runtime: Python 3.9

```

## Step 4: Write Lambda Function

upload your code inside lambda and click deploy

## Step 5: Create API Gateway

Go to REST api and click build

select new api and define your api name :- " registration-api "

create api

create resource

define resource name :- " register "

enable CORS and create resource

create method

method type :- " post "

integration type :- "lambda function"  // select your own lambda function

click on " /register " and then enable CORS

Access-Control-Allow-Methods :- " select POST & OPTION " and save

deploy api ( new stage -->  stage name (prod) ----> deploy

copy your invoke url and paste it on your script.js

## Step 6: Create website by using s3 and deploy your content

upload your index.html and script.js

## Step 7: Test the Application


=======================END=================================


