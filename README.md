<img width="1000" height="250" alt="image" src="https://github.com/user-attachments/assets/bedfc0f4-3053-4650-9cbf-e94e41c76d5a" />

# Azure Resource Group and Virtual Machine Setup Guide

This guide walks you through creating a **Resource Group** and **Virtual Machine (VM)** in Azure using the Azure Portal.

---

## Step 1: Log in to Azure Portal
1. Navigate to [https://portal.azure.com](https://portal.azure.com).
2. Sign in with your Microsoft/Azure account.

---

## Step 2: Create a Resource Group
1. In the left-hand menu, click **Resource groups**.
2. Click **+ Create**.
3. **Fill in details:**
   - **Subscription:** Select your Azure subscription.
   - **Resource Group Name:** Example: `Creation-Guide`.
   - **Region:** Choose the closest Azure region (e.g., East US, Canada Central).
4. Click **Review + Create** then **Create**.

   <img width="406" height="906" alt="image" src="https://github.com/user-attachments/assets/5f37c79d-12b7-41c4-a39b-b83afb1d959e" />


---

## Step 3: Create a Virtual Machine
1. In the left-hand menu, click **Virtual machines**.
2. Click **+ Create → Azure virtual machine**.
3. **Basics Tab:**
   - **Subscription:** Same as Resource Group.
   - **Resource Group:** Select the one you created (`Creation-Guide`).
   - **Virtual machine name:** Example: `osTicket-guideVM`.
   - **Region:** Same as Resource Group.
   - **Image:** Choose your OS (e.g., Windows 10 Pro or Ubuntu Server to use Linux).
   - **Size:** For labs, `Standard_B2s` is cost-effective.
   - **Administrator account:** Create a username and strong password.
   - **Inbound ports:** Check **RDP (3389)** to allow Remote Desktop access.

<img width="649" height="746" alt="image" src="https://github.com/user-attachments/assets/a7db04be-223b-40ab-b514-35a30afdcbe3" />
<img width="673" height="761" alt="image" src="https://github.com/user-attachments/assets/4c50aeed-5e01-4f5b-b414-12e273ec7364" />




4. **Disks Tab:**
   - Use the default (Standard SSD is recommended for labs).

5. **Networking Tab:**
   - Ensure a Public IP is assigned.
   - A virtual network and subnet will be created automatically.

6. **Review + Create:**
   - Wait for validation.
   - Click **Create** to deploy the VM.

---

## Step 4: Connect to the Virtual Machine
1. Once deployment finishes, open the VM resource in Azure.
2. Copy the **Public IP Address** from the overview.
3. Open **Remote Desktop Connection (RDP)** on your PC.
4. Enter the Public IP and log in using the username/password you created.

<img width="412" height="258" alt="image" src="https://github.com/user-attachments/assets/cf91f108-82f6-4932-b31d-1402c040f0bf" />

---

## Step 5: Configure the VM
- After logging in, install required software or configure it for your project.
- Keep all related resources (VM, network, IP) in the same Resource Group for easy management.

---

## Summary
**Create a Resource Group**  
**Deploy a Virtual Machine**  
**Access via RDP**  
**Configure for your needs**

---

## 📝 Notes
- Use strong credentials when creating your VM.
- Shut down or delete unused VMs to avoid incurring charges.
- Keep Resource Groups organized by project or environment.

