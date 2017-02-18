
```
./app_install.sh

# You will be prompted to enter the information needed before the applicaiton deploys.
# The process will look like this

Please provide the following details on your lab environment.

What is the address of your Mantl Control Server?
eg: control.mantl.internet.com
control.mantl.domain.com

What is the username for your Mantl account?
admin

What is the password for your Mantl account?
**HIDDEN**

What is the your Docker Username?
hpreston

What is the Lab Application Domain?
mantl.domain.com


***************************************************
Installing the demoapp as  class/hpreston
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  1508    0   997  100   511   1643    842 --:--:-- --:--:-- --:--:--  1642
{
    "acceptedResourceRoles": null,
    "args": null,
    "backoffFactor": 1.15,
    "backoffSeconds": 1,
    "cmd": null,
    "constraints": [],
    "container": {
        "docker": {
            "forcePullImage": true,
            "image": "hpreston/cicd_demoapp:latest",
            "network": "BRIDGE",
            "parameters": [],
            "portMappings": [
                {
                    "containerPort": 5000,
                    "hostPort": 0,
                    "protocol": "tcp",
                    "servicePort": 0
                }
            ],
            "privileged": false
        },
        "type": "DOCKER",
        "volumes": []
    },
    "cpus": 0.1,
    "dependencies": [],
    "deployments": [
        {
            "id": "7e659013-3b2e-4446-954e-2405c3ebc865"
        }
    ],
    "disk": 0,
    "env": {},
    "executor": "",
    "healthChecks": [
        {
            "gracePeriodSeconds": 300,
            "ignoreHttp1xx": false,
            "intervalSeconds": 60,
            "maxConsecutiveFailures": 3,
            "portIndex": 0,
            "protocol": "TCP",
            "timeoutSeconds": 20
        }
    ],
    "id": "/class/hpreston",
    "instances": 1,
    "labels": {},
    "maxLaunchDelaySeconds": 3600,
    "mem": 16,
    "ports": [
        0
    ],
    "requirePorts": false,
    "storeUrls": [],
    "tasks": [],
    "tasksHealthy": 0,
    "tasksRunning": 0,
    "tasksStaged": 0,
    "tasksUnhealthy": 0,
    "upgradeStrategy": {
        "maximumOverCapacity": 1,
        "minimumHealthCapacity": 1
    },
    "uris": [],
    "user": null,
    "version": "2016-07-01T12:45:10.685Z"
}
***************************************************

Installed
Wait 2-3 minutes for the service to deploy.
Then you can visit your application at:

http://class-hpreston.mantl.domain.com/hello/world


You can also watch the progress from the GUI at:

https://control.mantl.domain.com/marathon
```
    
