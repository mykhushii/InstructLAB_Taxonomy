# IBM Confidential 

## GLOBAL PROCESS SERVICES 

# Client 

##  Version: 1.0 

## Status: Draft 

## Client Payment Portal Inquiries-NPPI Mailbox 

The official version of this document is stored [Name of Database, e.g. IBM Document Control System (DCS) and if required to store in client’s database mentioned it too]. Any hard copy versions of this document are for REFERENCE ONLY. Users of this document are personally responsible for using official version, and for verifying that any copies are complete and of the official version. 

1 

### Document Information 

* 1.1
## About this Document 

This is official IBM guide document which describes how IBM Delivery Centre will perform the activity when the request is received from Supplier via NPPI mailbox. Supplier submits the Contact Us query through Invoice payment portal. This document will be used for future reference, either for IBM team or for Client Team. 

### 1.2 

Who should use this Document? 

This document is used by the AP exception team who reviews or work on NPPI Email box as needed. 

* 1.1
## Revision/Approval History 



| Version number | Effective Date | Summary of Changes | Author | Reviewer | Approver |
| --- | --- | --- | --- | --- | --- |
| 1.0 | 04/08/2022 | Draft | MS | RG |  |

2 

### Overview 

* 2.1
## Objective(s) 

Supplier emails are received in generic NPPI Mailbox inquiring multiple types of requests. This activity explains how to retrieve the Debit copies, Remittance, Payment questions and Audit confirmations. Exception team investigates each type of request and provide or forward to correct department basis of the request type. 

* 2.2
## Inputs & Outputs 



| Input | From |
| --- | --- |
| Email in NPPI Mailbox | Client Invoice Information Payment Portal- Suppliers |



| Output | To |
| --- | --- |
| Invoice exception Team | generic Email box, provide or forward to correct department basis of the request type to suppliers. |

Check the payment inquiries/ other requests received in NPPI 

## 3 Control Points 



| # | Sub process Activity | Sub process Activity Description | Control Objective(s) | Control Activity | Risk Assertions | Frequency (i.e. Event, Daily, Monthly, Quarterly, Annually) | Evidence |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | Invoice Exception | NPPI General inquiries | Review the Email and respond with resolution or direct to correct department | Check the inquiry received and action with TAT | Delay in payments and missed SLA/Escalation from suppliers | Daily/Asneeded | Email Tracker |
|  | Invoice Exception | Debit copies | Email and respond with resolution or direct to correct department | Check the inquiry received and action with TAT | Delay in payments and missed SLA/Escalation from suppliers | Daily/As needed | Email Tracker |
| 3 | Invoice Exception | Remittance | Review the Email and respond with resolution or direct to correct department | Check the inquiry received and action with TAT | Delay in payments and missed SLA/Escalation from suppliers | Daily/As needed | Email Tracker |
| 4 | Invoice Exception | Audit confirmation | Review the Email and respond with resolution or direct to correct department | Check the inquiry received and action with TAT | Delay in Audit confirmation will lead to missed SLA/Escalation from suppliers | Daily/As needed | Email Tracker |

2 

Review the 

### 3.1 Process Measurement Reports 

Request received should be worked/responded within the TAT. 

## 4 Roles & Responsibilities 

### 4.1 Description 



| Role | Responsibility |
| --- | --- |
| Invoice Exception | Check the payment inquiries/ other requests received in NPPI generic Email box, provide or forward to correct department basis of the request |

type to suppliers. 

Team 

### 4.2 Segregation of Duties (SOD) Matrix 

For the SOD assessment on conflicting tasks and accesses, please refer to the related Aggregate SOD (A-SOD). <SOD Matrix pending IBM GPS internal review and approval> 

## 5 Process Detail 

### 5.1 Overview 

Supplier emails are received in generic NPPI Mailbox inquiring multiple types of requests. This activity explains how to retrieve the Debit copies, Payment Remittance, Other questions, and Audit confirmations. Exception team investigate the type of request, provide or forward to correct department basis of the request type. 

#### Types of requests: 

* • Debit Copies
* • Payment Remittances
* • Invoice Inqueries (questions) - Generally need to provide status on invoice payment or forward
* • Audits Confirmations to right department

Once above requests are actioned, Emails are moved to respective completed folder basis of the request type. 

* • Completed : Except specific issues all others should moved to this folder.
* • Completed 2 : ONLY Remittances folder.
* • Debit Copies : ONLY Debit copies folder.
* • Audits Confirmations : ONLY Audits folder.
####  Frequency: 

Daily/As needed. 

