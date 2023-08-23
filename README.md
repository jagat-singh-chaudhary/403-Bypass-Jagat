# 403-Bypass-Jagat
### >_ Introduction

**403-Bypass-Jagat**
Tool to bypass 403/401. This script contain all the possible techniques to do the same. 

- **NOTE** : If you see multiple [200 Ok]/bypasses as output, you must check the Content-Length. If the content-length is same for multiple [200 Ok]/bypasses means false positive. Reason can be "301/302" or "../" [Payload] DON'T PANIC.
- Script will print `cURL` PAYLOAD if possible bypass found.

### >_ Preview
![403-Bypass-Jagat_priview](/403-Bypass-Jagat.mp4)

### >_ Help
```bash
root@Jagat_Singh:$ bash 403-Bypass-Jagat.sh -h
```
<img src="/403-Bypass-Jagat.png" alt="403-Bypass-Jagat" width="1000px">

### >_ Usage / Modes

- Scan with specific payloads:
  * [ `--header` ] Support HEADER based bypasses/payloads
    ```bash
    root@Jagat_Singh:$ bash 403-Bypass-Jagat.sh -u https://target.com/secret --header
    ```
  * [ `--protocol` ] Support PROTOCOL based bypasses/payloads
    ```bash
    root@Jagat_Singh:$ bash 403-Bypass-Jagat.sh -u https://target.com/secret --protocol
    ```
  * [ `--port` ] Support PORT based bypasses/payloads
    ```bash
    root@Jagat_Singh:$ bash 403-Bypass-Jagat.sh -u https://target.com/secret --port
    ```
  * [ `--HTTPmethod` ] Support HTTP Method based bypasses/payloads
    ```bash
    root@Jagat_Singh:$ bash 403-Bypass-Jagat.sh -u https://target.com/secret --HTTPmethod
    ```
  * [ `--encode` ] Support URL Encoded bypasses/payloads
    ```bash
    root@Jagat_Singh:$ bash 403-Bypass-Jagat.sh -u https://target.com/secret --encode
    ```
  * [ `--SQLi` ] Support MySQL mod_Security & libinjection bypasses/payloads [** New **]
    ```bash
    root@Jagat_Singh:$ bash 403-Bypass-Jagat.sh -u https://target.com/secret --SQLi
    ```
- Complete Scan {includes all exploits/payloads} for an endpoint [ --exploit ]
```bash
root@Jagat_Singh:$ bash 403-Bypass-Jagat.sh -u https://target.com/secret --exploit
```

##### Prerequisites
- apt install curl [Debian]

## Support
If you like `403-Bypass-Jagat` and it help you in work, money/bounty, pentesting, recon or just brings you happy feelings, please show your support ! 
