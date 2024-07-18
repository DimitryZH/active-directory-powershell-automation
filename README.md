# Active Directory PowerShell Automation

## Overview

This project consists of PowerShell scripts designed to automate various tasks within Active Directory (AD) environments. These scripts are intended for system administrators and IT professionals who manage Active Directory environments.

To navigate through this project and access the PowerShell scripts, please select any script by clicking on its name to view further details, including its purpose, usage instructions, and any prerequisites or dependencies.

## Scripts

<details>
<summary>Adding Servers into Domain</summary>

[Link to Adding Servers into Domain script](https://github.com/DimitryZH/active-directory-powershell-automation/blob/main/Adding_Servers_into_Domain.ps1)

### Prerequisites

- Windows PowerShell 5.1 or higher.
- Active Directory module for Windows PowerShell.
- Remote Server Administration Tools (RSAT) for Windows installed on the local system.
- Administrative privileges on the local system.

### Features

- Automates the process of joining servers to a domain.
- Configures the primary DNS IP address on the network adapter.

### Usage

1. Update the script with your domain details and DNS IP address.
2. Run the script with administrative privileges.

</details>

<details>
<summary>Active Directory User Creation</summary>

[Link to Active Directory User Creation script](https://github.com/DimitryZH/active-directory-powershell-automation/blob/main/Active_Directory_User_Creation.ps1)

### Prerequisites

- Windows PowerShell 5.1 or higher.
- Active Directory module for Windows PowerShell.
- SMTP server access for sending email notifications.
- Administrative privileges on the local system.

### Features

- Facilitates the creation of new user accounts in Active Directory.
- Sets a temporary password for new accounts.
- Sends email confirmations for newly created accounts.

### Usage

1. Update the script with your domain controller, mail server details, and any placeholders marked with "YOUR\_".
2. Run the script with administrative privileges.

</details>
<details>
<summary>Enable Active Directory Recycle Bin</summary>

[Link to Enable Active Directory Recycle Bin script](https://github.com/DimitryZH/active-directory-powershell-automation/blob/main/Enable_Active_Directory_Recylcebin.ps1)

### Prerequisites

- Windows PowerShell 5.1 or higher.
- Active Directory module for Windows PowerShell.
- Administrative privileges on the local system.
- The forest functional level must be Windows Server 2008 R2 or higher.

### Features

- Enables the Active Directory Recycle Bin feature.
- Allows for the recovery of deleted Active Directory objects.

### Usage

1. Run the script with administrative privileges.
2. No additional input is required; the script checks and enables the AD Recycle Bin feature if it is not already enabled.

</details>
<details>
<summary>Active Directory User Recovery</summary>

[Link to Active Directory User Recovery script](https://github.com/DimitryZH/active-directory-powershell-automation/blob/main/Active_Directory_User_Recovery.ps1)

### Prerequisites

- Windows PowerShell 5.1 or higher.
- Active Directory module for Windows PowerShell.
- The AD Recycle Bin feature must be enabled.
- Administrative privileges on the local system.

### Features

- Recovers deleted Active Directory users.
- Utilizes the AD recycle bin feature for user recovery.

### Usage

1. Run the script with administrative privileges.
2. When prompted, enter the name of the deleted user you wish to recover. The script will search for and recover the user account.

</details>

<details>
<summary>Inactive User Report in AD</summary>

[Link to Inactive User Report in AD script](https://github.com/DimitryZH/active-directory-powershell-automation/blob/main/Inactive_User_Report_in_AD.ps1)

### Prerequisites

- Windows PowerShell 5.1 or higher.
- Active Directory module for Windows PowerShell.
- Administrative privileges on the local system.

### Features

- Generates a report of inactive user accounts in Active Directory.
- Allows administrators to identify accounts that have not been used within a specified period.

### Usage

1. Update the script with the desired threshold for inactivity (e.g., 90 days).
2. Run the script with administrative privileges.
3. The script will output a report listing all user accounts that have been inactive for longer than the specified period.

</details>
<details>
<summary>Disabling Inactive Users in AD</summary>

[Link to Disabling Inactive Users in AD script](https://github.com/DimitryZH/active-directory-powershell-automation/blob/main/Disabling_Inactive_users_in_AD.ps1)

### Prerequisites

- Windows PowerShell 5.1 or higher.
- Active Directory module for Windows PowerShell.
- Administrative privileges on the local system.

### Features

- Identifies inactive user accounts in Active Directory based on a specified inactivity period.
- Automatically disables these inactive accounts to enhance security.

### Usage

1. Update the script with the desired threshold for inactivity (e.g., 90 days).
2. Run the script with administrative privileges.
3. The script will identify and disable user accounts that have been inactive for longer than the specified period.

</details>
