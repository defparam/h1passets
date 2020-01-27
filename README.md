# h1passets - List HackerOne private program assets
This python3 script will take your HackerOne host-session cookie and will automatically query for all your private programs assets that are in-scope and eligible for bounty. The script will then print those URLs to stdout.

## Usage
**h1passets \<Your HackerOne __Host-session Token\>**

## Example
```
bash> h1passets JGH92kd9...b5e
www1.private-bounty1-uri.com
api.private-bounty1-uri.com
*.private-bounty1-uri-cloud.com
secure.private-bounty2-uri.com
*.private-bounty2-uri.com
bash>
```
