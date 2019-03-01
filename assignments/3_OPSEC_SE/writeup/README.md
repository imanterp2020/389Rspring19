# Writeup 3 - Operational Security and Social Engineering

Name: Iman Schurman
Section: 0101

I pledge on my honor that I have not given or received any unauthorized assistance on this assignment or examniation.

Digital acknowledgement: Iman Schurman

## Assignment Writeup

### Part 1 (40 pts)

I would present myself as a worker for a common credit card company, say American Express.  I would call her under the pretense that there was a potential data breach and her card could have been affected, explaining that with her help we could quickly determine the probability of her being affected.  In the background would be sounds of a call center to make it feel more legitimate.

I would begin by asking her to confirm her email address which we already know is v0idcache@protonmail.com to reassure her of the legitimacy.   After that I would probe her for her pin to confirm her identity and access her account.  After that, I would pretend to be reviewing her account with her, and ask if she set the security questions to her account.  If yes, the I’d review the three questions and if no I’d ask her to set them now.  The questions would be: What's your mother's maiden name?, What city were born in?, What was the name of her first pet? As these are all pretty standard security questions, they would not raise suspicion.  

Once this is all set, I would ask her for one last favor after verifying her account is “secure”.  I would ask her for a survey as we try to collect data on how the breach may have happened.  I’d ask her simple questions like whether she uses a mobile app or web browser, phone or computer, etc… Somewhere in there I’d ask for her primary browser.  I’d then thank her for her time and wish her a good day.  


### Part 2 (60 pts)


Hello Elizabeth, you were wise to contact me about 1337Bank’s web server security issues.  There are many ways attackers will try to gain access to your systems, and our job is to make life as hard as we can for them.  In my analysis, there are a few basic vulnerabilities I discovered that you can eliminate or reduce.  The three main vulnerabilities I want to talk to you about are password strength, exposed ports, and public personally identifying information.

Let’s begin with your password strength.  It took me a total of 10 minutes to brute-force my way into your server using your login.  “linkinpark” is not a very secure password.  Not only is it a well known band, it has no variance in the character type.  It is best to alternate between numbers, symbols, lower case letters, and uppercase letters.  Additionally, your password should be random and not something meaningful to you.  You can check your password strength here: [https://howsecureismypassword.net] [1].  Additionally, the best passwords are completely random.  Consider looking into a password manager like Dashlane, Lastpass etc… 

Now let us also talk about exposed ports.  I was able to access your server by way of open port 1337.  Any attacker can easily find the port open using basic search skills in a matter of minutes.  An open port itself isn’t necessarily an issue, but it does present an opportunity for attackers to take advantage of if it’s not protected.  View your open ports by checking [www.t1shopper. com/tools/port-scanner] [2] by entering your IP address.  You can help protect your ports using firewalls so that when attackers search for open ports, none appear.  

My last recommendation for you is to limit your personal information online.  By merely knowing your username, v0idcache, I could find your accounts in twitter, reddit, pastebin etc… Consider using multiple usernames so they cannot all be linked together.  Further, your email is displayed publicly on your website.  If you would like to display a contact email, consider either creating a strictly work email, or hiding your information behind a generic contact form.  By using the same username throughout your accounts, I was able to access your server through your login much quicker because it made your choice of username obvious.  

As a final suggestion, look into intrusion detection systems (IDS) and intrusion prevention systems (IPS).  They will allow you to monitor the activity on your network and alert you to potential attackers such as myself brute-forcing your server.

