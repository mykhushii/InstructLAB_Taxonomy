1 

# Document Information 

## 1.1 About this Document 

This is official IBM guide document which describes how IBM Delivery Centre will prepare the Distribution Surcharge journal entry. This document will be used for future reference, either for IBM team or for Client Team. 

## 1.2 Who should use this Document? 

This document can be used by the General Accounting Associate who will be processing Distribution Surcharge (JE 198k) as well as by journal reviewer 

## 1.3 Revision/Approval History 



| Version number | Effective Date | Summary of Changes | Author | Reviewer | Approver |
| --- | --- | --- | --- | --- | --- |
| 1.0 | 19/05/2022 | Draft | Pk | siva | kl |

2 

# Overview 

## 2.1 Objective(s) 

The objective of the journal is to allocate Distribution Surcharge to appropriate cost of sale accounts for vehicle sold to Canada. 

### 2.1.1 

#### Frequency: 

Monthly (WD+1) 

### 2.1.2 

#### Source: 

Microsoft Outlook and SharePoint (Distribution Surcharge account balance) 

### 2.1.3 

### System Accesses: 

* •
* •
* • PeopleSoft via EUR 

OBIEE MBS Truck - IT Help Desk 

OBIEE Foreign Exchange Rates - IT Help Desk
## 2.2 Inputs & Outputs 



| Input | From |
| --- | --- |
| Email request | Client Business Partner |
| Output | To |
| Journal Entry Posted | Distribution Surcharge Account |

# Control Points 



| Sub process | Sub process Activity Description | Control Objective | Control Activity Risk Assertions | Frequency (i.e. Event, Daily, Monthly, Quarterly, | Evidence |
| --- | --- | --- | --- | --- | --- |
| Activity |  | (s) |  |  |  |
|  |  | Journals should be posted with Accuracy | level |  |  |

# 

## 
Annually) 

To Allocate Distribution Surcharge Journal to appropriate Cost of sale accounts for vehicle sold to Canada 

Distribution Surcharge 

1 (JE 198K) 

* 2.3 Process Measurement Reports Manual journal entries are reviewed and approved in line with Company policy prior to being posted (Higher

control) Combo Errors, Incorrect account numbers, Business units and operating units. 

Email provided by Gayle Carter 

Monthly (WD+1) 

Journal entry need to be posted by WD +1 to transfer or reclass the scholarship fee of $5 associated with each vehicle sold by Tulsa to Canada from Distribution surcharge account. 

# 3 Roles & Responsibilities 

## 3.1 Description 



| Role | Responsibility |
| --- | --- |
| Client Onshore (Tulsa Plant) | Provide input for the Journal entry |
| R2R Team(IBM) | Prepare and Post the Distribution Surcharge Journal |

# 4 Process Detail 

## 4.1 Overview 

To allocate Distribution Surcharge Journal to appropriate cost of sale accounts to vehicle sold to Canada 

Tulsa units sold to Canada have a $5 Scholarship fee attached to them. The $5 Scholarship fee feeds into the distribution surcharge account. We use Tulsa’s information to credit them back $5 per each unit that they indicate have the fee on it. If there is any remaining balance in the distribution surcharge account after crediting Tulsa, will credit the freight account. Usually the amount leftover is small. 

## 4.2 Process Description 

* 1. Gather source data for journal. 
	+ 1.1. An email is received each month from Accounting Associate Senior from Client, which contains a file indicating which units have a scholarship charge.Open the excel from the mail received. Refer "scholarship column (Column I”) for scholar ship fee. All line items that contains $5 need to be considered for preparation of the Journal.
* 2. Update previous journal file for current period. 
	+ 2.1. Go to M Drive >GA>Spread Sheet Control>Financial Statement Close>DanielleWehnerCopy and paste previous month excel fille to current month.
* 3. Rework journal file. 
	+ 3.1. Take the number of units with the $5 scholarship fee from the excel received via e-mail and enter into the cell D4 and D5 to the working excel. It is established in Client that the exchange rate for $5 USD equals to $7 CAD.
	+ 3.2. In cell G4 and G5 there is formula which calculate number of units multiplied by the exchange rate (Cell F4 multiplied by Cell D4 and Cell F5 multiplied by Cell D5).
	+ 3.3. In order to extract the account activity for the MRAS account 3650, login to OBIEE using the link mentioned below: 
	
	https://evalue.internationaldelivers.com/obi/analytics/saw.dll?bieehome.
	+ 3.4. Go to OBIEE and navigate through as mentioned below: 
	
	Dashboard >MBS Truck > MBS Journal Drill Down
	+ 3.5. Enter the details mentioned below: 
	
	
		- a) BU : 40800
		- b) MRAS Account : 3650 
			* d) Click on: Apply
			* e) Export to Excel
		- c) Journal Date: Current month date range.
	+ 3.6. Export the data to excel and paste to the Working file 2022\_04 APR22 JE 198K Distribution Surcharge” Tab OBIEE GL Balance”. 
	
	In order to extract Foreign Exchange rate, go to OBIEE and select the following: 
	
	
		- a) Dashboard>NFC>Treasure Rate>Foreign Exchange rate>
		- b) Enter current year and month
		- c) Click on applyNote : If the monthend close is April 2022 , select the foreign exchange rate of prior month in this scenario it is March 2022.
	+ 3.7. Click on Foreign Exchange Rates” tab on the screen.
	+ 3.8. Scroll down to ‘US Dollars per currency unit’. Consider the CAD/USD Exchange rate under Monthly Avg rate field. Click on ‘Export’ option to extract the data in to an excel file. JE 198K Distribution Surcharge”, ”MAV Rate” Tab. cell I7
	+ 3.9. Copy the extracted excel data and paste the same in the working file,”2022\_04 APR22
	+ 3.10. Copy and paste the ”CAD/USD rate” under the monthly Avg rate to the Cell I7.
	+ 3.11. Change the month in the Cell,”A1” .Value in Cell F1 will automatically pick the data from
* 4. Go to ”Tulsa Intercompany units” tab and update the data from the excel received via mail for $5 scholarship fee. Values in cell I9 and E13 would auto-populate. 

Go to ‘Entries tab’, Cell E8 is linked to “OBIEE GL Balance” Tab and Cell E9 is linked to cell G4. The balance in Cell E10 is the remaining balance in the surcharge account that should be considered as freight.
* 5. Cell E14 is a formula to calculate the $USD equivalent of the Canadian surcharge. Cell E15 is linked to cell G5. Cell E16 is a formula to calculate the difference, which is posted to the exchange gain/loss account.
* 6. Attach the mail received to the working sheet in the Entries” tab. Update the email attachments for the current month journal entry as highlighted in the above screenshot.
* 7. Refer Generic PeopleSoft Journal Entry desk procedure - Client\_R2R\_GA\_Peoplesoft Journal Entry Posting\_2022\_V1.0 in order to process the journal entry.

### 5 Definitions 

The following are definitions of acronyms used in this document: 



| Term | Definition |
| --- | --- |
| PS | PeopleSoft |

