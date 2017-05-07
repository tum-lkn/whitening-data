# Overview


This project contains the measurement traces of 802.15.4e Time Slotted Channel Hopping wireless sensor network, and tools for extracting the data from them.
Evaluation results of these traces have been used in the publication:


- S. Zoppi,  M. Gürsu, M. Vilgelm, W. Kellerer, **Reliable Hopping Sequence Design for Highly Interfered Wireless Sensor Networks**, 2017 IEEE LANMAN, Osaka, Japan, June 2017 (accepted for publication)


The data is distributed under the GNU GPLv3 license. If the data is used in a publication, we ask you to cite the above paper.
If you find any bugs or inconsistencies, please contact the authors.


# Project structure


# Requirements


Required packages can be found in `folder/file.txt`


# Usage


To reproduce the results of the paper, you can use provided script ... . For example, to plot figure #8 ....:


```bash
python script.py
```


# Raw traces


Raw data files structure:


[byte #1, byte #2, ..., byte #38]\tTIMESTAMP\n
[byte #1, byte #2, ..., byte #38]\tTIMESTAMP\n


Packet structure:


|Last sender addr |last ASN     |first ASN    | sequence Nr |padding| hop #1 addr | hop #1 retx | hop #1 frequency | hop #1 RSSI | hop #2 .... until hop #6 |
|-----------------|-------------|-------------|-------------|-------|-------------|-------------|------------------|-------------|--------------------------|
| 1               | 2-6 	| 7-11        | 12-13       | 14    | 15          | 16          | 17               | 18          | 19-38                    |
