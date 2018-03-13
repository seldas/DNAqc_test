# DNAqc_test
Test DNAqc toolbox with Zebra-fish genome sequences

## Zebra-fish Genome data
#### Table 1: Summary of Zebra-fish genome from Sanger-Institute:  
  
| Assembly Version |	Date |	Size (Gb) |	Fragments |	Clone Content	| Note | Download File
| --- | --- | --- | --- | --- | --- | --- |
|Zv2  |	2003 |	1.31 |	83,470 |	WGS	| Super-contigs | Zv2/Zv2.agp1.fasta.gz
|Zv3	|	2003 |	1.46 |	58,339 |	WGS	| Super-contigs | Zv3/Zv3.supercontigs.fa.gz
|Zv4	|	2004 |	1.56 |	21,333 |	36%	| Scaffolds | Zv4/Zv4.fasta.gz
|Zv5	|	2005 |	1.63 |	16,214 |	43%	| Scaffolds | Zv5/Zv5.fa.gz
|Zv6	|	2006 |	1.63 |	6,653 |	63%	| Scaffolds | Zv6/Zv6_scaffolds.fa.gz
|Zv7	|	2007 |	1.44 |	5,036 |	71%	| Scaffolds | Zv7/Zv7_scaffolds.fa.gz
|Zv8	|	2008 |	1.48 |	11,632 |	77%	| Top-Leve | Zv8/Zv8_toplevel.fa.gz
|Zv9	|	2010 |	1.41 |	4,560 |	83%	| Top-Level | Zv9/Zv9_toplevel.fa.gz
  
  
## DNAqc toolkit
DNAqc toolkit is one software developed by Gokhan et.al at National Center for Toxicological Research (NCTR). It is quite powerful.  

* General usage:
```java
Java -jar DNAqc.jar [general options] [command] [command options]  
```

* Available commands: (option with * means essential)
    - **reevaluate**:     Main function.
    - **generate1**:      Contig Generate command type 1 with given coordinates of contigs on the reference as input
    - **generate2**:      Contig Generate command type 2 with given desired contig lengths as input. The contigs' coordinates are randomly selected on the reference
    - **generate3**:      Contig Generate command type 3. This command can generate contigs with three types of distributions: NORMAL, GAMMA and UNIFORMwith possible mean, standard deviation of contig sizes and total number of contigs are specified by the user. The contig lengths are drawn from a normal distribution with the given parameters
    - **generate4**:      Contig Generate command type 4 with mean, standard deviation of contig sizes and depth of coverage are specified by the user. The contig lengths are drawn from a normal distribution with the given parameters
    - **alignandevaluate**:      Assing the quality score to the contigs calculated with respect to a reference genome
    - **model**:      Given a reference compute a multiple linear regression model to be used in evaluation

