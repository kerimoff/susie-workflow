# susie-workflow
Nextflow workflow for applying the [Sum of Single Effects (SuSiE)](https://stephenslab.github.io/susieR/) finemapping model to a large number of molecular QTLs.

# Usage

```bash
nextflow run main.nf\
 --qtl_results testdata/test_input.tsv\
 --cisdistance 200000 \
 --vcf_genotype_field GT\
 --permuted true\
 --n_batches 2\
 -resume \
 -profile finemapping  
```

# Dependencies
All of the dependencies of the workflow are listed in the [Dockerfile](https://github.com/kauralasoo/susie-workflow/blob/master/Dockerfile). Docker container is available from [kauralasoo/susie-finemapping](https://hub.docker.com/r/kauralasoo/susie-finemapping).

# Contributors
* Kaur Alasoo
* Masahiro Kanai