#### System Applications: 

Peoplesoft, Client Invoice Status Portal,NPPI Generic emailbox and Supplier management database. 

####  Queries: 

ZI\_AP\_PAID\_VCHRS\_ITEM\_REF (PAYMENT REMITTANCE) ZI\_AP\_VCHR\_PYMT\_DETAIL\_SPI (OPEN PAID INVOICES) ZI\_AP\_ERS\_VENDOR\_LIST 

### 5.2 Process Description 

Client Invoice Status Portal Overview- Suppliers have access to view below listed features & they go to portal and check the status basis of the request type. If they are unable to find any details before submitting to NPPI portal from their end, request is submitted via Contact Us option which is received in NPPI mailbox. 

* • Invoice Payment information- Vendor can view payment status basis of the Vendor# or invoice#.
* • Vendor communication Navigation Guide- Vendor can use this guide to navigate the portal.
* • Supplier Invoicing Requirements- This document is to know Vendor shipping location, who they shipped and how they billed, Also this information can be viewed in Clientsupplier.com
* • Debit Inquiry listings- Vendor can open the listing and determine the contacts to reach on the Debit disputes
* • Payment Cycle change Effective- Vendors can view daily pay cycle, majority of pay cycles on weekly every Monday. Mexico pay cycle is weekly,every Thursday’s.
* • Client Early Payments program- C2FO is dynamic discounting program, where vendor offer to a portal and select invoices that are paid early and discount to be paid early for Client. such invoice information vendor can view and sign up to this program.
* • Contact Us- Features is enabled to the vendors to reach out NPPI email box to get the required information.

#### Invoice Payment Information: 

Example:1 How vendor search Invoice payment information from the portal by entering the Vendor# and Invoice# to see Invoice is paid or not. Once required details are updated. Click on ”Search”. 

In the below Payment status is ”N” means not paid ”P” means Paid. 

All the Invoices ”Scheduled Pay Date” showing as future dates, same can be extracted and viewed by the vendor. 

If in case, any past due Invoices are found in vendor search, that can be submitted by the vendor via ”Contact Us” feature from the portal. Exception team should follow same steps to pull the Invoice payment information and send it back to vendor. 

Note: If the invoices are processed in BAAN application that would not show up in the portal, it would show up if it is processed through ”Peoplesoft, Oracle EBZ, Tolas and Avantis”. 

Example: 2 Another way Vendor can search the Invocie Payment status in Client portal is just to remove Invoice Number and update the date range and click on ”Date Range Search”. This data can be downloaded in excel. 

Contact Us Overiew: Click on ”Contact Us” feature from the Client Invoice Status Portal, It will show Inquiry types that suppliers can select. 

* 1. Inquiry Type: ”I have a question regarding my Invoice” - Supplier can select the option and update the required details like Email address, Vednor#, Invoice# and ASN/BOL# click on ”Send My Question” to trigger email to NPPI. ASN/BOL is required for Production Vendors. 

Note: Supplier can email to NPPI, if in case single invoice copy required.
* 2. Inquiry Type: ”I have a question regarding multiple Invoices” - Supplier is required to update multiple invoice details in template. Attach the file to NPPI and submit to NPPI. This template is required especially for Production PO’s. Click on ”Send My Question”.  Here is the template to be filled by the suppliers.
* 3. Inquiry type: ”Why was my Invoice Short Paid” - Supplier can go through the message below and retrive the details. if the shortage is due to pricing, supplier should email to xxx@Client.com. If they have further questions, use the option ”Other” in the Combo Box using the Contact Us feature to reach NPPI.
* 4. Inquiry Type: ”I need to change my bank Information”- Supplier can submit their inquiries directly to category manager. If vendor has further questions, use the option ”Other” in the Combo Box using the the ”Contact Us” feature to reach NPPI.
* 5. Inquiry Type: ”I need to change my remit to information”. This topic is covered in detail separately within this DTP.
* 6. Inquiry type: ”I did not receive a remittance” This topic is covered separately in detail within this DTP.
* 7. Inquiry Type: ”I do not recognize invoice reference on remittance”. If they do no t recognise the invoice in their remittance, it would majorily happen with production invoices where they are not paid to the vendor invoice. Further more examples should be covering under Production Customer Service.
* 8. Inquiry Type: Who is my category manager - Supplier requesting to know the Catergory Manager, they need use the NPPI Portal, update required fields and click on ” Send My Question”. 

Login to Peoplesoft Query Viewer. Select ”ZI\_AP\_CNTRCT\_BUYER\_INFO” Click on HTML option. 

