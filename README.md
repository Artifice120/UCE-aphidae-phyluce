# UCE-aphidae-phyluce
Commands used to find UCE seqeunces in aphid assemblies to build phylogeny

### containers and environment 
Containers and environments used here can be remade here

```
bash dependancies
```
paths for the singularity containers will need to be changed in the other scripts

### Obtaining the NCBI aphid refrence genomes

Used ncbi's cli tool datasets to access the api in a human readable way and renamed the files to only have the srr number

```
bash get-refs
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
