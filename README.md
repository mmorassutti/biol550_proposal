**Matthew Morassutti** 
**BIOL550	SPR’24	Week 6	Project Proposal**


**Draft Title:**

Resolving the Ranges of Two Species of _Arborimus_

**Question and Relevance:**

This project will clarify the ranges of two species of tree voles, red tree voles and Sonoma tree voles, that have previously been inferred though not directly assessed. This research aims to directly assess the northern range limit of the Sonoma tree vole and the southern range limit of the red tree vole by conducting phylogenomic analysis of ultraconserved elements (UCEs) of the nuclear genome and the entire mitochondrial DNA (mtDNA) genome. The primary source of molecular samples will be existing tissue collections and museum study skins, with some potential augmentation with samples extracted from feces collected from tree vole nests in trees north and south of the Klamath River. With these data I will resolve previous inferences of the range delimitation of both species most recently explored by Blois and Arbogast (2006). In this phylogenomic analysis, the flanking regions of UCEs and mtDNA will be examined to determine if these two species form reciprocally monophyletic clades, and if not, if this is the result of incomplete lineage sorting and/or recent introgression, and lastly to determine the range limits of these two species (McCormack _et al._ 2012, McLean _et al._ 2019, Zhang _et al._ 2019). Because _A. pomo_ is a Species of Special concern in California (CNDDB 2023), this study is important to understand the taxonomic relationship at the transition zone between _A. pomo_ and _A. longicaudus_. If their populations have the potential to be strongly impacted by invasive predators, it will be useful to get a better understanding of gene flow between seemingly isolated species and populations. If these species are able to navigate a purported barrier as wide as the Klamath River, this could be promising to the conservation of these species’ genetic diversity. Furthermore, by elucidating the complexity of the taxonomy of these species, resource managers may be able to advocate for their conservation with greater salience.  Currently there is no full nuclear genome for either species available in GenBank, so this research will contribute directly to the knowledge of the genetic diversity within each species.

**Focal Organism Introduction:**

Red tree voles (_Arborimus longicaudus_) and Sonoma tree voles (_A. pomo_) are arboreal rodents endemic to the Pacific Northwest and Northern California (Howell 1926). They are unique to other wildlife in this region, as they spend almost all of their life in the canopy of coniferous trees, feeding exclusively on their leaves (Taylor 1915). Terrestrial activity appears only to occur when adjacent trees are not connected by branch pathways (Swingle 2009). Both species build nests in the canopies of trees, between two and 65 meters in elevation above the forest floor (Biswell _et al._ 2000). Nests are generally spherical with a flat roof, contain one or more inner chambers, and display multiple entrance and escape tunnels (Howell 1926). The nests of males and subadult females are usually smaller than that of adult females, which have larger nests to include space for their offspring (Howell 1926, Taylor 1915). Nests may be as large as one meter in diameter and the result of several generations of tree vole activity (Adam and Hayes 1998). Nests are built against the boles of trees, in hollows or cavities, on forked trunks or broken treetops, or on closely spaced limb whorls of the forest canopy. Tree voles have also been documented using the dense branching structures of dwarf mistletoe (_Arceuthobium sp._) brooms as nesting substrate. In older trees with larger branches, tree voles may construct nests away from the bole of the tree, and nests have been observed in the outer crown of trees (Thompson and Diller 2002, Nicholas Kerhoulas, _pers. comm._). Tree voles typically nest in Douglas-fir trees but may also be found in grand fir (_Abies grandis_), Sitka spruce (_Picea sitchensis_), Western hemlock (_Tsuga heterophylla_), coast redwood (_Sequoia sempervirens_), and Pacific madrone (_Arbutus menziesii_), among others (Zentner 1977, Vrieze 1980, Meiselman and Doyle 1996, Nicholas Kerhoulas _pers. comm._). Because many of the aforementioned canopy structures used by tree voles are associated with mature trees, tree voles appear to favor stands of trees older than 80 years because of the more suitable nesting structures supported by a complex and mature canopy, though they may also be found in young stands (<80 years) (Huff _et al._ 1992, Meiselman and Doyle 1996, Lesmeister and Swingle 2017).

**Methods Overview:**

Genomic data will be extracted from dried museum study skins (n = 8) using QIAGEN DNeasy Blood and Tissue (QIAGEN, Valencia CA) DNA extraction kit following the manufacturer’s protocol and the DNA extraction protocol outlined in Kerhoulas et al. 2010. Genomic data will also be sourced from preserved tissue samples and/or existing extractions (n = 24, Murray 1995, Blois and Arbogast 2006). Individuals representing _A. albipes_, _A. longicaudus_, and _A. pomo_ will be included in this analysis, with _A. albipes_ as an outgroup. 

