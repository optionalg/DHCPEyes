# DHCPEyes :eyes:
**Intercept requests passively of DHCP from own network!**

<img 
src="https://raw.githubusercontent.com/vincenzogianfelice/DHCPEyes/master/media/demo.png"
alt="DemoImage"
/>

# Installation
###### Require python2.7 (also python3.5)

```
pip2 install -r requirements.txt
```

#### Windows
- First, install [WinPcap](https://www.winpcap.org/install/)
- After installed winpcap, run file exe after [downloaded](https://github.com/vincenzogianfelice/DHCPEyes/releases)
- For findings interfaces on Windows, digit in prompt:

```
netsh interface show interface
```

and copy the 4 column (```Nome interfaccia```/```Name interface```)

# Usage
```
    ____  __  ____________  ______
   / __ \/ / / / ____/ __ \/ ____/_  _____  _____
  / / / / /_/ / /   / /_/ / __/ / / / / _ \/ ___/
 / /_/ / __  / /___/ ____/ /___/ /_/ /  __(__  )
/_____/_/ /_/\____/_/   /_____/\__, /\___/____/
                              /____/

        * DHCP Passive Listener! (v1.0) *

Usage: ./dhcpeyes.py -i <interface>

Optional:
     -o <arg>  File Output Save
     -t <arg>  REQUEST types: DHCPR (request),  DHCPD (discover)
```
###### Examples
```
./dhcpeyes.py -i wlan0 -t DHCPR  # Intercept only DHCPREQUEST
./dhcpeyes.py -i wlan0  # Intercept all
```
**for windows**
```
./dhcpeyes.py -i "Connessione alla rete locale (LAN)" -t DHCPR  # Using "Connessione alla rete locale (LAN)" provided from output of command netsh
```

# Donazioni

**BTC:** *3EwV4zt9r5o4aTHyqjcM6CfqSVirSEmN6y*

# Contatti

**Email:** *developer.vincenzog@gmail.com*
