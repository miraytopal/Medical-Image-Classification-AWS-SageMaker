 #  ![aws-logo](https://github.com/miraytopal/Medical-Image-Classification-AWS-SageMaker/assets/75898277/a0f6bace-3715-4d90-9555-22ba9c22a183)  Medical-Image-Classification-AWS-SageMaker 
This repository contains a model for classifying whether a person has squamous cell carcinoma or adenocarcinoma based on the processing of chest scan data. In this repository, we will use AWS Sagemaker for training our model. 

### Setting up AWS SageMaker with Conda

If you haven't already installed the AWS Command Line Interface (CLI) on your local machine, you can follow these steps:

**1. Install AWS CLI:**

Download and install the AWS CLI from the official AWS CLI [website.](https://aws.amazon.com/cli/)
After installing, open your terminal or command prompt and run aws --version to confirm that it's installed correctly.

**2. Configure AWS CLI:**

Run AWS configure in your terminal and provide your AWS access key, secret key, default region, and output format (json, yaml etc). You can find these in your AWS account.

**3. Create a SageMaker Notebook Instance**

Go to the AWS Management Console.
Navigate to Amazon SageMaker.
Click "Create notebook instance."
Configure your notebook instance with a name, an IAM role with appropriate permissions, and choose the instance type.
For "Permissions and encryption," you can choose the default settings or customize as needed.
Review and create the notebook instance.

**4. Access Your SageMaker Notebook**

Once your notebook instance is created, click on "Open Jupyter" to access the Jupyter Notebook interface.

**5. Create a Conda Environment**

Inside your Jupyter Notebook, create a new Jupyter Notebook or Python script.

To create a Conda environment, you can use the following commands in a Jupyter Notebook cell:

```!conda create -n myenv python=3.8```

**6. Activate your Conda environment:**

```
!conda activate myenv
Install the necessary packages:
conda create --prefix ./env python=3.8
conda activate ./env
pip install boto3 awscli sagemaker
pip install tensorflow==2.1.0
conda install -c conda-forge notebook
python -m ipykernel install --user --name sagemaker
pip install jupyterlab
jupyter-lab
```

Resources
--
- https://sagemaker.readthedocs.io/en/stable/frameworks/tensorflow/using_tf.html

