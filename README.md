# Notes

Please note that while we add postgres and redis to the development environment, we don't do that for production.

In production we use the cloud-server provided environments, aka Managed Data Service Providers.

Temporary account details for the RDS postgres instance are stored in keepass.

Environment properties in Elastic Beanstalk are applied to all containers defined in `Dockerrun.aws.json`.

Errors in the application in AWS, if not present when running locally, are almost certainly down to incorrect environment variables.

The course instructions mean that all the contents of the repo are sent to AWS on "deploy" although only the Dockerrun.aws.json file is actually needed.