
    Add users with specific UIDs
    sudo adduser neymar -u 2010
    sudo adduser ronaldo -u 2016

    Add groups
    sudo groupadd barca
    sudo groupadd merengues

    Add users to the groups created above
    sudo usermod -a -G barca ronaldo
    sudo usermod -a -G merengues neyma

    List password entries for neymar and ronaldo
    [ec2-user@ip-172-31-15-71 ~]$ cat /etc/passwd | grep neymar
    neymar:x:501:501::/home/neymar:/bin/bash

    [ec2-user@ip-172-31-15-71 ~]$ cat /etc/passwd | grep ronaldo
    ronaldo:x:502:502::/home/ronaldo:/bin/bash


    List group entires for barca and merengues
    [ec2-user@ip-172-31-15-71 ~]$ cat /etc/group | grep barca
    barca:x:503:ronaldo

    [ec2-user@ip-172-31-15-71 ~]$ cat /etc/group | grep merengues
    merengues:x:504:neymar
