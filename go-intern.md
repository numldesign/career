### Objective
The objective of this assignment is to develop a simple file upload server using GoLang that supports concurrency and integrates with NGINX to handle multipart uploads for Git Large File Storage (LFS).

#### GoLang Server
- Create a GoLang HTTP server that can handle multipart file uploads.
- Implement concurrency using Goroutines to manage multiple file uploads simultaneously.
- Store uploaded files in a designated directory on the server.

> Tip: Consider performing the multipart upload directly to object storage without involving the backend. This approach can help you save on compute resources, reduce latency, and simplify the overall process.

#### NGINX Configuration
- Set up NGINX to reverse proxy requests to your GoLang server.
- Configure NGINX to handle multipart/form-data uploads and set appropriate limits on file size.
- Use the nginx-upload-module to manage file uploads efficiently.

#### Multipart Upload Handling
- Implement the logic for handling multipart uploads in your GoLang server.
- Ensure that the server can process large files by splitting them into smaller chunks if necessary, similar to how Git LFS operates.

> Tip: You may also opt to utilize the multipart upload functionality offered by your object storage provider.

#### Git LFS Integration
- Simulate the Git LFS upload process by returning appropriate responses as per the Git LFS API specifications.
- Implement endpoints for initiating uploads and finalizing them, mimicking the behavior of a Git LFS server.

#### Deliverables
- Source code hosted in a GitHub repository.
- An NGINX configuration file demonstrating how to set up the reverse proxy for your application.
- A README file explaining how to run your application, including any dependencies and setup instructions.
- Sample commands demonstrating how to use Git LFS with your server (e.g., git lfs push).
- A short video demonstration of the application in action.

#### Evaluation Criteria
- Functionality: The server should successfully handle multipart uploads and respond correctly according to Git LFS specifications.
- Concurrency: The implementation must effectively utilize Goroutines for handling concurrent uploads.
- NGINX Configuration: Properly configured NGINX that routes requests to the GoLang server and handles file size limits.
- Code Quality: Code should be clean, well-documented, and follow GoLang best practices.

#### Additional Resources
- [Git LFS Documentation↗](https://git-lfs.github.com/)
- [AWS S3 Multipart Upload↗](https://docs.aws.amazon.com/AmazonS3/latest/userguide/mpuoverview.html)
- [NGINX Upload Module↗](https://github.com/fdintino/nginx-upload-module)
- [Concurrency in Go↗](https://golang.org/doc/effective_go.html#concurrency)

> Note: The resources provided are for reference only. You are free to select any cloud object storage solution or any other NGINX upload module as a basis for implementing your solution.
