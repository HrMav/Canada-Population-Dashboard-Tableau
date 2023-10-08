# Canada-Population-Dashboard-Tableau

Using Canada Census Data from 2021 and 2016, a summary of Canada population Census and Religious Beliefs presented in Tableau.

Summary of Tableau calculated fields included in Dashboard:

Calculate Millenials:

IF [Year of Birth] >= 1981 AND
[Year of Birth] <= 1996 THEN     
[Population] 
ELSE
0
END


Calculated age group from 0 to 14 years

IF [Age] >= 0 
AND [Age] <= 14
THEN [Population]
ELSE 0
END

Calculate Men to Women Ratio

SUM([Men]) / SUM([Women])

