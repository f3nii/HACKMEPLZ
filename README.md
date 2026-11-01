# HACKMEPLZ
HACKMEPLZ

A fictional “hacker terminal” game built with Python and Tkinter. You play a hacker in a green-on-black terminal, breaking into made-up networks with movie-style commands. Everything is pretend, and nothing in it touches a real network or device.

How to run

Requires Python 3 with Tkinter (included with most Python installs). There are no other dependencies.

python hacker_terminal.py

Type help in-game for the full command list.

How to play

You start with 5 networks, rated 1 to 5 for difficulty. Connect to one with connect <#>, then work through the usual hack:

Scan the system (scan) for saved info and easier cracking.
Crack the password (nuke, brute, or hash).
Become admin (god).
Inject the ransomware (breach) to own the network and score points.

Every action raises a trace meter, and the harder the network, the faster it climbs. If it hits 100%, you get kicked out and the network stays on alert. Use phantom to wipe your trace between steps.

Features
5 networks with difficulty ratings, and a score that rewards a low trace.
Commands with long movie-style names and short shortcuts. Both always work.
A special bank-hack screen when you own the NorthBank Vault.
War-driving mode, unlocked after owning all 5 networks. You scan for nearby fictional phones and hack them for points. They build suspicion more slowly than networks.
A rare, extra-tough phone with a very sensitive anti-virus and a big bonus for beating it.
A hidden secret to find. 😉
Command history with the up and down arrow keys.
Disclaimer

This is a game. All networks, phones, people and data in it are made up. It contains no real hacking tools.

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
