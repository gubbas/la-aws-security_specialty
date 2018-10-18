# Objective
- Your objective is to create a rule in CloudWatch that responds to the EC2 CreateVpc API call (captured by CloudTrail), and in response, triggers a Lambda function which will enable VPC Flow Logs on any new VPCs.
 
- These Flow Logs will be written to a CloudWatch Log Group.
 
 - We've already created the Lambda function for you, so you need to create the rule.
 
 - Once the rule is in place, go ahead and create a new VPC. In a few minutes, you'll see that the rule executes the Lambda function, enabling VPC Flow Logs.
 
 - Go ahead and give this a try in your lab environment using the credentials provided.
 
 - Try it without watching the walkthrough video first.
 
 - See how you do, and then join me in the next video. Good luck!

# Enabling VPC Flow Logs with Automation

- `lambda_function.py` creates VPC Flow Logs for the VPC ID in the event
- `event-pattern.json` is the CloudWatch Rule event pattern for monitoring the `CreateVpc` API call.
- `test-event.json` is a sample CloudTrail event that can be used with the Lambda function, as it contains the VPC ID
- LINK here architectural diagram just uploaded


