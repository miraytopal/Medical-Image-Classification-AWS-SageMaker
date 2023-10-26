 #  ![aws-logo](https://github.com/miraytopal/Medical-Image-Classification-AWS-SageMaker/assets/75898277/a0f6bace-3715-4d90-9555-22ba9c22a183)  Medical-Image-Classification-AWS-SageMaker 
This repository contains a model for classifying whether a person has squamous cell carcinoma or adenocarcinoma based on the processing of chest scan data. In this repository, we will use AWS Sagemaker for training our model. 

### Setting up AWS SageMaker with Conda

**1. Install the AWS CLI**

If you haven't already installed the AWS Command Line Interface (CLI) on your local machine, you can follow these steps:

*Install AWS CLI:*

Download and install the AWS CLI from the official AWS CLI [website.](https://aws.amazon.com/cli/)
After installing, open your terminal or command prompt and run aws --version to confirm that it's installed correctly.

*Configure AWS CLI:*

Run AWS configure in your terminal and provide your AWS access key, secret key, default region, and output format (json, yaml etc). You can find these in your AWS account.

**2. Create a SageMaker Notebook Instance**

Go to the AWS Management Console.
Navigate to Amazon SageMaker.
Click "Create notebook instance."
Configure your notebook instance with a name, an IAM role with appropriate permissions, and choose the instance type.
For "Permissions and encryption," you can choose the default settings or customize as needed.
Review and create the notebook instance.

**3. Access Your SageMaker Notebook**

Once your notebook instance is created, click on "Open Jupyter" to access the Jupyter Notebook interface.

**4. Create a Conda Environment**

Inside your Jupyter Notebook, create a new Jupyter Notebook or Python script.

To create a Conda environment, you can use the following commands in a Jupyter Notebook cell:

```!conda create -n myenv python=3.8```

Activate your Conda environment:

```!conda activate myenv```

Install the necessary packages:

```!conda install -c conda-forge boto3 awscli sagemaker```

Resources
--
- https://sagemaker.readthedocs.io/en/stable/frameworks/tensorflow/using_tf.html

