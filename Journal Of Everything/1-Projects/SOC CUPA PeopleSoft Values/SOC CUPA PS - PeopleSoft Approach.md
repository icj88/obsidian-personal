# General Request for advice on implementation 

______
**From:** Ian Johnson [Ian.C.Johnson@uvm.edu](mailto:Ian.C.Johnson@uvm.edu)  
**Sent:** Wednesday, April 9, 2025 4:15 PM  
**To:** Susan Skalka [Susan.Skalka@uvm.edu](mailto:Susan.Skalka@uvm.edu)  
**Cc:** Caroline Cote (she/her) [Caroline.Cote@uvm.edu](mailto:Caroline.Cote@uvm.edu)  
**Subject:** Recommendation for new attributes in PeopleSoft

Hi Susan,

We would like to store two code attributes at the position level in PeopleSoft:

1. SOC codes (7 characters) – Currently in US_SOC_TBL linked to JOBCODE_TBL
2. CUPA codes (6 characters) – No dedicated table exists, to my knowledge

Both require infrequent updates (annually, to a handful of positions) and will primarily be used for reporting/analytics.

I’m considering either adding new or appropriating unused columns in POSITION_DATA to store this data. Having a dedicated lookup table for the CUPA codes would be ideal but may not be necessary for the use-case.

  
Before creating a formal ticket, do you have recommendations on the best approach?

Thanks,  
Ian
____
**From:** Susan Skalka [Susan.Skalka@uvm.edu](mailto:Susan.Skalka@uvm.edu) 
**Sent:** Wednesday, April 9, 2025 5:33 PM  
**To:** Ian Johnson [Ian.C.Johnson@uvm.edu](mailto:Ian.C.Johnson@uvm.edu)  
**Cc:** Caroline Cote (she/her) [Caroline.Cote@uvm.edu](mailto:Caroline.Cote@uvm.edu)  
**Subject:** RE: Recommendation for new attributes in PeopleSoft

Hi, I will think about the options and get back to you- Thanks, Susan
___
