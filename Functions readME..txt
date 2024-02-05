--FUNCTIONS TO EXTRACT THE SKILL KWEWORDS--

-- =MID([@[description_tokens]];FIND("'";[@[description_tokens]];1)+1;FIND("'";[@[description_tokens]];3)-1-FIND("'";[@[description_tokens]];1)) -- skill_1

-- =MID([@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3;FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)-7-FIND(",";[@[description_tokens]];1) + 3) -- skill_2

--=MID([@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3;FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-7-FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3) --skill_3


-- =MID([@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3;FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)-6 -FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3) -- skill_4

 

-- =MID([@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)-1+5;FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)-1+5)-8-FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)-1+5) -- skill_5



-- =MID([@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4;FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)-8 - FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4) -- skill_6


-- =MID([@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4;FIND("'";[@[description_tokens]];FIND("'"
;[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)-8-FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4 ) -- skill_7

-- =MID([@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4;FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)-8-FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)   --skill_8

-- =MID([@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4;FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)-8-FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)  -- skil_9


-- =MID([@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4;FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)-8-FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)--function_10

-- =MID([@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4;FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-3-FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)-1)  --function_11



-- =MID([@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-1)+4;FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-1)+4)-8-FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-1)+4)-- function_12



-- =MID([@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-1)+4)+4;FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-1)+4)+4)-8-FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-1)+4)+4)     --function_13


 -- =MID([@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-1)+4)+4)+4;FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-1)+4)+4)+4)-8-FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-1)+4)+4)+4) -- skill_14


 -- =mid([@[description_tokens]];find("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-1)+4)+4)+4)+4;find("'";[@[description_tokens]];find("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-1)+4)+4)+4)+4)-8-find("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-1)+4)+4)+4)+4)   -skill_15



 

find("'";[@[description_tokens]];find("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-1)+4)+4)+4)+4)+4  --first16


find("'";[@[description_tokens]];find("'";[@[description_tokens]];find("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND("'";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];FIND(",";[@[description_tokens]];1) + 3)+3)-2) +3)+4)+4)+4)+4)+4)+4)+4)-1)+4)+4)+4)+4)+4)-8   --last16


--FUNCTIONS FOR TRANSFORMING THE JOB TITLES--

=IF(ISNUMBER(SEARCH("Senior Data Analyst", Aa2)), "Senior Data Analyst", Aa2)
 
=IF(ISNUMBER(SEARCH("Senior Data Analyst", Aa2)), "Data Analyst", Aa2)
 
=IF(OR(ISNUMBER(SEARCH("", Aa2)), ISNUMBER(SEARCH("intern", Aa2)), ISNUMBER(SEARCH("trainee", Aa2)), ISNUMBER(SEARCH("internship", Aa2))), "Data Analyst Intern", Aa2)

=IF(ISNUMBER(SEARCH("scientist", Y2)), "Data Scientist", Y2)

=IF(OR(ISNUMBER(SEARCH("AI Data Specialist", Aa2)), ISNUMBER(SEARCH("Research & Evaluation", Y2)), ISNUMBER(SEARCH("Sr. Data Engg/ Data Modeler", Y2)), ISNUMBER(SEARCH("Azure Data Engneer", Y2)), ISNUMBER(SEARCH("Azure Data Engg W2", Y2))), "Data Engineer", Y2)



"FUNCTIONS FOR SHOWCASING THE APPROPRIATE TITLES ON THE DASHBOARD"



=IFS(AND(AG88 = "Business Analyst"; AG92 = "Grand Total"); AH92; AG88 = "Business Analyst"; AH88; AG88 = "Data Analyst"; AH88; AG88 = "Data Engineer";AH88; AG88 = "Data Scientist"; AH88) 



--OTHER FUNCTIONS I USED(SAMPLES)--


=RANK.EQ(Skills_tables!$Y114;Skills_tables!$Y$114:$Y$236) -- Assigning rankings

=VLOOKUP(Skills_tables!$G114;$B$2:$C$106;2;) -- grab titles, data and sums

=SUM(IF(ISNUMBER(Skills_tables!$H114:$V114); Skills_tables!$H114:$V114))  -- summarize tables with diferrent values




