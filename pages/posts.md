---
layout: default
title: posts
description: Jose V. Die's blog
---
[Home](../index.html)

<a href="#our-small-blow-against-the-system">2018 July</a>    
<a href="#pycon-charlas">2018 May</a>   
  

## Taxonomy identifiers and scientific names (NCBI) 
Córdoba, Feb 25, 2019.  

I have a long list of species names and my goal is to get the taxonomy identifiers from GenBank. 
I wrote some functions to fetch the NCBI ids. 

    
    get_tax_id <- function(scientific_name) {
      myterm = paste0(scientific_name,"[SCIN]")
      esearch = entrez_search(db = "taxonomy", term = myterm)
      esearch$ids
      }
      
    get_scientific_name <- function(taxid) {
      esumm <- entrez_summary(db="taxonomy", id=taxid)
      esumm$scientificname
      }
      
From species name to taxonomy id :

    mycicer <- c("Cicer macracanthum", "Cicer canariense", "Cicer chorassanicum", "Cicer cuneatum", "Cicer judaicum", 
            "Cicer yamashitae", "Cicer bijugum", "Cicer reticulatum", "Cicer echinospermum", "Cicer pinnatifidum", 
            "Cicer arietinum")
    
    mytaxids = sapply(mycicer, function(x) get_tax_id(x), USE.NAMES = FALSE)
      mytaxids
      [1] "200949" "200948" "107682" "92720"  "92719"  "92718" 
      [7] "90899"  "90898"  "90897"  "47088"  "3827" 

From taxonomy id to scientific name : 
       
    mynames = sapply(mytaxids, function(x) get_scientific_name(x), USE.NAMES = FALSE)
    mynames
     [1] "Cicer macracanthum"  "Cicer canariense"  
     [3] "Cicer chorassanicum" "Cicer cuneatum"     
     [5] "Cicer judaicum"      "Cicer yamashitae"   
     [7] "Cicer bijugum"       "Cicer reticulatum"  
     [9] "Cicer echinospermum" "Cicer pinnatifidum" 
     [11] "Cicer arietinum" 



## h Index
Córdoba, Feb 2, 2019.  
  
I just updated my old pkg. `h Index Over Years`. The R pkg. is based on the Citation record from SCOPUS and plots the h Index over the years for a given author. You can also estimate how long it takes on average to get 1 citation for your most highly accessed papers. You can download and install it from my [github](https://github.com/jdieramon/hIndex) repo in 3 very simple steps. 
  
    
    
## Data Analytics. Case study: A Ciencia Cierta
Córdoba, Jan 22, 2019.     
      
**A Ciencia Cierta** is a scientific dissemination Spanish radio show on 'CV radio'. You can find the podcasts on [IVOOX](https://www.ivoox.com/podcast-a-ciencia-cierta_sq_f1350590_1.html). I made a video-tutorial to study how the episodes length changed over time. The video is available on [YouTube](https://www.youtube.com/watch?v=nbSIXl6I8-4) and you can find the code [here](files/2019_21_01.md).   

  
## Recent NBS-LRR Gene Expansion in the Asparagus Genome
Córdoba, Nov 25, 2018.    
  
We performed a genome-wide analysis and comprehensive characterization of 49 NBS-LRR loci in the asparagus reference genome.  Take-away message:  
 1. NBS genes are unevenly distributed through the genome and nearly 50% of the genes are present in clusters. Chromosome 6 is significantly NBS-enriched and one single cluster hosts 10% of the genes.
 2. Recent duplications are likely to have dominated the NBS expansion with both tandem genes and duplication events across multiple chromosomes. Almost all the segmental duplications that we can detect have evolved from these recent events.
 3. Expression data revealed that most of the duplicated members within a group exhibited the same expression pattern, suggesting that the functional conservation of the duplicated family members is a major feature of the evolution of these genes.  
    
Read the paper in [Genes](https://www.mdpi.com/2073-4425/9/12/568/htm).    


## Our small blow against the system  
Córdoba, July 2, 2018.

Today, I got a manuscript review invitation. The authors studied a metabolic pathway, which I am very interested in. It's fruit quality-related. The methodolical approach was sound to me as well. The journal was open access and I try to support that philosophy by publishing in those journal or accepting their invitations. So, I almost made my decision when I read that they were expecting my comments within a week.   

For the reasons I have just explained I wanted to review the manuscript. The deadline was not acceptable, though. So, for the first time, I used the great 'small blow against the system' by [Stephen Heard](https://scientistseessquirrel.wordpress.com/2018/03/06/i-refuse-all-review-requests-with-deadlines-3-weeks-heres-why-and-how/). Thus, I sent to them the following:


*Dear Editor,*

*I’d be happy to review this manuscript, but not with a 7-day deadline.  For several reasons, I believe such short deadlines are unreasonable and work to the detriment of science. They foster unhealthy attitudes about the low value of peer review.  They encourage scientists to have unrealistic expectations for the speed of review and publication.  They drive journals to lower quality by competing based on speed rather than on the value added through peer review.* 

*So, I’d be happy to review with a 3-week deadline.  Let me know if that suits you.*

*Sincerely,*

*Jose V. Die*



They got back to me in 2 hours and were supportive wiht the idea that I needed more time.


<br>


## PyCon Charlas
Bethesda (MD), May 17, 2018.  

Recientemente he tenido el honor de participar en la selección de las charlas que han formado parte de las PyCon Charlas en la 
[PyCon](https://us.pycon.org/2018/) que acaba de celebrarse en Cleveland (OH). Es la primera vez que en una conferencia PyCon US, 
las presentaciones se hacen en un idioma distinto del inglés. Se trata de una gran iniciativa coordinada por **Mayela Sánchez**, 
**Mario Corchero** y **Naomi Ceder**, y una oportunidad para toda la comunidad pythonista hispanohablante, 
cada vez más numerosa tanto en América Latina como en Europa, de exponerse ante la conferencia Python más grande del mundo... [read more >>](files/2018_05_17.md) .  


<br>



## Auxin response factor gene family in chickpea genome 
Bethesda (MD), May 2, 2018.  

We performed a genome-wide analysis and comprehensive characterization of 24 ARF genes in the chickpea reference genome. Take-away message:  
 1. Phylogenetic analysis suggests that recent duplications have played a very limited role in the expansion of the ARF family.
 2. Diversification of the ARF gene family is based on duplications, variations in domain organization and alternative splicing. Concerning duplications, segmental, but not tandem duplications, have contributed to the expansion.
 3. Duplicated pair genes have evolved mainly under the influence of purifying selection pressure with restricted functional divergence.
 4. Promoter sequence analysis reveals an enrichment of several *cis*-regulatory elements related to symbiosis, and modulation of plant gene expression during the interaction with microbes.  
          
          
Read the paper in [BMC Genomics](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-018-4695-9).  