Once clicked on HTML, It will open the next screen. Update vendor number and click on ”View Results”. In View Results, can find Category Manager details which was updated in the ”Description” field. These details can be provided to the supplier. 

Note: Contract number ending with ”A” is for Production and ”C” is for Service Parts.
* 9. Inquiry Type: ”Other”- Suppliers can use Inquiry type ”Other” from the Combo Box. Update required information in the message box and click on ”Send My Question”. All these request notifications trigger to NPPI Emailbox to be worked upon by the Exception team.

##### 5.2.1 Debit Copies request received to NPPI. 

Scenario 1: RTV Type Debit Memo copy - Request received to NPPI email box from the suppliers, Example screenshot shown below. 

Note: Client issues debits throughout different sectors.There is a process that is used within database called supplier management. Certain debit copies related to business issues debit copies are also auto forwarded to the NPPI email box. They are automatically put in a completed folder called ”Debit copies”. If any request received for debit copies, go into the completed folder search if already available in the folder. 

For Warranty copies requests, need to let them know to contact the warranty team for their Debit copies. 

Go to “M” Drive, click on PAYSHARE->DATA->EXCEL->Debit Inquiry Listing to see what kind of PO requested for. RTV is part of Service Parts related as shown below in the screenshot. 

Go to Oracle Imaging Stellent, Copy the Debit Memo number, which was sent in the email, paste in the Invoice number field, and hit enter. 

Next screen will open along with PDF and Debit number. Double click on the PDF icon. 

Once double clicked on PDF icon from the Oracle Stellent, Debit copy will open as shown in the below. 

Save the Debit copy in local desktop, Go back to NPPI Email box and reply to the Supplier by attaching the Debit Copy . 

Post reply to the Supplier with Debit Copy, Move the Email to Completed Folder 

Note: When the Supplier is asking for the Debit Copies, Search with the Debit Memo number in the Email box or Debit copies completed folder, if we find the Debit Copy forward it to the supplier, if we do not find in the Email Box, Pull Debit Copy from the Oracle Website. 

#### Scenario 2: MCP Type Debit: 

Below is the example email received to NPPI requesting the MCP Debit copies from the supplier. 

Go to Plant local website portal, Copy the MCP Debit# paste it into “No” field. Select the check mark from “Estatus General” and then click on “Buscar” icon. In bottom of the screen, can view Debit copy is pulled. Then click on the No “111298”. 

Note: MCP Debit copies will not be available in Oracle Stellent and MCP part of Truck-Rework. 

Click on the No# 111298 as shown in above screenshot, it will go to the below screen where we need to click on the “Imprimir” option to view the MCP copy. Save the copy and reply to supplier with an attachment. For remaining MCP copies, follow same steps. 

#### Scenario 3: AFBE Type Debit copy: 

Request email received to NPPI email box. See below example screenshot asking about backup copy for AFBE. AFBE is related to “Pricing Discrepancies Inquiries” and those would auto email to NPPI. Note: All the copies are kept for 3 months in the mailbox, post that its auto deleted. If any 6 months old copy is requested by the supplier, exception team should go to specific website and pull the copy. Search with the Debit Nunber in the Debit Copies sub folder Email Box, which were auto sent to NPPI. Copy the email and attach to original request which was received from supplier. Reply to supplier with debit copy. 

#### Scenario 4: BR/SCC/SWR Type Debit: 

Request email received to NPPI email box. 

BR Type: BR Debits are debits that were auto emailed to NPPI. Copies are available in Debit copies sub folder. 

SCC Type: SCC Debits are issued by the Spring Field Facility. It’s not auto email and it’s not in Oracle. 

SWR Type: SCC Debits are issued by the Plant Facility. It’s not auto email and it’s not in Oracle. 

Copy the BR debit number, search in Debit copies sub folder. 

Copy the BR Debit copy auto email and paste to original email. 

For SCC and SWR debit copies provide the contact details to supplier to get the debit copies, also “CC” the respective contact which was taken from Debit listing inquiry list. 

For Point of Contact, need to refer the Debit Inquiry Spreadsheet. 

See example below: 

Scenario 5: AFB Debits: Vendors are requested to pull the excel spreadsheet when there is pricing issues and majority of them are from the Production vendors and should be provided in excel format, so that it’s easy for them to reconcile their books. 

Go to Pricing Database to pull the required AFB debit list. Click on “Vendor Excel Request - AFB/PR Invoices - by Invoice Date” and update the Date range. AFB debits are pulled by invoice date. Export the data to excel and forward it to the Supplier. 

