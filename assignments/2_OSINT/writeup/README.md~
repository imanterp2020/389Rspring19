# Writeup 2 - OSINT

Name: Iman Schurman
Section: 0101

I pledge on my honor that I have not given or received any unauthorized assistance on this assignment or examniation.

Digital acknowledgement: Iman Schurman

## Assignment Writeup

### Part 1 (45 pts)

1.  Elizabeth Moffet

2. 13/37th National Bank as Banking CEO:  [http://1337bank.money/] [1] 

3. First from a basic google search, v0idcache’s pastebin at [https://pastebin.com/WghDuAr7] [2] pops up in which I found a coversation with “f1inch” 
   discussing an important file “AB4300.txt”.  Next up, v0idcache’s reddit can be found in which they have only a single post - CMSC389R-{0M3G4LUL_G3T_pWN3d_N00b}.  
   The last link is a connection to the website which can be seen above.  On the website, it lists v0idcache’s email v0idcache@protonmail.com on the about page.  


   Now taking the username, I used inteltechniques username search tools to find v0idcache’s twitter which is how I found her name.  
   Additionally her twitter lists her as from the Netherlands, her job seen above, and the fact that she joined in Feb. 14.  
   Her tweets list an affinity for chinese food and her interest in “managing money in the digital age”.  

   Lastly a possible github account can be found at [https://github.com/v0idcache] [3] with a single contact, Chris “choward4”.  

4. 142.93.136.81 - Found using DNS trails to look up based on the domain name.  Using whoIs found it comes from Waterland NL, 
   created Feb. 6 2019 and updated Feb. 11th

5. Found in hidden directory: “secret_directory” CMSC389R-{h1ding_fil3s_in_r0bots_L0L} by using “robots.txt” on the website
   There’s also a hidden git repository with flag:  CMSC389R-{h1d3_s3cret_g1ts} found using nmap on the ip address with -A flag.  
  
6. Port 22 (SSH), Port 80 (http), Port 1337 (menandmice-dns) discovered by running t1shopper.com for ports 1-3000

7. Ubuntu Linux according to shodan using the ip address

8. CMSC389R-{h1dd3n_1n_plain_5ight} : website’s home page’s source code
   CMSC389R-{h0w_2_iNt0_DNS_r3c0Rd5} from using https://centralops.net/co/DomainDossier.aspx on the ip address listed above





### Part 2 (75 pts)

First thing I did was try and get the program running.  My search of open ports yielded 
only 1 abnormal 1, port 1337 so I first tried this one.  After verifying with nc the 
connection, I started my program.  To do this, I got a usable version of the rockyou.txt 
file but adding it to my directory to simply have it there.  Note I took it out to submit 
because it exceeded github’s size so the current link to that file does not work.  First I 
guessed that the username would be v0idcache because that was the only reasonable 
guess.  With that, I iterated over each word in the rockyou.txt file and attempted to 
access the server with each password until I found one that works.  

The password that worked was “linkinpark”.  With the password now found I “nc”d
Into the server and looked in the obvious home directory to find the flag file which 
yielded the flag “CMSC389R-{brut3_f0rce_m4ster}”

For fun, I still wanted to check what was in the other file that was referred to in the 
pastebin conversation.  That one yielded this “CMSC389R-{YWX4H3d3Bz6dx9lG32Odv0JZh}”
