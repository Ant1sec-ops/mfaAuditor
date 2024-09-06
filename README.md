# mfaAuditor
This powershell script will audit the MFA status of users in Azure cloud environment.



# Powershell Modules installation for MFA Auditor Script

## Steps to Install Azure Active Directory:

1. Open **Windows PowerShell** as an administrator.
   - Right-click the Windows PowerShell icon and select "Run as Administrator."
   
2. Install the **MSOnline** module by running the following command:
   ```powershell
   Install-Module MSOnline
   ```

3. If prompted to install the **NuGet Provider**, type `Y` and press Enter.

4. If prompted to install from the **PSGallery**, type `Y` and press Enter.

5. As an Administrator, run the following cmdlet to connect to Azure Active Directory:
   ```powershell
   Connect-MsolService
   ```

   > The `Connect-MsolService` command establishes a secure connection to Azure Active Directory.

## PowerShell Scripts:

- **MFA Auditor Script:**
   - Run the script using the following command:
     ```powershell
     .\mfaAuditor.ps1
     ```
   - The script generates a report at `C:\temp\MFAUsers.csv`.
   - Ensure that you have **Global Reader** access to audit MFA users successfully.

---

This README provides a step-by-step guide to installing powershell modules and audit Azure Active Directory and running the MFA auditor script.
