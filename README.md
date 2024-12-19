Host a Static Website on AWS S3
Step 1: Create an S3 Bucket

1. Access the S3 Console: Log in to your AWS Management Console and navigate to the Amazon S3 Console.
2. Click Create bucket: Locate and click the "Create bucket" button.
3. Enter a Unique Bucket Name: Provide a globally unique name for your bucket: `mybuc123455`.
4. Select a Region: Choose a region close to your target audience for better performance.
5. Uncheck Block All Public Access:
   - Scroll down to the "Bucket settings for Block Public Access" section.
   - Uncheck the "Block all public access" option.
   - Confirm by ticking the acknowledgment checkbox.
6. Create the Bucket: Click the "Create bucket" button to finalize the setup.

Step 2: Upload Website Files

1. Select Your Bucket: From the list of buckets, click on `mybuc123455`.
2. Click Upload: In the bucket view, click the "Upload" button.
3. Add Your Files:
   - Drag and drop your static website files (e.g., `index.html`, `style.css`, etc.) into the upload area, or use the "Add files" button.
4. Start the Upload: After verifying your files, click the "Upload" button to start the process.

Step 3: Configure the Bucket for Static Website Hosting

1. Navigate to the Properties Tab:
   - Inside your bucket, go to the "Properties" tab.
2. Enable Static Website Hosting:
   - Scroll down to the "Static website hosting" section and click "Edit."
   - Select the "Enable" option.
3. Specify Index and Error Documents:
   - Enter the name of your index document (e.g., `index.html`).
4. Save Changes: Click the "Save changes" button to enable static website hosting.

Step 4: Make the Files Public

1. Go to the Permissions Tab:
   - Navigate to the "Permissions" tab of your bucket.
2. Edit the Bucket Policy:
   - Scroll down to the "Bucket policy" section and click "Edit."
   - Copy and paste the following JSON policy, replacing YOUR_BUCKET_NAME with `mybuc123455`:
![Screenshot 2024-12-15 212707](https://github.com/user-attachments/assets/a5272c0a-0b8d-45a9-b48d-e6aeaa19e949)

   - Save the changes by clicking "Save changes."

Step 5: Access Your Website

1. Locate the Website Endpoint:
   - Return to the "Properties" tab of your bucket.
   - Scroll down to the "Static website hosting" section.
   - Copy the "Endpoint" URL (e.g., `http://mybuc123455.s3-website-us-east-1.amazonaws.com`).
2. Test Your Website:
   - Paste the endpoint URL into a web browser to view your hosted static website.

