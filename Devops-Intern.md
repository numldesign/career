### The Challenge
Write a [FastAPI](https://fastapi.tiangolo.com/) server to create a highly available [K3s](https://k3s.io/) cluster on [Azure Virtual Machine](https://learn.microsoft.com/en-us/python/api/overview/azure/compute?view=azure-python) using just simple API endpoints. Deploy CloudNativePG in the K3s cluster using [Helm charts](https://helm.sh/).

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
