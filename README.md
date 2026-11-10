### Chigetsu An OS for LLMs and Agent Development and Execution Platform

Have you ever imagined the fun of Linux shell, DOS, and their powers within you favorite AI?
Recovering, developing and sharing your Agents and prompts with everyone like good old OSS?
Not being bound by vendor and running stuff on your favorite LLM?

Easily in the same conversation switching between 'sub conversations' like programs? Piping your inputs with agents from different developers? Using other people's prompts as 'libraries' for your own, or maybe easily as scripts with parameters?

Using your cloud (compatible with it) as a hard-drive for your prompts and libraries you got from other people?
If it looks nice to you, now imagine tools, also made this way to help you develop other tools, started looking fun right?

## What the hell am I talking about:

It just started as me going random on new ideas (like always) on Gemini Pro. But I was going to develop a few agents for me, and more, I was going to develop a whole environment to help me better use Gemini Pro for my needs.
Those who know me are already used to how I operate. Scope bloat is almost my second name. I started by wanting to build Agent helpers. Then went to 'choosing what Agent helper', then to 'Also tools to help me develop Agent helpers', to 'languages and file formats to develop and define my Agent helpers'.

In the end I pretty much wanted to build my own OS-like existence to run on Gemini along with tooling for it.
You can get the project 'goals' for now on the documentations here, if you read you will understand how crazy I went in just a few hours. Those who want may join my fun, just reach to me on issues, even if we  have no code, open something like suggestions by me or something.

My goal is develop a environment that will exist in the context window that will let you invoke your 'shell' to run other stuff (without losing what you're doing), let you have more than one 'program' running (more than one output for a prompt, when not in the shell, for now, the goal is that the programs 'running' grab your input from the context until they exit. If a program exit, it may exit with all running with him if he invoked others (yeah API to call from your programs that will let him run others). Next we have the programs on the background (stopped) either because you used the shell inside the program, or because you started another program from the shell with it stopped, etc. And services that run on every input, but without interference of the program. Other ideas include hooking stuff from a program, this way I intend to make all my programs allow for notes to be taken to my google drive.

Likely reading this you think I went crazy right? So just think of this. None is actually a 'program'. They are prompts you developed, stored on a 'hard disk' (google drive for now). You just call them from your shell, pipe their outputs, run multiple together for same inputs, interrupt them and do other thing on the same 'conversation' and go on when you want, terminate it clearing him not 'dirtying' a conversation 'context', etc.

How? We will create prompts for it, not programs. Prompts to manipulate attention and read/store prompts from 'hard-drive' like google drive, as files. A whole prompt that will let, if you trigger it's capabilities on launch, with the previously configured options you made, can go a a DOS-like just run prompts as 'temporary stuff' to 'pipe prompts/run concurrent prompts/run background prompts'. Pipe them to files on drive, etc.

Why I'm doing this? Just because I had fun thinking and bloated the tool.

### Goals

The goal is to make an OS-like guy that is universal for your favorite LLM, since it's not a computer we're talking about, but an LLM, the whole concepts of Operating System, Boot Loader, BIOS, Program, Service, Script, Compiler, Object File, Assembly, Programming Language, Concurrency, Shell, Piping, I/O, and everything may look alien, or people may think it's behind the times, or even don't get. So the thing I'm talking about is a little bit  different here. Yeah, I do believe for local Ollama like  guys we can make a binary format to speed up the execution of scripts. But the whole way that AI works caused me to think about how different a Operating System is for it as well as the process of developing agents for AI using AI. People think AI made things easier, or killed programming. Yeah, when you make a truck that mixes concrete it becomes stupid to mix concrete with shovels, but on the other hand mixing concrete with shovels don't let you build skyscrapers. So the guy of the shovel, is he losing his job? No, because it's not the truck history. The guy with the shovel can build skyscrapers.

But people look at 'easy programming' and forget that we make tools to use them. And use tools for it. And above all, use the tools and create tools as they should, now as they were, or worse as your just learned it should be.

I called it Operating System, program, all that shit just to grab your attention.
What I want is 'attention controlling mechanisms', 'attention switching and coming back' and other things that we can make, don't know if they are useful for everyone, or if they 'solve other problems'. I know it's fun to think, I liked, and I want to develop this things having fun to solve my 'pains' while using my AI.

And more, I want people to go Open Source on a better way with the use of AI. I want ways to make developing AI Agents can become modular and free and sharable and easy. So, the next part is important. I don't like learning much as I link to just pop ideas out. This things I just was thinking 'so fun', without even looking how everyone is sharing their AI stuff or doing their AI stuff. It is more fun this way.

Later I'll write more about the stuff I was thinking and develop the tooling for it. Because the first freedom computers, and AI even more, gave us, is the power to create the tools and methods do create tools and methods, not just use what we get, make we we need and more what we want.

### Subsystems
## Kagutsuchi (迦具土)
This is our 'BIOS-like' script for Gemini.
The idea is just a prompt to access our persistent storage of Gemini and put there a prompt to read the user's  google drive for the 'disk folder'  of Kagutsuchi.

## Doppel
This will be our GRUB-like guy

## Chigetsu
Tbis is the OS kernel

## Other stuff
File formats:
-gdd (Gemini Description File - tentative)
-lml (XML made for LLMs to get a prompt on a structured way)

Programing Language: Enigmatic (more on later)
-Compiler (You may think what the hell?, just keep track here, more latter)
