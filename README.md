# Launching-a-Windows-Virtual-Machine-on-AWS-and-Accessing-it-from-a-Local-Linux-Machine
This project demonstrates how to launch a Windows Virtual Machine (VM) on Amazon Web Services (AWS) and securely access it from a local Linux system. It provides a clear, step-by-step guide to provisioning, configuring, and connecting to a cloud-based Windows environment using AWS EC2.

**Overview**

The goal of this setup is to enable remote access to a Windows environment hosted in AWS directly from a Linux machine. This can be useful for developers, system administrators, and students who need to test Windows-based applications, use Windows-only tools, or manage multi-OS environments seamlessly.

**Steps Involved**

1.Create an AWS EC2 Instance

  Log in to the AWS Management Console.
  Navigate to EC2 → Launch Instance.
  Choose a Windows Server AMI (e.g., Windows Server 2022).
  Select an instance type (e.g., t2.micro for free tier).
  Configure key pair authentication and allow RDP (port 3389) in the security group.

2.Obtain Administrator Credentials

  Once the instance is running, right-click → Get Windows Password.
  Decrypt it using the private key file (.pem) downloaded earlier.

3.Access from Local Linux Machine

  Install an RDP client such as remmina or rdesktop.
  Use the instance’s public IPv4 address and decrypted password to connect.
  Example command:rdesktop <public-ip>
  Optionally, use SSH tunneling for enhanced security.

**Key Features**

  ->Fully cloud-hosted Windows environment.
  ->Secure, remote access from Linux using RDP.
  ->Configurable networking and access controls.
  ->Ideal for cross-platform development and testing.

**YouTube Link**:-
  https://www.youtube.com/watch?v=HHDasKLYL-4

  
