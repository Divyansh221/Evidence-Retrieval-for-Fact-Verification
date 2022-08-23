## Evidence Retrieval for Fact Verification

Our aim in this project is to retrieve evidence for various Wikipedia article based claims. Fact verification is of great importance in the present scenario where fake news and claims are highly prevalent. Fact verification is generally a 2 step process which involves evidence retrieval and then analyzing the evidence to understand whether it supports or refutes the claim, but here we are concerned only with the retrieval process.

We have submitted the code by sharing a Google Colab, where all necessary packages can be imported and installed with a single click.
The project is implemented in a single Google colab file: IR_Project5.ipynb

	Link: https://colab.research.google.com/drive/1cTIVyd6SyMlnztqebPCGu4XLz-Ms-zlv?usp=sharing

## Instructions to Run:
1. Section 0:
> Contains all packages that will be required but may not be present in the runtime environment.
> Run the commands as required.
2. Dataset:
> Dataset is uploaded in google drive.

Link: https://drive.google.com/drive/folders/10CQ_BADLLNgALyTwC_18gmYzWL58cpG-?usp=sharing

> The folder is shared; add it to your drive and mount to the runtime environment (Code is provided).
3. Run the cells sequentially as in the notebook for Sections 1 through 3
4. The model can be run for different thresholds as required:
a. fuzz_threshold: Set the threshold for similarity in fuzzy matching layer of Document retrieval
> The lower the threshold, the better the results, however time consumption will be high.
> Henc we use thresholds in the range 50 to 65
b. similarity_threshold: Set the threshold for matching in the Tf-Idf and BERT models. 
> The lower the value, the more (not necessarily better) candidates we obtain.
c. num_doc: Number of documents retrieved in the Document Retrieval step. Set to 10.
d. num_claim: Number of claims, randomly selected, on which the model is tested. 
> Set to 5.
e. num_sentence: Number of evidence sentences finally retrieved as output of the model. 
> Set to 5.
5. Output:
> a. The output for normal string match on the retrieved documents are shown as base.
> b. The final output from the model is given from the last cell.
6. Accuracy:
> To check accuracy we can run the model on the training set of the FEVER dataset and manually check 
> the output against the given evidences.

## Links:
	Demo: https://drive.google.com/file/d/1rEPk3UKwTv81qCYwNsuV9bXbyCUDNWDY/view?usp=sharing
	Google Colab Notebook: https://colab.research.google.com/drive/1cTIVyd6SyMlnztqebPCGu4XLz-Ms-zlv?usp=sharing
			
