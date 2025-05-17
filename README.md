# stata-savio-notes

## Open OnDemand

- First log into [Open OnDemand](https://ood.brc.berkeley.edu/) (with your brc username/pin + one time password). This is a graphical interface to Savio with Rstudio, Jupyter and virtual desktop.

Select `Interactive Apps > Desktop`

![image](https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/87200dce-e07e-4574-add7-33fa9e2c90d0)





## Scheduling

<img width="560" alt="image" src="https://github.com/user-attachments/assets/933b0f70-f8da-4f9f-b8ce-103954480913" />


:point_up: The important fields are `SLURM Partition` and `Wall Clock Time`. Partition should be `savio4_htc` . Wall clock time should be the number of hours you'd like for your session to run.

You'll enter the queue. Lower wall clock times will have faster wait times but don't be shy about requesting more than you think you might need.


click `Launch Desktop`







## Remote Desktop

You'll see a funky desktop. Right click somewhere and select `Open Terminal Here`. On keyboard shift + command will right click. 


![image](https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/6e4f1044-41d8-469b-b112-fcb868d12009)


In the terminal, add the Stata software to your $PATH variable: `export PATH=$PATH:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/global/home/groups/fc_demog/stata18`

type `xstata-mp` to launch the GUI


Stata!

![image](https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/5ddc4cd3-2678-4704-a401-d9eb17d4d9c4)


<!--- Troubleshooting note: if the above does not work and you cannot run `xstata-mp` then you can also `cd` into `/global/home/groups/fc_demog/stata18` and run `./xstata-mp`

![image](https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/de74f6b1-8503-4d95-9a3d-5f1db6cc83d5) -->


Be sure to set your working directory to your own home directory: `/global/home/users/<your-username>`


## Using X Quartz on a Mac

Sometimes the virtual desktop in incompatible with the version of Stata. Another way of accessing Demography's Stata on Savio is to the X-Forwarding. 

- Open a terminal and ssh into the log-in node using the -X flag:

`ssh -X {savio-username}@hpc.brc.berkeley.edu`

- Start an interactive session on the htc4 node for an hour, tweak this command to your liking:

`srun -A co_demography -p savio4_htc --qos demography_htc4_normal -t 01:00:00 --cpus-per-task 8 --pty bash`

- Type `export PATH=$PATH:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/global/home/groups/fc_demog/stata18`

type `xstata-mp` to launch the GUI




## Transferring data 

Documentation on how to move things around: https://pages.github.berkeley.edu/demography/computing-lab/research-computing.html#storing-and-transferring-data-on-savio

If you prefer not to use terminal, open on demand provides a nifty file interface to upload (smaller files < 1GB) and download to your home and scratch directories:

<img width="328" alt="image" src="https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/f45c53ee-1592-4a91-a3ea-e46ee54b72c9">


<img width="1154" alt="image" src="https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/b6761c5f-f3db-45b8-87d0-4364fb2fe0e9">




