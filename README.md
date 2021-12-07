# Java AWS-Lambda Project
This is a Java project for developing AWS lambda functions. We must include AWS Java Lambda libraries, which aided us in writing the program by defining interfaces for Java applications running on the AWS Lambda platform.

In your pom.xml file, you must specify two significant dependencies for two important dependencies.
 - [aws-lambda-java-core](https://mvnrepository.com/artifact/com.amazonaws/aws-lambda-java-core)
 - [aws-lambda-java-events](https://mvnrepository.com/artifact/com.amazonaws/aws-lambda-java-events)

Check out the [official documentation](http://docs.aws.amazon.com/lambda/latest/dg/java-gs.html) for further information.

## Getting Started

### Prerequisites
- Before proceeding with this part, your local development machine must have the following installed:
  - GIT CLI - To clone this repository
  - pre install jdk and set it's path in system environment variable.
  - pre install maven and set it's path in system environment variable.

### 1. Cloning the repository
```bash
# Clone the Repo
git clone git@github.com:SusantoMandal/java-aws-lambda.git
``` 
### 2. Package lambda fucntion
You can utilize maven workspace to select package option by right-clicking on the project name.
This will create a .jar file for your project in the target folder, which you will then upload to aws-lambda-console.

### 3. Lambda function testing
After uploading the .jar file to your aws-console, you must update the handler according to your project's package and class name.
```
package_name.class_name::handleRequest
```
After you've updated the handler, test your lambda function.