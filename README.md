# Administration-of-Networks-Building-A-Small-Office-Network
School project creating a office network using Microsoft Server Active Directory with a team
Virtual Network Deployment Using Hyper-V 

Objective 

Design and implement a virtual network using Hyper-V that simulates a small enterprise environment. The project will demonstrate your ability to configure Active Directory services and security, network infrastructure, and client integration within a Windows Server ecosystem. 

Project Components 

Host Environment 

    Platform: Windows Server 2022 or higher with Hyper-V enabled 

    Virtual Network: Internal or Private virtual switch for VM communication 

Virtual Machines Configuration 

VM 1: Domain Controller 

    OS: Windows Server 2022 or higher 

    Roles & Features: 

    Active Directory Domain Services (AD DS) 

    DNS Server 

    DHCP Server 

    Group Policy Management 

    Configuration: 

    Create a new forest and domain (e.g., corp.local) 

    Configure DNS Zones and DHCP scopes 

    Create 8 Organizational Units (OUs) for departments or roles 

    Add 40 users and 40 computer accounts distributed across the OUs 

    Apply Group Policies to manage user and computer settings and security 

VM 2: Application & Resource Server 

    OS: Windows Server 2022 or higher 

    Roles & Features: 

    File Server (Secure Network Shares) 

    Internet Information Services (IIS) for web hosting 

    Print Server 

    Configuration: 

    Join to the domain 

    Create shared folders with NTFS and share-level permissions 

    Deploy default basic IIS website 

    Install and share a virtual or physical printer (extra credit for physical) 

VM 3: Client Workstation 

    OS: Windows 11 

    Purpose: 

    Join the domain 

    Validate domain connectivity and Group Policy application 

    Access network shares, IIS site, and printer 

Domain Integration 

    Ensure all VMs are connected to the same virtual switch 

    Configure static IPs or DHCP reservations as needed 

    Join VM 2 and VM 3 to the domain created on VM 1 

    Test domain functionality: 

    Log in with domain credentials on VM 3 

    Access shared resources and verify Group Policy enforcement 
