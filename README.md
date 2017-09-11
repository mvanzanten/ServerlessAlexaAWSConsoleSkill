ServerlessAlexaAWSConsoleSkill
====================
## Description

This project provides a Serverless Alexa Skill to control EC2 machines from within your AWS account. Instructions and additional features may come later, project is proof of concept.

## Provides

  * AWS Lambda code (Python 2.7)
  * Alexa Skill code

## Installation/Usage

There is currently no detailed instructions as the project is just a proof of concept. 

1. Visit the <a href="https://console.aws.amazon.com/lambda">AWS Lambda Dashboard</a> and click `Create function`
a. Choose `Author From Scratch`
b. Set Trigger to `Alexa Skills Kit`
c. Name your Function and set the Description
d. Set Runtime to `Python 2.7`
e. Zip up the index.py file in the ConsoleLambda directory and upload as Lambda function code
f. Set Handler to `index.handler`
g. Under Advanced settings set Timeout to `10 sec` and Memory to `512MB`
2. Configure an Alexa Skill using the contents of the ConsoleSkill folder and the ARN of your above Lambda Function in the <a href="https://developer.amazon.com/edw/home.html">Alexa Skills Dashboard</a>.
3. Return to the Lambda function and uncomment lines 29-31 and paste your Alexa Skills Application ID on line 30.

## Contributors
*Matthew Van Zanten

## License

This project is released under the MIT License. See the bundled LICENSE file for more details.
