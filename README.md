# CVE-2022-25949

A years-old exploit of a local EoP vulnerability in Kingsoft Antivirus KWatch Driver version 2009.3.17.77.

## 2009..?

I reported the issue in January 2014 and was notified of the CVE 8+ years later. I decided to upload this because it is amusing enough to find my old code and that it took that long.

Thus, this must not be a new vulnerability despite the new CVE -- a quick search showed multiple reports for the same-looking vulnerability already.

## Timeline

- Jan 12, 2014: I submit the issue to IPA
- Jan 15, 2014: IPA acknowledges the submission
- Mar 10, 2022: IPA notifies me for publication (I ignored it. I thought it was spam)
- Mar 15, 2022: An [advisary](https://jvndb.jvn.jp/en/contents/2022/JVNDB-2022-000021.html) published

I sill thank IPA for doing their parts and making my day.

## Notes

The vulnerable file appears to be [ffdedbaeccbcf0b697675b24ca313cbb8e1c9ba1bd2f0a0b58a2d6a04a038479](https://www.virustotal.com/gui/file/ffdedbaeccbcf0b697675b24ca313cbb8e1c9ba1bd2f0a0b58a2d6a04a038479/details)

```
//
// Exploit for Kingsoft Antivirus KWatch Driver (KWatch3.sys)
// Target File Version: 2009.3.17.77
// Affected Product: Kingsoft Internet Security 9 Plus
//

/*
------------------------------------------------------------------------------
Shellcode is located at 7E7E7E7E.
The device was opened as 00000020.
Shellcode was executed.
The SYSTEM shell was launched.
This process will be suspended for ever.

------------------------------------------------------------------------------
Microsoft Windows [Version 6.1.7601]
Copyright (c) 2009 Microsoft Corporation.  All rights reserved.

C:\Users\user\Desktop>whoami
nt authority\system
------------------------------------------------------------------------------
*/
```
