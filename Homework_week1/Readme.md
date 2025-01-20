# Homework for the first week

### Question 1. Understanding docker first run
Run docker with the python:3.12.8 image in an interactive mode, use the entrypoint bash.
    
What's the version of pip in the image?
   
The answer any can get with the command **pip list** and I'v got **24.3.1**

### Question 2. Understanding Docker networking and docker-compose
Given the following docker-compose.yaml, what is the hostname and port that pgadmin should use to connect to the postgres database?

The answer is **postgres:5433** because name of db container is postgres and first port in ports is the local port of host machine, second one is the container port.

### Question 3. Trip Segmentation Count

### Question 4. Longest trip for each day

### Question 5. Three biggest pickup zones

### Question 6. Largest tip

### Question 7. Terraform Workflow
Which of the following sequences, respectively, describes the workflow for:

Downloading the provider plugins and setting up backend,
Generating proposed changes and auto-executing the plan
Remove all resources managed by terraform`

The right answer is **terraform init, terraform apply -auto-approve, terraform destroy**

1.  **`terraform init`**: This command initializes the working directory, downloading the necessary provider plugins and setting up the backend if specified in the configuration files.  This is the first crucial step before any other Terraform operations.

2.  **`terraform apply -auto-approve`**: This command generates a plan showing the infrastructure changes Terraform will make and then automatically executes that plan without further user confirmation. The `-auto-approve` flag is used for automation and should be used with caution.  In a production environment, it's generally recommended to review the plan (`terraform plan`) before applying changes.

3.  **`terraform destroy`**: This command removes all the infrastructure managed by the Terraform configuration.  It's the final step to completely clean up resources created by Terraform.
