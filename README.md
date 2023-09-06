{
eventbridge
s3-events
{
  "Version": "2012-10-17",
  "Id": "example-ID",
  "Statement": [
      {
          "Sid": "Example SNS topic policy",
          "Effect": "Allow",
          "Principal": {
              "Service": "s3.amazonaws.com"
          },
          "Action": [
              "SNS: Publish],
          "Resource": "arn:aws: sns:us-east-1:66517863794: test",
          "Condition": {
           "ArnLike": {
               "aws:SourceArn": "arn:aws:s3:::test1234sdfd56"
            },
        "StringEquals": {
          "aws:SourceAccount": "665178635794"
        }
      }
    }
  ]
}