Scenario 6: Debit Dispute: Vendor disputes are sent to NPPI. Open the copy of debit and find the point of contact from the Invoice copy. Forward to the point of contact CC’d in NPPI and vendor on the disputes. 

Open the copy of Debit to find the point of contact and send it to them. 

Note: For Debit Disputes, supplier must contact via email which was provided in Debit copy or provide the Contact Details from the Debit Inquiry List. Also, Exception team do not reverse the Debit Memo, only provide the point of contact. 

Another example is shown below to find the point of contact for Disputes from the Invoice copy. 

### 5.3 Remittances 

Retrieving the remittances are from auto emails which are already in Completed 2 folder. Vendor# 56258 remittances details found in completed folder. Attach the remittance excel, send it to supplier. 

Remittance file looks like as shown below. 

Note: For ERS invoices, it gives the part number detail. But Service Parts is not ERS, it just gives them the invoice number and the amount of the invoice. Whereas if it's production- part number details with the quantity and the unit price and the extended price as well. These details should be available in the remittance file which are processed in PeopleSoft. 

#### Remittance pulling steps in Peoplesoft: 

Go to Peoplesoft Query. Click on the “ZI\_AP\_PAID\_VCHRS\_ITEM\_REF” 

Once clicked on the Query – in the Next screen update Vendor Code, Payment Reference # and click on “View Results”. 

Below screen will open, Update the Remit Vendor and Max Rows “3000”. 

Below data is pulled from the Query, this should be forwarded to supplier. 

#### In case the Vendor has not received remittance via Email: 

Email is received requesting to provide the remittances information with Vendor number. 

Login into PeopleSoft •Main Menu •Reporting Tools•Query•Query Viewer 

Select on • ZI\_AP\_PAID\_VCHRS\_ITEM\_REF • click on Excel as shown below. 

Below screen will appear, enter the Vendor Number and Payment References (Remittances Number) and click on View results 

Once clicked on view results, the excel sheet will appear. Then delete the 1st line. The invoice numbers which are paid will reflect on the excel sheet 

If Payment reference number is not provided by vendor, the below steps needs to be followed to pull the remittances with vendor number. 

Login to people soft•Main Menu•Accounts Payable•Review Accounts Payable Info•Payment. 

Enter the Vendor number in Remit Vendor field as shown below. Click on Search. 

Once clicked on search button, Below screen will appear. Sort out with ”Payment Date” and ”Payment Reference ID” to know recent payments made to the vendor. 

Export the data into excel, ‘A’ column shows the Payment references number. Remittance file also contains all other fields like Invoice#, Currency, Inv Date etc. 

Attach the excel sheet which contains payment information. Reply to the email request 

Scenario 2: Setting up Remittance Details in ”Supplier Management tool”. 

In few instances there may be changes in remittance email address from the suppliers or Suppliers have not received the remittances due to remittance check box updated as ”N” in Supplier Management portal. 

Below email request is received to update ”remittance email address” in Supplier Management portal. Once remittance email is updated. Vendor receives the remittance to their email automatically. 

Go to PAYSHARE -DATA-ACCESS, Login to Supplier Management- Click on ”SplrMgmnt” 

Click on ”Retrieve”. 

The below screen will appear, enter the Vendor number and click on OK 

Suppler Management – ”First page for Remittances”. 

Check if the Email Remittances is set to ”Y” or not. If it is updated as ”N”. Always make sure it is changed to ”Y” so that vendor will receive their remittances automatically. 

Once Email Remittance is set to ”Y”. Click on ”Save” button. 

Note:Team Code ”PP” Production vendors. 

Supplier Management- ”The second page is for Debit copies”. Request received to update the email ID as shown below. 

Note: Team Code ”SPI” for Service Parts. 

Go to supplier managment portal. Check if the Email Remittance field is set to “Y” or not. If it is updated as ”N”. Make sure its chaged to ”Y”. Go to Email field to update new ”Email ID” which is requested by the supplier via email. Click on ”Save”. 

Note: Always make sure Email Remittance should be set to “Y” so that Vendor will receive the Debit copies. 

### 5.4 Invoice Inquiries 

* 1. Request received for processing the payment along with Invoice and Vendor details.
* 2. Open the Invoice copy received in the Email and look for Customer PO number. Review attached PDF copy with Business Unit and PO number to determine whom to send it for payment processing from the ”Quick Reference Guide”.
* 3. Open Quick Reference Guide file for PO inquiries. (Refer to below spreadsheet to identify the correct department as per the PO series)
* 4. Cross check the PO series mentioned in the invoice copy with Quick Reference guide to identify the correct department to whom we need to reach out. Note: Above example PO 3XXXXXX is part of Service Parts and should go to xxx@Client.com to process.
* 5. Once reviewed with quick reference guide excel file, forward the email to the concerned Customer Service department. Move the email to completed folder.

