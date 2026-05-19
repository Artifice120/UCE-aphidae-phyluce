# UCE-aphidae-phyluce
Commands used to find UCE seqeunces in aphid assemblies to build phylogeny

Bash script Extract-UCE was run to build the initial Bait-seqeunces to be used on each genome to obtain the UCE's

```
sbatch Extract-UCE
```

The resulting baits from this script were then used to searh the UCE of each genome with lastz

```
sbatch lastz-baits
```
