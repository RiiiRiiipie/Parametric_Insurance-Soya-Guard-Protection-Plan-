# Parametric Insurance Policy Report 
## 1. Product Design
**Q: What is parametric insurance?**
A: Parametric insurance is a type of insurance that provides payouts based on predefined parameters or triggers, such as rainfall exceeding a certain threshold, rather than actual losses incurred. It is designed to be simpler and faster than traditional indemnity insurance, as it avoids the need for loss assessment.
**Q: How is the payout calculated in parametric insurance?**
A: The payout is based on a pre-agreed formula linked to the trigger event. For example, if the trigger is rainfall exceeding 200mm in a specific period, and the payout rate is $100 per mm above the threshold, the insured would receive $100 for every mm above 200mm.
**Q: What factors are considered in designing a parametric insurance product?**
A: Key factors include:
   - Identifying the risk and its impact.
   - Choosing measurable and reliable parameters.
   - Defining the trigger threshold.
   - Establishing a payout structure.
   - Ensuring the availability of trustworthy data sources for monitoring.
## 2. Perils Covered
**Q: What types of perils that we have covered in this policy?**
	A: We have covered the risk associated with :
   - Natural disasters (droughts, floods).
   - Weather-related risks (e.g., excessive rainfall, temperature extremes).
   - Agricultural risks (e.g., crop yield losses due to adverse weather).
   - Business interruptions linked to specific external events.
	B:Justification for choosing such perils :
a.	In this case our goal is to provide the best measurement for the soyabean yield in Indore district in Madhya Pradesh.
b.	From a research paper we have seen the influence of a rainfall and temperature on soyabean yield. https://www.ujecology.com/articles/influence-of-weather-and-climatic-conditions-on-soybean-yield-80840.html 
c.	The soyabean crop is widely affected by the excess or deficit rainfall and heat or cold stress.
d.	And according to the historical data the yield of soyabean was exponentially dropped in the years 2002 and 2015 in 2002 it was due to deficit rainfall and in 2015 it was due to excess and uneven distribution of the rainfall.

## 3. Triggers
**Q: Triggers associated with this policy.**
	A: Triggers are objective and measurable conditions that activate the insurance payout: 
	Triggers that we have achieved through analysis.  
a.	Rainfall exceeding 650mm in July to early august and the rainfall is less than 10mm during late September and early October or Rainfall falling below 150mm in July to early august and the rainfall is less than 10mm during late September and early October these both the cases cover the excess and deficit rainfall terms.
b.	If the consecutive rainfall for 5 days exceeds 250mm.
  These are the two triggers points that have impacted the soyabean yield most in past 25 years.
	The goal is to cover such events and provide the best financial remedy to the policy holders.

## 4. Data Sources
	Extracting the data from a verified source
a.	The first process of doing the analysis is obtaining the data from a valid source
b.	we are going to collect the data of the rainfall and the temperature for Madhya Pradesh state (Indore district)
c.	We are going to collect the data from IMD (India Meteorological Department) for the variables like rainfall and temperature.
d.	The yearly data for variables like rainfall and temperature form 2010 to the current available data.
e.	In case of temperature, we have data like tmin that is minimum temperature for a specific day and tmax is maximum temperature for a specific day.
f.	It also provides other kind of data but for now we will work with these variables.

## 5. Modelling and Pricing Approach
	Modeling refers to the process of creating mathematical and statistical representations of various factors that influence risk and financial outcomes.
a.	In the start of the process, we had three variables they are daily rainfall, minimum temperature per day and maximum temperature per day.
b.	Importing the data created by combining all the extracted data
c.	Exploratory Data Analysis
d.	Finding how our data is distributed.
e.	Correlation Between the variables that we have considered
f.	Boxplot to find the extreme values in our data set
g.	Importing the data of soyabean yield for Indore form year 1997 to 2022
h.	Plotting the soyabean yield to the see the rise and fall in the growth
i.	Importing the libraries that we require for the analysis.
j.	Extracting the data or the months that are required for the analysis
k.	The growth of the soyabean occurs from June to October so we will only consider the months from June to October.
l.	Also dividing the rainfall columns in sub parts to get more information about the data.
m.	Same for the temperature i.e. Daily minimum and maximum columns.
n.	So, from the sub divided column we can get some insights about the data which will be helpful for the creation of the parametric insurance.
o.	Obtaining the moving sum for 5 days
p.	Now dealing with the temperature columns
q.	Dividing the growth period of the soyabean in 6 different stages
r.	Obtaining the cumulative rainfall in different stages and their effects on the soyabean yield
s.	Using all this process we have found a suitable result for policy formation 
t.	Each Process is explained properly in the python code file with comments.
	Pricing in insurance involves determining the appropriate premium that policyholders should pay for coverage based on the assessed risks associated with their profiles.
a.	For Pricing the policy, we have analyzed the historical data for 25 years according to that we have decided certain  triggers and using those triggers we have formed a policy with reasonable premium and a good pay out in case of loss.
b.	All the analysis to obtain the expected loss is present in the python script 

## 6. Payout Structure
Sum Assured (Rs.) 	Monthly Premium (Rs.) (for six months only) 	 Yealy Premium (Rs.)
    40000	                          673	                               	   4033 

## 7. Back-Testing Results Data Sources
a.	We have done the Back-Testing using the historical data and have found the results for the year 2002 and 2015 as well as 2009 
b.	The year 2002 had faced a drought due to which there was an extreme  reduction in the soyabean yield 
c.	The year 2015 had faced a very heavy rainfall due to which there was a reduction in the soyabean yield

d.	The year 2009 was the year of extreme growth which occurs due to even distribution of the rainfall.

## 8.Conclusion
Parametric insurance is a powerful tool for managing risks associated with measurable and predefined events. By leveraging objective triggers and reliable data, it ensures transparency, speed, and efficiency in payouts, making it an ideal choice for perils like rainfall variability, natural disasters, and agricultural risks. Continuous validation through back-testing and robust methodology enhances its effectiveness and trustworthiness.
