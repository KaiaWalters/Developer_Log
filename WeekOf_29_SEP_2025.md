



How to create an image and container in docker 

I learned how to detect which path is being used to execute docker commands using the terminal. There is a diference between globally installed docker via npm install -g docker and downloading docker desktop to access the docker commmand. 

terminal commands are connected to paths that are excuted via the terminal for example "docker" is connected to a script which caused issues and confusions when I first ran docker compose watch. To investigate i used 

type docker 
which -a docker 

https://www.youtube.com/watch?v=Tpyh88yymaA


I learned how to detect the prescence of an app in the applications folder 

ls /Applications/Docker.app

I learned how to change the path connected to the docker command 

export PATH="$PATH:/Applications/Docker.app/Contents/Resources/bin/"


Revisited how to rebase and merge in git 

...
How to override nested dependency versions 

I was having an issue where the project was relying on multple version s of @clerk/shared@3.27.0. This is not the solution to the problem, but I thought it was interesting that you can change waht dependencies pakcages rely on using overrides in the package.json. I don't do a lot of work in the file besides resolving conflicts between branches, information on how to control this file piqued my interested. 

How do I override nested NPM dependency versions
http://stackoverflow.com/questions/15806152/ddg#48524488


...

How to resolve dependency versioning issues 

view all packages withing a project and their versions
npm ls -- depth = 0 

the "extraneous" label within the package.lock file means that a package is not defined in the project but is listed as a dependancy 

I found that cursor does not take into consideration how different dependencies will interact with eachother in the same environment which can cause conflicting packages to produce bugs. I spent some time exploring ways that the team could avoid conflicts between packages but I need to spend more time on this to understand what specific packages are causing conflicts. 

I think we can do a better job of versioning our package json file between deploys to production

path mapping in typescript can cause files to lose track of where they should import from. For example between my branch and the dev branch, I was aliasing src as ./*. The typescript config file should be versioned too and changes to this file should be highlighted in PR descriptions since they impact the whole project. This was my fault, but I'm learning how important that is when working with a large team that is moving fast. 


...
New Commands 

Make changes to a file from the terminal using a linux command 
More information: https://www.linuxjournal.com/content/mastering-text-manipulation-sed-command

This could be good to know for scripting in the future

SED -i 

view all packages withing a project and their versions
npm ls -- depth = 0 