Note: Include all parties in your email reply. When addressing to concerned dept to take an action and make sure their email ID are included in ”To” section, remaining all receipents can move into ”CC”. 

If there are any attachments received in original email request should be added, when routing to correct department. 

#### Other Inquries:- 

#### Example 1: 

Request received inquiring about ”Multiple Invoices Question” as mentioned below. 

Open the Excel sheet attached in email. 

Note: If Customer PO Ends with the ”A series”. It should be for ”Production Parts”. 

Determined that the PO series is part of Production. This file should be forwarded to ”Production Customer Service” department for processing. 

Move email to Completed folder. 

#### Example: 2 

Request received in NPPI for the ”Invoice Question”. 

Open the Invoice copy whcih is attached in the email. 

Review the PO with Quick Reference Guide. Here is PO series mentioned with 82XXXX series per the Onshore update 83XXXX series customer PO is part of Mexico. 

Go back to NPPI email box, Forward the email along with Invoice copy to ”AP Mexico Customer Service” and ”DL AP.Escodedo” for processing. Move email to Completed folder. 

#### Example: 3 

Email received with an AR aging report as an attachment. 

Open both aging spread sheets. Aging report contains all the Invoices and Customer PO numbers. In this case a lot of contracts should be involved. Always look for the Customer PO number to identify right department. This should be determined based on the customer PO from Quick reference Guide. 

Once determined the right department based on the Customer PO’s, forward the email to concerned departments by adding attachments. Once email is forwareded, move the email to Completed folder. 

#### Example: 4 

Monthly vendor Statements are received to NPPI email box. Majority of them will not ask for the payment information. 

Customer service team do not review current month invoices and do review only past due invoices. During statement review if any invoices found as past due, CS team will send an email to the vendor asking for the spreadsheet. 

Post receipt of the spreadsheet. Search the right department based on the Customer PO from the quick reference guide and route it to right department for processing. 

Here is the example email which was received to NPPI along with the statements. 

### 5.5 Audit Confirmation 

This process main ojective is to provide confirmation of vendor payments per audit firm request. Audit confirmations email received to ”Service Parts Customer Service” that email should be forwarded to NPPI email box. 

Vendor has an auditor who is reviewing their Receivables and Payables as a part of the Audit process. Those vendors send an email to their suppliers vendors, to find out the payments for certain invoices are in their system to be paid. Such instances vendors reach out to NPPI for the Payment details along with Invoice Date. 

* 1. Request received to NPPI email box requesting Audit confirmations. Identify the Vendor name and Vendor Code received in email subject line as shown below. Note: Few instances, vendors can send the Audit Confirmation request to ”Service Parts Customer Service. It will be routed to NPPI mailbox to priovide the details.
* 2. Open the attached PDF copy. Check the Invoice Date which was requested.
* 3. Login to Peoplesoft•Favourites•MainMenu•Reporting tools•Query•Query Viewer select(ZI\_AP\_VCHR\_PYMT\_DETAIL\_SPI\_V2)
* 4. Search with Vendor code and update the date range. (For example if invoice date is 17/08/202, update the date as 01/08/2021). This query will pull all the Open and Paid Invoices. Remit Vndr- Vendor Number 

Begin Invoice Date- Invoice Date ( Date should be based on the requirement) 

End Invoice Date- ”t” today’s date. ( No need to update current date, ”t” means today’s date)
* 5. After entering required details, click on View Results.
* 6. Once clicked on view results, Go to other Query Peoplesoft•Favourites•MainMenu•Reporting tools•Query•Query Viewer Query select- (ZI\_AP\_VCHR\_PYMT\_DETAIL\_SPI\_V2) extract the details into excel sheet.
* 7. Once Excel is extracted, sort out with Invoice number column in the Alphabetical oder A- Z for vendor reference.
* 8. Save the file name as ”Remittance Details”.
* 9. Send the file to the requestor by attaching the remittance file.
* 10. Move the email to Completed folder.

The following are definitions of acronyms used in this document: 



| Term | Definition |
| --- | --- |
| PS | Peoplesoft |
| BU | Business Unit |
| NPPI | Client Payment Portal Inquiries |
| AR | Accounts Receivable |
| NISP | Client Invoice Status Portal |

