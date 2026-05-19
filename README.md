# UCE-aphidae-phyluce
Commands used to find UCE seqeunces in aphid assemblies to build phylogeny

### Obtaining the NCBI aphid refrence genomes

Simply used ncbi's cli tool datasets to access the api in a human readable way

```
datasets download genome taxon "Aphididae" --reference
```

### Create Baits

Bash script Extract-UCE was run to build the initial Bait-seqeunces to be used on each genome to obtain the UCE's

```
sbatch Extract-UCE
```

### Extract UCE with baits

The resulting baits from this script were then used to searh the UCE of each genome with lastz

```
sbatch lastz-baits
```
