# Jenkins and AWS

## Jenkins

### What is CI and CD
CI
- Stands for Continuous Integration
- Allows developers to integrate code into a shared repo several times. Integrating regularly allows for quick error detections

CD
- Stands for Continuous deployment
- developers or teams release software in short cycles, ensuring that the software can be reliably released at any time
### What is an automation server
An application that exposes programmable objects to other applications. Automation servers are sometimes called Automation components.
### Why do we restrict build and how
We restrict builds so that others do not have access to these builds and make unwanted changes that can break the code.

To restrict, you could set an SSH key using github.

## AWS

### What is an EC2
An EC2 (Elastic computer) is an AWS machine that can be scalable
### How do I SSH into an EC2


```
ssh -i <key> user@machine.ip
```
This command allows you to access your machine with a specific ip

```
scp -i <key> file user@machine.ip:/path/location/
```
This command allows you to copy files onto an AWS machine
```
rsync <-avz>
```
synchronizes files and folders between two locations over a remote shell
