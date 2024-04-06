# stata-savio-notes

## Open OnDemand

- First log into [Open OnDemand](https://ood.brc.berkeley.edu/) (with your brc username/pin + one time password). This is a graphical interface to Savio with Rstudio, Jupyter and virtual desktop.

Select `Interactive Apps > Desktop`

![image](https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/87200dce-e07e-4574-add7-33fa9e2c90d0)


## Scheduling

[![image](https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/34fed54f-f0ee-43ae-9e20-4d5fb5932c08)
](https://files.slack.com/files-tmb/T04D70QSMFG-F06SZUCKQTF-c2ac974021/image_720.png)

:point_up: The important fields are `SLURM Partition` and `Wall Clock Time` . Partition should be `savio2` or `savio3` . Wall clock time should be the number of hours you'd like for your session to run.

you'll be queued. Lower wall clock times will have faster wait times. 

![image](https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/e0e1ce65-a545-4a4e-a11a-395b5aa55b88)

click `Launch Desktop`

![image](https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/4a1435e2-a2e2-4c49-9d6b-46ea9fedda72)


## Remote Desktop

You'll see a funky desktop. Right click somewhere and select `Open Terminal Here`


![image](https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/6e4f1044-41d8-469b-b112-fcb868d12009)


`cd` into `/global/home/groups/fc_demog/stata18` and run `./xstata-mp`

![image](https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/de74f6b1-8503-4d95-9a3d-5f1db6cc83d5)

Stata!

![image](https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/5ddc4cd3-2678-4704-a401-d9eb17d4d9c4)


## Transferring data 

I have some documentation on how to move things around: https://pages.github.berkeley.edu/demography/computing-lab/research-computing.html#storing-and-transferring-data-on-savio

If you prefer not to use terminal, open on demand provides a nifty file interface to upload (smaller files < 1GB) and download to your home and scratch directories:

<img width="328" alt="image" src="https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/f45c53ee-1592-4a91-a3ea-e46ee54b72c9">


<img width="1154" alt="image" src="https://github.com/berkeley-demography/stata-savio-notes/assets/20607201/b6761c5f-f3db-45b8-87d0-4364fb2fe0e9">




