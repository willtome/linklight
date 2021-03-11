# Ansible Workshop - Smart Management Automation

In this workshop you will learn how to get the most from Red Hat Smart Management subscription and the Ansible Automation Platform.

## Table of Contents
- [Ansible Workshop - Smart Management Automation](#ansible-workshop---smart-management-automation)
  - [Table of Contents](#table-of-contents)
  - [Use Cases](#use-cases)
  - [Lab Diagram](#lab-diagram)
  - [Lab Setup](#lab-setup)
    - [Deployment](#deployment)
    - [Configure](#configure)
      - [**Step 1 - Setup Ansible Tower**](#step-1---setup-ansible-tower)
      - [**Step 2 - Create a Project**](#step-2---create-a-project)
      - [**Step 3 - Create Job Template**](#step-3---create-job-template)
    - [Your Workshop Environment](#your-workshop-environment)
  - [Guide](#guide)

## Use Cases
We will focus on 5 main customer pain points:
- Compliance (OpenSCAP Scanning) and Vulnerability Management
- Patch Management
- System Baselining and Drift
- CentOS to RHEL conversion + upgrade
- Custom Repositories

## Lab Diagram
![](https://lh3.googleusercontent.com/TFkdkKSfTtqbwE4i0ZDTyzvKCojXgeYuIrxIq4kgK6RqiiVU54msgOjGObQEqskvi6BUilA8YoRJg5rdSq-NFC47L6GC3PFhaTmBc9fKBaUX1Axcm_u0UiuRDNJxDrTjsTfUqUpi)

## Lab Setup

### Deployment
- Option 1: [AWS Provisioner](https://github.com/redhat-partner-tech/partner-tech-days-march2021/blob/main/integrated-mgmt-workshop/provision-aws.md) (awscli)  
- Option 2: [RHPDS](https://github.com/redhat-partner-tech/partner-tech-days-march2021/blob/main/integrated-mgmt-workshop/provision-rhpds.md) (Coming soon)

### Configure
After the workshop is deployed, you will need to configure the environment<br>
1)[Configure Workshop Environment](https://github.com/redhat-partner-tech/partner-tech-days-march2021/blob/main/integrated-mgmt-workshop/intro.md)<br>

This step will configure the environment as follows:
- Configure Activation Keys and Lifecycle environments
- Register Servers to Satellite Server

<br>
2) TBD
#### **Step 1 - Setup Ansible Tower**

Login to the Automation Platform:

Open your browser and navigate to the Ansible Tower UI link provided on the attendance page. Login with the username `admin` and the password from your attendance page.

#### **Step 2 - Create a Project**

From the navigation section on the left side of the Automation Platform homepage, select **Project**. Click the green **Create** button in the top right corner. 

Create a project using the `https://github.com/heatmiser/automated-smart-management-2.git` as the source git repository. Enable the checkbox **Update on Launch**.

#### **Step 3 - Create Job Template**


### Your Workshop Environment

In this workshop you'll work in a pre-configured lab environment. You will have access to the following hosts:

| Role                 | Inventory name |
| ---------------------| ---------------|
| Automation Platform  | ansible-1      |
| Satellite Server     | satellite      |
| Managed Host 1       | node1-rhel     |
| Managed Host 2       | node2-rhel     |
| Managed Host 3       | node3-rhel     |
| Managed Host 4       | node4-centos   |
| Managed Host 5       | node5-centos   |




## Guide
Workshop Presentation: [Partner Content Hub](http://redhat-partner.highspot.com)<br>
*You will need a Red Hat Partner Connect account/login to access. Don't have one, look [here](https://connect.redhat.com/en/support)*
* [Exercise 1: Compliance / Vulnerability Management](2-compliance)
* [Exercise 2: Patch Management / OS](3-patching)
* Exercise 3: System Baseline / Drift (See presentation)
* [Exercise 4: CentOS to RHEL conversion + upgrade](4-convert2rhel)
* [Exercise 5: Custom Repositories](5-customrepo)
