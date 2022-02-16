# boto3_lambda
## What you'll need:
  - Python 3
  - Pip - Python package manager
  - AWS Lambda Account
  
## How to Setup an AWS Lambda Python Function
### Create a python virtual environment
1.  Install python's virtualenv
    - In a terminal window navigate to your project directory
      ```
      cd ~/dev/boto3_lambda
      ```
    - Install virtualenv
      ```
      pip install virtualenv
      ```
    - Create a virtual environment
      ```
      virtualenv env
      ```
    - Activate the virtual environment
      ```
      source env/bin/activate
      ```
2.  With the virtualenv activated, we need to install the Python dependencies boto3 and dotenv
      - boto3 is the AWS SDK for Python
      - dotenv reads key-value pairs from a .env file and can set them as environment variables
    ```
    pip install boto3 python-dotenv
    ```
3.  Before we go further, in the same terminal session (your virtualenv) verify that boto3 and dotenv exist
    ```
    python
    >>> import boto3
    >>> boto3.__version__
    '1.18.46' <=== your version may be different
    >>> import dotenv
    >>> quit()
    ```
