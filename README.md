# Deploy Web app on AWS S3 Using Github Actions


![download](https://github.com/Pavithra1640/Handtime-webapp-project/assets/165140491/7f4c1f03-98d6-41a5-b210-7ac85d01f975)

- **What is Github Actions?**
- Github actions is powerful continuous integration and continuous deployment (CI/CD) platform provided by GitHub.it simplifiles the process of building,testing and deploying code directly-from the github repositories.
- to create workflow in Github Actions,you can use the YAML-based configuration file.Each step represents a task,such as building your code,running tests or deploying it to a server.
- By using the github actions you can define your workflow in a simple and straightforward manner.
- **Now, Let's Begin the Deployment Process !!! **
- **Step 1: Create a New Repository in Github**
- **Step 2: Add and Commit Code to GitHub Repository**
     - Once the repository is created, Use the git commands to commit the code and push it to your GitHub repository
- **Step 3: Create an S3 Bucket**
 - AWS Management Console and create an S3 Bucket.Remember to select a region for the bucket. Also allow public access.
- **Step 4: Configure Bucket Policy for Public Access**
    - To allow public access to the objects in your S3 Bucket, you need to set up a bucket policy.Navigate to the bucket's properties, select "Permissions," and click on "Bucket Policy." Add the following policy
    ![s3bucket policy](https://github.com/Pavithra1640/Handtime-webapp-project/assets/165140491/03941175-8b9d-40b6-9aa5-5a04c1ac3df5)
 - **Step 5: Create an IAM User and Generate Security Credentials**
        -    Assign the necessary IAM policies to this user, allowing access to S3 and any other services 
             required for your deployment
        -   Generate the IAM User's access key and secret key, as we will need them later to configure GitHub 
            Secrets.
 - **Step 6: Set Up GitHub Secrets for AWS Credentials**
        - Go to your GitHub repository, click on "Settings," then "Secrets." go to actions Here, click on "New Repository Secret"  to add your AWS access key and secret key as secrets 
          named AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY, respectively
   
   ![github credential](https://github.com/Pavithra1640/Handtime-webapp-project/assets/165140491/72710edf-6d41-41f9-9b15-38bdd085605d)

- Step 7: Create the GitHub Actions Workflow
      - In your GitHub repository, navigate to the "Actions" tab and click on "Set up a workflow yourself."
       - Create a new file named .github/workflows/main.yml
  
![main yaml file](https://github.com/Pavithra1640/Handtime-webapp-project/assets/165140491/933b12c8-0dc3-479c-b4f3-707a4732f2fe) 
 
- **Step 8: Commit Changes and Trigger Deployment**
- **Step 9: Enable Static Website Hosting for the S3 Bucket**
- **Step 10: Access Your Portfolio Website 🌐**
- 
  ![final output](https://github.com/Pavithra1640/Handtime-webapp-project/assets/165140491/90369160-2e7e-4eef-bf3c-3d0f792324b3)

  ![finalo](https://github.com/Pavithra1640/Handtime-webapp-project/assets/165140491/e3591f7d-5c72-4706-9d7d-55b2fed54d63)

