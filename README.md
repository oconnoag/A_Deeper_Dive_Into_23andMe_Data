# A Deeper Dive into 23andMe Data 
### Alijah O'Connor
<small>Based on the R tutorial posted on <a href="https://dabblingwithdata.wordpress.com/2018/07/16/analysing-your-23andme-genetic-data-in-r-part-1-importing-your-genome-into-r/">here</a> on dabblingwithdata.wordpress.com.</small>

23andMe is a company that specializes in personalized genetic reports for the purposes of providing information about ancestry, health, and personal traits. Human DNA is over 99% identical from person to person; however, there exist small variations in each person's genome called small nucleotide polymorphisms (SNPs). Based on these SNPs, researchers can conduct observational studies that find correlations between certain SNPs and Diseases. 23andMe utilizes this idea of SNPs-Disease correlation by genotyping thousands of SNPs in each client's genome and determines whether or not particular SNPs relevant to a disease exist in that client's genome.


After a client's analysis is completed, they are given access to a dashboard containing the relevant information about what their genes are saying (expressed as likelihoods). Most individuals that use 23andMe as a service, however, do not realize that the 23andMe analysis is not necessarily complete. There are many published reports on SNPs that are not (yet) considered by the 23andMe team in their analyses due to lack of general consensus. Luckily, with the power of this Jupyter Notebook, one can look into their own SNP data and make their own conclusions. 
<br><br>
*Disclaimer:  make your own conlusions at your own risk -- biology is complicated, so don't be too rash in finalizing your beliefs*

<b>Requirements:</b>
- Python3+
    Pandas
- 23andMe Raw Data (text file)
- gwas_data.csv in current working directory
