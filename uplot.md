# uplot

statistical analysis visualization

```
ps aux | awk '{print $1}' | uplot count
https://github.com/red-data-tools/YouPlot

echo -e "from numpy import random;" \
        "n = random.randn(10000);"  \
        "print('\\\n'.join(str(i) for i in n))" \
| python3 \
| uplot hist --nbins 20

curl -sL https://git.io/ISLANDScsv \
| sort -nk2 -t, \
| tail -n15 \
| uplot bar -d, -t "Areas of the World's Major Landmasses"

curl -sL https://git.io/AirPassengers \
| cut -f2,3 -d, \
| uplot line -d, -w 50 -h 15 -t AirPassengers --xlim 1950,1960 --ylim 0,600

curl -sL https://git.io/IRIStsv \
| cut -f1-4 \
| uplot scatter -H -t IRIS

curl -sL https://git.io/IRIStsv \
| cut -f1-4 \
| uplot density -H -t IRIS
```

