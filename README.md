# FRT PROJECT
 EcoSculpture: Future Ready Talent Internship Project
# EcoSculpture Website

## Overview

The EcoSculpture Website is an online platform dedicated to providing a centralized hub for a diverse range of sustainable products. It aims to simplify the adoption of an environmentally friendly lifestyle by offering a user-friendly interface and a curated catalog of eco-conscious goods.

## Key Features

1. **Centralized Hub:**
   - Explore a variety of sustainability-focused products on a single platform.

2. **Comprehensive Catalog:**
   - Curated selection ranging from daily essentials to specialized items.

3. **User-Friendly Interface:**
   - Intuitive design for a seamless and enjoyable shopping experience.

4. **Clear Categorization:**
   - Efficient categorization for quick and easy navigation.

5. **Educational Resources:**
   - Access information and resources on sustainability to make informed choices.

6. **Community Engagement:**
   - Join a community of eco-conscious individuals, share tips, and engage in discussions.

7. **Vendor Collaboration:**
   - Products sourced from vendors committed to sustainable practices.

8. **Responsive Design:**
   - Optimized for various devices to ensure accessibility.

9. **Transparent Practices:**
   - Highlight eco-friendly and ethical aspects of each product.

10. **Feedback Mechanism:**
    - Provide feedback for continuous improvement of the platform.

## Azure Core Services Used

# Service Number 1
### Azure Blob Storage

Azure Blob Storage is a scalable object storage solution provided by Microsoft Azure. 

It is commonly used to store and manage large amounts of unstructured data, such as images, videos, documents, and more.

In this project 'EcoSculptures' I have typically used azure storage container to store all the images on the website.

Then you I have accessed those images using the SAS URL generated by azure and integrated them in my website.

Working of azure storage:

