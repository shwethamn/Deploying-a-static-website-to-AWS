Project1: 
Host the static website on S3 (simple storage services)
I have created my personal portfolio website using html, css and JavaScript codes.
Hosting a static webpage using Amazon S3 (Simple Storage Service) is straightforward and involves a few key steps. Here's a step-by-step guide to get you started:
Prerequisites:
1.	AWS Account: Ensure you have an AWS account. If not, sign up at AWS.
2.	AWS CLI or Management Console: You can perform these steps using the AWS Management Console or AWS CLI.
Step 1: Create an S3 Bucket
1.1.	Log in to the AWS Management Console:
o	Navigate to AWS Management Console.
 

o	Sign in with your AWS credentials.
 

 


1.2.Create a New S3 Bucket:
•	In the search bar, type S3 and select it.
 

•	Click Create bucket.
 
 

•	Provide a unique name for the bucket. This name must be globally unique across all AWS users.
•	 Choose a region closest to your target audience.
•	 Keep the rest of the options at their default settings for now.
•	 Click Create bucket.
 
Step 2: Upload Your Static Website Files
 2.1. Navigate to Your S3 Bucket:
•	In the S3 dashboard, click on the bucket you just created.
 
 
Upload Files:
•	Click the Upload button.
 
•	Add your website files (e.g., HTML, CSS, JavaScript, images, etc.) by either dragging them into the browser window or using the Add files option.
 
•	Click Upload to upload the files.
 

Step 3: Make the Bucket Public
Since you're hosting a public static webpage, you need to make the bucket's contents publicly accessible.
1.	Bucket Policy:
•	Go to the Permissions tab of your S3 bucket.
 
•	Click on Bucket Policy.


•	Add the following policy to make your content publicly accessible

 
 

2.	Enable Static Website Hosting:

•	In the Properties tab of your bucket, scroll down to Static website hosting.
 
•	Enable static website hosting.

 

•	Set Index document to index.html (or the main file of your website).

•	Set Error document to error.html (optional but recommended for handling errors).

•	Click Save changes.
 

Step 4: Access Your Website
After enabling static website hosting, S3 provides a URL for your hosted website.
1.	Find the S3 URL:
•	In the Properties tab, under Static website hosting, you'll see an endpoint URL like
 
•	Use this URL to access your hosted static website.
 
