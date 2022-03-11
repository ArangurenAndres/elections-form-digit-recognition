# Elections form digit recognition and classification

## The follwoing project consist on a deep learning model developed to extract the handwritten digits contained in the elections forms used by the Colombian government, this documents are open access docs. 

## The model is being developed in order to avoid fraud in the elections given that in last years there is strong evidence of forms and handwritten digits being altered in order to modify the voting records. 

A general overview : 

The model is in current development and the main goal is to develop a reliable model that will eventually allow to extract the following information from the documents:
1. QR code : contains unique identifier of the form
2. Hand written digits : extract the digits related to voting records

The model general workflow can be divided in the following steps : 

1. Automatic scan of the document reshaping the input photo into a fixed shape
2. Extraction of regions of interest (meaning their reference coordinates in the scanned document)
3. Information retrieval (QR code, decode information) and for handwritten digits , classification of single digit from 0-9
4. Fill form containing form information : an initial dictionary is filled with the form information, this info will be successively added into a database


To thest the current model 
In folder "api_extraccion" download the doc_scanner.ipynb jupyter notebook
