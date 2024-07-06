## DevOps Intern Challenge Question

### The Challenge

Set up a highly available web application on GCP using K3s. The application is written in Python and requires a PostgreSQL database. The application should be accessible via a custom domain name.

### Your task is to:

1. Create a K3s cluster with High Availability Embedded etcd for fault-tolerant.
2. Deploy the Python web application to the K3s cluster using Helm charts. The app should connect to a PostgreSQL database.
3. Set up a PostgreSQL database in GCP and configure the app to connect to it.
4. Configure DNS to point a custom domain name to the K3s cluster's load balancer IP.
5. Write a Python script to automate the entire setup process. The script should:
    - Create the GCP nodes and K3s cluster
    - Deploy the app and database
    - Configure DNS
6. Document the architecture and steps in a README file.

### Bonus points for:
- Using Terraform or Pulumi to provision GCP nodes.
- Implementing SSL/HTTPS for the web app
- Monitoring and logging set up for the cluster

Please provide the Python script, Helm charts, and documentation in a GitHub repo. Be prepared to walk through your solution and discuss the architecture and technologies used.
