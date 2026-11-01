# HACKMEPLZ

A fictional "hacker terminal" game built with Python and Tkinter. You play a hacker in a green-on-black terminal, breaking into made-up networks with movie-style commands.

**Everything in this game is pretend.** Nothing in it touches a real network or device, and it contains no real hacking tools.

## How to run

Requires Python 3 with Tkinter (included with most Python installs). There are no other dependencies.

```
python hacker_terminal.py
```

Type `help` in-game to see the command list.

## How to play

You start with 5 networks, rated 1 to 5 for difficulty (1 is the easiest, 5 is the hardest). Connect to one with `connect <#>`, then work through the usual hack:

1. **Scan** the system (`scan`) to get saved info and make cracking easier.
2. **Crack the password** (`nuke`, `brute`, or `hash`).
3. **Become admin** (`god`).
4. **Inject the ransomware** (`breach`) to own the network and score points.

Every action raises a **trace** meter, and the harder the network, the faster it climbs. If it hits 100%, you get kicked out and the network stays on alert. Use `phantom` to wipe your trace between steps.

A strong run on a hard network looks like this:

```
connect 4
scan
hash
phantom
god
phantom
breach
```

## Features

- 5 networks with difficulty ratings, and a score that rewards keeping your trace low
- Long movie-style commands with short shortcuts (both always work)
- A special bank-hack screen when you own the NorthBank Vault
- **War-driving mode**, unlocked after owning all 5 networks: scan for nearby fictional phones and hack them for points. Phones build suspicion more slowly than networks
- A rare, extra-tough phone with a very sensitive anti-virus and a big bonus for beating it
- A hidden secret to find 😉
- Command history with the up and down arrow keys

## Commands

### Game commands

| Command | What it does |
|---|---|
| `help` | Shows the command list in-game |
| `networks` (also `targets`, `ls`) | Lists the targets |
| `connect <#>` | Breaks into a target network (or a phone, while war-driving) |
| `disconnect` (also `exit`, `logout`) | Leaves the current target |
| `status` | Shows your progress, firewall state and trace |
| `clear` | Clears the screen |

### Hacking commands

You must be connected to a target to use these.

| Full command | Shortcut | What it does |
|---|---|---|
| `ssh nuke` | `nuke` | Cracks the password |
| `--bruteforce` | `brute` (also `bruteforce`) | Brute forces the password. Better odds than `nuke`, but very noisy |
| `./hashbreaker --wordlist=NEVERMORE --threads=999 --bruteforce` | `hash`, `hashbreaker`, `jam_device` | Brute forces through the firewall and cracks the password. The loudest command |
| `sudo ./phantom.exe --cloak --erase-traces --no-logs` | `phantom`, `log_out` | Wipes your trace |
| `sudo ./godmode --universe=local --permissions=ALL` | `god`, `godmode` | Makes you admin. Needs the password first |
| `matrixctl breach --firewall=omega --inject=zero_day` | `breach` | Injects the ransomware and owns the target. Needs admin |
| `cryptd --scan=deep --entropy=9999 --silent` | `scan` | Silent scan that shows saved info and makes cracking easier |

Typing the full version of a command works the same as its shortcut. The shortcuts always use all of a command's flags, so `phantom` does a full trace wipe. To wipe only part of your trace, type the long command with just some of the flags.

### War-driving commands

| Command | What it does |
|---|---|
| `wardrive` | Starts war-driving and scans for nearby phones (unlocks after you own all 5 networks) |
| `drive` | Moves to a new spot with new phones |
| `home` | Goes back to the network targets |

While war-driving, use the same hacking commands on phones. Phones are rated 1 to 3 for difficulty and use a 4-digit PIN. They build **suspicion** instead of trace, and they build it at half speed. If suspicion hits 100%, the owner spots the van and that phone disappears.

## Disclaimer

This is a game. All networks, phones, people, accounts and data in it are made up.
