1. Download Terraform

2. Configure your variables for Terraform:

```
subscription_id = "<Subscription ID>"
tenant_id = "<Tenant ID>"
client_id = "<Client ID>"
client_secret = "<Client Secret>"
publickey = "<SSH Public Key>"
my_public_ip = "Your IP Address"
```

3. Initialize Terraform

`terraform init`

4. Create Terraform plan

`terraform plan -var-file="/mnt/c/terraform/variables.tfvars"`

5. Apply (deploy) Terraform plan

`terraform apply -var-file="/mnt/c/terraform/variables.tfvars"`


If the server needs to be deleted, run

`terraform destroy -var-file="/mnt/c/terraform/variables.tfvars"`