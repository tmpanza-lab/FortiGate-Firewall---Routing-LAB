# FortiGate Firewall - Routing & Security Profiles LAB

## Objective

The FortiGate FW - Routing & Security Profiles Lab project is aimed to provide hands-on experience with configuring, managing, and optimizing FortiGate's routing and security features. This lab focuses on both network connectivity and security, ensuring that participants can implement secure and efficient network configurations in real-world environment.

### Skills Learned

- Configuring static and dynamic routing on FortiGate firewalls.
- Implementing and troubleshooting OSPF, BGP, and RIP protocols.
- Optimizing traffic flow through effective routing strategies.
- Managing hybrid routing setups (static + dynamic) and integrating diverse networks
- Ensuring connectivity and redundancy using FortiGate's routing features.
- Critical thinking and analytical skills to address complex routing and security scenarios.



### Tools Used

- FortiGate VM: A virtual appliance used in virtualized environments, such as VMware or Hyper-V
- FortiOS Web Interface (GUI)
- FortiOS Command Line Interface (CLI)
- FortiView Dashboard: Built-in monitoring tool for real-time traffic and event analysis.
- Backup and Restore Tools
- FTP/HTTP/HTTPS Servers: For uploading firmware or serving configurations during the lab.
- Traffic Generation Tools
- GNS3 for simulated network devices (e.g., routers, PCs, or switches) to test


