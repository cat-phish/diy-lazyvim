# DIY-LazyVim
I went through ~/.local/share/nvim/lazy/Lazyvim and tried to replicate the structure and functionality in my own ~/.config/nvim directory. 
Some things about the structure I changed to my own personal taste. For the most part, each plugin is in its own lua file. The exception 
being that some plugins LazyVim injects settings from one plugin to another. For example Co-Pilot adds setting to the Lualine config if 
you have it enabled. These plugins that other plugins add settings to I have included in lua/core and loaded them first so that there are 
no errors. Everything in lua/plugins/extras is loaded by default. The best way to load these is to move them to whatever other lua/plugins 
folder you think is most appropriate. All of the other plugins folders are loaded by default in init.lua. Not all of the defualt enabled 
plugins will be 1 to 1 with LazyVim, meaning I've enabled some by default that you would have to do manually with LazyVim. I'm not interested 
in really maintaining this as a 1 to 1 mirror of LazyVim, this was mostly a personal project to migrate my own LazyVim config into my 
own personal config in order to have more fine tuned control over my own config. I am open to suggestions and pull requests if you think 
there's something that could be implemented better.
