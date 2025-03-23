# osTicket-Creating-and-Working-Tickets

This lab build off of: [osTicket: Post Installation Configuration](https://github.com/RobGaughan/osTicket-Post-Installation-Configuration)

## Environments and Technologies Used

- Microsoft Azure
- Virtual Machines
- osTicket

## Operating Systems Used 

- Windows 10 Pro, version 22H2 - x64 Gen2
 
## High-level Configuration Steps

1. As an end-user create a ticket
2. As a Help Desk Agent, observe the ticket’s properties
3. Set Properties to the ticket


## Configuration

### As an end-user create a ticket

Navigate to http://localhost/osTicket/open.php

I have created a ticket as karen describing an online banking system being down:

![image](https://github.com/user-attachments/assets/c958b676-fa5a-4adb-b16b-f5f13600559e)

### As a Help Desk Agent, observe the ticket’s properties

Navigate to http://localhost/osTicket/scp/login.php

login as agent John Doe:  

Username: `john`  
Password `osTicketPassword123!`

#### Observe the ticket end-user karen created

As you can see everything is set to default including, priority, "assigned to" and SLA

![image](https://github.com/user-attachments/assets/13722557-2a17-443e-b6b8-5aa049626918)

Because of the severity of this ticket mainly because end users can't access a system (online banking) I will configure the following: 

Update the SLA Plan to Sev-A the most severity SLA so the issue will be worked on ASAP

![image](https://github.com/user-attachments/assets/cadbffb7-c6c3-4119-9d15-f7e05b04c6e6)


Update the help topic to "Business Critical Outage" because "Report a prolbem" isnt as relevant for this ticket

![image](https://github.com/user-attachments/assets/101aed75-c2b5-47e6-bef0-015516d85894)

Next I will assign the ticket to the online banking team

![image](https://github.com/user-attachments/assets/905071a0-7394-4388-bf8a-d601668807dd)

Now let observe the changes made: 

As you can see towards the bottom a log was created for each entry we changed 

![image](https://github.com/user-attachments/assets/5c562c96-aafe-41eb-aee7-93630bea81ce)


