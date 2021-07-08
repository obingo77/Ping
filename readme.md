1..255 | % {echo "192.168.137.$_"; ping -n 1 -w 100 192.168.137.$_ |
Select-String ttl}

ping -c 1 127.0.0.1 &> /dev/null && echo success || echo fail
