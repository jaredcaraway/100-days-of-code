# #100DaysOfCode Log - Round 1 - Jared Caraway

The log of my #100DaysOfCode challenge. Started on Saturday, March 24, 2018.

## Log

### R1D1 - March 24, 2018
I learned some new Terminal commands today - if you press Ctrl+W, you can delete a word at a time. If you want to repeat a command, hold Alt and type in the number of times you want it repeated, followed by the keyboard shortcut - so to delete the last three words you've entered, you'd press Alt+3 followed by Ctrl+W. Nifty.

I recently upgraded my laptop's HDD to a SSD, and the difference is amazing. I put the old HDD into my desktop PC upstairs (which is also now primarily running on an SSD) as a secondary drive. I also installed Mint Linux on both, and I'm loving it so far - my last daily OS was Ubuntu 16.04 LTS, and so far I haven't really missed it (largely because they're so similar).

The downside to the new SSD on my laptop is that I didn't transfer anything over, so I'm starting from scratch. This has caused a bit of a headache when I start working on a project on one and switch to the other; I realized I needed a solution to sync files between the two machines. After experimenting with a manual networking setup that wasn't quite to my satisfaction and a very disappointing implementation of Dropbox, I discovered the free open-source utility called Syncthing. I installed it on both machines, added a startup command for both so that the server runs whenever I start either one, and dropped the stuff I wanted shared into the default directory that was created in my home directory...and it worked with no hassle at all. It's exactly what I needed, and it's going to make my work a lot smoother.

I am currently learning binary trees. I understand the basic concepts, now I just need to figure out how to get them to translate into code. This is going to require relearning recursion, which I haven't worked with in some time. Ultimately, I'll use this knowledge to solve a coding problem that is asking me to serialize and deserialize a binary tree. I could switch to Python and use their built-in "pickling" functionality, but I think I'm going to remain focused on JavaScript until I have obtained a fairly solid mastery of the language.

### R1D2 - March 25, 2018
Today I continued my education on binary trees. I was initially confused about how to decide which node to set as root - take the middle element in an array, maybe? I asked the question on an IRC channel I frequent, and someone clarified that it doesn't really matter, since the tree will sort itself out when done properly. It seems like you can just start with the first element in an array, whether or not it's sorted, and get largely the same result as if you'd started in the middle. An interesting feature of a binary tree is that it will often not be balanced - the left and right subtrees will not be symmetrical.

I learned that there are, as far as I know, only two search algorithms: breadth-first search (BFS) and depth-first search (DFS). In the former, you search starting with the root and examining first the left and then the right child nodes, then the left and right nodes of each of those nodes, and so on until you've searched the entire tree or found the search term. With DFS, you search along the left edge of the tree until you hit a node with no further left children, search the right child node (if any), then return to the level above to check the right nodes backward to the root node, at which point you begin the same search pattern starting with the root node's right child.

In the process of learning about binary trees, I did a bit of reading on heaps as well. They follow a similar form of organization, but do not have the same strict sorting criteria. Heaps tend to be more balanced than binary trees in terms of overall structure, but are not as efficient.

I'd really like to jump in and start coding the answer to the binary search tree serialization problem, but I'm finding that educating myself before going in blind is probably the better way to go. Binary trees appear to be an important concept that I'll need to have in my toolbox, so it's better for me to take the time to understand the concept rather than stitch together some code that's just good enough to solve the coding challenge but which I'll quickly forget about as I move forward.

### R1D3 - March 26, 2018
Today, my coding focused mainly on the MEAN stack - MongoDB, Express, Angular, and Node. Creating a MEAN app involves a lot of moving parts - creating routes, installing packages, creating data models for my database - but it's fascinating seeing under the hood at how everything interconnects.

I continued my education on the topic of binary trees as well today. In the process, I homed in on the subject of classes in JavaScript. An interesting fact I learned about JS classes is that, since it is a prototype-based language, creating an instance of a JS object does not simply make a copy based on the class template; the instance is linked to the prototype, and any methods or attributes added to the prototype after objects are instantiated will add that data to the preexisting objects. I never would have guessed!