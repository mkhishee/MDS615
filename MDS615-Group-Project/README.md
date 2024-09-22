Code Documentation

1. JavaScript Navigation

The application employees “JavaScript” to manage the “ Home, Calendar, Music Player, and Photo Upload” menu based on users’ choice.

Explanation:

Purpose: provides users with options between the “Home, Calendar, Music Player, and Photo Upload” sections. When one section is chosen, the non-used parts are hidden.

Key Functionality: “The addEventListener” uses link navigation, providing the chosen content is displayed.



2. Calendar Functionality

The Calendar function allows the users to update events based on the current month. Also with option to navigate between months while managing event data.

Explanation:

Purpose: manages the calendar’s function, enabling  users to move between months and organize events.

Key Features: The calendar shows the dates with the event and option to change the  months.

3. Music Player Functionality

It supports the most popular audio formats, allowing users to upload and play their music files and has the control features such as play, pause, next, previous, and volume adjustment.

Explanation:

Purpose: provides  music file upload, playback control, and volume adjustment functions.

Key Features: Most commonly used music formats  navigation through the uploaded playlist is included.



4. Photo Upload Functionality

The option of uploading and displaying of photos before they are saved is provided for the users. Personal experience has also been improved through this feature since users receive real-time previews of the images they upload.

Explanation:

Purpose: Enables users to upload image files and also display the image in the form of a gallery for the users to preview.



Key Features: Users are also able to upload more than one image as well as they are able to see even previews of the images real time.



AWS S3 Deployment

The application has been deployed using Amazon Web Services (AWS) Simple Storage Service (S3). AWS S3 is a cloud-based hosting service which offers high-performance and flexible storage for static content and making it suitable for a site like this web scaffold.

Steps to Deploy on AWS S3

Create an S3 Bucket:

Navigating to S3. section

Creating bucket and by naming it, and ensure the bucket is set to Public for static website hosting.

Static Website Deployement:

In Properties section enabling the  Static website hosting.

Upload Files:

Upload all the project files (HTML, CSS, JavaScript) into the S3 bucket.

Ensure the files are set to public-read for access via a web browser.

Access the Application:

Once the files are uploaded, the application is accessed via the provided S3 URL.

During this process it could not accessed through the link, so a code was used in the Bucket policy of the Permission section. This code  is a JSON document that defines permissions for accessing the objects in the bucket, giving permission to public access.

Also, another code was deployed in a Cross-Origin Resource Sharing (CORS) in the bucket. which controls the access to resources located out of the domain from which the request created. 