# Using the LRZ computing resources

## How to connect
1- Review the info of the LRZ about the available [cluster.](https://www.lrz.de/services/compute/linux-cluster/overview/)   
2- Select the desire cluster to connect. Here we are going to connect to lxlogin8.lrz.de      
3- Connect using Terminal or other similar program.  
```bash
ssh yourusername@lxlogin8.lrz.de
```    
4- If connecting for the first time a message like this will appear.  
```
The authenticity of host '128.199.138.34 (128.199.138.34)' can't be established.
RSA key fingerprint is 90:8c:7d:f8:ae:1a:09:60:44:08:3b:d9:c9:f7:c4:76.
Are you sure you want to continue connecting (yes/no)?
```  
Type yes  
```
Warning: Permanently added '128.199.138.34' (RSA) to the list of known hosts.
```  

5- Type your password.  

6- You are connected and message will be printed to the screen.  
```
  Welcome to the CoolMUC3 KNL/Omnipath cluster, one of the Linux cluster 
  systems operated by Leibniz Supercomputing Centre (LRZ).  
  Please read the introductory documentation on the LRZ web site
  http://www.lrz.de/services/compute/linux-cluster
  and 
  https://www.lrz.de/services/compute/linux-cluster/coolmuc3/
  
  Note that the front end node itself is not a KNL system, but a standard
  Xeon processor, so is only intended for cross-compilation.
  Please do not run any extensive computational programs on the front end 
  node. Instead, please submit SLURM batch scripts for production jobs, 
  and SLURM interactive shells for testing and short-running programs.
  Misuse of the interactive resources will lead to violating accounts being
  blocked from access to the cluster.
--------------------------------------------------------------------------------
```


## Where are the programs?
All the programms are installed in a specific folder to avoid duplications and waste of time. Each cluster can have different ways to run the programs. Here we are going to show how to run programs already installed for our use.  

**NOTE: This will not in other systems (*e.g.* different PATH, or using modules)**

If your system use modules click [here.](/modules.md)

To learn how to install locally in your folder click [here](/locally.md)

1- We installed all the programs we may need in this location.  
```
/home/hpc/pn69xe/di29vos2/ignite_tools/bin
```   
You need to add this to your PATH so each time you type the name of a program the system will now where to look for it.  

2- Use a text editor to add the programs PATH to your `.bashrc` file. You can use nano, vim, or your favorite text editor. Make sure to be in your home folder. If not sure just type `cd` and you will get there.  

3- Open the `.bashrc`. Note thet there is a `.` befroe the name. This mean is an invisible file. To learn more of this click [here.](invisible.md)  
```
nano .bashrc 
```   

4- Add the following line to the end of the `.bashrc` file.  
```bash
export PATH="$PATH:/home/hpc/pn69xe/di29vos2/ignite_tools/bin"   
```   
Save and close the file.  

5- Log out and log in back to confirm the changes. Or simply type:
```bash
source ~/.bashrc
```  

##  Working on the terminal
Now that you are connected to the terminal and have the PATH for the programs you can go to the next section.  
[Next section]()






