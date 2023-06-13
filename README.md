# Transformers for super enchancers classification
Super enhancers (SE) are long regulatory sequences in the genome. It has been shown that these elements largely determine the identity of cells both in the course of normal development and in pathology, influencing the expression of key genes. They are of interest for medicine, especially for understanding the mechanisms of development of tumors. Therefore, an important task prior to experimental validation is the search for these genetic elements using computational approaches. Most of the existing algorithms for their search require not only the DNA sequence, but also the data of expensive additional experiments. Our goal was to develop an algorithm for SE prediction that uses only information about the DNA sequence. We applied neural network models based on transformers and obtained results that have a biological basis. The results obtained by us in the future will help in the further development of methods for predicting super enhancers and the study of their structure.<br>
<br>
We decided to use the dataset collected to implement the DeepSE (Q.-Y. Ji et al., 2021) and imPROSE (Khan and Zhang, 2019) models. <br>
We performed DNABERT (Y. Ji et al., 2021) and GENA-LM fine-tuning. Fine tuning was carried out first for the classifier, and then for all layers of the model for both models.<br>
<br>
The fine-tuning code can be found in GENA_LM.ipynb, the analysis of the results using cuptum is in ./explainability <br>
##### Literature
1) Ji, Q.-Y., Gong, X.-J., Li, H.-M., Du, P.-F., 2021. DeepSE: Detecting super-enhancers among typical enhancers using only sequence feature embeddings. Genomics 113, 4052–4060. https://doi.org/10.1016/j.ygeno.2021.10.007 <br>
2) Khan, A., Zhang, X., 2019. Integrative modeling reveals key chromatin and sequence signatures predicting super-enhancers. Sci Rep 9, 2877. https://doi.org/10.1038/s41598-019-38979-9 <br>
3) Ji, Y., Zhou, Z., Liu, H., Davuluri, R.V., 2021. DNABERT: pre-trained Bidirectional Encoder Representations from Transformers model for DNA-language in genome. Bioinformatics 37, 2112–2120. https://doi.org/10.1093/bioinformatics/btab083
