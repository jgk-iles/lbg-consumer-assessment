# Assumptions

1. The campaign dataset is only a fraction of the total mortgage back book, meaning that data available in that set is unavailable for the rest of the mortgage back book.
2. Goal is to create a model which targets customers so a higher proportion would accept - so we should be optimising for precision (minimising false positives). 
3. The frames match up in order (I have asserted this) but in the real world we would join these tables properly on a common key.
4. We can use the age field in campaign in the mortgages frame because dob is in there - in reality we make some calculation of age from dob.
5. Capital gain/loss is that paid by the owner on sale of a previous property. 