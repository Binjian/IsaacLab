---

# All-In-One docker of Isaac Lab
This repository provides a unified dockerfile for the installation of 

- IsaacLab with IsaacSim 4.5, 
- the conda virtual environment 'h-gym' of HumanoidGym with IsaacGym 
- and the conda virtual environemnt 'h-bench' of Humanoid Bench.

It's built upon the original IsaacLab Dockerfile.base to extend the further two environments in the hope to alleviate the chores of upgrading HumanoidGym and Humanoid Bench on the current and future updates of the upstream IsaacLab and the IsaacSim. 

All three repositories are cloned under '/workspace'. The deprecated IsaacGym will be downloaded from NVidia official repo and stored under '/workspace' as well. 

# switching virtual environments
After docker build, please use the commands 
- 'lab',
- 'gym'
- 'bench'

in bash respectively to enter the corresponding virtual environments. The library dependencies and the virtual environments are updated by these commands.

# the original Isaac Lab README
Please refer to the original Isaac Lab README for installing Isaac Lab features, in particular the specification for the original Isaac Lab docker:

[The original Isaac Lab README](./README-isaac-lab.md)
