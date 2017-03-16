# Tableau-Calculated-Fields

# Dates

### Difference in dates:

(DATEDIFF('day', [Requested Date Original], [Inspection Scheduled])) * 0.68

### Current date field:

date(today())

# Creating bins:

IF [Disp Code 2] == "E1" THEN 1 

ELSEIF  [Disp Code 2] == "E2" THEN 1 

ELSEIF  [Disp Code 2] == "E6" THEN 1 

ELSEIF  [Disp Code 2] == "E7" THEN 1 

ELSEIF  [Disp Code 2] == "E8" THEN 1 

ELSE 0 

END



IF contains("XX, H1, E1,E2,E3,E6,E7, E8, EA, EB, EC, EE, EZ, F1, F2, F3, F4, F5, F6, F7, 
F8, F9, G2, G3, G4, G5, G6, G7, G8, G9",[Disp Code 2])

OR 

contains("XX, H1, E1,E2,E3,E6,E7, E8, EA, EB, EC, EE, EZ, F1, F2, F3, F4, F5, F6, F7, 
F8, F9, G2, G3, G4, G5, G6, G7, G8, G9",[Disp Code])



=true THEN 1 ELSE 0 
