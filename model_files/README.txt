*** Sticky ***
Release 2 is current and at this directory. 
iRhtoC and iRhtoN are the model versions for carbon and nitrogen limited conditions, respecitvely. They are identical except for the biomass reaction, acyl composition reaction, and GAM.

*** Update log ***
Hoang Dinh, 2020-08-07
Curating xylitol and arabitol metabolism, one carbon metabolism, AKGD and GCC representation, aldehyde dehydrogenase isozymes, various mitochondrial transporters, proline degradation pathway, and FADH2 oxidation pathway.
Add OAADC_c
Remove PFK_3_c due to lack of evidence
Curate NADHcplxI_c_m's GPR based on pmid:32789504, merging metagenes corresponding fragments of a complete gene

Hoang Dinh, 2020-06-30
First upload now called "release1", described in https://dx.doi.org/10.1016%2Fj.mec.2019.e00101, accounting for 1108 genes.

Update model to "release2", accounting for 1113 genes, with the following major changes:
- Peroxisomal and mitochondrial beta-Oxidation pathway is curated, gene functions were searched and linked, poly-unsaturated fatty acid beta-oxidation pathways (up to C18:3) were unlumped.
- Add de novo carnitine biosynthesis pathway => required for mitochondrial beta-oxidation / not in S. cerevisiae
- Fix ATP synthase stoichiometry to 3 ATP / 10 proton. Re-calibrate GAM

KBase model format is no longer supported due to technical issues.

Hoang Dinh, 2019-04-09
As of current, the gene-protein-reaction rules in model SBML (.xml) file are errorneous due to a bug in "cobra.io.write_sbml_model". Please use the model in the JSON (.json) format if possible. Information provided in the excel files are also correct.<br>

Hoang Dinh, 2019-06-27
GPR in SBML model fixed. Add SBML model with gene ID changes for KBase's genome integration feature. However, due to the strict requirement of gene ID matching between genome and model, pseudogenes to model spotaneous reactions ("SPONT"), accessory protein subunits ("TRUE"), and reactions with unknown enzymes ("UNKNOWN") are removed on KBase.
