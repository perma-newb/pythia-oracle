#### Pythia-Oracle
Project page is [here](https://exposit.github.io/pythia-oracle/). My blog is [here](https://exposit.github.io/katamoiran/). Eventually I'll make a more detailed project page. Likely, anyway.

##### What is it?

Pythia is a framework to run solo adventures. It uses Python 2.7 and Kivy and will probably run on any platform they will. I wrote it with two goals in mind; first, I wanted to be able to generate content on the fly for my multi-player sandbox campaign while keeping track of that content and second, I wanted to be able to run solo characters through adventures that would surprise me. There are many great GM emulating tools out there, software and print. This is what works for me.

##### Solo RPG Gaming! How does that even work?

The basic procedure I use is pick a system, make a character, fire this program up, and start asking questions. Type in a question like "Am I in a room?" and hit the "???" button. If the answer is yes, type in a room description. If no, maybe the hero is in a cave. Or a spaceship. Or in a forest. Ask again to find out!

... or don't. You can play however you want to! Pythia just seeks to facilitate that play. You can also use it to generate random content for a multi-player campaign.

##### How do I install this?

Install Kivy, following the [installation instructions](https://kivy.org/docs/installation/installation.html) for your OS and Python 2.7. The instructions are very comprehensive and cover pretty much everything you'll need, step by step. They will get you through installing Python (or identifying if it's already installed) and through installing Kivy.

[kivy installation](https://kivy.org/docs/installation/installation.html)

If you can't find python but you're sure it's installed, be sure to check your paths and environment variables!

Once that's all done, you'll need to clone or download this repository. If you know how to use git, you're good to go, clone away. Otherwise, click the green 'clone or download' button on the main pythia-oracle github page, and select 'download zip'. Unzip this archive somewhere easy to find (desktop, Documents folder, etc).

Finally, open up a terminal window and navigate to the folder you just unzipped. Type in 'python pythia.py' (you may need to use 'kivy pythia.py' instead depending on how you installed kivy). You should see a bunch of messages scroll by, largely complaining that the layout is too small, and then the program will appear.

##### Customization/Setup

If the app window is too big or two small, close it down and open up the 'pythia.py' file in your favorite text editor. Change the numbers in the kivy.config.Config.set lines to something that's more suitable for your resolution.

`kivy.config.Config.set ( 'graphics', 'width', 1280 )`<br>
`kivy.config.Config.set ( 'graphics', 'height', 725 )`

If it is just the font that is too small, open up config.py and change the number after 'basefontsize' to the size you'd prefer; this may make some of your buttons or labels crowded if you go too big but you can always change it back! Note, if you already have a game created you'll need to change the basefontsize in saves/gamename/variables.txt as well (this include the quicksave).

To shut down, click the x in the upper left of the main window or just close the terminal. You'll find your save games in the same folder under 'saves'. Content is saved pretty frequently but be sure to hit the 'save' button before closing down to be sure.

I recommend playing around in the quicksave a bit until you figure out what kind of output (and input) the various buttons expect! To reset the quicksave, just delete the entire quicksave folder in the saves folder, then remake it at the title screen.

Note: the system expects a quicksave folder to be present and weird things might happen if you decide not to keep one.

##### Wait, I want more tables!

I don't blame you. I use a ton more myself but I don't think it'd be cool to use other authors' content without asking. So I've started asking!

Until then, you have a couple of options; you can use the "pick one" buttons to get weighted answers from a copy-pasted table on the fly, or you can add in whatever tables you like in the code. I've included a sample as a guide. If the tables are created by you or you have permission from the original author and you want to share them, drop me a line and I'll add a link to them here (or put them in the repo).

Happy Solo Gaming!

##### License Stuff

The MIT License (MIT)
Copyright (c) 2016 exposit

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
