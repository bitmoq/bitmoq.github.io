---
title: MFA Enablement in Salesforce
layout: blog
category: [Salesforce, Security]
excerpt: With MFA being enforced in Salesforce, how does it play well with and without SSO. In this blog, we explain what exactly do you need to know to get this right.
comments: true
type: blog
permalink: /blog/:title/
published: true
---

# What is MFA
Multi factor Authentication (MFA), as the name suggests, uses multiple authentications to ensure that the right user is accessing a system. For example, in a login screen when you type username and password and hit Login button, the system might ask you to type in a code from an Authenticator app installed on your phone. So, it verifies the users in multiple ways and ensures that the system access is always secure.

# When did Salesforce enforce MFA
- MFA, or in other words, Multi Factor Authentication requirement in Salesforce went into effect on **01 February 2022** as per the **[Salesforce Trust and Compliance Documentation](https://www.salesforce.com/company/legal/trust-and-compliance-documentation/)**. This means that **all Salesforce customers are contractually required to use MFA to access Salesforce products**.
- Auto-enablement of MFA for all Salesforce Products are almost completed. The core Salesforce Products built on Salesforce Platform will finish **auto-enablement by the end of February 2024**. Mostly, your org might have already been auto-enabled by now.
- This MFA requirement is only applicable for users who use the Salesforce UI Login screens.

# Which Salesforce Products fall under the MFA requirements?
1. All products built on the Salesforce Platform, including: Sales Cloud, Service Cloud, Analytics Cloud, B2B Commerce Cloud, Experience Cloud, Industries products (Consumer Goods Cloud, Education Cloud, Financial Services Cloud, Government Cloud, Health Cloud, Manufacturing Cloud, Nonprofit Cloud, Philanthropy Cloud), Marketing Cloud Audience Studio (formerly DMP), Marketing Cloud Account Engagement (powered by Pardot), Platform, Salesforce Essentials, Salesforce Field Service, and partner solutions
2. B2C Commerce Cloud
3. Heroku
4. Marketing Cloud Engagement (powered by Email, Messaging, and Journeys)
5. Marketing Cloud Intelligence (powered by Datorama)
6. Marketing Cloud Social
7. MuleSoft Anypoint Platform
8. Quip products
9. Tableau Cloud

# Which Salesforce Products are excluded from MFA requirement?
1. MuleSoft Anypoint Platform On-Premises Edition.
2. On-Premises Tableau Server and Tableau Public. In addition, Tableau Desktop, Tableau Prep, Tableau Content Migration Tool (CMT), and Tableau Resource Monitoring Tool (RMT) are excluded, unless connected to Tableau Cloud.

# What happens to Organizations who doesn't use Single Sign On (SSO)
Since Salesforce auto-enables MFA, it becomes mandatory for all users in the organization to follow MFA via Salesforce Authenticator.

<blockquote class="blockquote-danger">
    <p>Salesforce Administrator has the ability to disable the MFA option for users if they are not ready or not supposed to be enforced. But keep in mind that this contractually violates the compliance which Salesforce requires its customers to abide by.</p>
</blockquote>

# How to enable MFA?
## Switch ON MFA in entire org
To enable MFA for all internal users in your org:
 1. From Setup, in the Quick Find box, enter Identity, and then select Identity Verification.
 2. Select Require multi-factor authentication (MFA) for all direct UI logins to your Salesforce org.

![MFA Org Wide](/assets/img/mfa-org-wide.png)

## Switch ON MFA in SAML SSO
- In Setup, go to "Single Sign-On Settings"
- Open the SAML configuration
- You will see an option named "**Use Salesforce MFA for this SSO Provider**". Tick this if you need Salesforce MFA to be enforced for this SSO.

![SSO MFA](/assets/img/saml-sso-mfa.png)

<blockquote class="blockquote-danger">
    <p>Disclaimer: You should consult and seek approval from your SSO IAM Team prior to marking the "Use Salesforce MFA for this SSO Provider" as checked.</p>
</blockquote>

# How to exempt MFA?
- Create a permission set or do the following on the concerned profile.
- In System Permissions, assign the **Waive Multi-Factor Authentication for Exempt Users** user permission

![Waive MFA](/assets/img/waive-mfa-permission-set.png)


# Who should be exempt from MFA?
1. User accounts for test automation tools and system integration users
2. User accounts for Robotic Process Automation (RPA) systems
3. Users assigned an Employee Community license
4. Logins using a certificate service that requires a PIN before users can select or receive a user certificate (for example, when logging in with a PIV or CAC card)
5. Logins using a combination of a trusted device and a trusted network


# What happens to Organizations who use Single Sign On (SSO)
Users who are provisioned into Salesforce via SSO won't be affected by these enforcements or auto-enablement. Since SSO itself requires you to authenticate and confirm your identity before it lets you inside Salesforce. 

<blockquote class="blockquote-warning">
    <p>As per the Salesforce Compliance requirement, you are still required to enable MFA for the SSO enabled users. This is to ensure that if someone reset's their password and tries to directly access Salesforce, MFA will come into action.</p>
</blockquote>

# What about API Only Users
The MFA requirement doesn't apply to system integration login types via the API.

# Are there a sequence of steps other than the ones listed above to ensure MFA enablement?
Use the "**Multi-Factor Authentication Assistant**" on your Setup and follow the steps listed in **Get Ready**, **Roll Out** and **Manage**

![MFA Authentication Assistant](/assets/img/mfa-authentication-assistant.png)

# Summary
- If your Salesforce users are accessing Salesforce via SSO or via API, MFA will not be enforced for these persona.
- If your Salesforce users are accessing Salesforce via Salesforce Login UI, then MFA is mandatory for those. Salesforce Admin should make sure these users are not exempted from MFA.
- Make sure to complete the "Multi-Factor Authentication Assistant" steps in Setup
