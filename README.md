# HACKMEPLZ
Game commands

Command	What it does
help	Shows the command list in-game
networks (also targets, ls)	Lists the targets
connect <#>	Breaks into a target network (or a phone, while war-driving)
disconnect (also exit, logout)	Leaves the current target
status	Shows your progress, firewall state and trace
clear	Clears the screen

Hacking commands (you must be connected)

Full command	Shortcut	What it does
ssh nuke	nuke	Cracks the password
--bruteforce	brute (also bruteforce)	Brute forces the password; better odds, very noisy
./hashbreaker --wordlist=NEVERMORE --threads=999 --bruteforce	hash, hashbreaker, jam_device	Brute forces through the firewall and cracks the password; the loudest command
sudo ./phantom.exe --cloak --erase-traces --no-logs	phantom, log_out	Wipes your trace
sudo ./godmode --universe=local --permissions=ALL	god, godmode	Makes you admin; needs the password first
matrixctl breach --firewall=omega --inject=zero_day	breach	Injects the ransomware and owns the target; needs admin
cryptd --scan=deep --entropy=9999 --silent	scan	Silent scan that shows saved info and makes cracking easier

War-driving commands

Command	What it does
wardrive	Starts war-driving and scans for nearby phones (unlocks after you own all 5 networks)
drive	Moves to a new spot with new phones
home	Goes back to the network targets
