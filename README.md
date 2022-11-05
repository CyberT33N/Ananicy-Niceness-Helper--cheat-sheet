# Ananicy Cheat Sheet

<br><br>

## Guides
- https://www.maketecheasier.com/control-apps-priorities-with-ananicy-linux/

<br><br>

## Good 2 know
- A niceness of -20 is the highest priority and 19 is the lowest priority. The default niceness for processes is inherited from its parent process and is usually 0.







<br><br>
________________________________
________________________________
<br><br>


# Install
```shell
# To install it on Ubuntu, Mint, Debian, and compatible distributions, use:
git clone https://github.com/Nefelim4ag/Ananicy.git
./Ananicy/package.sh debian
sudo dpkg -i ./Ananicy/ananicy-*.deb

# If you are on Arch, Manjaro, or another similar distribution, you can install it with:
git clone https://github.com/Nefelim4ag/Ananicy.git /tmp/ananicy
cd /tmp/ananicy
sudo make install
```

```shell
sudo systemctl enable ananicy
sudo systemctl start ananicy
```






























<br><br>
________________________________
________________________________
<br><br>

# Rules

<br><br>

## Default rules
```shell
cd /etc/ananicy.d/00-default/
```

<br><br>

## Available types
```shell
ananicy dump types
```

<br><br>

## Add your own rules
```
cd /etc/ananicy.d/00-default/
sudo nano youProcessname.rules
// { "name": "timeshift", "type": "BG_CPUIO", "nice": 17, "ioclass": "idle" }
```

