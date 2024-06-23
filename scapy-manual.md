sudo scapy - accessing Scapy from within the Linux terminal, as root.



lsc() - find out all the available commands that Scapy provides for packet captures, handling, decoding and analysis.



ls() - see all the network protocols that Scapy provides support for.



ls(BOOTP) - see the packet fields, structure and default values for each network protocol.



print(sniff.__doc__) - see all the available parameters that the sniff() function can take.



pkt = sniff(iface = 'enp0s8', count =  5) - an example of sniffing 5 packets on interface enp0s8.



pkt.show() - returns 5 records, the 5 network packets that the sniff() function has detected.



pkt[0] - returns detailed information on the first packet (index 0) in the capture.



pkt[0].show() - the same information as before, but a cleaner output.



pkt[0][2] - returns a certain layer from within the packet (in this case, the 3rd layer - positioned at index 2).



pkt[0][ICMP] - returns the same result as above, only that we are specifying the name of the layer, instead of its index.



pkt[0][2].summary() - returns a summary of the information about a certain layer.



pkt[0][1].src - returns the value corresponding to a certain parameter inside a certain layer.