![Picture](ressources/header.png?raw=true)
# TaskReceiver Plugins
This is the official TaskReceiver Plugin repo. Choose wisely! You should be able to find binarys in the _/bin_ folder in the future, for now you will have to compile yourself. At the end of the page you can find a summary of all aviavle plugins and their states. Happy Tasking!

## Contributing
### Contributing in form of plugins
Create a new repo called _TaskReceiver.Plugins.YourGithubName_. After that head over to [the plugin repo](https://github.com/Kimmax/TaskReceiver.Plugin) and create a fork, clone to your workstation.
Now you open a shell and change into _TaskReceiver.Plugin/Plugins_ and add your plugin as a submodule here. Than you can fire up your IDE, add reference to the Base Plugin and start working! When you are done commit and push your changes on your repo and if you would like to publish commit and push to your TaskReceiver.Plugin fork and open a pull request. Done!  

#### TL;DR:  
1. Create a new repo called _TaskReceiver.Plugins.YourGithubName_.  
2. Fork [the plugin repo](https://github.com/Kimmax/TaskReceiver.Plugin)  
Setup workspace:  
```
$> git clone https://github.com/YourGithubName/TaskReceiver.Plugin
$> cd TaskReceiver.Plugin/Plugins
$> git submodule add https://github.com/YourGithubName/TaskReceiver.Plugins.YourGithubName
```  
Do work inside _TaskReceiver.Plugin/Plugins/TaskReceiver.Plugins.YourGithubName_ (Add reference to TaskReceiver.Plugin, implement ITaskReciverPlugin!)  
Publishing:  
```
$> cd TaskReceiver.Plugin/Plugins/TaskReceiver.Plugins.YourGithubName
$> git commit -a -m "[Commit message]" && git push --all
$> cd TaskReceiver.Plugin/Plugins
$> git commit -a -m "Added TaskReceiver.Plugins.YourGithubName" && git push --all
```
Head over to [the compare page](https://github.com/Kimmax/TaskReceiver.Plugin/compare) and open a pull request.
Get approved → ??? → Profit.

## All plugins
| Name  | Description  |  Trigger | State  |  Not working | Author
|---|---|---|---|---|---|
| WMPMaster  |  Controls Windows media player from Windows7 and above | /music/wmp  | Partial working  | Set volume to absoulte value|  [Kimmax](https://github.com/Kimmax)
