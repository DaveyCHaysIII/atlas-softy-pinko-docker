# atlas-softy-pinko-docker
This is our Docker project for Atlas

notes:

task0
-Easy money, just a simple ubuntu server

task1
-got that task to spit out the requested http barf but no way of really testing it (localhost:5252 shows nothing)

task2
-I had to replace the copy location of the frontend from /var/www/http/... to /usr/www/http/... and I can't be assed to change it back just to be graded. "it works on my machine". But can confirm, and have proof, that it is dishing soft pink goodness.

task3
-This one was interesting, after revisiting and playing with it I was able to see movement on both the server and the frontend, AND this is the first time I noticed the "Hello, World!" bit above the H1. Proof that I did it right!

task4
-This one took me the longest and is where I discovered most of the faults in the previous tasks, and this was the first that really let me see the content being served. 

task5
-Took just about as long as task4, also noticed weird bug where chrome will display softy pinko but firefox will only show the apache web server stock page... I dunno why apache is running on my machine in the first place but after I tried disabling it it reenabled itself so it must mean to be there. I'm not gonna argue, ol' reliable mr chrome got me where I needed to go.
-This one took the most fiddling with names and variables to get running correctly, but eventually got it going (with proof)

task6
-I didn't want to change my backend/frontend naming, so the .txt file gives the command for backend, not back-end
-suprisingly easy to run multiple instances of a server, however as I learned if you assert a container name in the .yml file it will throw an error, literally removing the container name line fixes it (each instance needs a unique name which docker provides for you)

Learned a lot! Trickier than I thought, really had to chew through a lot of this, though to be fair I was also trying to figure out things like "server", "backend", "proxy", "round-robin" and so forth- all concepts we have yet to go over in class. I might almost suggest a small project before this one going over some of those concepts before jumping into this one, cause remember: most of us are absolute tech beginners and might not off hand know anything about http shenanagins. 