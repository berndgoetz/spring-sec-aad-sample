# Introduction

This code tests AAD Spring Boot Starter. It is based on the code at 
https://github.com/Microsoft/azure-spring-boot/tree/master/azure-spring-boot-samples/azure-active-directory-spring-boot-backend-sample

# Preparations

Use the tutorial at https://docs.microsoft.com/en-us/java/azure/spring-framework/configure-spring-boot-starter-java-app-with-azure-active-directory?view=azure-java-stable
for the setup of the app registration.

Make sure you set the permissions "Group.Read.All" and "User.Read" in your app registration and run the admin consent
for the group permission.

Set the "oauth2AllowIdTokenImplicitFlow" to true in the manifest.

Set client id and secret, and tenant id in application.properties.

If you're behind a firewall, set the VM options accordingly, e.g.

```
-Dhttp.proxyHost=yourhttpproxyhost 
-Dhttp.proxyPort=yourhttpproxyport 
-Dhttp.nonProxyHosts="localhost|*.mycompany.com|etc" 
-Dhttps.proxyHost=yourhttpsproxyhost 
-Dhttps.proxyPort=yourhttpsproxyport 
-Dhttps.nonProxyHosts="localhost|*.mycompany.com|etc"
```
