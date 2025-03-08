# 403-Bypass-Jagat
### Introduction

**403-Bypass-Jagat**
Tool to bypass 403/401. This script contain all the possible techniques to do the same. 

- **Note:** If multiple `[200 OK]` responses or bypasses appear in the output, please verify the Content-Length. If the Content-Length is identical for multiple `[200 OK]` responses or bypasses, it indicates a false positive. Possible reasons could include "301/302" redirects or "../" [Payload]. **Do not panic.**

- The script will output the `cURL` payload if a potential bypass is detected.

### Installation
   * `git clone https://github.com/jagat-singh-chaudhary/403-Bypass-Jagat.git`
   * `cd 403-Bypass-Jagat`
   * `chmod +x 403-Bypass-Jagat.sh`
   * `sudo apt install figlet`  - If you are unable to see the logo as in the screenshot

### Video Preview

![403-Bypass-Jagat](https://github.com/jagat-singh-chaudhary/403-Bypass-Jagat/blob/main/403-Bypass-Jagat.gif)

###  Help
```bash
Jagat_Singh:$ bash 403-Bypass-Jagat.sh -h
```
<img src="/403-Bypass-Jagat.png" alt="403-Bypass-Jagat" width="1000px">

### Usage / Modes

- Scan with specific payloads:
  * [ `--header` ] Support HEADER based bypasses/payloads
    ```bash
    Jagat_Singh:$ bash 403-Bypass-Jagat.sh -u https://target.com/secret --header
    ```
  * [ `--protocol` ] Support PROTOCOL based bypasses/payloads
    ```bash
    Jagat_Singh:$ bash 403-Bypass-Jagat.sh -u https://target.com/secret --protocol
    ```
  * [ `--port` ] Support PORT based bypasses/payloads
    ```bash
    Jagat_Singh:$ bash 403-Bypass-Jagat.sh -u https://target.com/secret --port
    ```
  * [ `--HTTPmethod` ] Support HTTP Method based bypasses/payloads
    ```bash
    Jagat_Singh:$ bash 403-Bypass-Jagat.sh -u https://target.com/secret --HTTPmethod
    ```
  * [ `--encode` ] Support URL Encoded bypasses/payloads
    ```bash
    Jagat_Singh:$ bash 403-Bypass-Jagat.sh -u https://target.com/secret --encode
    ```
  * [ `--SQLi` ] Support MySQL mod_Security & libinjection bypasses/payloads [** New **]
    ```bash
    Jagat_Singh:$ bash 403-Bypass-Jagat.sh -u https://target.com/secret --SQLi
    ```
- Complete Scan {includes all exploits/payloads} for an endpoint [ --exploit ]
```bash
Jagat_Singh:$ bash 403-Bypass-Jagat.sh -u https://target.com/secret --exploit
```

### Prerequisites
- apt install curl [Debian]


## ☕ Buy Me a Coffee

If you find our work helpful and would like to support us, consider buying us a coffee. Your support keeps us motivated and helps us create more awesome contents and Tools. ❤️

☕ **Support Us Here:** [https://buymeacoffee.com/jagatsingh](https://buymeacoffee.com/jagatsingh)
