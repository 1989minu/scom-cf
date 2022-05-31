The cfn-nag reported three warnings for the cf template

1) Bucket Policy is unavailable
2) The bucket is not encrypted
3) The access-logs were not enabled



The following additions were made in the code to mitigate these.

1) A Bucket Policy was added which restricts access to traffic coming via a particular VPC end point

2) Default encryption was added utilizing SSE-S3

3) Access logs were enabled with the logs being written to a designated logging bucket 