**Chapter 2: Database soundness** 

Chapter describes techniques to archieve schema soundness,
this boils down to:
* Table should represent single subject
* Table should have a primary key 
* Table shouldn't have any multipart (FullName: John Doe) or multivalue columns (Certifications: {1, 2, 3})
* Table shouldn't have any computed values (make sure computations are in *SELECT*)
* Table shouldn't have unnecessary duplicate columns

**Keys**

primary key should:
* identify each row uniquely
* key should contain unique values
* for every given record there should be a key
* keys shouldn't be a multipart column
* key shouldn't be modified