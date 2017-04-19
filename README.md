# Fuzzy Telegram
*A simple vanilla PHP web application displaying random quote of the day.*

->This application used LAMP stack to develop.

->It is connected to AWS for CI/CD using differnet services.

-> Services used to for Continuous Integration and delivery are Elastic Beanstalk, Code Pipeline, S3 bucket, IAM, RDS and EC2.

-> Durng intergration process, tests are ran using PHPHunit and .ebextension file.

->.ebextension file has container commands to run test after the project has been deployed on Beta version.

-> Intergration stage will have PHPunit container command. If any test fails, following code will not move forward in pipeline.

-> Lambda function will be invoked and it will store Stactic files (HTML, CSS, JS, images) in S3 bucket.

