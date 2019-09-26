# AWS-SQS---Message-Queues
### Sendmsg
### Receivemsg
## Create 3 Standard Queues

Create 3 Standard Queues
* QueueA "https://sqs.us-2.amazonaws.com/..../messageQueueA"
* QueueB "https://sqs.us-2.amazonaws.com/..../messageQueueB"
* QueueC "https://sqs.us-2.amazonaws.com/..../messageQueueC"



LAB: SQS & Lambda

* Create Lambda functions that are triggered by each of the 3 Queues
* Write your functions in Javascript
* They should perform the same task that your Java apps do
* Confirm that as you publish, you are seeing your app and the lambdas handle the 
    queued messages at scale
    
    
 * [cloudwatch](/lambdaclient/assets/cloudwatch.png)
 * [cloudwatch log detail](/lambdaclient/assets/cloudwatchlog.png)
 * [queue](/lambdaclient/assets/queue.png)
 
### Create an SNS Topic
 * Name this topic “TaskComplete”
 
 * Create a Lambda function that creates a subscriber
 * The lambda function should take in a phone number as the event parameter
 * This phone number should be registered as an “SMS” subscriber to your topic
 * Create a Lambda function that triggers a notification
 * This lambda function should publish a message to your topic
 * Once published, SNS should then send a text message to the the subscriber you 
   created in the previous step
   
   * [subscriber](/lambdaclient/assets/subscribtiontask.png)
   * [publisher](/lambdaclient/assets/taskpublisher.png)
   
Pairs/Team
* Roman 
* Travis
