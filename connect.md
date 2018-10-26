# Using the LRZ computing resources

### How to connect
1- Review the info of the LRZ about the available [cluster](https://www.lrz.de/services/compute/linux-cluster/overview/).  
2- Select the desire cluster to connect.  
3- Connect using Terminal or other similar program. Here we are going to connect to lxlogin8.lrz.de   
```bash
ssh yourusername@lxlogin8.lrz.de
```    
4- If connecting for the first time type y in the message it will appear.

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





