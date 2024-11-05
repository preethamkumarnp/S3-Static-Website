# S3-Static-Website
This project demonstrates how to host a static website using AWS Simple Storage Service (S3). By leveraging S3’s static website hosting feature, you can easily deploy a website with minimal cost and effort.

# Step-by-Step Guide
Follow these steps to host your static website on AWS S3:

1. On your AWS console, search for “S3” on the search bar and select “S3” when it appears

   ![Screenshot 2024-11-05 171211](https://github.com/user-attachments/assets/1105256e-74c8-4915-a721-672ea5efee34)

2. Click on “Create bucket”
   
     ![Screenshot 2024-11-05 171228](https://github.com/user-attachments/assets/030b6947-c136-4e76-bad4-6ded1a12884a)
3. Give a “Bucket name” to the bucket. Remember that the name has to be unique compared to all world-wide buckets
4.  Unselect “Block all public access” to allow internet users access to your website
5.   Click on “Create bucket” at the bottom

   ![Screenshot 2024-11-05 171238](https://github.com/user-attachments/assets/85542fa2-8cfc-416b-977a-2016eca8b618)
6.  Once created, view your bucket in the list of buckets and select it
7.   Under the “Properties” tab,

  ![Screenshot 2024-11-05 171251](https://github.com/user-attachments/assets/c5622240-293e-43c4-a885-7278bbf5e3a5)
8. Click on “Enable” , and then select “Host a static website”. Choose the default home page of your site (the document in the bucket that acts as the homepage). Enter the names of the index document and the error document. The index document acts as the homepage while the error document is returned when there is an error. The error document is not compulsory.Click “Save changes”

   ![Screenshot 2024-11-05 171314](https://github.com/user-attachments/assets/9392ccf4-a2e5-4ede-9b0c-fc6759bc355f)
9. Once “Static website hosting” is enabled, the bucket endpoint is created.
    
   ![Screenshot 2024-11-05 171303](https://github.com/user-attachments/assets/5b1fb046-a0ad-46b5-9520-f1f6c3dab0a5)
10.  Next we need to create a bucket policy to enable access to the files. Navigate to the Permissions tab and under the “Bucket policy” section, enter the following policy
     Ensure to change the Resource to your bucket’s arn, followed by “/*”

  ![Screenshot 2024-11-05 171342](https://github.com/user-attachments/assets/bb622776-3cd7-46a0-9c63-d1f884a506f4)

13.  Create and upload your website files. Note that you need to have the “index.html” (name specified in step (8)as the index document)      
  ![Screenshot 2024-11-05 171401](https://github.com/user-attachments/assets/b1074da4-ce5a-425b-82e2-54fd9bd72f63)

14. Copy the link provided by aws and paste it on the Browser and can see that your Website is Hosting
    ![Screenshot 2024-11-05 171322](https://github.com/user-attachments/assets/701026c4-a938-4341-8ee3-6135b638ec3f)
