# Information-disclosure-



Easy information disclosure:-

cat hosts.txt | httpx -path //server-status?full=true -status-code -content-length

cat hosts.txt | httpx -ports 80,443,8009,8080,8081,8090,8180,8443 -path /web-console/ -status-code -content-length




ffuf -H "User-Agent: PENTEST" -c -w "/path/to/wordlist.txt" -maxtime-job 60 -recursion -recursion-depth 2 -u $URL/FUZZ
