# Error
${red}
./dist.sh line 9: raven-cli: command not found
error:  was not a number. Halting distribution with critical error.
- Line 9 in dist.sh: mempoolsize=$(raven-cli getmempoolinfo  | grep size | awk '{print $2}' | sed 's/,//g')
- Note:  There are two spaces in the error line between "error:" and "was not".  Not sure if that means something.


# Cheat Sheet
## For Linux
_____________
1. Download Raven Core
2. Go to bin where raven-qt is
3. $./raven-qt
4. Write down 12 words
5. Once sync starts $CTRL+c in the terminal
6. Find, then edit and save raven.conf(Appendix 1)
8. Go to bin where raven-qt is
9. Make file called dist.sh(Appendix 2)
11. Make file called addresses.txt(Appendix 3)
13. Open terminal
14. $sudo chmod u+x raven-qt
15. $sudo chmod u+x ravend
16. $./raven-qt -reindex
17. Wait for full sync
18. CTRL+c
19. $./ravend
20. Wait for full sync
21. Open new tab
22. $raven-cli
23. $sudo chmod u+x dist.sh
24. $./dist.sh


## Appendix

1.raven.conf text
https://github.com/corviato1/RavencoinAssetDistributor/blob/master/.raven/raven.conf 

2. dist.sh text
https://github.com/corviato1/RavencoinAssetDistributor/blob/master/dist.sh 

3. addresses.txt example:
https://github.com/corviato1/RavencoinAssetDistributor/blob/master/addresses.txt 






