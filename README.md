# Project: Investigate a Dataset - FBI Gun Data

## Introduction

### Dataset Description 


The following dataset is from the FBI's National Instant Criminal Background Check System (NICS). The NICS is used to determine whether or not a potential gunbuyer is eligible to legally purchase firearms or explosives. Firearms sellers call into the NICS system to confirm the customer does not have a criminal record or is ineligible to make a purchase. The columnal data contains the number of firearm checks by month, state, and type as recorded by gun shop owners and pawn shops selling guns in a given month. Data exists only if a call was made and does not include private sales.

Below is a list of data categories listed in the csv.

'month',
 'state',
 'permit',
 'permit_recheck',
 'handgun',
 'long_gun',
 'other',
 'multiple',
 'admin',
 'prepawn_handgun',
 'prepawn_long_gun',
 'prepawn_other',
 'redemption_handgun',
 'redemption_long_gun',
 'redemption_other',
 'returned_handgun',
 'returned_long_gun',
 'returned_other',
 'rentals_handgun',
 'rentals_long_gun',
 'private_sale_handgun',
 'private_sale_long_gun',
 'private_sale_other',
 'return_to_seller_handgun',
 'return_to_seller_long_gun',
 'return_to_seller_other',
 'totals'

The NICS data can also be supplemented with U.S. state level census data csv for further insights. Most variables just have one data point per state (2016), but a few have data for more than one year.

The github repository's README containing the FBI NICS Data lists important details needed to understand the data including possible methods for analysis. The details are as follows:
>...The FBI’s background check numbers come with caveats: ... many checks are for concealed carry permits, not actual gun sales. ...the FBI’s numbers don’t include private gun sales, many of which do not require a background check. Despite those vagaries, the FBI’s NICS numbers are widely accepted as the best proxy for total gun sales in a given time period.

>...Note: Sales estimates are calculated from handgun, long gun and multiple-gun background checks. Permit checks and other categories of background checks are excluded. In California, multiple-gun checks were excluded because data was inconsistent. Because state laws differ, sales levels between states cannot be directly compared.

> ...To convert background checks into estimated sales, we (New York Times) relied on a method suggested in the Small Arms Survey by Jurgen Brauer, a professor at Georgia Regents University. Each long gun and handgun check was counted as 1.1 sales. Each multiple-gun check was counted as two sales. Permit checks and other types of checks were omitted. The multiplier is an estimate based on Mr. Brauer's interviews with gun shop owners.



### Question(s) for Analysis



#### Question 1:
What (5) US states/territories have had the highest gun sales in the last (30) days?
#### Question 2 :
What is the overall trend of gun purchases in California in the last (36) months?



#### Data Anlysis Method
Because of the caveats stated above in the data description section, I have chosen theses questions and will be using the Small Arms Survey method designed by Jurgen Brauer, a professor at Georgia Regents University. A method previousy used by the New York Times in their 2015 research piece on US Gun sales estimates:

- Each long gun and handgun check was counted as 1.1 sales. 
- Each multiple-gun check was counted as two sales. 
- Permit checks and other types of checks were omitted.
- In California, multiple-gun checks will be excluded because data is inconsistent.

Note: The multiplier is an estimate based on Mr. Brauer's interviews with gun shop owners
