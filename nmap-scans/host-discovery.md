# Nmap Host Discovery & Service Enumeration

## Host Discovery
\\\ash
nmap -sn 192.168.56.0/24 -oA results/host-discovery
\\\

## Top Ports + Service/Version
\\\ash
nmap -sV -sC -Pn --top-ports 100 192.168.56.101 -oA results/target-101
\\\

## Tips
- Save XML (\-oX\) if you want to parse later
- Capture screenshots of terminal results for README snippets
