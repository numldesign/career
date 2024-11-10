### The Challenge
Set up a highly available web application on Azure using K3s. The application is written in Next.js and requires a PostgreSQL database (using CloudNativePG). The application should be accessible via a custom domain name.

#### Your task is to:
- Create a [K3s cluster with High Availability using Embedded etcd](https://docs.k3s.io/datastore/ha-embedded?_highlight=hig) for fault tolerance.
- Deploy the [CloudNativePG](https://github.com/cloudnative-pg/charts) to the K3s cluster using Helm charts. The PostgreSQL database should have an HTTP endpoint to connect.
- Configure DNS to point a custom domain name to the K3s cluster's load balancer IP.

#### Automate the entire setup process by writing a script that:
- Creates the Azure nodes and K3s cluster.
- Deploys the PostgreSQL (CloudNativePG) database.
- Configures DNS.
- Document the architecture and steps in a README file.

#### Options for Implementation
- Use Azure SDK directly or Pulumi for provisioning Azure resources.
    - For more information on using the Azure SDK for Python, refer to [Azure SDK for Python](https://learn.microsoft.com/en-us/azure/developer/python/sdk/azure-sdk-overview).
    - For Pulumi, check out [Pulumi Azure Documentation](https://www.pulumi.com/azure/).
- Implement [Ingress Nginx Controller](https://kubernetes.github.io/ingress-nginx/) as a reverse proxy to handle incoming requests and provide SSL termination.
- Implement [Cert Manager](https://cert-manager.io/docs/) to manage SSL certificates.

#### Bonus points for:
- Setting up monitoring and logging for the cluster.

Please provide the automation script, Helm charts, and documentation in a GitHub repository. Be prepared to walk through your solution and discuss the architecture and technologies used.
