# #100DaysOfCode Log - Round 1 - Jared Caraway

The log of my #100DaysOfCode challenge. Started on Saturday, March 24, 2018.

## Log

### R1D1 - March 24, 2018
I learned some new Terminal commands today - if you press Ctrl+W, you can delete a word at a time. If you want to repeat a command, hold Alt and type in the number of times you want it repeated, followed by the keyboard shortcut - so to delete the last three words you've entered, you'd press Alt+3 followed by Ctrl+W. Nifty.

I recently upgraded my laptop's HDD to a SSD, and the difference is amazing. I put the old HDD into my desktop PC upstairs (which is also now primarily running on an SSD) as a secondary drive. I also installed Mint Linux on both, and I'm loving it so far - my last daily OS was Ubuntu 16.04 LTS, and so far I haven't really missed it (largely because they're so similar).

The downside to the new SSD on my laptop is that I didn't transfer anything over, so I'm starting from scratch. This has caused a bit of a headache when I start working on a project on one and switch to the other; I realized I needed a solution to sync files between the two machines. After experimenting with a manual networking setup that wasn't quite to my satisfaction and a very disappointing implementation of Dropbox, I discovered the free open-source utility called Syncthing. I installed it on both machines, added a startup command for both so that the server runs whenever I start either one, and dropped the stuff I wanted shared into the default directory that was created in my home directory...and it worked with no hassle at all. It's exactly what I needed, and it's going to make my work a lot smoother.

I am currently learning binary trees. I understand the basic concepts, now I just need to figure out how to get them to translate into code. This is going to require relearning recursion, which I haven't worked with in some time. Ultimately, I'll use this knowledge to solve a coding problem that is asking me to serialize and deserialize a binary tree. I could switch to Python and use their built-in "pickling" functionality, but I think I'm going to remain focused on JavaScript until I have obtained a fairly solid mastery of the language.