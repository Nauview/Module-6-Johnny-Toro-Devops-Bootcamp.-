# Module-6-Johnny-Toro-Devops-Bootcamp.-
Module 6 of the techworld by nana bootcamp. 

For this module, I had to build and use nexus repository manager to store artifacts. 

After creating the droplet (Virtual machine) with the necessary resources, I installed nexus from the sonatype website, and created a new user and group to be able to run the service. 

As we can see on the image we have the nexus folder with the runtime of the app and the sonatype folder with the configuration files. 

The service is running on the port 8081 after enabling it in the firewall. 

![Nexus Running on Server](./assets/images/Nexusonserver.png)


I was able to access the UI of the nexus repository manager on my Browser. 

![Nexus running on browser](./assets/images/Nexusbrowser.png)

We can see the different default repositories and their types and formats. 

![Nexus repositories](/assets/images/repositories.png)

I was able to publish one of the gradle artifacts we had created in earlier lessons by adding the plugin to the configuration file with the address, authentication method and credentials. 

![Nexus](/assets/images/Published%20artifact..png)

I created my own user and gave it the minimum permissions to publish. 

![User](/assets/images/User.png) 

I was also able to see that I could create cleanup policies, like the one with the image that takes all the artifacts on the repo as was placed with the regular expression, this one would clear all artifacts, however, we need to compact the blob store if we want to free the space once its needed. 

![Cleanup Policies](/assets/images/Cleanup%20policy..png)\

