Check running processes
Inspect one systemd service
Capture a small troubleshooting flow

Run and record output for at least 6 commands

Include 2 process commands (ps, top, pgrep, etc.) - 
----------------------------------------------------------------------------
--grep (global regular expression print) command - it search for a perticular string/keywork from a file and print lines matching the patterns. we ca use it with file directory or process to get the required output.

syntax- grep [option] pattern [file]

grep -i "keyword" file - to ignore the upper case and lower case while searching
grep -v "keyword" file - to search everything except given keyword 
grep -c "keyword" file - to print howmany times given keyword present in the file 
grep -w "keyword" file - search for exact match of given keywork in the file
grep -n "keyword" file - to print the line number of the matches of given keyword in the file

Check man for more grep options 

egrep - you can use it with pipe command to search multiple words from the file - ex - egrep "word1|word2|word3" [file]
pgrep - process grep used to check pid or process related info ex - { ps -ef | grep nginx } or { pgrep nginx }
fgrep - if you wannt to find any word with exact extension or if contaons any symbol in it
zgrep - if you want to search anything in zipped file 
----------------------------------------------------------------------------

Include 2 service commands (systemctl status, systemctl list-units, etc.)

sudo systemctl start/stop <service name> - to start or stop the process
sudo systemctl status <service name> - to check the status
sudo systemctl restart <service name> - to restart the service
sudo systemctl enable <service name> - to make service auto start whenever system is restarted 


Include 2 log commands (journalctl -u <service>, tail -n 50, etc.)
Pick one service on your system (example: ssh, cron, docker) and inspect it
Keep it simple and actionable

