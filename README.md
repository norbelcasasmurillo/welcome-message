<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>Active Directory - Group Policy Management: Welcome Message</h1>
This tutorial explains how to configure a welcome message using Group Policy Management in Active Directory.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to create, work, and resolves tickets within osTicket](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>

<p>

![image](https://github.com/user-attachments/assets/102870fa-43ca-4c71-a73c-8dbce9327109)

</p>
<p>
Domain Controller -> Server Manager -> Tools -> Group Policy Management 
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/e1ae9225-5f31-4179-b176-5227a4f442f5)

</p>
<p>
Locate "Default Domain Policy" within the Forest. Then right click it and click edit.
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/1eecadd6-2775-441c-b2f4-a658fe6b7da4)

</p>
<p>
Computer Configuration -> Policies -> Window Setting -> Security Setting -> Local Policies -> Security Options
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/7b946c40-d0e1-4245-86f1-62e050101fa1)

![image](https://github.com/user-attachments/assets/94dc63e2-6462-4f40-8df7-2757af1380b1)


</p>
<p>
Scroll down and locate Interactive Logon ("Message Title ..." and "Message Text ...")
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/2c943a71-0543-4b65-bb92-cd0d7d18d82d)

</p>
<p>
Click on "Interactive Logon: Message Title". Select the Define box. Type the Company Name. Then, click Apply, followed by OK.
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/48a40103-ef6d-4260-b132-1a131e4e1eb9)

</p>
<p>
Click on "Interactive Logon: Message Text". Select the Define box. Type the Company Policy. Then, click Apply, followed by OK.
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/68cab069-40be-40c2-b94e-37bccf04fcda)

</p>
<p>
Close all tab processes. Open a Command Prompt. Enter the command gpupdate /force. Once complete, then enter the command logoff.
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/f8c0c54b-4542-4999-bd0c-a92e61b6ec98)

</p>
<p>
Attempt to log in. A blue screen with a message should appear. 
</p>
<br />

