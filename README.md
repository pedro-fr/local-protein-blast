# local-protein-blast
Script to run a local protein blast using different databases.
## Create database
To create a BLAST database, use the `makeblastdb` command from the BLAST+ suite. Here is an example:

```sh
makeblastdb -in input.fasta -dbtype prot -out my_database
```

- `-in input.fasta`: Specifies the input FASTA file containing protein sequences.
- `-dbtype prot`: Indicates that the database type is protein.
- `-out my_database`: Specifies the name of the output database.

Ensure that you have the BLAST+ suite installed and properly configured in your environment.

## Run blastp
To run a BLASTP search, use the `blastp` command from the BLAST+ suite. Here is an example:

```sh
blastp -query query.fasta -db my_database -out results.txt
```

- `-query query.fasta`: Specifies the input FASTA file containing the query protein sequences.
- `-db my_database`: Indicates the database to search against.
- `-out results.txt`: Specifies the name of the output file to save the results.

