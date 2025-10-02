



learned how to create an image and container in docker 

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


