# Cradlepoint AWS IoT Greengrass v2 Container

### Purpose:
This image runs the AWS IoT Greengrass v2 Container.  

### Setup Container:
Create a new container project on your Cradlepoint router and enter the following into the project compose tab:  
> Change the AWS environment variables to your settings.  For more information about how to retrieve these credentials, see [Requesting temporary security credentials in the IAM User Guide](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp_request.html).

```yaml
version: '2.4'
services:
  aws-iot-gg:
    image: "cpcontainer/aws-greengrass"
    environment:
     - PROVISION=true
     - AWS_ACCESS_KEY_ID=AKIAIOSFODNN7EXAMPLE
     - AWS_SECRET_ACCESS_KEY=wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
     - AWS_SESSION_TOKEN=AQoDYXdzEJr1K...o5OytwEXAMPLE=
```

### Docker homepage:  
https://hub.docker.com/r/cpcontainer/aws-greengrass
