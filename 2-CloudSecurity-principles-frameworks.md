# Cloud Security Principles and Frameworks

### <u>Levels of abstraction in AWS</u>
You can think of the levels of abstration like renting different types of properties:

**Virtual Machines (VMs):** Like renting an entire house. You have control over everything inside but also have to manage everything yourself.
<br/>

**Containers:** Similar to renting an apartment. You have your own space, but some resources like heating or water are managed by the building.<br/>

**Serverless/Functions:** It's like staying in a hotel. You just use the room without worrying about maintenance or utilities.<br/>

Each level offers different control and ease of use. VMs give you more control but require more management, while serverless is more about focusing on what you want to do (like coding) without worrying about the underlying infrastructure.

---

### <u>What are the control plane and data plane responsible for in container abstraction?</u>

**Control Plane:** Responsible for managing the state of the system, such as scheduling containers, maintaining application states, and handling scaling. It's the brain of the operation, making decisions about the infrastructure.

**Data Plane:** Handles the actual processing of the data, including networking and communication between containers, and the execution of application logic. It's the workhorse, carrying out the tasks assigned by the control plane.

*Both are crucial for the efficient functioning of containerized applications, with the control plane focusing on management and orchestration, and the data plane on execution and operation.*

---





### <u>Where does AWS Lambda fall in the layers of abstraction and what makes it so special?</u>
AWS Lambda falls into the **serverless computing** layer of cloud abstraction. It's special because it allows users to run code without managing servers. With Lambda, you just upload your code, and it handles everything needed to execute and scale your code with high availability. Users pay only for the compute time consumed, making it cost-effective for various applications, especially those with variable or sporadic usage patterns.

<br/> 

###### Readings / Resourses to Review
###### [AWS Architecture Blog - Compute Abstractions on AWS: A Visual Story](https://aws.amazon.com/blogs/architecture/compute-abstractions-on-aws-a-visual-story/) <br/>
[13 Compliance Frameworks for Cloud-based Orgs](https://www.horangi.com/blog/13-compliance-frameworks-for-cloud-based-organizations)<br/>
[Cloud Security Alliance (CSA)](https://cloudsecurityalliance.org)<br/>
[Cloud Controls Matrix (CCM)](https://cloudsecurityalliance.org/research/cloud-controls-matrix/)<br/>
[CSA Security Guidance for Cloud Computing](https://cloudsecurityalliance.org/research/guidance/)
