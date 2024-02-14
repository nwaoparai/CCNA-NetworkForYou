C:\>ping 192.168.1.2

Pinging 192.168.1.2 with 32 bytes of data:

Reply from 192.168.1.2: bytes=32 time=12ms TTL=128  
Reply from 192.168.1.2: bytes=32 time<1ms TTL=128  
Reply from 192.168.1.2: bytes=32 time<1ms TTL=128  
Reply from 192.168.1.2: bytes=32 time<1ms TTL=128  

C:\>ping 192.168.1.1

Pinging 192.168.1.1 with 32 bytes of data:

Reply from 192.168.1.1: bytes=32 time=1ms TTL=128  
Reply from 192.168.1.1: bytes=32 time<1ms TTL=128  
Reply from 192.168.1.1: bytes=32 time<1ms TTL=128  
Reply from 192.168.1.1: bytes=32 time<1ms TTL=128  

Router>en  
Router#config t  
Enter configuration commands, one per line.  End with CNTL/Z.  
Router(config)#int f0/0  
Router(config-if)#ip add 192.168.1.1 255.255.255.0  
Router(config-if)#no shut  

Router(config-if)#  
%LINK-5-CHANGED: Interface FastEthernet0/0, changed state to up  

%LINEPROTO-5-UPDOWN: Line protocol on Interface FastEthernet0/0, changed state to up  

Router(config-if)#^Z  
Router#  
%SYS-5-CONFIG_I: Configured from console by console  

Router#config t  
Enter configuration commands, one per line.  End with CNTL/Z.  
Router(config)#int f0/1  
Router(config-if)#ip add 192.168.20.1 255.255.255.0  
Router(config-if)#no shut  

192.168.1.2 pinging 192.168.20.2  
C:\>ping 192.168.20.2  

Pinging 192.168.20.2 with 32 bytes of data:  

Reply from 192.168.20.2: bytes=32 time=1ms TTL=127  
Reply from 192.168.20.2: bytes=32 time=27ms TTL=127  
Reply from 192.168.20.2: bytes=32 time=2ms TTL=127  
Reply from 192.168.20.2: bytes=32 time=11ms TTL=127  

![V2NETWORKFORYOU](https://github.com/nwaoparai/CCNA-NetworkForYou/assets/46776355/16ee28e7-bd79-46f0-aec7-c4999ffeab45)
