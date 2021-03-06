[home](https://adminadminctf.github.io/ctf/)

# File transfer
We get a pcap file which we open in WireShark. It comprises only 28 packets from only two different hosts - so this challenge should not be too difficult. Usually we would first navigate through the TCP streams via right-click on a TCP packet -> ```Follow``` -> ```TCP Stream``` to get an idea of what is (roughly) going on. Here we only need to scroll a little to see that a JPEG picture has been transferred (see screenshot below, grey row).

![Imgur](https://i.imgur.com/xmTFv2r.png)

We probably could extract the picture manually, but WireShark already comes with the exact feature required here. Navigate to ```File``` -> ```Export Objects``` and select the only file available. Save it somewhere as .JPEG and enjoy the flag!

![Imgur](https://i.imgur.com/yPQMpfL.jpg)

## actf{0ver_th3_w1re}
