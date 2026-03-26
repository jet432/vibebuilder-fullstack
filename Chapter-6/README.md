# Chapter 6 — Cloud, Infrastructure & CI/CD

## Overview

This chapter covers the concepts and hands-on skills needed to provision cloud infrastructure and automate deployments. Students will launch a real EC2 instance, deploy a web server manually, and then automate the same deployment using GitHub Actions.

---

## Lab

| File | Description |
|------|-------------|
| [Lab — Deploy to EC2 with CI/CD](./Lab-Deploy-EC2-CICD.md) | End-to-end lab: launch EC2 with Terraform, deploy nginx with a shell script, then automate with GitHub Actions |

---

## Folder Structure

```
Chapter-6/
├── Lab-Deploy-EC2-CICD.md         ← lab instructions
├── ec2-setup.sh                   ← shell script to install nginx
├── IAM-Student-Policies.md        ← AWS IAM policies for student accounts
├── hello-cicd/                    ← sample GitHub repo for the CI/CD lab
│   ├── index.html
│   └── .github/workflows/
│       └── deploy.yml
└── terraform-ec2/                 ← Terraform to launch EC2
    ├── main.tf
    ├── variables.tf
    ├── outputs.tf
    └── ssh-keys/                  ← generated private key (git ignored)
```

---

## Prerequisites

- [ ] AWS CLI installed and configured (`aws configure`)
- [ ] Terraform installed (`terraform -version`)
- [ ] Git installed and GitHub account ready
- [ ] AWS IAM user with student policies attached (see [IAM-Student-Policies.md](./IAM-Student-Policies.md))
