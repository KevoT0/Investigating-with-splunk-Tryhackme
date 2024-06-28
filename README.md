# Investigating-with-splunk-(Tryhackme:SOC Level 1)


<H2>Description</H2>
This is a hands-on project on SIEM making use of Splunk.
<br/>

<h2>Unilities Used</h2>
-<b>Splunk Enterprise</b>

<h2>Enviroments Used</h2>
-<b>Tryhackme Virtual Machine</b>

<h2>Walk-through</h2>
<h3><b>Questions</b></h3>
<img src="https://i.imgur.com/uOI9O7t.png" height="80%" width="80%" alt="Investigating with splunk"/>

<h3>Here are the steps taken to solve the Problems</h3>

Q1. Finding the Number of events in splunk
<img src="https://i.imgur.com/VOnkcdH.png" height="80%" width="80%" alt="Investigating with splunk"/>
<br>

Q2. Figuring out the new Username? 
<img src="https://i.imgur.com/zpNJat2.png" height="80%" width="80%" alt="Investigating with splunk"/>
<br>
I searched for the EventID to discover sucessfully created Backdoorwhich was used in the Splunk Search to find the answer.

<img src="https://i.imgur.com/SqZUNfG.png" height="80%" width="80%" alt="Investigating with splunk"/>

Q3. Finding the full path regisry key of the backdoor of the new User?

<img src="https://i.imgur.com/Lu0Q0sH.png" height="80%" width="80%" alt="Investigating with splunk"/>

