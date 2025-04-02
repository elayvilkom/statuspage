# Statuspage Application Deployment with ArgoCD and Terraform

This project deploys a comprehensive statuspage application on an AWS EKS cluster, leveraging ArgoCD for continuous delivery and Terraform for infrastructure provisioning. It provides a robust, transparent system for communicating the health and availability of your services.
---------------------------------------------------------------------------------------------------------------------
## Components:

* **Statuspage:**
    * This is the core application, providing a public-facing dashboard to communicate service health.
    * It displays real-time status updates, incident reports, and scheduled maintenance announcements.
    * In this project, Statuspage is configured to monitor the health of Prometheus, Grafana, and itself.
    * It leverages the RDS PostgreSQL database for persistent data storage, and Elasticache Redis for caching, ensuring performance and reliability.
    * By using statuspage, we provide transparency to our users, and reduce support overhead.
    * It is configured to use the AWS loadbalancer controller to provide an external endpoint.
* **Prometheus:** For monitoring and collecting metrics from the EKS cluster and applications.
* **Grafana:** For visualizing metrics and creating dashboards to monitor system health.
* **AWS Load Balancer Controller:** To manage AWS Load Balancers for ingress, providing external access to the applications.
* **RDS PostgreSQL:** A managed relational database service used by Statuspage for data persistence.
* **Elasticache Redis:** A managed in-memory data store used by Statuspage for caching, enhancing performance.
---------------------------------------------------------------------------------------------------------------------
## Key Statuspage Functionality in this Project:

* **Real-time Monitoring:** Statuspage displays the current health of Prometheus, Grafana, and the Statuspage application itself.
* **Incident Reporting:** In case of service disruptions, Statuspage allows for quick creation and publication of incident reports.
* **Scheduled Maintenance:** Planned maintenance windows can be communicated to users in advance.
* **External Access:** The AWS Load Balancer Controller ensures that the Statuspage dashboard is accessible to external users.
* **Database and Cache:** RDS and Redis provide a stable and performant backend for Statuspage.
---------------------------------------------------------------------------------------------------------------------
## Prerequisites
* git installed
* terraform installed
* aws cli installed 
* eksctl installed
---------------------------------------------------------------------------------------------------------------------  
**Project Structure**

... (rest of your project structure section)
---------------------------------------------------------------------------------------------------------------------
## Deployment Steps 
* Clone our git repository
```bash
    git clone https://
    ```
* Activate terraform -Inside of terraform diractory 
```bash
    terraform apply
    ```
---------------------------------------------------------------------------------------------------------------------

