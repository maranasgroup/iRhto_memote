Hoang Dinh, 2019-04-09
As of current, the gene-protein-reaction rules in model SBML (.xml) file are errorneous due to a bug in "cobra.io.write_sbml_model". Please use the model in the JSON (.json) format if possible. Information provided in the excel files are also correct.<br>

Hoang Dinh, 2019-06-27
GPR in SBML model fixed. Add SBML model with gene ID changes for KBase's genome integration feature. However, due to the strict requirement of gene ID matching between genome and model, pseudogenes to model spotaneous reactions ("SPONT"), accessory protein subunits ("TRUE"), and reactions with unknown enzymes ("UNKNOWN") are removed on KBase.
