# An Overview
## What is Multi Factor Authentication?
Multi Factor Authentication(MFA) is an authentication method that requires the user to provide two or more verification factors in order to gain access to a resource such as an application, an online account, or a VPN. MFA is an essential component of an effective identity and access management (IAM) policy.it's main purpose is to increases the security of your organization by requiring your users to identify themselves with more than just a username and password. With MFA, users can authenticate themselves with three main methods:

1. What they know eg passswords and pins

2. What they have eg Tokens and badges.

3. As well as what they are eg; fingerprints and face ID

## Enabling MFA on AWS using the Identity and Access Management centre

To do this, you would need a virtual MFA App that can generate OTP(mostly 6-digits). These Virtual authenticator apps support multiple tokens on a single device and use the time-based one-time password (TOTP) algorithm. Some of AWS supported apps includes: Twilio Authy Authenticator, Duo Mobile,
