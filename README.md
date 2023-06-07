# CC-Exploration

## Vertex AI

<p align="center">
    <img width="393" alt="Screenshot 2023-06-08 at 00 45 45" src="https://github.com/C23-DF02-DiskusAI-Dicoding-Indonesia/CC-Exploration/assets/132810595/57450aa0-04c2-45aa-b953-0ece968f6229">
</p>

We prepared the flow for Custom Training ML Model Workflow using Vertex AI just in case the Machine Learning team found dificulties while training their model.

<details>
<summary>More Details</summary>
<br>
</default>

The Custom Training ML Model Workflow in Vertex AI involves several steps to train and deploy a machine learning model. Here is an explanation of the workflow:

1. Data Preparation: The workflow starts with preparing the data for training. This may involve extracting data from a SQL database or other data sources and transforming it into a suitable format for training.
2. Model Development: Once the data is prepared, the next step is to develop the machine learning model. This typically involves writing code in a programming language such as Python and using machine learning libraries/frameworks like TensorFlow or PyTorch. The model code will define the architecture of the model and specify how it should be trained.
3. Containerization: After developing the model, it needs to be packaged into a container. Docker is commonly used to create containers that encapsulate the model code, dependencies, and runtime environment. The containerization process ensures that the model can be easily deployed and run consistently across different environments.
4. Container Image Registry: The containerized model needs to be stored in a container image registry, such as Google Container Registry. This registry serves as a centralized repository for storing and managing container images.
5. TPU (Tensor Processing Unit) Configuration: If you want to leverage TPUs for training your model, you need to configure the TPU resources in Vertex AI. TPUs are specialized hardware accelerators designed to accelerate machine learning workloads.
6. SSD (Solid State Drive) Storage: During training, you may need to store and access large amounts of data efficiently. Using SSD storage can provide fast read/write speeds, improving the overall training performance.
7. Compute Engine: Vertex AI allows you to choose the compute resources for training your model. You can select the appropriate compute engine specifications based on your model's requirements, such as CPU, memory, and GPU.
8. Replica Configuration: For distributed training or handling large datasets, you can configure multiple replicas to parallelize the training process. This helps to accelerate training and improve scalability.
9. Model Artifacts: During the training process, the model generates artifacts such as trained weights, checkpoints, and evaluation metrics. These artifacts represent the learned knowledge of the model and are crucial for later stages of the workflow.
10. Model Resource in Vertex AI: Once the training is complete, you can create a model resource in Vertex AI. This resource serves as a container for storing and managing the trained model artifacts. It provides a centralized location for deploying and serving the model.



## VPC Network
A VPC (Virtual Private Cloud) Network is a service provided by Google Cloud Platform (GCP) that allows you to create and manage isolated virtual networks in the cloud environment. In the context of Cloud Run, VPC Networks serve several purposes such as Network Isolation, Connectivity to internal resources, Securing access to Cloud Run, Routing, and Traffic management.

<details>
<summary>More Details</summary>
<br>
</default>

1. Click "VPC Network" or "Networking" on the left sidebar.
2. Click "Create VPC Network" or "Create Network" to create a new network.
3. Provide a name for your VPC network and configure the necessary options. Choose the appropriate subnetting mode and IP options based on your requirements, ensuring to enable Private IP if you want to secure access to Cloud Run.
4. Click "Create" or "Done" to create the VPC network.
5. Once the VPC network is created, you can connect it to Cloud Run by configuring a VPC Connector. Go back to the main Google Cloud Console page.
6. Select or create the project associated with Cloud Run.
7. Click "Cloud Run" or "Serverless" on the left sidebar.
8. Choose the Cloud Run service you want to connect to the VPC network.
9. On the service detail page, locate the "Connections" or "Networking" section and select "Edit and deploy new revisions".
10. In the configuration page, find the "VPC Connector" or "Networking" option and click "Add VPC Connector" or "Connect to VPC".
11. Select the VPC network you want to connect from the available list. You can also configure the subnet and other settings if needed.
12. After configuring the VPC Connector, click "Save" or "Deploy" to save the changes and apply the configuration to Cloud Run.
