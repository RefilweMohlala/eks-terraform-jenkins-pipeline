#  Terraform EKS Cluster Deployment

##  Project Overview
This project automates the deployment of an Amazon EKS (Elastic Kubernetes Service) cluster on AWS using **Terraform**. It covers everything from VPC creation to IAM role setup and cluster deployment — all in a clean, reusable infrastructure-as-code setup.

---

##  Prerequisites
Ensure you have the following installed and configured:

- **AWS CLI** (Configured with `aws configure`)
- **Terraform** (v1.5 or later)
- **kubectl** (Optional: For interacting with the cluster)
- **AWS IAM permissions** to create VPCs, EKS clusters, EC2 instances

---

## 📁 File Structure

```bash
📂 terraform-eks-cluster
│
├── 📄 main.tf        # Core Terraform script
├── 📄 outputs.tf     # Outputs to display cluster details
└── 📄 README.md      # Project documentation
```

---
## 📸 Screenshots
Terraform Apply
![terraform apply](https://github.com/user-attachments/assets/7f153492-6fc1-471d-b15e-2e1a01c08263)
Terraform Output
![terraform output](https://github.com/user-attachments/assets/927065e8-b78a-4d3b-b21b-6e824fa24fef)
Running EKS Cluster
![running eks cluster](https://github.com/user-attachments/assets/2c890b70-d1dd-4675-849d-2d7ffe41d1d0)


---

## 🔥 Cleanup (Important to Avoid Costs!)
```bash
terraform destroy -auto-approve
```

✅ Verify no resources remain:
```bash
aws eks list-clusters
aws ec2 describe-instances
```

---

## 💡 What You’ll Learn
- **Terraform basics and advanced AWS resource provisioning**
- **EKS cluster creation with VPC, Subnet, and IAM role setup**
- **How to destroy infrastructure to avoid costs**

---

## 🔧 Tech Stack
- **Terraform** — Infrastructure as Code (IaC)
- **AWS** — EKS, VPC, IAM
- **Kubernetes** — Cluster orchestration

---

## 🌟 Credits
Built with ❤️ by Refilwe

---

Happy Terraforming! 🛠️