![i3](https://github.com/rashi1904/frt3/assets/129835335/612d9e05-8c24-41a7-9dc5-218918c0f995)

When integrating Azure Blob Storage into a project website, you typically follow a series of steps:

## Step 1: Access Azure Portal
- Go to [Azure Portal](https://portal.azure.com/).

## Step 2: Sign In or Create an Azure Account
- Sign in to your existing Azure account or create a new one.

<img width="924" alt="s1s2" src="https://github.com/rashi1904/frt3/assets/129835335/b94f1c8b-1bc4-4b0c-8549-1e17040f4842">

## Step 3: Create a Storage Account
- In the Azure Portal, navigate to the "Create a resource" section.

  ![s1s3 1](https://github.com/rashi1904/frt3/assets/129835335/0a07144b-5ce3-46dd-b810-b8b5227627e3)

- Search for "Storage account" and select it from the list of available resources.

  <img width="959" alt="s1s3 2" src="https://github.com/rashi1904/frt3/assets/129835335/b40778e2-6ba5-4a81-ab5f-a766ea9a4bb2">

- Click on the "Create" button to initiate the storage account creation process.

<img width="696" alt="s1s3 3" src="https://github.com/rashi1904/frt3/assets/129835335/79bf39c7-bce8-4dd0-b7dd-d84ec02a315f">

## Step 4: Configure Storage Account
- Fill in the required details such as Subscription, Resource Group, Storage account name, and Region.
- Choose the desired performance and redundancy options (Standard or Premium) based on your project's requirements.

<img width="861" alt="s1s4" src="https://github.com/rashi1904/frt3/assets/129835335/af4664e4-cbc9-435a-894e-3dbb0947638f">

## Step 5: Review and Create
- Review the configuration settings to ensure they meet your needs.
- Click on the "Review + create" button.

<img width="647" alt="s1s5" src="https://github.com/rashi1904/frt3/assets/129835335/5fc2c394-4c95-42b8-95a4-7cc83301a9e6">

## Step 6: Create the Storage Account
- Review the summary information, and if everything looks correct, click on the "Create" button to create the storage account.

## Step 7: Access Keys
- Once the storage account is created, navigate to the storage account in the Azure Portal.
- In the left-hand menu, under "Settings," select "Access keys" to obtain the access keys for authentication.

![s1s7](https://github.com/rashi1904/frt3/assets/129835335/10c61c8f-a662-4c9c-9152-3702fff12e21)

## Step 8: Access Storage Account
- You can now access and manage your storage account, serving as the parent resource for your blobs.

<img width="942" alt="s1s8" src="https://github.com/rashi1904/frt3/assets/129835335/d93d531c-0fb9-48f7-912c-b0b8c53b07ca">

## Integrated SAS token of URL in website code:

<img width="954" alt="integration" src="https://github.com/rashi1904/frt3/assets/129835335/f0e469c0-99f2-4805-bf98-0be4063c68d8">

## Note
- Ensure that you securely manage and store the access keys, as they are used for authenticating and authorizing access to your storage resources.

## Container Deployment Image (For Blob Storage)

![deployment-img](i1.png)

# Now, after following the above steps, we finally deploy the website using:
# Service Number 2
### Azure Static Web Apps

Azure Static Web Apps is a cloud service provided by Microsoft Azure that simplifies the deployment and hosting of static web applications. It is designed to streamline the process of building, deploying, and scaling modern web applications, particularly those built using popular static site generators or frameworks. Here are key features and information about Azure Static Web Apps:
1. **Static Site Hosting:**
   - Host static web applications with support for HTML, CSS, JavaScript, and other static files.

2. **Integration with Serverless APIs:**
   - Seamlessly integrate with Azure Functions for serverless APIs to add dynamic functionality.

3. **Built-in CI/CD:**
   - Take advantage of built-in continuous integration and continuous deployment (CI/CD) capabilities.

4. **GitHub Actions Integration:**
   - Leverage GitHub Actions for defining workflows that build, test, and deploy your static web application.

5. **Automatic Scaling:**
   - Automatically scale to handle varying levels of traffic with global distribution for low-latency access.

# Steps to follow:

## Step 1: Deploy Your Website to Azure Static Web Apps
- Create or navigate to your Azure Static Web Apps resource in the Azure Portal.

<img width="940" alt="s2s1 1" src="https://github.com/rashi1904/frt3/assets/129835335/41b8d6e3-2d21-44f8-a109-960127f0ad43">

- In the Static Web Apps settings, connect your GitHub repository or other supported source control.

<img width="599" alt="s2s1 2" src="https://github.com/rashi1904/frt3/assets/129835335/d62025e2-95cf-4e6d-9814-df527067f2fe">

- Configure the build settings for your web app.

<img width="937" alt="s2s1 3" src="https://github.com/rashi1904/frt3/assets/129835335/3e016cf5-847a-4dfb-82c9-22a55cba8429">

## Step 2: Configure Deployment
- During the deployment configuration, select the storage account you created as the hosting option for your static website.

<img width="304" alt="s2s2" src="https://github.com/rashi1904/frt3/assets/129835335/a4529e15-be86-44fd-b44c-bcaf2e947e37">
 
- Azure Static Web Apps will automatically deploy and configure your website to use the Storage Account for hosting.

## Step 3: Access the Website
- Once the deployment is complete, you can access your static website using the provided URL in the Azure Static Web Apps settings.
  
<img width="416" alt="s2s3" src="https://github.com/rashi1904/frt3/assets/129835335/c269b0eb-56c2-45df-8c64-fe62f0f40769">

#### Below is the hosting URL to access the website!

### Hosting URL:
https://gray-glacier-0f3bdf510.4.azurestaticapps.net/

(**DISCLAIMER**: Might not work if credits get over. In that case, access with following URL:
https://rashi1904.github.io/frt3/ )

## Hosting Deployment Using Static Web Apps

![Alt Text](i2.png)

# Project Demo:

![Alt Text](home.png)

![Alt Text](about.png)

![Alt Text](po.png)

![Alt Text](po1.png)

![Alt Text](testimonial.png)

![Alt Text](blog.png)

![Alt Text](contact.png)


### Installation
1. Clone the repository.
   ```bash
   git clone https://github.com/rmk1904/frt3.git/
