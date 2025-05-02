<H1><a href="https://tryhackme.com/room/neighbour">NEIGHBOUR</a></H1>
<img src="Images/Screenshot1.png" width=600>
<H3>TryHackMe-Neighbour room was a Challenge that more focused on "IDOR"/Insecure direct object references problem.</H3>
<p>Hello Hacker!, even though there might be no one will see this writeup, because the challenges is WAY to easy.. ( Yea, it only cost 5 min ._. )</p>
<p>But i spend my time to make this writeup, because there might be someone out there that have difficulties on this Easy challenges ( Yea, It's you! )</p>
<p>SO.. Don't waste time, and let's get hacking!!</p>

<H2>## Input the Target IP to Browser</H2>
<img src="Images/Screenshot2.png" width=600>
<p>After you input the target IP Machine to your virtual machine browser/Attackbox Browser. You will found Login page</p>
<img src="Images/Screenshot3.png" width=600>
<p>Here's the easiest part, just type the Ctrl + U, it will led you to view-source page</p>
<img src="Images/Screenshot4.png" width=600>
<p>And here's where we get leaked information!, you'll found it when you do the same as i do</p>
<p>So just type the input to login page</p>
<img src="Images/Screenshot5.png" width=600>
<p>Yup!, We finally enter the Cloud</p>
<H2>## IDOR Vulnerabilities</H2>
<p>And here's where the IDOR is exist</p>
<p>If you see the parameter "user" in the search bar, you notice that our username "guest" is exist</p>
<p>That mean the username are visible in the search bar</p>
<img src="Images/Screenshot8.png" width=600>
<p>Let's try change the parameter</p>
<img src="Images/Screenshot6.png" width=600>
<p>Now you see that the parameter are easily changed even without password ( Hope there's no website that have issues like this )</p>
<H2>## CAPTURE THE FLAG</H2>
<p>Change the parameter to your neighbour usernames ( Not your real neighbour ._.)</p>
<p>The clue is inside the view-page source that we have found before.</p>
<img src="Images/Screenshot7.png" width=600>
<p>You got it?, Cool!</p>
<p>Even though this is WAY too easy, but atleast it can get yourself a knowledge or new insight about IDOR ( If you are really new in this field )</p>

<H3>SO That's for Neighbour writeup, Thank you for visiting:D </H3>
