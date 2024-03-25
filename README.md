# Generate clinical plans from patient-physician audio interviews using AWS managed services

These notebooks demonstrate how to generate clinical plans from patient-physician audio interviews using AWS Managed services and Claude 3 generalised large language model family.  

## Prerequisites
- Verify that model access to Anthropic's Claude 3 Sonnet and Haiku is granted to the account being used, see documentation here: [Amazon Bedrock Model Access](https://docs.aws.amazon.com/bedrock/latest/userguide/model-access.html)

## Setup Instructions
1. The notebook is designed to run with Amazon SageMaker Studio. To use Studio, you will need to setup a SageMaker Domain. For instructions on how to onboard to a Sagemaker domain, refer to this [link](https://docs.aws.amazon.com/sagemaker/latest/dg/gs-studio-onboard.html).

2. Update your SageMaker execution role (created when you initially setup the Sagemaker Domain) -- `arn:aws:iam::<AWS_ACCOUNT_ID>:role/service-role/AmazonSageMaker-ExecutionRole-<TIMESTAMP>` -- to contain the following IAM policies:

- AmazonBedrockFullAccess
- AmazonTranscribeFullAccess


## Usage Instructions
1. Open SageMaker Studio and import the file [ClinicalPlansWithClaude3_AmazonTranscribe.ipynb](ClinicalPlansWithClaude3_AmazonTranscribe.ipynb) from this project.
2. Run all cells in the Jupyter Notebook provided. The notebook has a Setup section in the beggining with additional instalation instructions.