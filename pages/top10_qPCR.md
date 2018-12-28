# Revisar mi 3'5' ratio
# revisar mi mRNA quality review 


* Vandesompele J, De Preter K, Pattyn F, Poppe B, Van Roy N, De Paepe A, Speleman F (2002a) Accurate normalization of real-time quantitative RT-PCR data by geometric averaging of multiple internal control genes. Genome Biol 3:RESEARCH0034
* Vandesompele J, De Paepe A, Speleman F (2002b) Elimination of primer–dimer artifacts and genomic coamplification using a two-step SYBR Green I real-time RT-PCR. Anal Biochem 303:95–98
* Ramakers C, Ruijter JM, Deprez RH, Moorman AF (2003) Assumption-free analysis of quantitative real-time polymerase chain reaction (PCR) data. Neurosci Lett 13:62–66
* Dheda K, Huggett JF, Bustin SA, Johnson MA, Rook G, Zumla A (2004) Validation of housekeeping genes for normalizing RNA expression in real-time PCR. BioTechniques 37:112–119 . 
* Radonic A, Thulke S, Mackay IM, Landt O, Siegert W, Nitsche A (2004) Guideline to reference gene selection for quantitative real-time PCR. Biochem Biophys Res Commun 23:856–862
* Dheda K, Huggett JF, Chang JS, Kim LU, Bustin SA, Johnson MA, Rook GAW, Zumla A (2005) The implications of using an inappropriate reference gene for real-time reverse transcription PCR data normalization. Anal Biochem 344:141–143 . 
* Hugget J, Dheda K, Bustin S, Zumla A (2005) Real-time RT-PCR normalisation; strategies and considerations. Genes Immun 6:279–284 
* Perez-Novo CA, Claeys C, Speleman F, Cauwenberge PV, Bachert C, Vandesompele J (2005) Impact of RNA quality on reference gene expression stability. BioTechniques 39:52–56
* Fleige S, Walf V, Huch S, Prgomet C, Sehm J, Pfaffl MW (2006) Comparison of relative mRNA quantification models and the impact of RNA integrity in quantitative real-time RT- PCR. Biotechnol Lett 28:1601–1613
* Fleige S, Pfaffl MW (2006) RNA integrity and the effect on the real-time qRT-PCR performance. Mol Aspects Med 27:126–139
* Derveaux S, Vandesompele J, Hellemans J (2010) How to do successful gene expression analysis using real-time PCR. Methods 50: 227–230.


the qBase software (Hellemans et al. 2007) 

Today, qPCR is commonly considered a simple and mature technique; qPCR is an accurate, sensitive and fast technology for gene 
expression measurements. However, the apparent simplicity of the qPCR technology has made it vulnerable to a lack of clarity 
and transparency in the scientific literature, leading to few publications reporting in detail how results have been obtained. 
It is not that qPCR is intrinsically inaccurate, but rather it is the lack of a systematic procedure and performance that can 
lead to erroneous results and conclusions (Derveaux et al. 2010; Hugget et al. 2005). 
  
This is a summary of major steps steps required throughout the entire workflow that may influence the accuracy and reliability 
of results.


### DNAse treatement
A suitable strategy is to perform a proper DNase treatment followed by a careful check for the absence of DNA through qPCR 
analysis of a target on the crude RNA (Vandesompele et al. 2002b).

### Normalization
Normalization remains one of the most difficult tasks in qPCR (Dheda 2004). The use of reference genes is commonly accepted as 
the most appropriate normalization strategy (Hugget et al 2005). Normalization with suboptimal internal controls may result in 
different estimated values and lead to erroneous interpretations (Dheda 2005). Therefore, reference-gene-based normalisation is a major step in a qPCR experiment. 
It corrects for variable starting amounts of RNA and for differences in reverse transcription (RT) efficiency, since the 
references are exposed to the same preparation steps as the gene of interest (Bustin et al. 2005; Hugget et al. 2005; Radonic 
et al. 2004; Udvardi et al. 2008). To avoid the bias caused by a fluctuation in expression level of a single reference gene, Vandesompele et al. (2002) 
propose that at least several control genes be used and develop the statistical algorithm geNorm. The program defines a 
stability measure (M) as the average pairwise variation between a gene and all other reference genes in a given set of samples. 
Genes with the lowest M values have the most stable expression. The geNorm software represents one of the most commonly used 
algorithms to evaluate candidate reference genes by their average gene transcript expression stability across samples and has 
established itself as the de facto standard method (Derveaux et al 2010). 

 

Reference gene-based normalization corrects for variable starting amounts of RNA and for differences in RT efficiency (Udvardi et al 2007). 

Numerous studies have shown that the expression of these ‘classic’ genes can be regulated under various situations (Czechowski et al. 2005; Dheda et al. 2005).

a reference gene with stable expression can vary considerably under different conditions or tissues (Gutierrez et al. 2008a Plan J )



