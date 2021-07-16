# forfend

Cloud Compliance as Code with Open Policy Agent

## AWS

This is based heavily on the AWS Blog Post ([Compliance as Code for Amazon ECS using Open Policy Agent, Amazon EventBridge, and AWS Lambda](https://aws.amazon.com/blogs/containers/compliance-as-code-for-amazon-ecs-using-open-policy-agent-amazon-eventbridge-and-aws-lambda/))
which focuses on detecting ECS workloads which use Docker images that do not come from a trusted Docker registry
([source code](https://github.com/aws-samples/amazon-ecs-compliance-as-code-opa)). I had been independently
assessing Open Policy Agent for a few use cases and thought AWS Lambda and EventBridge could be a great way to
implement this, and was thrilled to find actionable code that validated my assumptions.

The initial goal is to expand on the Docker policy and look to incorporate events from other AWS services
that have the ability to run Docker workloads such as AWS Elastic Beanstalk and AWS Lambda.