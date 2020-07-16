# OSCP Course (PWK updated 2020) Review

Hello, I've just gotten the email from Offsec notifying my of my pass. If you are reading this, you are probably in the position I was in a few months back - deciding whether to go for the PWK course, or already doing the course and deciding if you are ready to take the exam. 

As you might already know, the course consists of lab time in an environment to practice your basic pentesting skills, and an intense proctored 23h45m exam to prove them (hint: it's not that hard, read below)

Overall, it has been a great journey which taught me a lot about myself as well. The course was painful, as I spent days and nights filled with anxiety and uncertainty. But now that its over and looking back, I'm truly grateful for the experience :)

This post, like many others on the interwebs that have helped me out greatly, is meant to help sort out any uncertainties you might have about the course or exam in general (due to the NDA with Offsec I will not divulge any information about the exam other that what is publicly available). 

I'll also include some links and resources which I found useful.

***

### Background

First, a little background about myself. I have a Diploma in Infosec and Bachelors in CS, and have about 1.5 years of working experience in a global SI/consulting firm doing cybersecurity work (mostly cyber defense infrastructure implementation, with the odd Vulnerability Assessment here and there, but nothing really "pentest" related). I would say that I have a good foundation in server side scripting (python, .NET) and a fair understanding of Unix and Windows AD administration.

***

### Pre-PWK

6 months before taking the exam, I started playing with Hackthebox and rooted 3 active machines and 4 retired ones. Then I got lazy and put it aside, but the OSCP was always on my mind. COVID came and with quarantine/work-from-home I decided not to give myself any more excuses. 

Somewhere around the end of March/early April I decided to bite the bullet and register for the PWK with 3 months of lab access. During the 2 weeks before the course started, I went back to HTB and rooted 11 retired boxes (with walkthroughs) and 1 active box. The retired boxes were based on [TJ Null's list](https://docs.google.com/spreadsheets/d/1dwSMIAPIam0PuRBkCiDI88pU3yzrqqHkDtBngUHNCw8/edit#gid=1839402159).

***

### PWK Start

The day I received the course access, I immediately started with the course material with the goal of completing the exercises before starting the labs.  The updated material is really lengthy (850+ pages), but it is definitely doable, and it has some really interesting stuff towards the end (AD attacks). 

For the coursework I dedicated 8 hours a day on weekdays and 14-17 hours on the weekends. However I found myself always getting distracted and not being able to keep my focus. By the end of the 3rd week, I was at module 20 out of a total of 25 modules. As I was getting seriously burned out, and concerned that the time was ticking for the labs, I decided to take a pause on the coursework and head into the labs.

Overall the coursework covers a range of basic pentesting knowledge not limited to:

- Web attacks (XSS, SQL injection)
- Service attacks with public exploits
- Stack based buffer overflows
- AD attacks (kerberos golden/silver tickets, pass-the-hash)

I found the materials a good read but depending on your skill level, you might find them too basic. It definitely is not enough to tackle the labs though, but it is a really good starting point to know what to look out for. What I think Offsec is trying to do with the course material is to teach you to teach yourself, and that to me is more important for the journey ahead.

Note: If you don't already know, you can get an additional bonus 5% in the exam for submitting all of the course exercises and reports for 10 machines. Personally I feel that it's not worth going for, as I spent 4-5 weeks just on the exercises alone.

***

### Labs

I did the labs sequentially by IP address (although Offsec recommends not to). I skipped some that were too hard, or had dependencies. For the labs I dedicated around 6-8 hours on a weekday and 10-17 hours on the weekends. 

At 7 weeks into the course (4 weeks in the lab), I had rooted around 25 lab machines. I then spent the next few days revisiting and rooting a few other machines, bringing the total to 30 lab machines rooted. 

At this point I was getting burnt out (again) as it was just an endless daily routine of launching my VM, working on the lab, and worrying about the exam. The combination of dread, anxiety, and isolation meant that I wasn't in a good place mentally.  I had decided to reschedule my exam from 1 month after the course ends, to the next day after the course end date. 

The reasons for doing so were:

- After completing 30 machines in the lab, it was getting really predictable/I felt like I didn't have anything more to learn from the labs (with respect to the exam). The labs themselves were fine, and the boxes were quite well made, but I guess it was just enough for me. To add, I wasn't very confident still as I was checking the forums here and there for hints sometimes.
- I didn't have the confidence to pass, nor did I expect to pass, but I just wanted to see what the exam was like - to size it up, so I could clear the doubts I had about the exam. As another fellow student [said](https://www.youtube.com/watch?v=6ea9F2vcDlY&t), the exam was a bogeyman at the back of my head and to find my peace I had to meet it. 

At this point, with 4 weeks left to go to the end of course and the exam date, I spent my time on the following:

- 1 week to complete course modules 20-25
- 1 week to write the reports for lab machines. I included 12 machines (for good measure), and used [this template](https://github.com/whoisflynn/OSCP-Exam-Report-Template) for my reports. I also checked through my course exercises, and completed those that were not done or incorrect.

***

### Exam Prep

With 2 weeks to go before the exam, I decided to abandon the labs (not sorry) and work on some other things. As you can see I was starting to decrease my pace and getting more rest (physical and mental) in preparation for the exam.

- I spent some time to go through these Windows and Linux Privesc courses by [Tib3rius](https://github.com/Tib3rius) (creator of Autorecon) on Udemy:

  - [Windows Privilege Escalation](https://www.udemy.com/course/windows-privilege-escalation/)

  - [Linux Privilege Escalation](https://www.udemy.com/course/linux-privilege-escalation/)

  These courses are really helpful as they revisit some of the PE techniques from the OSCP material, and include some new ones that are more advanced. Highly recommended.

- Went back to HTB and did 9 more boxes from [TJ Null's list](https://docs.google.com/spreadsheets/d/1dwSMIAPIam0PuRBkCiDI88pU3yzrqqHkDtBngUHNCw8/edit#gid=1839402159). You can check out my [HTB profile](https://www.hackthebox.eu/home/users/profile/137466) to see the boxes I've done. Some of the boxes I did not escalate as I found the PE method way too convoluted or CTF-like. By this point I had a total of 26 boxes done on HTB.
- Revisited and refined my BOF methodology. I would recommend that you develop a good workflow for yourself. The coursework teaches you more or less everything you need to know, just find a way to condense it into something that works for you. During this time I practiced on stack buffer overflows like [brainpan](https://medium.com/@rihazz13/buffer-overflow-brainpan-e48a0a4b61f0), and was able to get my timing down to around 9mins, including taking of screenshots.

***

### OSCP Exam

My exam was scheduled for 12pm on a Sunday. A few days before, I started to adjust my sleeping time to ensure that I would have the maximum amount of rest before (melatonin helped). I went to sleep at 2am the day before and had planned to wake up at 11am so I could last throughout the exam. Unfortunately due to reasons unknown I woke up at 8am and couldn't go back to sleep.

15 minutes before, I started the ID with the proctor. I faced some issues with the focus of my webcam, and spent a while trying to verify my ID. For this, I would recommend to get a decent webcam if you are able to. I had the Logitech C922 on pre-order (stocks are low globally due to the pandemic), but couldn't receive it in time for the exam.

At 12pm on the dot, I received the exam connection pack. I spent about 5-10mins reading through the instructions and setting up [AutoRecon](https://github.com/Tib3rius/AutoRecon) for an automated scan of the exam environment.

I completed the buffer overflow in 50mins. It could be faster but I spent more time making sure each step was done properly. This is where your workflow will really help you out. As the saying goes, *"more haste, less speed"*. That said, the faster you can complete this, the more time you buy for the rest of the exam. I've included some tips below.

My strategy was to complete the buffer overflow and head for the 2x 20 points machine. With that and the lab report, I would have enough points to pass. I didn't go straight for the 10 point as in my mind it wouldn't help me in passing. 

6.5 hours into the exam, I got my first user shell on the 20 point machine. 

12 hours into the exam, I still had only the first user shell. At this point I was starting to get really anxious as I thought that I would fail. I was not getting anywhere fruitful and everything felt like going "one step forward, two steps back". Do not despair if you encounter this, apparently it's common and normal to feel that way during the exam :D

I decided to modify my strategy and work on the 10 point machine. To my pleasant surprise I rooted it within 10 minutes. It was a huge confidence and morale booster.

In the next 4 hours, I managed to escalate on the 20 point box that I had a user shell for, and obtain a user shell on the 25 point machine. By this time I already had enough points to pass. I spent a further 45 mins to escalate to root on the 25 point box. By this time Metasploit was not used yet.

I was 17 hours into the exam with 7 hours to go, and I was just left with one 20 point machine. I tried all ways and means to break it, even using my Metasploit allowance, but I still could not find a way in. Note: before using your Metasploit allowance, you should thoroughly enumerate the other boxes to make sure that they don't have an exploit that is notoriously difficult to set up manually.

21 hours into the exam, I decided to slow things down. I spent the next 1 hour checking my notes and screenshots to make sure I got everything. I also made doubly sure that the proof keys were submitted correctly.

At hour 22, 10am the next day, I decided to call it quits as the fatigue was getting to me. I pinged the proctor to end the exam, made sure all my screenshots were backed up, and headed to sleep.

I then woke up at 3pm and worked on my report for the next 12 hours. I double and triple checked the reporting for grammatical and formatting errors.

I received the confirmation email within 3 days of submitting the report.

***

##### Exam Tips

- **Buffer overflow**: It's a pretty straightforward stack based buffer overflow with some bad characters. Be meticulous, and check through every step. When developing your workflow, take the time to step through the debugger and understand what each step is doing (see it with your eyes). Understanding is more important than rote learning, as it will help you greatly in troubleshooting when you run into errors. What worked for me was adding "checking steps" as part of my workflow to verify that each step did not result in an unseen errors that propagated down the line.

- **Rotation**: Set a hard time limit for each box, and move on unless you have a ***really*** compelling reason not to. This will avoid the trap of falling into rabbit holes as you have the chance to look at it again with a fresh pair of eyes. I set a timer using the Windows clock to give myself a time limit of 90mins on each box.

- **Note taking**: Take good notes during enumeration that will help you to jog your memory when you revisit the box again. Write it systematically in a way that you know you would be able to carry on from where you left off with a minimal amount of downtime (i.e. reduce context switching overhead :D)

- **Be flexible**: in your strategy, and your exploitation. Expect to encounter the unexpected. Keep an open mind during the exam, but also have a good foundation to fall back on. Always have a strategy but be prepared to deviate from it if the situation calls for it.

- **Keep it simple**: Occam's razor - gravitate towards the most likely solution given the evidence presented. For each possible solution, make a checklist (mentally or otherwise) of conditions to succeed or fail. If you can find 1 or more conditions that fail your hypothesis, you should consider it failed and move on, avoiding a potential rabbit hole. There are two very good writeups of lab machines in the forum, which you will gain access to after starting the course.

- **Backups**: always plan to fail. Take snapshots of your VM before and during the exam. Backup your notes regularly to cloud. I created a "rescue pack" of my personal cheatsheet, notes and tools that I could instantly download and unzip should my VM unexpectedly fail on me. I also kept a base image of Kali just in case I couldn't boot into my VM.
- **Take Breaks**: try to go for a 5 min break every 2 hours, and a 20-30min break every 10 hours at least. It will help you to clear your mind and be more effective afterwards. Remember to eat and be comfortable.

Ultimately, the exam is not as hard as most people make it out to be (apart from the 20 point machine I could not get). It tests you more on your enumeration and methodology than anything else. 

Sometime through your course, you will realize that its not so much about knowing ***how*** to exploit Application X but ***where*** to look for exploitable points. Time management is also a big part of the exam, so automate where you can and always be systematic and logical in considering potential solutions. As they say, *"insanity is doing the same things ..."*

***

### Overall Tips

- Keep your lab notes tidy, and condense useful commands into a readable "copy paste" style cheatsheet. You never know when you might need them.
- SQL Injection: [MsSQL](https://perspectiverisk.com/mssql-practical-injection-cheat-sheet/), [MySQL](http://pentestmonkey.net/cheat-sheet/sql-injection/mysql-sql-injection-cheat-sheet)
- Reverse shells: [Pentestmonkey Reverse Shell Cheatsheet](http://pentestmonkey.net/cheat-sheet/shells/reverse-shell-cheat-sheet)
- Linux privilege escalation: [Linux Smart Enumeration Script](https://github.com/diego-treitos/linux-smart-enumeration), [GTFOBins](https://gtfobins.github.io/)
- Windows privilege escalation: [winPEAS Script](https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite/tree/master/winPEAS), [fuzzysecurity](http://www.fuzzysecurity.com/tutorials/16.html), [guif.re](https://guif.re/windowseop) 

Take care of your mental health too, due to the nature of the course and expense occurred to pay for the course, it might feel a bit hard to take a break on the labs (I always felt guilty). Try to take a day off once in awhile to rest and recharge, keep in touch with your partner or family and friends. 

***

### Acknowledgements

I would like to thank my girlfriend for always being understanding about my limited free time during the course. Also to [Julian](https://www.linkedin.com/in/juliantanws/) who has been a great help and mentor. And to my family for being accommodating. Not forgetting [Mate Mate](https://www.facebook.com/matemate.sg/) for all the 18 hour days and pulling through the exam (I drank 5 bottles :D)