#MIQE
With the aim of offering a consensus on the minimum experimental data necessary for evaluating qPCR, the MIQE Guidelines have been recently published (Bustin et al. 2009).

Bustin SA, Benes V, Garson JA, Hellemans J, Huguett J, Kubista M, Mueller R et al (2009) The MIQE Guidelines: minimum information for publication of quantitative real-time PCR experiments. Clin Chem 55:611–622



Undoubtedly, the plant research community benefits from biomedical analyses, and the introduction of different technologies 
usually occurs after they have been implemented in mammalian or bacterial research. These problems have been known and 
publicized for quite a long time, and the plant scientific community has gradually recognized the need for more robust 
standards

In the field of plants, Gutierrez et al. (2008b) elegantly demonstrated recently that a reference gene with stable expression in one organism may exhibit a different expression pattern in another organism; even when studying the same organism, no reference gene could be considered as a universal reference, signifying the importance of studies aimed at the identification and/or validation of the expression stability of certain reference genes. In a high-impact study performed by Czechowski et al. (2005), it was shown that the identification of novel genes that had not previously been considered as internal controls could outperform traditional references in terms of expression stability.
The number of studies aimed at validating the presumed stability in the expression of certain reference genes studies in human and animal research contrasts with the very little attention that the validation and/or identification of reference genes has received in the plant sciences (Gutierrez et al. 2008a)
the importance of systematic validation has not been integrated in qPCR analysis (Guénin et al. 2009). As a consequence, genes currently used as references for qPCR analysis in plants are almost exclusively putative reference genes (Gutierrez et al. 2008b). 


#RNA quality
RNA quality is one of the crucial parameters that must be addressed in a gene expression profiling experiment (Bustin and Nolan 2004). The enormous impact that the lack of knowledge regarding the extent of RNA degradation has on the interpretation of results is well known (Fleige et al. 2006; Fleige and Pfaffl 2006; Perez-Novo et al. 2005).

# PCR amplification efficiency
the formation of secondary structures in the amplified fragments. This is often underestimated and consequently not considered during the different preparative steps of the qPCR experiment; however, hairpins overlapping primer annealing sites significantly hamper efficient annealing and negatively impact PCR amplification efficiency (Hoebeeck et al. 2005).
Thus, secondary structure evaluation in the amplicons should be routinely integrated into quality assurance of the qPCR workflow (Derveaux et al. 2010; Hoebeeck et al. 2007). 

the PCR efficiency (E) of each primer pair estimated from the data obtained from the exponential phase of each individual 
amplification plot and the equation (1 + E) = 10slope (Ramakers et al. 2003). 
With this method, the E value is derived from the log slope of the fluorescence versus cycle number curve for each particular 
primer pair, does not require standard curves and yields very similar amplification efficiencies compared to methods based on 
series of template dilutions (Czechowski et al. 2005).
This study was of notable importance because it led to the identification of superior reference genes compared with those 
that were available previously. The approach of identifying better reference genes from the orthologs of other plant species 
that were known to be stably expressed has proved to be more efficient than that of randomly testing endogenous genes


#qBASE
CV 
The maximisation method as PCR run set-up was chosen because it has the important advantage of not suffering from technical (run-to-run) variation between the samples (Hellemans et al. 2007).


* Udvardi MK, Czechowski T, Scheible W-R (2008) Eleven golden rules of quantitative RT-PCR. Plant Cell 20:1736–1737
* Gutierrez L, Mauriat M, Guénin S, Pelloux J, Lefebvre JF, Louvet R, Rusterucci C et al (2008a) The lack of a systematic validation of reference genes: a serious pitfall undervalued in reverse transcription-polymerase chain reaction (RT-PCR) analysis in plants. Plant Biotechnol J 6:609–618
* Guénin S, Mauriat M, Pelloux J, Van Wuytswinkel O, Bellini C, Gutierrez L (2009) Normalization of qRT-PCR data: the necessity of adopting a systematic, experimental conditions-specific, validation of references. J Exp Bot 60:487–493
* Gutierrez L, Mauriat M, Pelloux J, Bellini C, Van Wuytswinkel O (2008b) Towards a systematic validation of references in real-time RT-PCR. Plant Cell 20:1734–1735
* Graeber, K., Linkies, A., Wood, A. T. A., and Leubner-Metzger, G. (2011). A guideline to family-wide comparative state-of-the-art quantitative RT-PCR analysis exemplified with a Brassicaceae cross-species seed germination case study. Plant Cell 23, 2045–2063. doi: 10.1105/tpc.111.084103
* De Keyser, E., Desmet, L., Van Bockstaele, E., and De Riek, J. (2013). How to perform RT-qPCR accurately in plant species? A case study on flower colour gene expression in an azalea (Rhododendron simsii hybrids) mapping population. BMC Mol. Biol. 14:13. doi: 10.1186/1471-2199-14-13