*Ref 1: Network Diagram*
![image](https://github.com/user-attachments/assets/21c5626d-1c21-4ee4-982c-7b5f1d56a933)





## STEPS

####### Router Interface Configuration ########
![image](https://github.com/user-attachments/assets/a2811f57-8fa0-41f7-94e0-6748165c1b53)
 

# RIP CONFIGURATION #
![image](https://github.com/user-attachments/assets/d12cd24f-fae5-4489-be34-0435b1ad5f32)
![image](https://github.com/user-attachments/assets/6f65d96a-e588-4331-8778-289491f40354)
 
 
### ROUTER ###
![image](https://github.com/user-attachments/assets/a7c69373-9da8-455f-8410-098536b60563)
![image](https://github.com/user-attachments/assets/49dfa856-c11a-4c21-a3d2-43ff752cab2f)
 
 


# OSPF CONFIGURATION #

### FORTIGATE ###
![image](https://github.com/user-attachments/assets/631cb6bf-6a5b-49bb-b58c-5167ced10321)
 




### ROUTER ###
![image](https://github.com/user-attachments/assets/4657da2a-14b5-48b8-8039-2b8f49974ea9)
![image](https://github.com/user-attachments/assets/5ff4be1b-1f84-4e60-b9c9-0a9c9ee5b045)
![image](https://github.com/user-attachments/assets/9d67354a-97c3-42d3-87ba-bfd10c3d6a78)
 
 
 



# BGP CONFIGURATION #

### FortiGate ###
![image](https://github.com/user-attachments/assets/5d1389dc-fd29-42a4-be11-fe497cfe3c22)
 


### ROUTER ###
![image](https://github.com/user-attachments/assets/8cb1e6ef-e41e-45ae-9b22-2489e126eb4c)
![image](https://github.com/user-attachments/assets/272c6d27-fee3-45b2-84a3-e4b10a029625)
![image](https://github.com/user-attachments/assets/03357fca-feea-4346-aa28-57f65612f711)
 
 
 

## Print routing table entries ##

get router info routing-table all
![image](https://github.com/user-attachments/assets/1693e6b5-3da1-4c8c-bd51-02f6c6b7b728)
 


### Default Static Route Toward internet ###
![image](https://github.com/user-attachments/assets/e86acf25-7934-43a3-9dd6-c3aae55cd07f)

 


### Static Route ####
![image](https://github.com/user-attachments/assets/cbd9cd3c-e39b-4b91-b7ef-bc597ee1e6fd)
 


### Check Routing Table ###
![image](https://github.com/user-attachments/assets/f8e0164b-fe0d-402c-ab3f-9524436fcceb)
![image](https://github.com/user-attachments/assets/18c618af-acd0-4225-aeaf-256dae2a982e)
 
 


Security Profiles

Antivirus Profiles
![image](https://github.com/user-attachments/assets/1ec1bc86-7d22-4f3e-a943-83d70046f3e4)
 
Custom AV
![image](https://github.com/user-attachments/assets/c65d3ddb-719f-4419-a0e0-3cf78f3af82a)
 
Now we have our profile, too, now the profile is created but has not applied yet, so to apply it, we need to go to the policy and object.

And here in firewall policy.
![image](https://github.com/user-attachments/assets/7f4eae52-82e3-4f89-ac17-bddbff7412e8)

 
Here it is and now we have antivirus in our policy.

So now, the policy is activated.
![image](https://github.com/user-attachments/assets/156999aa-db2c-4ae2-8078-84681c87bb27)
 

Web Filter
So basically, in short, web filter is a technology that is used to prevent users from viewing certain ads or web sites.
![image](https://github.com/user-attachments/assets/fe3d354b-989e-4940-9d9e-13175a67e4ee)
![image](https://github.com/user-attachments/assets/a244884d-c8ab-4845-baea-f8bd10277fb3)
![image](https://github.com/user-attachments/assets/7a175fad-6ac1-427a-81c2-9dbbd1067d37)
![image](https://github.com/user-attachments/assets/dba7e32b-16e2-4c61-ae68-9714ecc8e34d)
 ![image](https://github.com/user-attachments/assets/0f9fab6c-f249-402a-8401-0a5259a67982)

 


 

 

 

DNS Filter
DNS filter, you can block access based on domain name resolution, so from that, we can say that Web Filter give us more granular control than DNS Filter.
![image](https://github.com/user-attachments/assets/4513ea97-b9ec-444f-b45f-910ed8295cbf)

 
# FortiGuard Category Based Filter
![image](https://github.com/user-attachments/assets/9a954372-a174-4c33-9a80-43f087015474)

 



Static Domain Filter
![image](https://github.com/user-attachments/assets/6583d683-189c-4308-83bd-bba8f4ac0e93)

 


So first then this translation allows you to translate a result of IP address of a domain to another IP address that you can specify
![image](https://github.com/user-attachments/assets/efaa7978-57c7-4d94-84cd-d09438413e5d)
![image](https://github.com/user-attachments/assets/d44df7f7-dc3e-4849-b4d0-0866b39e8e11)

 

 

Now our profile is created, the next step, of course, is to apply it to our policy.

So we'll go to firewall policies.
![image](https://github.com/user-attachments/assets/f6cf9b89-899d-4395-b068-7ec3064a1503)
![image](https://github.com/user-attachments/assets/0aa7525a-b005-4feb-a50d-b9db78bf64e7)
 
 

So this is all for DNS Filter and for security profiles
![image](https://github.com/user-attachments/assets/8c64c49f-4f32-4916-9b1f-152516ca5ec3)
 

## Application Control

So let's go to application control and now let's know what application control is application control detect applications based on their positions.

Its application has a unique position that it won't you fly it after the detection.

We can apply different action to the application, like a allow monitor block or quarantine can also help us detect applications that consume a lot of bandwidth in our network so we can apply them traffic shaping to limit and control their uses of bandwidth to it.

So like all security profiles, you can see that there is some default profiles.
But again, we are not going to use them, so I will create my own profile.
![image](https://github.com/user-attachments/assets/345e2e69-d347-452e-8e3b-5167820344f6)
 
Create a name
![image](https://github.com/user-attachments/assets/b6268cbb-7f83-4325-83da-b8779ac43d78)
 

Now let's see what is the difference between each action.

So for a monitor, it's allowing the application to pass and it logs a live application.

And for allow, it's only allowed the application, but there is no log for block.

It's of course, broken and therefore quarantine.

It's quarantined the IP of the user that you're trying to access this application for a certain time.

If you want to modify the time you can press the quarantine application like that, we will press it.

![image](https://github.com/user-attachments/assets/84ecfc5f-730b-4b13-96b7-ecf37e4f7a39)

 

So that it for the configuration on the profile.

I will do it OK.

And now our profile is created again.

The profile is created, but it's not applied yet, so to apply as we need to go to the policy framework policy.
![image](https://github.com/user-attachments/assets/9e9f9561-d565-406d-bd6c-64876f8f2b1d)


 

Now our profile is assigned to the policy 
![image](https://github.com/user-attachments/assets/d703dc9e-ae62-4e0b-ac2a-5ffb97089941)
![image](https://github.com/user-attachments/assets/1073c7ca-f462-4432-828f-2d522dc593b7)
 


 


This is how to bandwidth o this is all for application control.
![image](https://github.com/user-attachments/assets/b88574bf-88ab-4e90-beb7-8c9da275973b)
![image](https://github.com/user-attachments/assets/0d9f68d1-2f44-449c-934d-1a7864232d77)




** IPS Configuration **
![image](https://github.com/user-attachments/assets/e01ea893-f68f-4e47-806e-8d9d106baeb2)
![image](https://github.com/user-attachments/assets/00700e3a-60da-4da5-87d0-d29aef17a177)
![image](https://github.com/user-attachments/assets/b36ab110-5044-4fd3-b32a-e44b249a8c66)
![image](https://github.com/user-attachments/assets/6feca48c-587b-4f79-985a-f630fe03a8b3)
![image](https://github.com/user-attachments/assets/e3c4737e-623d-492a-80a7-8da2e32368a1)
![image](https://github.com/user-attachments/assets/087b70a0-c033-40dd-a83b-3dd04a321b01)
![image](https://github.com/user-attachments/assets/ea18d1c2-b59a-4fb4-8471-9ab5744b65f3)

 
 

** File Filter
![image](https://github.com/user-attachments/assets/cab752bd-9976-4185-917c-d90c02cf6138)
![image](https://github.com/user-attachments/assets/851e1fc4-929b-4a6b-aabf-88d6b0069815)

 

 
