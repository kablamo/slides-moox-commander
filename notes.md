# MooX::Commander

Hi my name is Eric and I am kablamo on metacpan.  I work for DuckDuckGo.  Its
an awesome company to work for.  We are hiring.  You should check it out.

I do devops and so I end up creating a lot of command line apps.  After
a few years of this I started having opinions about command line apps.

# Example
So my focus here is for creating apps with commands and subcommands like git or
dzil or for example, this pie-factory app which is unfortunately imaginary
and not a real app.

You can see there are a bunch of actions or commands.  Some commands have
subcommands.  Each command can accept its own set of arguments and options.
And we want to be able to parse out that information.

# Help for commands

There is a help command to get help about any of the other commands.  You can
also use -h and --help.

# Help for subcommands

There is a help command to get help about any of the other commands.  You can
also use -h and --help.

So I think an app should have all this stuff but building all that
infrastructure is boring and time consuming so thats why I created
this module

# A note about usage

One of my opinions is that usage is a personal thing and that it can vary 
from app to app.  I think about these apps like I think about web apps.
Kind of.  So not every web app has the exact same user interface and menu
design.  Everyone could just use bootstrap.js but in practice people have
personal preferences and its boring and there are extenuating circumstances
where that doesn't work.  Also I spent a lot of time thinking about usage and
looking at modules on CPAN and in other languages and trying to figure out the
right answer and there are a lot of clever ideas out there.  But making usage
flexible and beautiful and customizable is a really hard problem imo and I
basically just gave up and decided I didn't actually care because its not that
hard to just write out and maintain usage statements by hand.

So now I've spent the first half of my talk telling you what my module doesn't
do, lets talk about what it does do.

# Project layout

lets start with the project layout.  Again I'm thinking about these apps
similar to web apps.  So when we build a web app we separate the logic into mvc
- model view controller.  I have never gone as far as separating out the view
code but I do think its a good idea to separate the presentation/controller
logic from the rest of your logic.  So basically these command classes are the
view and the controller.

