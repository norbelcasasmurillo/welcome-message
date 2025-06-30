<p align="center">

![image](https://github.com/user-attachments/assets/b88b3ef5-eafc-4553-ba84-aba8c75d7797)
</p>

<h1>Active Directory - Group Policy Management: Welcome Message</h1>

This tutorial walks through configuring a custom welcome message that appears at user login, using **Group Policy Management within an Active Directory domain environment**. You'll learn how to centrally manage this setting via a Group Policy Object (GPO) applied through Active Directory.<br />


<h2>Why Use a Login Welcome Message?</h2>
Displaying a custom message at login is a simple but powerful way to share important information with users before they access their desktops. Organizations commonly use these messages for:

- Legal disclaimers and compliance notices

- Company policies or security warnings

- General announcements or support contact info

- By configuring this through Group Policy, you can ensure consistent messaging across all domain-joined computers.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines – Optional)
- Remote Desktop (RDP) (Optional) 
- Group Policy Management
- Active Directory

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- A working Domain Controller
- At least one domain-joined client machine.
  

<h2>Configuration Steps</h2>

<p align="center">
Domain Controller (Log in) -> Server Manager -> Tools -> Group Policy Management 

</p>
<p>

![image](https://github.com/user-attachments/assets/36eab2ae-5384-47de-8bf6-49af6aef959f)
</p>
<br />

<p align="center">
Locate "Default Domain Policy" within the Forest. Then right click it and click edit.

</p>
<p>

![image](https://github.com/user-attachments/assets/eacccd92-6463-42c3-98ae-3febad367ada)
</p>
<br />

<p align="center">
Computer Configuration -> Policies -> Window Setting -> Security Setting -> Local Policies -> Security Options

</p>
<p>

![image](https://github.com/user-attachments/assets/d9757b3f-d330-4119-8ca4-5f7f77837548)
</p>
<br />

<p align="center">
Scroll down and locate Interactive Logon ("Message Title ..." and "Message Text ...")

</p>
<p>


![image](https://github.com/user-attachments/assets/987351f4-957d-4bea-817a-75280e599067)
</p>
<br />

<p align="center">
Click on "Interactive Logon: Message Title". Select the Define box. Type the Company Name. Then, click Apply, followed by OK.

</p>
<p>

![image](https://github.com/user-attachments/assets/4b9fa55d-0acb-441a-8d8a-a71619336e56)

</p>
<br />

<p align="center">
Click on "Interactive Logon: Message Text". Select the Define box. Type the Company Policy. Then, click Apply, followed by OK.

</p>
<p>

![image](https://github.com/user-attachments/assets/ab453143-6e07-4720-9b99-51bfeabd0b08)

</p>
<br />

<p align="center">
Close all tab processes. Open a Command Prompt as Administrator. Enter the command gpupdate /force. Once complete, then enter the command logoff.

</p>
<p>

![image](https://github.com/user-attachments/assets/7388c8ce-5d64-4d17-b853-690609b76c33)
</p>
<br />

<p align="center">
Attempt to log in. A blue screen with a message should appear. 


</p>
<p>

![image](https://github.com/user-attachments/assets/f8c0c54b-4542-4999-bd0c-a92e61b6ec98)
</p>
<br />

<h3 align="center">Conclusion</h3>

<p align="center">

**Well done!** You've successfully configured a custom login welcome message using Group Policy in Active Directory. This is a simple yet effective way to communicate important information, such as company policies or legal notices, to users at login. Remember to test your settings across different user accounts to ensure proper deployment. Great job on completing this tutorial!</p>

