# notes
Trick for getting wireshark data from other computer in host computer
ssh root@192.168.12.12 sudo -S tcpdump -i any -U -s0 -w - 'not port 22' | wireshark -k -i -
