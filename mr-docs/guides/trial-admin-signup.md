---
author: davepinch
description: Learn how to obtain and assign a viral license so users can sign up for the free Dynamics 365 Guides trial
ms.author: davepinch
ms.date: 06/15/2022
ms.topic: article
title: Obtain and assign a viral license to enable users to sign up for a free trial of Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# Obtain and assign a viral license to enable users to sign up for a free trial of Dynamics 365 Guides

Anyone can [sign up for a free trial of Dynamics 365 Guides](trial-signup.md). Some companies restrict employees from using work email to sign up for trials, however. If that’s true  for your company, a user will see the following message when they try to sign up for the free trial.

![Screenshot of Let's get started dialog box with error message.](media/known-issues-trial-email.jpg "Screenshot of Let's get started dialog box with error message")

In this case, an Azure Active Directory admin will need to use the following procedure to obtain and assign a viral license so a user can sign up for the free trial. 

## Obtain and assign a viral license

> [!NOTE]
> You must be an Azure Active Directory System Admin or Global Admin to do this procedure.  

1. Temporarily allow viral licenses by running these commands using Azure PowerShell:
   ```
   # Unblock/block adhoc (aka “Viral”) Licenses in Active Directory
   # one time installation of the PowerShell module
   Install-Module -Name MSOnline
    
   # sign in with azure aad account
   $Msolcred = Get-credential
   Connect-MsolService -Credential $MsolCred
    
   # Set Allow adhoc subscription TRUE
   Get-MsolCompanyInformation | fl AllowAdHocSubscriptions
   Set-MsolCompanySettings -AllowAdHocSubscriptions $true
   Get-MsolCompanyInformation | fl AllowAdHocSubscriptions
   ```

2. Acquire a Dynamics 365 Connected Guides viral license for your company by going to the following page: https://signup.microsoft.com/create-account/signup?isAdminSignup=true&products=50374fc8-8587-4df7-b8bf-e1a3699c11ae&ali=1 

    ![Dynamics 365 Guides Trial screen.](media/admin-trial-signup-viral-trial.jpg "Dynamics 365 Guides Viral Trial screen")
  
3. Block viral licenses again by running these commands using Azure PowerShell:

   ```
   # Set Allow adhoc subscription FALSE
   Set-MsolCompanySettings -AllowAdHocSubscriptions $false
   Get-MsolCompanyInformation | fl AllowAdHocSubscriptions
   ```

4. Assign the viral license to any user that needs to use Dynamics 365 Guides, through the normal process in the 
[Microsoft 365 admin center](https://admin.microsoft.com/#/users).

    ![Screenshot of Microsoft 365 admin center.](media/admin-trial-signup-admin-portal.jpg "Screenshot of Microsoft 365 admin center")
 
5. After a user is assigned a viral license, they can sign up by using the [Dynamics 365 Guides "Try for free" link](ttps://dynamics.microsoft.com/get-started/?appname=guides). 

    ![Screenshot of Dynamics 365 Guides marketing page with Try for free link.](media/admin-trial-signup-try-for-free.jpg "Screenshot of Screenshot of Dynamics 365 Guides marketing page with Try for free link")
    
## See also

- [Sign up for a free Dynamics 365 Guides trial](trial-signup.md)
- [Trial FAQ](trial-faq.md)
