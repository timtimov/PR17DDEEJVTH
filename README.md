# PR17DDEEJVTH
Seminarska naloga, Podatkovno rudarjenje

## Data

We got data from [Kaggle](https://www.kaggle.com/murderaccountability/homicide-reports), it has reports about murders commited in US between 1980 and 2014. <br/>
Data comes in a csv file, it is presented in a table with rows and columns, each row describes a murder and columns represent "attributes" about that murder, such as victim and perpetrators sex, weapon used, agency that tried to solve this murder, was it solved or not... <br/>
In this data there were also unknown values, always marked as "Unknown", for some atributs like weapons we tried to "calculate" which weapon was used, for this we used attributes such as victim and perpetrators sex.<br/>


## Findings

We tried to find some interesting things in the data.<br/>

### Which sex and which race commits more murders in US.<br/>
![alt text](https://github.com/bambuco2/PR17DDEEJVTH/blob/master/spol_umor.png)

![alt text](https://github.com/bambuco2/PR17DDEEJVTH/blob/master/race_umor.png)
<br/>
So from this two graphs we can see that when it comes to sex murders are not even close. Males commit way more murders than Females.<br/>
And for race, we can see that whites and blacks are usually the perpetrators. Whites are slighty more frequent, but not by much.

### Which agencies are the most effective when it comes to murder solving .<br/>

'County Police': 0.66<br/>
'Municipal Police': 0.68<br/>
'Special Police': 0.71<br/>
'Sheriff': 0.78<br/>
'Regional Police': 0.79<br/>
'State Police': 0.82<br/>
'Tribal Police': 0.92<br/>
<br/>
From this we can see that Tribal and State police are the most effective when it comes to murder solving, but this is also effected by number of the cases they have to solve.<br/>
Tribal police has only had about 50 murders between 1980 and 2014, thus giving them more time to solve each murder.<br/>

### Frequency of weapons used.<br/>
![alt text](https://github.com/bambuco2/PR17DDEEJVTH/blob/master/orozja.png)

From this graph we can see, that handgun is the most popular weapon when it comes to murders. No suprise there, since pretty much anyone can get a handgun in US. They are cheap, easy to use and also distances you from your victim.

![alt text](https://github.com/bambuco2/PR17DDEEJVTH/blob/master/orozje_native.png)

But if we look at weapon used and we devide them in groups by races, we can see an interesting result for Native Americans, they 
prefer knife over handguns unlike other races.

### Relationship between perpetrator and victim.<br/>

When we look at relationship between victim and perpetrator we see nothing interesting, victims know their perpetrators, "Acquaintance" is the most common relationship.
But if we devide relationship into two groups by sex of the perpetrators, we can see some very interesting things.


![alt text](https://github.com/bambuco2/PR17DDEEJVTH/blob/master/odnos_male.png)
The first graph represents males, they seem to murder complete strangers.<br/>
![alt text](https://github.com/bambuco2/PR17DDEEJVTH/blob/master/odnos_female.png)
If we look at this graph, that represents females, we can see, that their victims are usually very personal, like husband and boyfriend.

### Finding similarities between years

##### Average age of victims and perpetrators
For each year, I've calculated the average ages of both victims and perpetrators, to see are there any diffrences between them. As show by the data, the victims are 3-4 years older than the perpetrators
on average, and we see slight increase in the victims age in the years 2012 and 2014.

![alt text](https://github.com/bambuco2/PR17DDEEJVTH/blob/master/avg_age.png)

##### Relationships and Weapons used

Here i've calculated the victims relationship with the perpetrator:
1980 -> [('Acquaintance', 5499), ('Stranger', 3667), ('Wife',   915),  ('Friend', 828), 	 ('Husband', 630)]
1981 -> [('Acquaintance', 5324), ('Stranger', 3698), ('Wife',   866),  ('Friend', 841), 	 ('Husband', 638)]
1982 -> [('Acquaintance', 5105), ('Stranger', 3851), ('Wife',   817),  ('Friend', 717), 	 ('Husband', 535)]
1983 -> [('Acquaintance', 4813), ('Stranger', 3355), ('Friend', 830),  ('Wife',   827), 	 ('Husband', 542)]
1984 -> [('Acquaintance', 4632), ('Stranger', 3479), ('Wife',   791),  ('Friend', 727), 	 ('Girlfriend', 428)]
1985 -> [('Acquaintance', 4864), ('Stranger', 2947), ('Wife',   851),  ('Friend', 790), 	 ('Girlfriend', 448)]
1986 -> [('Acquaintance', 5075), ('Stranger', 2887), ('Friend', 1083), ('Wife', 814), 		 ('Girlfriend', 505)]
1987 -> [('Acquaintance', 4775), ('Stranger', 2816), ('Friend', 1019), ('Wife', 788), 		 ('Girlfriend', 429)]
1988 -> [('Acquaintance', 4720), ('Stranger', 2692), ('Friend', 836),  ('Wife', 765), 		 ('Girlfriend', 456)]
1989 -> [('Acquaintance', 4941), ('Stranger', 2982), ('Friend', 1001), ('Wife', 646), 		 ('Girlfriend', 498)]
1990 -> [('Acquaintance', 5143), ('Stranger', 3478), ('Friend', 931),  ('Wife', 718), 		 ('Girlfriend', 458)]
1991 -> [('Acquaintance', 4760), ('Stranger', 3814), ('Friend', 867),  ('Wife', 737), 		 ('Girlfriend', 498)]
1992 -> [('Acquaintance', 4582), ('Stranger', 3671), ('Friend', 938),  ('Wife', 724), 		 ('Girlfriend', 523)]
1993 -> [('Acquaintance', 4701), ('Stranger', 3878), ('Friend', 967),  ('Wife', 735), 		 ('Girlfriend', 615)]
1994 -> [('Acquaintance', 4611), ('Stranger', 3533), ('Friend', 838),  ('Wife', 656), 		 ('Girlfriend', 536)]
1995 -> [('Acquaintance', 4088), ('Stranger', 3551), ('Friend', 661),  ('Wife', 633), 	     ('Girlfriend', 506)]
1996 -> [('Acquaintance', 3836), ('Stranger', 2837), ('Wife',   636),  ('Friend', 556), 	 ('Girlfriend', 460)]
1997 -> [('Acquaintance', 3567), ('Stranger', 2522), ('Wife',   575),  ('Friend', 511),		 ('Girlfriend', 466)]
1998 -> [('Acquaintance', 3102), ('Stranger', 2290), ('Wife',   640),  ('Friend', 469), 	 ('Girlfriend', 458)]
1999 -> [('Acquaintance', 2769), ('Stranger', 1887), ('Wife',   556),  ('Girlfriend', 460),  ('Friend', 440)]
2000 -> [('Acquaintance', 2436), ('Stranger', 2061), ('Wife',   597),  ('Girlfriend', 450),  ('Friend', 324)]
2001 -> [('Acquaintance', 2517), ('Stranger', 2295), ('Wife',   608),  ('Girlfriend', 453),  ('Friend', 383)]
2002 -> [('Acquaintance', 2675), ('Stranger', 2441), ('Wife',   595),  ('Girlfriend', 467),  ('Friend', 411)]
2003 -> [('Acquaintance', 2709), ('Stranger', 2280), ('Wife',   542),  ('Girlfriend', 487),  ('Friend', 388)]
2004 -> [('Acquaintance', 2605), ('Stranger', 2289), ('Wife',   565),  ('Girlfriend', 467),  ('Friend', 346)]
2005 -> [('Acquaintance', 2616), ('Stranger', 2501), ('Wife',   581),  ('Girlfriend', 485),  ('Friend', 348)]
2006 -> [('Acquaintance', 2809), ('Stranger', 2407), ('Wife',   556),  ('Girlfriend', 459),  ('Friend', 391)]
2007 -> [('Stranger', 	  2431), ('Acquain.', 2392), ('Wife',   572),  ('Friend', 508), 	 ('Girlfriend', 493)]
2008 -> [('Acquaintance', 2242), ('Stranger', 1754), ('Wife',   567),  ('Friend', 511), 	 ('Girlfriend', 504)]
2009 -> [('Acquaintance', 2226), ('Stranger', 2207), ('Wife',   627),  ('Girlfriend', 480),  ('Friend', 460)]
2010 -> [('Stranger',     2142), ('Acquain.', 2065), ('Wife',   594),  ('Girlfriend', 509),  ('Friend', 442)]
2011 -> [('Acquaintance', 2082), ('Stranger', 1989), ('Wife',   551),  ('Girlfriend', 494),  ('Friend', 421)]
2012 -> [('Stranger',     2137), ('Acquain.', 1992), ('Wife',   525),  ('Girlfriend', 517),  ('Friend', 396)]
2013 -> [('Acquaintance', 1924), ('Stranger', 1863), ('Wife',   515),  ('Girlfriend', 488),  ('Friend', 384)]
2014 -> [('Stranger',     1961), ('Acquain.', 1821), ('Wife',   502),  ('Girlfriend', 430),  ('Friend', 382)]

We can see that acquaintance and stranger are the two most common relationships between the victim and the perpetrator throughout the years. The diffrences between early 1980s to the rest is that there are significant amount
of husbands being killed at that period, but later we see that the main perpetrators are mostly men, with wife and girlfriend being the usual victims.

