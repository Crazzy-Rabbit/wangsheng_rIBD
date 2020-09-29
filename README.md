## R dependencies
1. optparse
2. GenomicRanges

## How to use

```bash
Rscript calculate_rIBD.R -h
```
```
Usage: calculate_rIBD.R [options]

Options:
        -h, --help
                Show this help message and exit

        -v, --verbose
                Print extra output [default]
    
        -q, --quietly
                Print little output
    
        -i IBD-FILE, --ibd-file=IBD-FILE
                the IBD file that contains three poputions
    
        -f IBD-FORMAT, --ibd-format=IBD-FORMAT
                set format of input file [default beagle]
    
        -x XLIST, --xlist=XLIST
                ID list of introgressive population with outgroup
    
        -y YLIST, --ylist=YLIST
                ID list of sister population of x
    
        -z ZLIST, --zlist=ZLIST
                ID list of outgroup
    
        -o OUT-FILE, --out-file=OUT-FILE
                set the name of output file [default out]
    
        -w NUMBER, --window-size=NUMBER
                specify the window size [default 20000]
    
        -s NUMBER, --step-size=NUMBER
                specify the step size [default 10000]
```

## Example

```bash
Rscript calculate_rIBD.R -i example/Tibetan-Zebu-Yak.Chr28.beagle.ibd -x example/Tibetan.list -y example/Zebu.list -z example/Yak.list -o Tibetan-Zebu-Yak.Chr28 -w 20000 -s 10000
```

## Reference
1. Bosse, M., Megens, H., Frantz, L. et al. Genomic analysis reveals selection for Asian genes in European pigs following human-mediated introgression. Nat Commun 5, 4392 (2014). [https://doi.org/10.1038/ncomms5392](https://doi.org/10.1038/ncomms5392)
2. Wu, D., Ding, X., Wang, S. et al. Pervasive introgression facilitated domestication and adaptation in the Bos species complex. Nat Ecol Evol 2, 1139-1145 (2018).[https://doi.org/10.1038/s41559-018-0562-y](https://doi.org/10.1038/s41559-018-0562-y)
