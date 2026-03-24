Do a ping sweep to check if the host is alive?

for i in {191..204}; do if ping x.x.x.$i -c 1 -W 1 ; then echo "Host $i is reachable."; else echo "Host $i is unreachable."; fi; done
