---
layout: essay
type: essay
title: "Meteor Gotchas"
date: 2017-10-19
labels:
  - Software Engineering
  - Meteor
---

# Meteor Problems
Problem 1, when I close a meteor window, it would not let me run another one unless I rebooted
my computer. I googled and googled, and tried what I saw on the internet and it wouldn't work. Then, I 
analysed the message I received, and it was something along the lines of "Can't use port 3000, being used". Then I used the command "sudo fuser -k 3000/tcp", and killed the process on the port. Meteor was
still running in the background even though I closed it. That took some analysing and searching on stackoverflow.com.

Problem 2, I would get frustrated when I would make changes and nothing would happen to the file that I
edited. This was a relatively quick fix that should not have been a problem, but it was. I would make a
change to a file and wait for meteor to update, which it wouldn't, then manually refresh, then finally restart meteor. This would be about 20-30 minutes of fumbling, but after I stopped and took a break,
I realized that I never imported the file! So, when things go wrong in the future, I try solve it quickly, then if I fail, I just calm down and take a break. After the break, with a clear mind, I will
be able to solve it, especially if it is trivial.

Meteor has many things running, so many things can go wrong, but that is just part of the learning process.
