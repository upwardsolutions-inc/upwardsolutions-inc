## About Me

👨‍💻 With over 20 years of experience in the IT industry and more than 7 years specializing in cloud technologies like AWS, Azure, and GCP, I have dedicated my career to helping businesses transform and leverage technology effectively. My expertise spans across cloud architecture, security, and IT governance, with a keen focus on preparing professionals for Cloud, Security, and IT Governance certifications.

## 📜 Certifications: 
I hold multiple AWS certifications, including AWS Certified Solutions Architect Associate, AWS Certified Specialty in Security, and AWS Certified Specialty in Databases. Additionally, I am certified in HashiCorp Terraform and have earned the COBIT 2019 Foundation Certificate in IT Governance, showcasing my commitment to maintaining high standards of governance and security within IT frameworks.

🎓 In addition to my technical roles, I am passionate about education and have served as an instructor on Udemy, delivering courses that prepare students for AWS, Azure, and GCP certifications. My goal is to empower individuals and organizations to achieve their best by providing high-quality training and consulting.

## About Upward Solutions Inc
🚀 Upward Solutions Inc. is a forward-thinking IT consulting firm dedicated to guiding businesses through digital transformation with a strategic focus on cloud solutions, security, and IT governance. Our mission is to enable our clients to navigate complex cloud environments, optimize their operations, and achieve long-term success. With extensive experience in AWS, Azure, and GCP, we offer comprehensive consulting services in cloud architecture, security, and solution design.

📚 At Upward Solutions Inc., we believe in the power of knowledge and continuous learning. That’s why we also focus on training and certification preparation, helping professionals and businesses stay ahead in an evolving digital landscape. Whether you are looking to enhance your cloud infrastructure, secure your data, or upskill your team, we are here to provide tailored solutions to meet your unique needs.


## 🚀 Projects

### 🔧 Built DevOps Pipeline using Azure DevOps and Code Repository to Deploy Resources in AWS Environment
Designed and implemented a robust DevOps pipeline on the **Azure platform**, leveraging **Azure DevOps** for continuous integration and continuous delivery (CI/CD). The solution utilized **Azure Repos** for source code management and **Azure Pipelines** to automate build, test, and deployment processes. The entire DevOps pipeline was automated using **Terraform Infrastructure as Code (IaC)**, allowing for consistent and repeatable deployments of infrastructure and applications in an **AWS** environment. Resources were deployed in a secure manner, ensuring best practices for security and compliance. By fully utilizing Terraform, the pipeline ensured scalable, reliable, and efficient deployments while minimizing manual intervention and reducing deployment time.

![Local Image](projects/Code_Artifacts_Integration%20_Diagram.png)

### User Migration from AWS Cognito to PingID
#### Problem Statement
AWS Cognito does not provide native disaster recovery support, making it challenging for organizations to ensure business continuity in the event of service disruptions or data loss. Implementing a custom disaster recovery solution within AWS Cognito can be tedious and resource-intensive, leading to potential risks and inefficiencies in managing user authentication and identity management. To address these limitations and enhance security, scalability, and disaster recovery capabilities, PingID has been chosen as a replacement for AWS Cognito.

#### Migration Approaches

##### A. On-Demand User Migration 🔄

- **Overview**: Users are migrated to PingID as they log in or access services.
- **Process**:
  1. Users log in through AWS Cognito 🔑.
  2. Check if the user is already in PingID.
  3. If not migrated:
     - Extract user data 📥.
     - Transform and create user account in PingID 🔒.
     - Notify users of migration 📧.
  4. Send verification email ✅.
  
- **Advantages**:
  - Minimal disruption for users 🔄.
  - Reduced initial workload for IT teams 💼.

- **Challenges**:
  - Potential delays during first login ⏳.
  - Need for robust error handling ⚠️.

---

##### B. Bulk User Migration 📊

- **Overview**: All user accounts are migrated to PingID in a single operation.
- **Process**:
  1. Extract all user data from AWS Cognito 📥.
  2. Transform data to fit PingID's requirements 🔄.
  3. Create user accounts in PingID using API or bulk import 🛠️.
  4. Migrate passwords (or prompt for reset if necessary) 🔑.
  5. Notify users of migration 📧.
  6. Verify and test post-migration access ✅.
  
- **Advantages**:
  - Seamless user experience 🚀.
  - Comprehensive migration reduces repeated processes 📊.

- **Challenges**:
  - High initial workload for IT teams ⚙️.
  - Potential downtime during migration ⏳.
