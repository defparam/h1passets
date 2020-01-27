# h1passets - List HackerOne private program assets
This python3 script will take your HackerOne host-session cookie and will automatically query for all your private programs assets that are in-scope and eligible for bounty. The script will then print those URLs to stdout.

## Usage
**python3 h1passets \<Your HackerOne __Host-session Token\> \<catagory\>**

Catagories: url, mobile, other, hardware, all (default: url)

## WARNING
**THIS SCRIPT HANDLES YOUR H1 SESSION TOKEN WHICH CONTAINS YOUR HACKERONE PRIVATE DATA AND THE PRIVATE DATA OF YOUR HACKERONE CUSTOMERS. BECAREFUL WHEN HANDLING THIS TOKEN.**

It is suggested that you assign your token into a variable once using `export` and pushing the env variable into the script's argument list (as shown in the examples).


## Examples
```
bash> export H1_TOKEN="JGH92kd9...b5e"
bash> python3 h1passets $H1_TOKEN
www1.private-bounty1-uri.com
api.private-bounty1-uri.com
*.private-bounty1-uri-cloud.com
secure.private-bounty2-uri.com
*.private-bounty2-uri.com
bash>
```
```
bash> export H1_TOKEN="JGH92kd9...b5e"
bash> python3 h1passets $H1_TOKEN hardware
John's widgets
Jane's widgets
bash>
```
