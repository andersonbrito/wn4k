# Nextstrain build pipeline for the [WestNile 4K Project](https://westnile4k.org/)


**This is the repository used to build [nextstrain.org/WNV/NA](https://nextstrain.org/WNV/NA)**

---

## Installation / Set-Up
```
Under construction
```

## File Structure
```
Under construction
```

## Data download

#### Downloading all genomes and metadata from scratch

To automatically download data (genomes and metadata) from NCBI, run the following command. This will generate the basic inputs to run the analysis.

```
python download_sequences.py --mode separate
```

This will get all genome sequences and associated metadata from NCBI.

#### Downloading only new entries, appending new data to existing files

If existing files are provided (see examples inside `input_files` folder above), the command below will avoid re-downloading entries already present in the files (genomes and rows of metadata), and will resume the download of entries not yet present in the existing files.

```
python download_sequences.py --sequences sequences.fasta --metadata metadata.tsv --mode append
```

The argument `--append` above will append the newly downloaded sequences and metadata rows at the bottom of the corresponding files. If `--separate` is used, separate files will be generated. If names for `--outpu1` and `--outpu2` are provided, those will be the names of the newly generated FASTA file and metadata, respectively.


## Run the build
```
Under construction
```

#### Visualise the results
```
Under construction
```
#### Deploy the JSONs to nextstrain.org
```
Under construction
```