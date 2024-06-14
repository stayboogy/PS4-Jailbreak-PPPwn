# stayboogy_PS4-Jailbreak-PPPwn

## For PS4 OFW 11.00 ONLY

## For Linux Machine ONLY - Will Never Work On Windows - Don't Waste Time With Windows

## Everything PreCompiled - No Work To Be Done - No Stupid Bullshit Directions


### How To Jailbreak


#### Step 1 - in Linux:

- install scapy
```sh
sudo apt install scapy
```
- determine your ethernet device id - enp1s0 is mine and the default
```sh
sudo ifconfig
```
- copy goldhen.bin to root of a usb drive formatted exFat and plug into PS4
- connect cat5 cable from PC network port to PS4 network port

#### Step 2 - on PS4:

- Go to `Settings` and then `Network`
- Select `Set Up Internet connection` and choose `Use a LAN Cable`
- Choose `Custom` setup and choose `PPPoE` for `IP Address Settings`
- Enter anything for `PPPoE User ID` and `PPPoE Password`
- Choose `Automatic` for `DNS Settings` and `MTU Settings`
- Choose `Do Not Use` for `Proxy Server`
- Test Internet Connection


#### Step 3 - in Linux:

- open terminal from within this git folder
- replace "enp1s0" in following command with the correct id of your ethernet device from Step 1
```sh
sudo python3 pppwn.py --interface=enp1s0 --fw=1100
```

