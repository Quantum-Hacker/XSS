**Quantum-XSS Tool**

**Overview**
This tool is runnning based on BASH scripting and this tool is used to automate your XSS finding task like it can able to find RXSS & BXSS mostly.

**Features**
Fetch URLs from Wayback Machine and gau.
Filter and identify potential XSS vulnerable URLs using GF Patterns.
Support for Blind XSS payload injection.
Automate XSS scanning using Dalfox.
Save and organize results in structured directories.

Prerequisites
To run Custom-XSS, you need to have the following tools installed on your system:

Waybackurls-https://github.com/tomnomnom/waybackurls

gau-https://github.com/lc/gau

gf-https://github.com/tomnomnom/gf

Dalfox-https://github.com/hahwul/dalfox



**Installation**
Clone this repository:

git clone https://github.com/Quantum-Hacker/XSS

cd Quantum-XSS

chmod +x XSS.sh

**Usage**
The tool provides flexibility in its usage by allowing the user to run various configurations based on the domain, output preferences, and Blind XSS payloads.


./XSS.sh -d <target.com>

./XSS.sh -d <target.com> -b <blindxss.xss.ht>

./XSS.sh -d <target.com> -o <outputfile.txt>

./XSS.sh -d <target.com> -b <blindxss.xss.ht> -o <outputfile.txt>



**Command-line Arguments**

Argument        Description

-d, --domain    The target domain to perform XSS scanning on. (required)

-b, --blind     The Blind XSS payload URL to be injected for testing. (optional)

-o, --output    The file to store results. Defaults to results.txt if not specified.

-h, --help      Display the help message.

-v, --version   Display the current version of the tool.




**Example**

./XSS.sh -d example.com -b blindxss.example.ht -o xss_results.txt

In this example:

The script scans example.com for potential XSS vulnerabilities.
It injects the provided Blind XSS payload (blindxss.example.ht) during the scanning process.
The results are saved in xss_results.txt.