# Lab 1: AWS S3 Bucket

## Props (attributes)
- `bucketName?`
- `versioned?`
- `publicReadAccess?`

## Logical ID
## Physical ID

## Steps to Create any AWS Resource using CDK V2

### Step 1:
- Create a folder on the Local Drive
- Open the folder in VSCode Editor
- Open Terminal 

### Step 2: Create the app
- Make a directory `infra` (or any other based on your choice)
  - `mkdir infra`
- Change directory with `cd`
  - `cd infra`
- Initialize the app by using `cdk init` command. Specify the programming language
  - `cdk init app --language typescript`

### Step 3:
In the `lib/infra-stack.ts` file:
- Import the modules/packages (All or specific Construct from the Module) for AWS services being created 
  - `import * as lambda from 'aws-cdk-lib/aws-lambda'` (example)

### Step 4:
- Define Scope, Logical ID, and Props
  - Scope = `this`
  - Logical ID = Logical ID Name (Different from physical Id)
  - Props - Add the attributes to create the Resources - AWS documentation or Editor code Complete

### Step 5: Build the app (optional)
Build (compile) after changing your code. AWS CDK -- the Toolkit implements it but a good practice to build manually to catch syntax and type errors.
- `npm run build`

### Step 6: Bootstrap (One Time)
Deploys the CDK Toolkit staging stack in S3 bucket.
- `cdk bootstrap`

### Step 7:
Synthesize an AWS CloudFormation template for the app.
- `cdk synth`

### Step 8: Deploying the Stack
Deploy the stack using AWS CloudFormation.
- `cdk deploy`

### Step 9: Modifying the app
The AWS CDK can update deployed resources after you modify your app. To see these changes, use the `cdk diff` command.
- `cdk diff`

### Step 10: Destroying the app's resources
- `cdk destroy`