#PONMF

Predicting protein functions through non-negative matrix factorization regulated by protein-protein interaction network and gene functional information

Developer:Lun Li from Kunming University of Science and Technology.

## Instructions to PONMF(version 1.0.0)


Requirement
-----------------------------------------------------------------------------------------------------------------------
* 8GB memory
* MATLAB R2016a or later

------------------------------------------------------------------------------------------------------------------------




Input data descriptions
------------------------------------------------------------------------------------------------------------------------


The folder './yeastdata/P' store the yeast data for BP process.
The folder './yeastdata/C' store the yeast data for CCprocess.
The folder './yeastdata/F' store the yeast data for MFprocess.
The folder './humandata/P' store the human data for BP process.
The folder './humandata/C' store the human data for CC process.
The folder './humandata/F' store the human data for MFprocess.

The file './data/yeastdata/P/Pgp.txt' is the matrix of protein and Goterm association.The entry Xij equaling 1 represents connection between the i-th go and j-th protein related to the list above, and 0 otherwise.
The file './data/yeastdata/P/Pgogo.txt' is the adjanceny matrix of the interaction newtwork of go and go.
The file './data/yeastdata/P/ppi.txt' is the adjanceny matrix of the interaction newtwork of protein and protein.
------------------------------------------------------------------------------------------------------------------------





parameter interpretation
------------------------------------------------------------------------------------------------------------------------

n_parameter:The tuning parameter of interactome information for integrating ppi network information into the model.

s_parameter:The tuning parameter of interactome information for integrating gogo network information into the model.

u_parameter:The tuning parameter of Frobenius norm based regularization to prevent over-fitting problem.

v_parameter:The tuning parameter of Frobenius norm based regularization to prevent over-fitting problem.

k:protein or goterm representation in the K dimension.



Output data descriptions
------------------------------------------------------------------------------------------------------------------------
result1:PONMF
result2:PONMF-1
result3:PONMF-2
result4:PONMF-3
result5:PONMF-4
------------------------------------------------------------------------------------------------------------------------
