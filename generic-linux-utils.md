Do a ping sweep to check if the host is alive?

```
prefix="x.y.z"; for i in {1..20}; do if ping $prefix.$i -c 1 -W 1 ; then echo "Host $prefix.$i is reachable."; else echo "Host $prefix.$i is unreachable."; fi; done
```
