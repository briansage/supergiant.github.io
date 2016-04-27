# Installing Supergiant

Create a Supergiant app cloud on AWS in minutes. Supergiant is open-source and free forever. AWS hardware usage rates apply.

### Linux & Mac OSX

The Supergiant command line interface will automatically install Supergiant on AWS EC2. It can be initiated from your computer’s command line with the following curl command:

```
bash <(curl -L https://supergiant.io/installer)
```

The command line interface will ask questions as you go. Have ready:

* An [AWS EC2 key pair](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html) in a file named kube-admin in US East
* An [AWS access key and secret key](http://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSGettingStartedGuide/AWSCredentials.html) with full administrative access [(?)](http://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started_create-admin-group.html)
* Preferred Kubernetes username
* Preferred Kubernetes password
* If you are using OSX, [Homebrew](http://brew.sh/) is recommended.

### Windows

An easy command line installer is coming. For this release, you may download our experimental binaries from the [latest release on GitHub](latest release on GitHub).
