# Tableau-Calculated-Fields

# Dates

###Difference in dates:

(DATEDIFF('day', [Requested Date Original], [Inspection Scheduled])) * 0.68

#Creating bins:

IF [Disp Code 2] == "E1" THEN 1 
ELSEIF  [Disp Code 2] == "E2" THEN 1 
ELSEIF  [Disp Code 2] == "E6" THEN 1 
ELSEIF  [Disp Code 2] == "E7" THEN 1 
ELSEIF  [Disp Code 2] == "E8" THEN 1 


ELSE 0 
END