To determine if there is evidence of introgression among the genomes of _A. longicaudus_ and _A. pomo_, ultraconserved elements (UCEs) will be used to resolve the phylogenetic history of the genus _Arborimus_ (Faircloth _et al._ 2012, Meiklejohn _et al._ 2016). These are sections of the genome that remain constant across many species, in this case all tetrapods (Bejerano _et al._ 2004, Siepel _et al._ 2005, Stephen _et al._ 2008, Janes _et al._ 2011). Because of this, these sections will be targeted for sequencing, and assess the variation and similarities among the flanking regions of UCEs across the genome to give insight to phylogenetic patterns across the ranges of _A. longicaudus_ and _A. pomo_ (Mills _et al._ 2023). This analysis also recovers the entire mtDNA genome of each individual, which will be compared to the phylogenies generated using UCEs to discern whether any non-specific clades are the result of introgression or the result of incomplete lineage sorting (Mills _et al._ 2023).

UCE and mtDNA sequencing will be outsourced to Arbor Biosciences (Ann Arbor, Michigan) and their MyReads NGS services, including library preparation, target enrichment with myBaits UCE Tetrapods 5kv1 probe set (http://ultraconserved.org), pooling, and sequencing will be used. All indexed reads will be demultiplexed with the Arbor Biosciences Standard DNA (8-plex capture) and Degraded DNA (4-plex capture) packages. 

Phylogenetic analysis will follow methods outlined in Mills et al. 2023. In phyluce software, the v.1.6.2 bioinformatics pipeline will be used. Raw UCE reads will be trimmed using Illumiprocessor (Faircloth 2013), a wrapper for Trimmomatic v.036 (Bolger _et al._ 2014) included in the phyluce pipeline (Faircloth 2015). Loci will be assembled in Trinity v1 (Grabherr _et al._ 2011) using the phyluce script assemblo_trinity. Assemblies will be matched to the UCE probes, assemblies will be extracted, and individual UCE loci will be aligned in MAFFT (Katoh and Standley 2013), and edges will be trimmed with GBlocks (Castresama 2000). UCE flanks will be conservatively trimmed to remove poorly represented nucleotide positions within core UCEs, and assembly errors will be removed (McLean _et al._ 2019).

To assess for presence of genetic introgression, the loci of the UCEs from each genome in the dataset will be partitioned using the entropy-based method SWSC-en to isolate the core and both flanks of each UCE (Tagliacollo and Lanfear 2018). Further consolidation of each partition will be run through PartitionFinder2, which also will identify the best substitution model for each partition based on AICc score (Lanfear _et al._ 2017). Maximum-likelihood phylogenies will be estimated using these consolidated partitions using IQ_TREE (Nguyen _et al._ 2015), the ultrafast bootstrap method (UFboot; Hoang _et al._ 2018), and the approximate likelihood ratio test (SH-aLRT; Anisimova _et al._ 2011) with 1,000 replicates. 

Phylogenies will be estimated using a coalescent-based method, as many UCEs contain a weak phylogenetic signal. UCE loci will be sorted using the phyluce_align_get_informative_sites script and the dataset will be reduced to the top quartile of loci. A maximum-likelihood phylogeny will be constructed using IQ-TREE with branch supports obtained from UFboot and SH-aLRT and all branches with less than 10% bootstrap support will be collapsed (Mills _et al._ 2023, Zhang _et al._ 2019). Phylogenies will be used to estimate species using ASTRAL-III (Rabiee _et al._ 2019). If case species do not form monophyletic groups, individuals will be left as operational taxonomic units (OTUs). 

To ensure that any nonspecific clades are not due to incomplete lineage sorting, the mitogenomes will be extracted from Trinity assemblies by identifying the longest contigs in each assemble with GATK (McKenna _et al._ 2010). Mitogenomes will be aligned to the _A. longicaudus_ cyt-b mitogenome (KY753947) using MAFFT in Geneious (v2021.0), using GBlocks to mask hypervariable regions that may be saturated and poorly aligned (Castresana 2000). Annotations in Geneious will be based on the available _A. longicaudus_ annotation. Each gene except protein-coding genes will be subsetted into individual partitions and split into three partitions corresponding to codon position. PartitionFinder2 will consolidate and estimate the best substitution for each partition. A maximum-likelihood tree will be estimated in IQ-TREE with branch supports obtained using UFboot and SH-aLRT (Mills _et al._ 2023). 


**Works Cited:**

Adam, M. D., Hayes, J. P. 1998. _Arborimus pomo_, _Mammalian Species_, 593, 1–5.

Anisimova M., Gil M., Dufayard J. F., Dessimoz C., Gascuel O. 2011. Survey of branch support methods demonstrates accuracy, power, and robustness of fast likelihood-based approximation schemes. _Systematic Biology_, 60, 685–699.

Bejerano, G., Pheasant, M., Makunin, I., Stephen, S., Kent, W. J., Mattick, J. S., Haussler, D. 2004. Ultraconserved elements in the human genome. _Science_, 304, 5675, 1321–1325. 

Biswell, B., Blow, M., Finley, L., Madsen, S., Schmidt, K. 2000. Survey protocol for the red tree vole, _Arborimus longicaudus_ (=_Phenacomys longicaudus_ in the Record of Decision of the Northwest Forest Plan). Version 2.0. Portland, OR: U.S. Department of Agriculture, Forest Service and U.S. Department of the Interior, Bureau of Land Management. 32.

Blois, J. L., Arbogast, B. S. 2006. Conservation Genetics of the Sonoma Tree Vole (_Arborimus pomo_) Based on Mitochondrial and Amplified Fragment Length Polymorphism Markers. _Journal of Mammalogy_, 87, 950–960.

California Natural Diversity Database (CNDDB). April 2023. Special Animals List. California Department of Fish and Wildlife. Sacramento, CA.

Castresana, J., 2000. Selection of conserved blocks from multiple alignments for their use in phylogenetic analysis. _Molecular Biology and Evolution_, 17, 540–552.

Faircloth, B. C. 2013. Illumiprocessor: a trimmomatic wrapper for parallel adapter and quality trimming. http://dx.doi.org/10.6079/J9ILL. 

Faircloth, B. C. 2015. PHYLUCE is a software package for the analysis of conserved genomic loci. Bioinformatics, 32, 786–788.

Faircloth, B. C., McCormack, J. E., Crawford, N. G., Harvey, M. G., Brumfield, R. T., Glenn, T. C. 2012. Ultraconserved elements anchor thousands of genetic markers spanning multiple evolutionary timescales. _Systematic Biology_, 61, 717–726.

Grabherr, M. G., Haas, B. J., Yassour, M., Levin, J. Z., Thompson, D. A., Amit, I., Adiconis, X., Fan, L., Raychowdhury, R., Zeng, Q., Chen, Z., Mauceli, E., Hacohen, N., Gnirke, A., Rhind, N., di Palma, F., Birren, B. W., Nusbaum, C., Lindblad-Toh, K., Friedman, N., Regev, A. 2011. Full-length transcriptome assembly from RNA-Seq data without a reference genome. _Nature Biotechnology_, 29, 644-652.

Hoang, D. T., Chernomor, O., von Haeseler, A., Minh, B. Q., Vinh, L. S., 2017. UFBoot2: Improving the ultrafast bootstrap approximation. _BioRxiv_, 35, 518–522.

Howell, A. B. 1926. Voles of the genus _Phenacomys_, II: Life history of the red tree mouse _Phenacomys_. _North American Fauna_, 48, 39–66.

Huff, M. H., Holthausen, R. S., Aubry,  K.B. 1992. Habitat management for red tree voles in Douglas-fir forests. General Technical Report. PNW-GTR-302. Portland, OR: U.S. Department of Agriculture, Forest Service, Pacific Northwest Research Station. 1–16.

Janes, D. E., Chapus, C., Gondo, Y., Clayton, D. F., Sinha, S., Blatti, C. A., Organ, C. L., Fujita, M. K., Balakrishnan, C. N., Edwards, S. V. 2011. Reptiles and mammals have differentially retained long conserved noncoding sequences from the amniote ancestor. _Genome Biology and Evolution_, 3, 102–113.

Katoh, K., Standley, D. M. 2013. MAFFT multiple sequence alignment software version 7: improvements in performance and usability. _Molecular Biology and Evolution_, 30, 772–780.

Kerhoulas, N. J., Arbogast, B. S. 2010. Molecular systematics and Pleistocene biogeography of Mesoamerican flying squirrels. _Journal of Mammalogy_, 91, 654–667. 

Lanfear, R., Frandsen, P. B., Wright, A. M., Senfeld, T., Calcott, B. 2017. Partitionfinder 2: New methods for selecting partitioned models of evolution for molecular and morphological phylogenetic analyses. _Molecular Biology and Evolution_, 34, 772–773.

Lesmeister, D. B., Swingle, J. K. 2017. Field Guide to Red Tree Vole Nests. U.S. Department of Agriculture, Forest Service, Pacific Northwest Research Station.

McCormack, J. E., Faircloth, B. C., Crawford, N. G., Gowaty, P. A., Brumfield, R. T., Glenn, T. C. 2012. Ultraconserved elements are novel phylogenomic markers that resolve placental mammal phylogeny when combined with species-tree analysis. _Genome Research_, 22, 4, 746–754.

McKenna, A., Hanna, M., Banks, E., Sivachenko, A., Cibulskis, K., Kernytsky, A., Garimella, K., Altshuler, D., Gabriel, S., Daly, M., DePristo, M. A. 2010. The Genome Analysis Toolkit: A MapReduce framework for analyzing next generation DNA sequencing data. _Genome Research_, 20, 1297–1303.

McLean, B. S., Bell, K. C., Allen, J. M., Helgen, K. M., Cook, J. A. 2019. Impacts of Inference Method and Data set Filtering on Phylogenomic Resolution in a Rapid Radiation of Ground Squirrels (_Xerinae_: _Marmotini_). _Systematic Biology_, 68, 298–316.

Meiklejohn, K. A., Faircloth, B. C., Glenn, T. C., Kimball, R. T., Braun, E .L., 2016. Analysis of a rapid evolutionary radiation using ultraconserved elements: Evidence for a bias in some multispecies coalescent methods. _Systematic Biology_, 65, 612–627.

Meiselman, N., Doyle, A. T. 1996. Habitat and microhabitat use by the red tree vole (_Phenacomys longicaudus_). _The American Midland Naturalist_, 135, 33–42. 

Mills, K. K., Everson, K. M., Hildebrandt, K. P. B., Brandler, O. V., Steppan, S. J., Olson, L. E. 2023. Ultraconserved elements improve resolution of marmot phylogeny and offer insights into biogeographic history. _Molecular Phylogenetics and Evolution_, 107785. 

Murray M. A. 1995. Biochemical systematics of the genus _Arborimus_. M.A. thesis, Humboldt State University. Arcata, California.

Nguyen, L.-T., Schmidt, H. A., Von Haeseler, A., Minh, B. Q. 2015. IQ-TREE: A Fast and Effective Stochastic Algorithm for Estimating Maximum-Likelihood Phylogenies. _Molecular Biology and Evolution_, 32, 1, 268–274. 

Rabiee, M., Sayyari, E., Mirarab, S. 2019. Multi-allele species reconstruction using ASTRAL. _Molecular Phylogenetics and Evolution_, 130, 286–96.

Siepel, A., Bejerano, G., Pedersen, J. S., Hinrichs, A. S., Hou, M., Rosenbloom, K., Clawson, H., Spieth, J., Hillier, L. W., Richards, S., Weinstock, G. M., Wilson, R. K., Gibbs, R. A., Kent, W. J., Miller, W.,  Haussler, D. 2005. Evolutionarily conserved elements in vertebrate, insect, worm, and yeast genomes. _Genome Research_, 15, 8, 1034–1050.

Stephen, S., Pheasant, M., Makunin, I. V., Mattick, J. S. 2008. Large-scale appearance of ultraconserved elements in tetrapod genomes and slowdown of the molecular clock. _Molecular Biology and Evolution_, 25, 2, 402–408. 

Swingle, J. 2009. Home range areas and activity patterns of red tree voles (_Arborimus longicaudus_) in Western Oregon. _Northwest Science_, 83, 273–286.

Tagliacollo, V. A., Lanfear, R. 2018. Estimating improved partitioning schemes for ultraconserved elements. _Molecular Biology and Evolution_, 35, 1798–1811.

Taylor, W. P. 1915. Description of a new subgenus (_Arborimus_) of Phenacomys, with a contribution to the knowledge and distribution of _Phenacomys longicaudus_. Proceedings of the California Academy of Sciences, 5, 111–161. 

Thompson, J. L., Diller, L. V. 2002. Relative abundance, nest site characteristics, and nest dynamics of Sonoma tree voles on managed timberlands in Coastal Northwest California. _Northwestern Naturalist_, 83, 91.

Vrieze, J. M. 1980. Spatial patterning of red tree mouse, _Arborimus longicaudus_, nests. M.A. thesis, Humboldt State University. Arcata, California.

Zentner, P. L. 1977. The nest of _Phenacomys longicaudus_ in northwestern California. M.A. thesis, California State University. Sacramento, California.

Zhang, Y. M., Williams, J. L., Lucky, A. 2019. Understanding UCEs: A comprehensive primer on using ultraconserved elements for arthropod phylogenomics. _Insect Systematics and Diversity_, 3, 1–3.

