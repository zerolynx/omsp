# [OMSP-INFO-01] Applications
## Description
It is increasingly common for vehicles to have entertainment systems that allow the user to install and use different applications that could help it while driving or resting moments. Systems based on Android Auto and Apple Carplay provide access to a large ecosystem of applications, with which users can interact with their smartphones through the screens of their vehicles. Likewise, there are different types of systems, those based on proprietary software, on Linux distributions, etc.

Every day, many brands like Tesla, implement new updates of their systems where they add new entertainment options for users. However, although users cannot choose which applications will be implemented, all of this as a whole expands the possibilities of the users to interact with the vehicles, and in this way, the attack surface itself.

It is especially important that all applications implemented in these systems are well designed. As well as running safely in a controlled sandbox environment that prevents escalate to the main core of the vehicle. Similarly, no application should allow evading the security measures implemented by the system.

![OMSP](/images/applications.png)

Example: Web browsing (2) through YouTube (1)

## How to Test

**Application Sandbox Environment**
* Each application runs in a separate sandbox environments. This isolates apps from each other and protects apps and the system from malicious apps.

**Principle of least privilege**
* The application will not have any permission that is not supposed to have. For example:
    * If the application does not require to access files, any use case of the application that results in accessing file scheme should be notified.
    * If the application does not require to access contact list, any use case of the application that results in accessing contact list should be notified.

**Denial of Service**
* None application can cause a denial of service in the case that the user perform an incorrect use case that could trigger an application hang. In terms of denial of service, it is understood as that state of the system that does not allow the user to interact with it.

## Tools

## References

*  ["Application Sandbox". Android Open Source Project.](https://source.android.com/security/app-sandbox)
