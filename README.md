# Hosting an E-commerce Website Using Amazon CloudFront

## Steps to Perform:

1. **Upload Website Files to S3 Bucket**  
   - Upload `index.html` and `style.css` files to an S3 bucket.

2. **Configure S3 Bucket Permissions**  
   - Navigate to the **S3 bucket settings**.
   - Under the **Permissions** tab, locate the **Block public access settings** and ensure public access is blocked.

3. **Set Up an S3 Bucket Policy for CloudFront**  
   - Click on **Bucket Policy** and apply the policy specified in `s3_policy_cloudfront`.

4. **Create a CloudFront Distribution**  
   - Navigate to the **CloudFront Console** and create a distribution.

5. **Configure CloudFront Origin Settings**  
   - Under the **Origin** section, perform the following steps:
     - Set the **Origin Domain Name** to your S3 bucket.
     - Set **Origin Access** to **Origin Access Control (OAC)**.
     - Click **Create Control Setting** and attach it to your S3 bucket.

After completing these steps, your e-commerce website will be successfully hosted using CloudFront, ensuring enhanced performance and security.

