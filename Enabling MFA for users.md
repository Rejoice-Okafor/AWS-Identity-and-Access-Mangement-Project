# An Overview
## What is Multi Factor Authentication?
Multi Factor Authentication(MFA) is an authentication method that requires the user to provide two or more verification factors in order to gain access to a resource such as an application, an online account, or a VPN. MFA is an essential component of an effective identity and access management (IAM) policy.it's main purpose is to increases the security of your organization by requiring your users to identify themselves with more than just a username and password. With MFA, users can authenticate themselves with three main methods:

1. What they know eg passswords and pins

2. What they have eg Tokens and badges.

3. As well as what they are eg; fingerprints and face ID

## Enabling MFA on AWS using the Identity and Access Management centre

To do this, you would need a virtual MFA App that can generate OTP(mostly 6-digits). These Virtual authenticator apps support multiple tokens on a single device and use the time-based one-time password (TOTP) algorithm. Some of AWS supported apps includes: Twilio Authy Authenticator, Duo Mobile,Microsoft Authenticator, Google Authenticatoretc.

### Steps for enabling MFA on an IAM User.

1. Firstly login to the AWS management console and navigate to the IAM center  https://console.aws.amazon.com/iam/

![Screenshot (208)](https://user-images.githubusercontent.com/112861600/192897743-37f3e4be-f149-4eb9-bb31-8f66548379db.png)

2. In the IAM pane by your left, choose users and In the User Name list, choose the name of the intended MFA user. During this project, the MFA of the root account was enabled, so if you are enabling MFA for thr root user, just click on the enable MFA button close to the root user.

3. Click on the Security credentials tab and open then choose the Activate MFA button 

![Screenshot (209)](https://user-images.githubusercontent.com/112861600/192898445-b236c894-324e-469c-8f88-6810883557d0.png)

4. Select Virtual MFA device in the Activate MFA Device wizard, and then click Continue.
IAM generates and displays virtual MFA device configuration information, including a QR code graphic. The image depicts the "secret configuration key," which is available for manual entry on devices that do not support QR codes.

![Screenshot (210)](https://user-images.githubusercontent.com/112861600/192899348-dbcf7524-f12e-4a44-af5a-58579b599250.png)

5. On your screen,Select Show QR code and then scan the QR code with the Virtual MFA device. You could select the camera icon or an option similar to Scan code, and then scan the code with the device's camera. After scanning is complete, it generates two codes(OTP) for you withing a 30 seconds interval which you yould be required to input into the two boxes.

6. After inputing the two OTPs, click on Assign MFA and wait for few seconds for your request to be complete. You would the get a prompt telling you that the MFA has been enabled.


![Screenshot (211)](https://user-images.githubusercontent.com/112861600/192900817-6356cd23-b2bf-4f7b-a2b7-aeff8e00eb97.png)

&. Navigate back to the IAM dashboard and review the changes made. The root user now has Multi Factor Authentication enabled.

![Screenshot (212)](https://user-images.githubusercontent.com/112861600/192901123-74934626-529d-47d3-933b-688dbc7b9ed6.png)
