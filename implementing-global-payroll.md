Oracle Fusion
Cloud Human
Resources

Implementing Global Payroll

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

G34713-08

Copyright © 2026, Oracle and/or its affiliates.

Author: Oracle Human Resources Information Development Team

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Contents

Get  Help  ................................................................................................................................    i

1 Let’s Get Started

1

Overview  ............................................................................................................................................................................................    1

Setup Tasks for Implementing Global Payroll ..........................................................................................................................   2

Responsive User Experience Setup ............................................................................................................................................  6

Integration With Other Applications ..........................................................................................................................................   8

Payroll Concepts to Understand ................................................................................................................................................  13

Application Tools ..........................................................................................................................................................................  74

Prerequisite Tasks ........................................................................................................................................................................  113

Setup Task List for HCM ............................................................................................................................................................  114

Setup Task List for Financials ...................................................................................................................................................  117

Setup Task List for Payment Reconciliation ..........................................................................................................................  119

2 Elements, Earnings and Deductions

123

Payroll Elements ..........................................................................................................................................................................  123

Earnings and Deductions .........................................................................................................................................................   129

Element Classifications ..............................................................................................................................................................  139

Element Employment Level .....................................................................................................................................................   146

Element Configurations ............................................................................................................................................................   147

Element Input Values ................................................................................................................................................................   166

Standard Element Entries .........................................................................................................................................................   172

Element Eligibility .......................................................................................................................................................................   179

Voluntary Deductions ................................................................................................................................................................   182

Involuntary Deductions .............................................................................................................................................................   192

Net-to-Gross Earnings ..............................................................................................................................................................   198

FAQs for Elements .....................................................................................................................................................................  204

3 Calculation Cards and Calculation Values

209

Payroll Calculation Information ..............................................................................................................................................   209

Payroll Calculation Information Formulas .............................................................................................................................   215

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Calculation Cards ........................................................................................................................................................................  223

Calculation Value Definitions ..................................................................................................................................................   228

Calculation Factors .....................................................................................................................................................................  237

4 Rates and Values by Criteria

241

Rate Definitions ...........................................................................................................................................................................  241

Values Defined by Criteria .......................................................................................................................................................   285

5 Payroll Processing Rules

315

Payroll Process Configuration Groups ...................................................................................................................................   315

Restrict Payroll Processing .......................................................................................................................................................  326

Optimize Performance of Multi-Thread Processes ............................................................................................................   328

Optimize Performance of the Payroll Background Process ..............................................................................................  329

Logging and Monitoring the Payroll Background Process ...............................................................................................   330

Expedited Processing ................................................................................................................................................................   332

6 Payroll Definition Details

335

Payroll Definitions ......................................................................................................................................................................   335

Pay Frequency ............................................................................................................................................................................   342

Periodicity  ....................................................................................................................................................................................     344

Consolidation Groups ................................................................................................................................................................  347

Time Definitions .........................................................................................................................................................................  349

Run  Types  ....................................................................................................................................................................................     352

Object  Groups  .............................................................................................................................................................................     353

7 Payroll Balances

357

Balance Definitions ....................................................................................................................................................................   357

Balance Groups and Usages ...................................................................................................................................................   365

Balance Exceptions ....................................................................................................................................................................   372

Balance Exception Report ........................................................................................................................................................   377

Copy Balances During Global Transfer .................................................................................................................................   382

FAQs for Balances ......................................................................................................................................................................  385

8 Payments

387

Bank Accounts ............................................................................................................................................................................  387

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Payment Methods .....................................................................................................................................................................   394

Organization Payment Methods .............................................................................................................................................  395

Personal Payment Methods ....................................................................................................................................................  408

Third-Party Payment Methods ................................................................................................................................................  418

Third-Party Payments ...............................................................................................................................................................  425

Reprocess Rejected EFT Payments ........................................................................................................................................  429

Configure Payslips and Checks ...............................................................................................................................................  433

9 Events, Retroactive Pay and Proration

451

Payroll Event Groups .................................................................................................................................................................   451

Retroactive Pay ...........................................................................................................................................................................  455

10 Auditing and Data Validation

461

Audit Payroll Business Objects ................................................................................................................................................  461

Audit Element Security Profiles ..............................................................................................................................................  462

Payroll Validations for Absence and Time Entries .............................................................................................................   463

Audit  Policies  ..............................................................................................................................................................................     464

Audit Configuration for Business Object Attributes ..........................................................................................................   465

Audit  Reports  ..............................................................................................................................................................................    466

Data Security in Payroll Data Validation Reports ...............................................................................................................   467

11 Implementing Payroll Costing

469

Overview of Payroll Costing ....................................................................................................................................................  469

12 Implementing Payroll Core

471

Overview of Payroll Core ..........................................................................................................................................................   471

Setup Tasks for Implementing Payroll Core .........................................................................................................................   471

TRU Defaulting Rules for Payroll Core ..................................................................................................................................  474

Considerations to Assign Employee Details Using TRU Currency ..................................................................................  475

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Get Help

Get Help

There are a number of ways to learn more about your product and interact with Oracle and other users.

Get Help in the Applications

  to give you access to contextual help. If you don't see any help icons on
Some application pages have help icons
your page, click your user image or name in the global header and select Show Help Icons. If the page has contextual
help, help icons will appear.

Get Training
Increase your knowledge of Oracle Cloud by taking courses at Oracle University.

Join Our Community
Use Cloud Customer Connect to get information from industry experts at Oracle and in the partner community. You
can join forums to connect with other customers, post questions, suggest ideas for product enhancements, and watch
events.

Share Your Feedback
We welcome your feedback about Oracle Applications user assistance. If you need clarification, find an error, or just
want to tell us what you found helpful, we'd like to hear from you.

You can email your feedback to oracle_fusion_applications_help_ww_grp@oracle.com.

Thanks for helping us improve our user assistance!

i

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Get Help

ii

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

1  Let’s Get Started

Overview

Use the Application Implementation Consultant role (ORA_PAY_APPLICATION_IMPLEMENTATION_CONSULTANT_JOB)
to access the Workforce Deployment offerings in the Setup and Maintenance and start an implementation of Cloud
Payroll.

Refer to the Functional Setup Manager guide to manage the opt-in and setup of your offerings.

Workforce Deployment Offering
You use this offering to set up enterprise structures, legal entities, and organizations to create and maintain information
related to people, employment, and work structures. This offering also has tasks for you to define payroll business
objects required for processing and costing payroll, processing payments, and generating statutory reports.

This table outlines the primary functional areas of this offering. For the full list of functional areas and features in this
offering, use the Associated Features report. Review the report when you plan the implementation of your offering. The
setup steps required for payroll vary depending on your business requirements.

Functional Area

Description

Legal Structures

Manage legal entities, legal reporting units, tax reporting units, payroll statutory units, legal authorities,
 legal registrations and jurisdictions, and legal authorities.

Organization Structures

Manage organization structures, business units, and organization models that best suit your business
process.

Workforce Structures

Manage locations, divisions, departments, jobs, positions, and grades.

Elements and Formulas

Configure elements and formulas to record earnings and deductions for processing payroll and
reporting.

Payroll

Define payroll objects and payment methods required for payroll calculations and reporting, and
processing and making payments.

Related Topics

• Plan Your Implementation

• About This Administering Global Payroll Costing Guide

• Payroll Cost Allocation Key Flexfield Structure

1

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Setup Tasks for Implementing Global Payroll

Use to understand options and determine the sequence of tasks to implement global payroll.

To implement the Oracle Fusion Global Payroll application, sign-in as a user with Application Implementation Consultant
or Payroll Implementor role and opt into the offerings applicable to your business requirements.

Before you begin implementing Global Payroll, you must complete:

•

•

Initial application setup.

Implementation of Global Human Resources and the requisite HR setup tasks for implementing and processing
payroll. For more information, refer to the Implementing Global Human Resources guide.

Security Reference
The tasks that people can do and the data that they can see depend on their roles, duties, and privileges. For
information about these factors, see these two guides:

• Securing HCM

• Securing Reference for HCM

Workforce Deployment Offering
Use this offering to set up enterprise structures, legal entities, and organizations to create and maintain information
related to people, employment, work structures, and statutory requirements. The offering also includes tasks for
defining payroll business objects required for processing and costing payroll, processing payments, and generating
statutory reports.

This table lists the setup tasks required to implement the Global Payroll application. Perform all of these tasks from the
Setup and Maintenance work area.Use My Enterprise on the Home page to navigate to Setup and Maintenance. Most
of these tasks are under the Workforce Deployment offering unless otherwise specified in the first column of this table.

Setup Tasks for Implementing Global Payroll

Implementation Tasks List

Task Name

What you must do

Where to Find Information

Prerequisite Tasks for Payroll Setup

Setup and Maintenance

Create an Implementation Project

• Offering: Customer Data

Manage Territories

Management

• Functional Area: Application

Extensions

• How You Use Implementation
Projects to Manage Setup

• Manage Setup Using

Implementation Projects

• Create Countries

Create an implementation project
and select the enabled Workforce
Deployment offering to generate
the initial list of setup tasks
required to implement the Global
Payroll application.

If you're unable to find a
specific country in the Manage
Geographies page, create the
country. Use this country to set up
your organization and other setup
tasks.

2

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Implementation Tasks List

Task Name

What you must do

Where to Find Information

Select Default Currency

Define Common Applications
Configuration/Define Geographies
for HCM

Manage Geographies

Define Common Applications
Configuration/Define Features by
Country or Territory

Features by Country or Territory

Use the territory code and name
to verify geographies, create legal
addresses, and select the country
extension.

On the Manage Territories page,
 select the default currency for the
country. This is the currency in
which balances are accumulated
for this legislation.

Use the territory code to verify
predefined geographies and load
any additionally required local
geographies. You can import
Oracle-licensed data from Loqate,
for those countries where the data
is available.

Select the correct product for
your legislation. The country
extension setting ensures that
certain payroll-related features,
such as element templates, work
correctly in your implementation.

• Manage Currencies

• Geographies for HCM

• How Country Extensions are

Selected

Select Address Style and Address
Validation

Check the address style and
address validation for your country.

• Change Address Styles and
Address Validation Settings

Define Common Applications
Configuration/Define Enterprise
Structures for HCM

Manage Legislative Data Groups

Define at least one Legislative
Data Group for each country your
enterprise operates in.

Define Common Applications
Configuration/Define Enterprise
Structures for HCM/Define Legal
Jurisdictions and Authorities for
HCM

Manage Legal Addresses

Manage Legal Jurisdictions

Manage Legal Authorities

Define Common Applications
Configuration/Define Enterprise
Structures for HCM/Define Legal
Entities for HCM

Manage Legal Entity

Manage Legal Entity Registrations

Create legal addresses for all
organizational units of the
enterprise before you create legal
entities.

Review the predefined jurisdictions
for your country and create any
jurisdictions you require for
specific local taxes.

All legal entities must be registered
against a jurisdiction that is
governed by a legal authority.
Create legal authorities as required
for your country.

Create all legal entities that apply
to the enterprise you are setting
up. Designate the legal entity as
a legal employer and as a payroll
statutory unit (PSU) for payroll.

Define registration details of the
legal entity you create. Register
them with the appropriate
government or legal authorities

• Enterprise Structures

• Legal Entities, Business Units,
 and Reference Data Sets

• Legislative Data Groups

• What's a legal address?

• Overview of Legal Jurisdiction

and Authorities

• Create Legal Jurisdictions,
 Addresses and Authorities

• Legal Entities

• Legal Entities, Business Units,
 and Reference Data Sets

3

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Implementation Tasks List

Task Name

What you must do

Where to Find Information

Define Common Applications
Configuration/Define Enterprise
Structures for HCM/Define Legal
Entities for HCM/Define Legal
Reporting Units for HCM

Manage Legal Entity HCM
Information

Manage Legal Reporting Unit

Manage Legal Reporting Unit
Registrations

Manage Legal Reporting Unit HCM
Information

Define Payroll Legislations

Configure Legislations for Human
Resources

Payroll Setup Tasks

Define Payroll Legislations

Configure Payroll Legislations

Define Common Applications
Configuration/Define Enterprise
Structures for HCM/Define Legal
Entities for HCM

Define Common Applications
Configuration/Define Enterprise
Structures for HCM/Define Legal
Entities for HCM/Define Legal
Reporting Units for HCM

Define Payroll/Define Payroll
Business Definitions

Legal Entity Calculation Cards

Legal Reporting Unit Calculation
Cards

• Payroll Lookups

• Payroll Value Sets

• Descriptive Flexfields for

Payroll

• Extensible Flexfields for

Payroll

for the purpose of claiming and
ensuring legal or commercial rights
and responsibilities.

Manage legal entity HCM
information to include statutory
components as required.

Define legal reporting units (LRU)
also known as tax reporting units,
 to group employee records for tax
and social reporting.

• Legal Entities

• Legal Entities, Business Units,
 and Reference Data Sets

Define registrations details of
the LRU and register them with
the appropriate government
or legal authorities for the
purpose of claiming and ensuring
legal or commercial rights and
responsibilities.

Review the LRU that employs and
pays workers. Define statutory
requirements as required.

Create the legislative rules for
your country. Legislative rules
govern default values and how you
manage employee records in your
organization. Configure payroll
relationship rule for your country
and map a person type to a payroll
relationship type.

Create the payroll legislative data
for your country. Set up elements,
balances, and other payroll-related
data for implementations.

Review and edit predefined
calculation cards for payroll
statutory units. The payroll process
uses the calculation rules defined
on the cards to calculate earnings
and deductions.

Review and edit predefined
calculation cards for tax reporting
units. The payroll process uses the
calculation rules defined on the
cards to calculate earnings and
deductions.

• Legislation

• Payroll Relationships

• Legislation

• Payroll Relationships

• Calculation Cards

• Calculation Factors

• Wage Basis Rules

Create lookups, value sets,
 and descriptive and extensible
flexfields that you need to support
payroll.

• Define Lookups

• FAQs for Define Lookups

• Manage Value Sets

• FAQs for Manage Value Sets

• HCM Flexfields Setup

4

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Implementation Tasks List

Task Name

What you must do

Where to Find Information

Define Payroll/Define Earning and
Deduction Definitions

• Elements

• Element Classifications

Calculation Value Definitions

Payroll Calculation Information

Values Defined by Criteria

Rate Definitions

Component Group Rules

• Balance Definitions

• Balance Groups

• Balance Group Usages

• Balance Exceptions

• Balance Exception Reports

• Manage Banks

• Manage Bank Branches

• Manage Bank Accounts

Define Payroll/Define Balance
Definitions

Define Payroll/Define Payment
Methods/Set Up Banks, Branches,
 and Accounts

• HCM Flexfields Maintenance

• Elements, Earnings and

Deductions

• Calculation Value Definitions

• Payroll Calculation

Information

• Payroll Calculation

Information Formulas

• Values Defined by Criteria

• Rate Definitions

• Component Group Rules

• Payroll Balances

The application provides many
predefined elements that cannot
be modified at the implementation
level. Define additional elements as
required.

Review the tables that hold
the rates and values used to
calculate earnings, deductions and
exemption amounts. Create new
calculation definitions as needed.

Review the payroll calculation
information rules and definitions
generated for user-defined
elements. These rules and
definitions are used for calculation
of earnings and deduction
amounts.

Create the criteria rules or
evaluation conditions that
determine a particular value or
rate.

Review the predefined rate
definitions and create new
definition as needed. The rate
definition can either be a derived
rate or a value defined by criteria.

Review the rules defined for
earnings and deductions that
belong to the same component
group and create new rules.

The application provides many
predefined balances. Review the
definitions of predefined balances
and create new definitions,
 including assigning dimensions
and feeds.

Create and edit banks, branches,
 and accounts.

• Bank Accounts

Define Payroll/Define Payment
Methods

Organization Payment Methods

Define Payroll/Define Pay
Frequency

Consolidation Groups

Review predefined organization
payment methods and create
new methods and their payment
sources.

• Payment Methods

• Organization Payment

Methods

Review the consolidation groups
assigned to payroll definitions and
create new groups. They let you
process the results from more than
one payroll in a single action.

• Consolidation Groups

5

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Implementation Tasks List

Task Name

What you must do

Where to Find Information

Time Definitions

Payroll Definitions

Define Payroll/Define Fast
Formulas

User-Defined Tables

Fast Formulas

Define Payroll/Define Payroll Flow
Patterns

Payroll Flow Patterns

Review predefined time definitions
and create or update static and
dynamic intervals of time.

Create and update payroll
definitions that specify the
payment frequency, processing
schedule, and other parameters.

Review the predefined table
structures and create and update
new user-defined table structures.

Review predefined formulas and
create new ones to validate or
calculate data for payroll.

Review the predefined payroll flow
patterns and create new patterns
to meet specific requirements.

• Time Definitions

• Payroll Definitions

• Run Types

• Pay Frequency

• Periodicity

• User Defined Tables

• Fast Formulas

• Payroll Flows

Other Document References
For more detailed information about the setup tasks and other related applications and tasks, refer to these guides at
docs.oracle.com/cloud/latest/globalcs_gs/docs.htm.

•

Implementing Global Payroll

• Administering Global Payroll

• Administering Global Payroll Flows

• Administering Fast Formula

• Administrating Payroll Costing

•

•

•

•

Implementing Absence Management

Implementing Benefits

Implementing Time and Labor

Implementing Workforce Compensation

Responsive User Experience Setup

Profile Options for Redwood User Experience Setup for Payroll

Redwood is the new user experience in Oracle HCM applications. Many pages and flows have been recreated in the
Redwood toolset Visual Builder Studio (VBS) to improve the user experience by creating cohesiveness through the
application.

6

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Some of the Redwood pages are enabled, by default. You will need to enable the respective profile options for other
pages to get the Redwood user experience. In addition, you also need to enable the ORA_HCM_VBCS_PWA_ENABLED
profile to enable the HCM Redwood pages. However, we recommend you evaluate your business requirements before
enabling the Redwood experience.

This table lists the profile options to enable or disable the Redwood experience for the following pages in Global Payroll.

Page

Payslips

Profile Option Code

Default Value

ORA_PAY_PAYSLIPS_REDWOOD_ENABLED

No

Payroll Relationships

ORA_PAYROLL_RELATIONSHIPS_REDWOOD_

No

ENABLED

Year-End Documents

ORA_PAY_YEAR_END_DOCUMENTS_

No

REDWOOD_ENABLED

Deep Links

You can use deep links to provide easy navigation directly to a page in the HCM Cloud application.

You can also use deep links for mobile responsive pages on your intranet, custom and third-party applications, or in a
document. This helps people run transactions in the HCM cloud and provides quick access to their HR information.

To access deep links:

1. Open the main menu.
2. Go to Tools> Deep Links.
3. Copy the URL for a deep link.
4. Paste the URL in the appropriate location.

When you open Deep Links, you find a list of all available deep links.

Search Logic Profile Options for Client List of Values

You can use the logic <codeph>CONTAINS</codeph> to create the client list of values. This returns results containing
the characters you enter.

Optionally, for individual list of values, you could change this logic to <codeph>STARTS WITH</codeph>, to return
results that start with the search characters you enter.

For example, when you search for a person with the name John Smith while using the logic CONTAINS, you can search by
'jo' or 'sm' or 'th'. When you use the logic STARTS WITH, your search must start with 'j'.

Use the logic STARTS WITH when your list contains thousands of values (more than 15,000 records) to improve the search
performance. Or, if you don't partition your data by set ID.

7

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Note:  If you change the search logic for a client list of values, the logic changes in all pages where the list of values is
used.

Related Topics

• Search Logic Profile Options for Client List of Values in Global Human Resources

Use Transaction Design Studio to Configure Field Displays

Use the Transaction Design Studio (TDS) to configure transactions and pages for responsive applications. TDS is
available within the HCM Experience Design Studio.

You can control the visibility of attributes that are displayed either as Delivered or Enabled, and the availability of fields
and sections of a transaction based on the user's role, person's business unit, or legal employer.

By default, the responsive pages display the often used attributes and hide the less often used attributes. Use Page
Composer to personalize the responsive pages and display the attributes and tabs delivered within the feature.

Here's how you start HCM Experience Design Studio:

1. Sign in to the application as Human Capital Management Application Administrator with Access HCM Page
Configurator (HRC_ACCESS_HCM_TRANSACTION_CONFIGURATOR_PRIV) privilege. This privilege provides
you access to TDS in HCM Experience Design Studio.

2. Enable a sandbox to compose data for configuring business objects. On the Home page, click the HCM

Experience Design Studio quick action under the My Client Groups tab.

3. Under Settings and Actions, click Edit Pages.
4. Select the site layer and click OK.

Related Topics

• Overview of Page Modification

Integration With Other Applications

Time and Labor

Overview of Time, Absence, and Pension Data for Payroll
You can automate the regular import of time card entries, absence entries, and pension enrollments.

Load Data Options
The application that you use to record time, absences, and pensions determines options for importing data to payroll.
This table lists the applications for transferring data to payroll.

8

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Source Application

Data Load Options

Time card

• For Oracle Fusion Time and Labor, submit the Load Time Card Batches process.

• For third-party time applications, you can load time cards using HCM Data Loader.

Absences

• For Absence Management, use the Absence Records task to record an absence and transfer it

directly to the person's absence calculation card.

When you set up the plan in Absence Management, select the Transfer absence payment
information for payroll processing check box. Find this setting in the Payroll Integration
section of the Entries and Balances tab on the Create Absence Plan page.

• For third-party absence applications, you can load absence records using HCM Data Loader.

Pensions

You can load benefits and pension calculation cards using HCM Data Loader.

The availability of this process depends on the implementation for your country or territory.

Related Topics

• Example of Loading Payroll Time Cards

• Example for Loading Absence Records

• Guidelines for Loading Calculation Cards

Prerequisite Payroll Setup for Importing Time Entries
Before you can import time card entries to process in a payroll run or extract for a third-party payroll provider, complete
payroll setup tasks.

These tasks vary depending on your configuration, specifically whether your enterprise:

• Uses Oracle Fusion Time and Labor or a third-party time provider

• Uses Oracle Fusion Global Payroll or a third-party payroll provider

• Requires workers to submit a time card if their pay is calculated using time entries

This figure and table lists the tasks that depend on each of these configuration choices.

9

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

All configurations create elements for use with time cards. This table describes the remaining setup tasks and processes
that vary based on your configuration.

Task

Applies To

Create elements for time card entries

All configurations

Create rate definitions and associate with
the elements if the rate is different from
the default salary rate

Elements whose rate isn't the default salary rate

Determine which value definitions would
override the criteria for the rate definition

Optional for all configurations

10

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Task

Applies To

Determine which cost segments workers
complete on their time cards

Optional for all configurations

Record costing overrides at the element
entry level by having workers specify the
account to charge on their time cards.

Note:
If you enable costing overrides, ensure
that you're using the segments that are
enabled for element entry level costing
in the Cost Allocation key flexfield.

Create an HCM extract definition of time
card elements

Third-party time provider

Determine process to transfer time card
entries to payroll:

Third-party time provider

• Use the Load Time Card Batches
process to upload time entries to
calculation cards.

• Use HCM Data Loader to load

element entries.

Schedule process to transfer time card
entries

Optional for all configurations

As an example, schedule the Load Time
Card Batches process:

• After normal working hours to
distribute the load on server

• To run more frequently during time
periods when most employees
submit their time cards

Create an HCM extract definition that
includes time entries

Third-party payroll provider

Notify HR to select Time Card Required
field at the Terms or Assignment level
when a new hire's pay calculations depend
on time cards.

Optional for all configurations

11

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Related Topics

• Time Card Required Option

• Create Time Card Elements for Time Entries

• Extract Components

• Enable Overrides for Time Elements Using Values Defined by Criteria

Absence Management

Integrate Absence Management with Global Payroll
Use Oracle HCM Cloud Absence Management to set up and enroll persons in absence plans. Transfer absence
information to Cloud Payroll for processing and paying absences.

Select these different quick actions under the My Client Groups tab to integrate Absence Management with Cloud
Payroll.

Steps

Create an absence plan, such as an
Accrual, Qualification, or No Entitlement
plan.

Tasks

Absence Plans

Create absence types based on predefined
absence patterns and associate them to
the absence plans.

Absence Types

Create rate definitions to use in calculating
accrual and liability balances.

Rate Definitions

Create absence elements.

Elements

Complete these payroll integration
information:

Absence Plans

Note:
Find these settings in the Payroll Integration section of the Entries and Balances tab on the Create
Absence Plan page.

• Select the Transfer absence payment
information for payroll processing
check box.

• Select the element for the plan in

the Element field. The element links
the absence plan to the calculation
component shown on the person's
calculation card.

• Optionally, specify rates. These rates
override rates specified elsewhere.

Enroll persons in the absence plan:

Absence Records

12

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Steps

Tasks

• Add the plan and provide the
entitlement date information.

• For accrual plans, select the Run
Accruals for Selected Plan task
action.

Chapter 1
Let’s Get Started

After the information is set up, use the Absence Records task to record an absence. When the absence is approved, the
daily and summary breakdown information is automatically transferred to payroll.

You can then process the payroll that includes these absence entries and view the resulting absence balances on the
person's Statement of Earnings. After you process and archive payments, you can view the resulting absence balances
on the person's payslip.

Related Topics

• Define Payroll Elements to Process Absences

• Rates Used to Calculate Absences in Payroll

• How Many Salary Bases to Create

•

Import Absence Entries to Payroll

Payroll Concepts to Understand

Date Effectivity

Date Effectivity Overview
Date effectivity preserves a history of changes made to the attributes of some objects. As a Professional user, you can
retrieve and edit past and future versions of an object.

Many Human Capital Management (HCM) objects, including person names, assignments, benefits plans, grades, jobs,
locations, payrolls, and positions are date-effective.

Logical and Physical Records
Date-effective objects include one or more physical records. Each record has effective start and end dates. One record is
current and available to transactions. Others are past or take effect in the future. Together, these records constitute the
logical record or object instance. For a date-effective logical row, which is a collection on contiguous temporal physical
rows, each physical row CreatedBy (CREATED_BY) and CreationDate (CREATION_DATE) are the same.

This table shows changes to the department manager attribute in a department business object. Each row represents a
single physical record.

Physical Record

Effective Start Date

Effective End Date

Department Manager

4

18 January, 2022

C. Woods

13

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Physical Record

Effective Start Date

Effective End Date

Department Manager

3

2

1

15 October, 2021

17 January, 2022

A. Chan

13 June, 2020

14 October, 2021

T. Romero

22 March, 2019

12 June, 2020

G. Martin

Note:  The physical record number doesn't appear in the record.

Effective End Dates in Physical Records
Every physical record except the last has an effective end date. The update process adds this date, which is the day
before the effective start date of the next record, whenever you update the object.

Object End Dates
You can enter a final effective end date for some date-effective objects. For example, terminating an assignment adds
a final effective end date to the assignment. Alternatively, the End Date action may be available. If you end date a date-
effective object, then it isn't available to transactions after that date. But the object's history is retrievable.

Status Values in Date-Effective Objects
Some date-effective objects, such as grades and jobs, have both effective dates and status values. When the object
status is Inactive, the object isn't available to transactions, regardless of its effective dates. Setting the status to
Inactive makes objects unavailable to transactions. If you can't enter an effective end date for an object, then changing
its status has the same effect.

Future-Dated Changes
For date-effective objects, you can enter future changes. For example, you enter the worker promotion shown in this
table on 25 July, 2022 to take effect on 18 October, 2022.

Physical Record

Effective Start Date

Effective End Date

Grade

2

1

18 October, 2022

14 December, 2020

17 October, 2022

IC2

IC1

Physical record two becomes current on 18 October, 2022. From 14 December, 2020 until 17 October, 2022 physical
record one is current and available to transactions. If you can access the object history, you can see physical record two
before it takes effect.

When future-dated changes exist, other actions may be limited. For example, to end this worker's assignment before
the promotion takes effect, you must first delete the promotion.

14

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Date-Enabled Objects
Some objects, such as work relationships, are date-enabled rather than date-effective. They have start and end dates
that define when they're available, but they have no history of changes. New attribute values overwrite existing attribute
values.

Related Topics

• How You Delete Physical Records from Date-Effective Objects

• Examples of Updating Date-Effective Objects

• Examples of Correcting Date-Effective Objects

• How You Make Multiple Updates to Date-Effective Objects in One Day

How You Delete Physical Records from Date-Effective Objects
The effect of deleting a physical record from a date-effective object depends on the record's position in the object's
history.

Consider the date-effective object, which has three physical records, shown in this table.

Physical Record

Effective Start Date

Effective End Date

Attribute Value

3

2

1

15 August, 2022

30 October, 2021

14 August, 2022

10 June, 2020

29 October, 2021

C

B

A

Intermediate Records
If you delete physical record two, where the attribute value is B, then the object is as shown in this table after the
deletion.

Physical Record

Effective Start Date

Effective End Date

Attribute Value

2

1

15 August, 2022

10 June, 2020

14 August, 2022

C

A

If physical records exist both before and after the deleted record, then the deletion adjusts the dates of the surrounding
records automatically. The effective end date of the previous record is now the day before the effective start date of this
record. This change closes the gap in the object's effective dates.

First or Only Records
In most cases, you can't delete the first or only physical record.

15

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

If you can delete the first physical record, then the object exists from the effective start date of the next physical record
(30 October, 2010 in this example). If only one physical record exists, then deleting that record is the same as deleting
the object.

Final Records
If you delete the final physical record, then the deletion removes the effective end date automatically from the previous
physical record (14 August, 2011, in this example).

Country Extensions

How Country Extensions are Selected
Use the Features by Country or Territory task under Payroll in My Client Groups, to select the correct product for your
legislations. The country extension setting ensures that certain payroll-related features, such as element templates,
work correctly in your implementation.

By default, each country's extension is set to Human Resources or None, which means no payroll product is selected.
If you plan to use payroll or any predefined payroll interface extracts for a country or territory, you must set its country
extension to the appropriate payroll setting.

The options available for selection is given here.

• Payroll

• Payroll Interface

• Human Resources or None

For some countries or territories, the options available for selection may be restricted.

Setting the country extension to Payroll ensures that all payroll features function correctly. The other product settings
you select control the functions of payroll-related features when you aren't using Global Payroll.

Payroll
The implications of setting the country extension to Payroll are as given here.

• When creating elements, the element templates generate formulas and other associated items that are required

for costing or payment processing in Global Payroll.

• The new-hire process includes country-specific features, such as automatic generation of calculation cards for

statutory deductions and validation of address formats.

• Payroll definitions require associated organization payment methods. You must select payment methods that

include a payment source.

• Defining payment sources requires source banks in Oracle Fusion Financials.

Payroll Interface
The implications of setting the country extension to Payroll Interface is as given here.

• The element templates for creating regular and supplemental earnings elements generate associated objects,
such as input values, formulas, and balances. These objects are required for including employee data in the
Calculate Gross Earnings process.

16

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

For all other elements, the simplified element templates create only the element and no associated objects.

• The new hire process includes country-specific validations.

• Validations on payroll objects are less restrictive to support sending employee bank information as follows:

◦ No requirement for payment sources in organization payment methods
◦ No dependency on source banks in Financials

Human Resources or None
The implications of setting the country extension to Human Resources or None is as given here.

• The element templates for creating standard earnings, supplemental earnings, direct payments, and taxable
benefits elements with flat amount calculation rule generates the element definition and three input values,
such as amount, periodicity and full time equivalent. This template for percentage calculation rule generates
percentage input value and factor input value for factor calculation rule. It doesn't generate any other objects,
such as fast formulas and balances.

• The element templates for creating the other elements generates only the elements and not the associated

objects, such as input values, formulas, or balances.

You can configure these elements to meet your specific business requirements, such as adding input values
and formulas to a compensation element.

• Certain countries or territories have additional country-specific validation.

• Validations on payroll objects are less restrictive, as with the Payroll Interface setting.

Select Country Extensions
This example demonstrates how to configure payroll-related features for countries and territories in an enterprise.

The Vision enterprise has employees in several countries with different payroll arrangements:

•

•

•

In the United States and United Kingdom, the enterprise pays employees using Oracle Fusion Global Payroll.

In France, the enterprise extracts and sends payroll-related data to third-party payroll provider using Payroll
Interface extract definitions.

In China, the enterprise stores only HR data in Oracle Fusion Applications and doesn't require any data for
payroll purposes.

The following table summarizes the key decisions to consider while deciding on the product usage for a country.

Decisions to Consider

In This Example

Do your plans include processing payrolls
within Oracle Fusion for any country?

Yes, using Global Payroll in the US and UK

Do your plans include extracting or
transferring payroll-related data to a third-
party provider for any country?

Yes, using Payroll Interface extracts in France

Do your plans include processing only HR
details?

Yes, using Global HR in China

17

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Decisions to Consider

In This Example

How to Set the Extension

1. Select the Features by Country or Territory task from My Client Groups > Show More > Payroll.
In the Selected Extension list, select the country extension for the countries as shown in this table.
2.

The following table lists the country names and the product usage that you can select for this scenario.

Country

Extension

United States

United Kingdom

France

China

Payroll

Payroll

Payroll Interface

Human Resources or None

3. Click Save, and then click Done.

Related Topics

• Change Address Style and Address Validation Settings

Geographies, Address Styles, and Country Extensions
To implement payroll, you must first understand payroll feature choices and concepts. You can then plan your payroll
implementation using the Functional Setup Manager. Functional Setup Manager enables rapid and efficient planning,
configuration, implementation, deployment, and ongoing maintenance of the application through administration.

Payroll Feature Choices
As part of feature choices for payroll processing you:

• Select the correct country extension setting for each of your countries and territories on the Features by

Country or Territory page. The country extension setting ensures that certain payroll-related features, such as
element templates, work correctly in your implementation.

• Select the Payroll Costing Options to cost your payroll and the appropriate subledger accounting rules.

• Select the appropriate precision for the currency of each country or territory where you're processing payroll.

• Set the currency of each country or territory where you're sending payroll data to a third-party payroll provider.
However, don't select that country or territory as a feature choice. Select the Payroll Interface extension on the
Features by Country or Territory page.

18

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Geography Structures
You can use the geography structure to define geography types for a country and then relate the geography types.

For example, you can define geography types called State, City, and Postal Code. Then you can rank the State
geography type as the highest level within the country, the City as the second level, and the Postal Code as the lowest
level within the country structure.

A geography structure is a hierarchical grouping of geography types for a country. The following table describes the
geography structure for the United States.

Level

1

2

Geography Type

State

County

19

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Level

Geography Type

3

4

City

Postal Code

Geography Validations
After defining the geography hierarchy, you need to specify the structure for the country.

You can choose which address style format you would like to use for the country, and for each selected address style
format you can map geography types to address attributes. You can also select which geography types to include in
address validation or tax validation, and which geography types will display in a list of values during address entry in
other user interfaces. The geography validation level for the country, such as error or warning, can also be selected.
Geography validation determines the geography mapping and validation for a country's address styles, and the overall
address validation control for a country.

The No Styles Format address style format is the default address style format for a country. By defining the mapping
and validation for this format you will ensure that validations can be performed for any address in the country. After the
No Styles Format is defined you can set up additional mapping for specific address styles.

For each address style format, you can define the following:

• Map to attribute

• Enable list of values

• Tax validation

• Address validation

• Address validation control

Attribute Mapping
For every address style format, you can map each geography type to an address attribute. For example, you can
map the State geography type to the State address attribute for the United States, or map the State geography type
to the County address attribute for the United Kingdom. The geography types that appear are based on how the
country structure is defined. The list of address attributes that appear are based on address formats delivered with the
application, or your customer defined address formats.

Note:  You only need to map geography types that you want to use for address or tax validation purposes.

20

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

21

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Enable List of Values
Once a geography type is mapped to an attribute, then you can specify whether the geography type will appear in a
list of values during address entry in user interfaces. It is very important to review carefully if you want to enable a list
of values. You should only enable a list of values if you have sufficient geography data imported or created for that
geography. If the setup for master geography data is incomplete, then the geography data is either not imported or
created. As a result, the list of values for the address attribute doesn't list any geography data.

Once you have enabled a list of values for an address attribute, you can only select the geography data available for the
geography type. This means that if a specific geography value isn't available in the geography hierarchy, you can't create
an address with a different geography value.

Note:  Enable List of Values applies to the UI only. It doesn't apply to import, web services, or REST APIs. For these, all
of the required geography types must have a value in the request when creating or updating an address.

Tax Validation
You can also specify whether a geography type will be included in tax validation. For example, for the United States
North America address style format you specify that County, State, and City are used for tax validation. This will mean
that when a transaction involves an address with the North America address style, the address must have the correct
county, state, and city combination based on the geography hierarchy data, to be considered valid for tax calculation.

Address Validation
You must set up address validation for those geography elements that you plan to use in your application. Address
validation checks whether geography elements of an address such as state, city, postal code, and so on are valid as per
master geography data. Setting up validation also helps ensure that the addresses are correct and deliverable during
entry. You can select states or other address elements from lists to ensure accuracy during entry. For example, when
you enter a postal code, the application can validate if the postal code exists. Note that address validation isn’t the same
as address verification. Address Verification updates and enhances your address. Address verification depends upon
Oracle or any third-party address verification services to perform verification.

You can specify whether a geography type will be included in address validation. For example, when the user enters a
United States address using the North American address style format, the address must have the correct country, state,
and postal code combination based on geography hierarchy data to be considered geographically valid.

If an address element is mapped to a geography type, but not selected for geography validation usage, then during
address entry suggested values are provided for the address element, but the address element isn't validated.

You need to verify that the default mapping between Geography Type and Map to Attribute is valid in the Geography
Mapping and Validation region and update it if required when you define geography validation.

After setting geography validation, all features that directly and indirectly depend upon geographies are impacted. For
example, multiple applications such as ERP, CX, and SCM that use geographies are impacted.

Oracle recommends that you use the following valid mapping for the countries that Loqate supports:

Country Name

Country Code

Geography Type

Map to Attribute

Andorra

AD

• Country
• Parroqia
• Settlement

• Country
• State
• City

22

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Country Name

Country Code

Geography Type

Map to Attribute

• Postal Code

• Postal code

Angola

AO

Argentina

AR

Australia

Austria

AU

AT

Belgium

BE

Bolivia

BO

Bosnia and Herzegovina

BA

• Country
• Provincia
• Municipio
• Comuna
• Localidad

• Country
• Province
• Department
• Municipality
• Postal Code

• Country
• State
• City
• Postal Code

• Country
• Bundensland
• Bezirk
• Gemeinde
• Postal Code

• Country
• Gewest
• Provincie
• Gemeente
• Postal Code

• Country
• Departmento
• Provincia
• Canton

• Country
• District
• Kanton
• Opcine

• Country
• Province
• County
• City
• Additional address

attribute 2

• Country
• Province
• County
• City
• Postal code

• Country
• State
• City
• Postal code

• Country
• State
• County
• City
• Postal code

• Country
• Additional address

attribute 1

• Province
• City
• Postal code

• Country
• Additional address

attribute 1

• Province
• City

• Country
• Additional address

attribute 1

• Province
• County

23

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Country Name

Country Code

Geography Type

Map to Attribute

Brazil

Bulgaria

BR

BG

Canada

CA

Cayman Islands

KY

Chile

China

CL

CN

Note:
China geography structure is
supported but geocoding isn't
supported.

Croatia

HR

• Nasalje
• Postal Code

• Country
• State
• City
• Postal Code

• Country
• Oblast
• Obshhina
• Settlement
• Postal Code

• Country
• Province
• City
• Postal Code

• Country
• Island
• District
• Postal Code

• Country
• Region
• Provincia
• Kommune
• Postal Code

• Country
• Province
• City
• Postal Code

• Country
• Zupanije
• Grad
• Postal Code

• City
• Postal code

• Country
• State
• City
• Postal code

• Country
• Additional address

attribute 1

• Province
• City
• Postal code

• Country
• Province
• City
• Postal code

• Country
• State
• City
• Postal code

• Country
• State
• County
• City
• Postal code

• Country
• Province
• City
• Postal code

• Country
• Province
• City
• Postal code

24

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Country Name

Country Code

Geography Type

Map to Attribute

Cuba

Cyprus

Czech Republic

CU

CY

CZ

Denmark

DK

Dominican Republic

DO

Ecuador

Estonia

Finland

EC

EE

FI

• Country
• Provincia
• Municipio
• City
• Postal Code

• Country
• Periochi
• Dimos
• Postal Code

• Country
• Kraj
• Okres
• Obec
• Postal Code

• Country
• Amt
• Settlement
• Postal Code

• Country
• Provincia
• Municipio
• Town
• Postal Code

• Country
• Province
• Canton
• City
• Postal Code

• Country
• Maakond
• Vald
• Postal Code

• Country
• Maakunta
• Kunta

• Country
• Province
• County
• City
• Postal code

• Country
• Province
• City
• Postal code

• Country
• State
• County
• City
• Postal code

• Country
• Province
• City
• Postal code

• Country
• Province
• County
• City
• Postal code

• Country
• Province
• County
• City
• Postal code

• Country
• State
• City
• Postal code

• Country
• State
• Locality

25

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Country Name

Country Code

Geography Type

Map to Attribute

France

FR

Germany

Great Britain

Greece

Guadalupe

Guam

DE

GB

GR

GP

GU

Guernsey

GG

• Settlement
• Postal Code

• Country
• Region
• Department
• Commune
• Postal Code

• Country
• Bundesland
• Gemeinde
• Postal Code

• Country
• County
• Township
• Postal Code

• Country
• Periferia
• Nomi
• Dimotika
• Postal Code

• Country
• Commune
• Postal Code

• Country
• State
• County
• Municipality
• Postal Code

• Country
• City
• Parishes
• Villages
• Postal Code

• City
• Postal code

• Country
• Additional address

attribute 1

• State
• City
• Postal code

• Country
• State
• City
• Postal code

• Country
• State
• City
• Postal code

• Country
• State
• County
• City
• Postal code

• Country
• City
• Postal code

• Country
• State
• County
• City
• Postal code

• Country
• City
• Additional address

attribute 2

• Additional address

attribute 3
• Postal Code

26

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Country Name

Country Code

Geography Type

Map to Attribute

Hungary

HU

Iceland

India

Indonesia

Ireland

IS

IN

ID

IE

Isles of Man

IM

Israel

Italy

IL

IT

• Country
• Megye
• Jaras
• Telepules
• Settlement
• Postal Code

• Country
• Jaras
• Telepules
• Settlement
• Postal Code

• Country
• State
• City
• Postal Code

• Country
• Province
• City
• Postal Code

• Country
• Province
• Post County
• Postal_Code

• Country
• Locality
• Settlement
• Postal Code

• Country
• District
• Subdistrict
• City
• Postal Code

• Country
• Regione

• Country
• Additional address

attribute 1

• Province
• County
• City
• Postal code

• Country
• Province
• County
• City
• Postal code

• Country
• State
• City
• Postal code

• Country
• Province
• City
• Postal code

• Country
• State
• City
• Postal Code

• Country
• City
• Additional address

attribute 2
• Postal code

• Country
• State
• County
• City
• Postal code

• Country

27

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Country Name

Country Code

Geography Type

Map to Attribute

Jamaica

Japan

Jordan

Kenya

Latvia

Liechtenstein

JM

JP

JO

KE

LV

LI

Lithuania

LT

• Provincia
• Comune
• Postal code

• Country
• Parish
• Settlement

• Country
• Prefecture
• City
• Postal Code

• Country
• Muhafazat
• Liwa
• Tajma
• Postal Code

• Country
• County
• Division

• Country
• Rajons
• Pilseta
• Postal Code

• Country
• Wahlkreis
• Gemeinde
• District
• Postal Code

• Country
• County
• Municipality
• Ward
• Postal Code

• Additional address

attribute 1

• Province
• City
• Postal code

• Country
• State
• City

• Country
• State
• City
• Postal code

• Country
• State
• County
• City
• Postal code

• Country
• State
• City

• Country
• State
• City
• Postal code

• Country
• Additional address

attribute 1

• State
• City
• Postal code

• Country
• State
• County
• City
• Postal code

28

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Country Name

Country Code

Geography Type

Map to Attribute

Luxembourg

LU

Malaysia

MY

Malta

MT

Martinique

MQ

Mexico

MX

Netherlands

NL

New Zealand

NZ

Norway

NO

• Country
• Canton
• Commune
• Settlement
• Postal Code

• Country
• State
• District
• Subdistrict
• Postal Code

• Country
• Region
• Local_Council
• Postal Code

• Country
• Department
• Arrondisement
• Commune
• Postal Code

• Country
• State
• Municipality
• Locality
• Postal Code

• Country
• Province
• Municipality
• Town
• Postal Code

• Country
• Region
• Town
• Postal Code

• Country

• Country
• State
• County
• City
• Postal code

• Country
• State
• County
• City
• Postal code

• Country
• State
• City
• Postal code

• Country
• State
• County
• City
• Postal code

• Country
• State
• County
• Additional address

attribute 2
• Postal code

• Country
• Province
• County
• City
• Postal code

• Country
• State
• City
• Postal code

• Country

29

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Country Name

Country Code

Geography Type

Map to Attribute

Oman

OM

Peru

Poland

Portugal

PE

PL

PT

Puerto Rico

PR

Qatar

Reunion Island

QA

RE

• Fylke
• Kommune
• Postal Code

• Country
• Muhafazah
• District
• City

• Country
• Region
• Provincia
• Distrito
• Postal Code

• Country
• Wojewodztwo
• Powiat
• Gmina
• Postal Code

• Country
• Distrito
• Concelho
• Settlement
• Postal Code

• Country
• Commonwealth
• Municipio
• Barrio
• Postal Code

• Country
• Municipality
• Zone

• Country
• Region
• Department
• Commune
• Postal Code

• Province
• City
• Postal code

• Country
• State
• County
• City

• Country
• Province
• County
• City
• Postal code

• Country
• Province
• County
• City
• Postal code

• Country
• Province
• County
• City
• Postal code

• Country
• State
• County
• City
• Postal code

• Country
• State
• City

• Country
• State
• County
• City
• Postal code

30

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Country Name

Country Code

Geography Type

Map to Attribute

Romania

RO

Russia

RU

San Marino

Singapore

Slovakia

SM

SG

SK

Slovenia

SI

South Africa

ZA

• Country
• Region
• County
• Settlement
• Locality
• Postal Code

• Country
• Federal_District
• Federal_Subject
• Oblast
• Postal Code

• Country
• Comune
• Postal Code

• Country
• Region
• District
• Postal Code

• Country
• Kraj
• Okres
• Obec
• Postal Code

• Country
• Regija
• Upravna Enota
• Obcina
• Settlement
• Postal Code

• Country
• Additional address

attribute 1

• Province
• County
• City
• Postal code

• Country
• Additional address

attribute 1

• State
• City
• Postal code

• Country
• State
• Postal code

• Country
• State
• City
• Postal code

• Country
• Province
• County
• City
• Postal code

• Country
• Additional address

attribute 1

• Province
• County
• City
• Postal code

• Country
• Province
• District_Municipality
• Local_Municipality

• Country
• Province
• County
• City

31

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Country Name

Country Code

Geography Type

Map to Attribute

South Korea

Spain

Sri Lanka

Swaziland

Note:
This country maybe labeled
Eswatini in Manage Territories.

Sweden

Switzerland

Taiwan

Thailand

KR

ES

LK

SZ

SE

CH

TW

TH

• Postal Code

• Country
• Jibang
• Siti
• Postal Code

• Country
• Autonomous_Community
• Province
• City
• Postal Code

• Country
• Province
• District
• Divisional_Secretariat
• Postal Code

• Country
• District
• Inkhundla
• Town
• Postal Code

• Country
• Lan
• Settlement
• Postal Code

• Country
• Kanton
• Bezirk
• Gemeinde
• Postal Code

• Country
• County
• Town
• Postal Code

• Country

• Postal code

• Country
• State
• City
• Postal code

• Country
• Additional address

attribute 1

• Province
• City
• Postal code

• Country
• Province
• County
• City
• Postal code

• Country
• Province
• County
• City
• Postal code

• Country
• Province
• City
• Postal code

• Country
• State
• County
• City
• Postal code

• Country
• State
• City
• Postal code

• Country

32

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Country Name

Country Code

Geography Type

Map to Attribute

Tunisia

Turkey

TN

TR

United Arab Emirates

AE

United States

US

Uruguay

Vatican City

Vietnam

UY

VA

VN

• Region
• Changwat
• Amphoe
• Postal Code

• Country
• Governorate
• Delegation
• Postal Code

• Country
• Sehir
• Ilce
• Kasaba
• Postal Code

• Country
• Emirate
• City
• Area
• Postal Code

• Country
• State
• County
• City
• Postal Code

• Country
• Departamento
• City
• Postal Code

• Country
• Municipal
• Settlement
• Postal Code

• Country
• Region
• Tihn

• Additional address

attribute 1

• State
• City
• Postal code

• Country
• State
• City
• Postal Code

• Country
• Province
• County
• City
• Postal code

• Country
• State
• City
• Additional address

attribute 2
• Postal Code

• Country
• State
• County
• City
• Postal code

• Country
• State
• City
• Postal code

• Country
• Province
• City
• Postal code

• Country
• Additional address

attribute 1

33

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Country Name

Country Code

Geography Type

Map to Attribute

• Quan
• Thank Pho
• Postal Code

• Province
• County
• City
• Postal code

Note:  For either the tax or address validation, don't skip any level unless you're certain that the selected geography
types can uniquely identify geographies. For example, the United States country structure is: State, County, City,
and Postal Code, and you want to select just State and Postal Code for address or tax validation. However, for the
combination of California and 94065, the city can be either Redwood Shores or Redwood City. In this case, you should
also select at least the City geography type for address or tax validation.

Address Validation Control
You can select the address validation level for a country. Validation will check if the entered address maps
to the geography hierarchy data available for the country, and the address validation control determines
whether you can save an address that didn't pass validation during address entry. For example, if the

34

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

validation level is Error, then an address can't be saved if the values don't match the geography hierarchy data.

These are the address validation levels you can choose:

• Error - only completely valid addresses can be saved, with all mandatory address elements entered.

• No Validation - all addresses can be saved including incomplete and invalid addresses.

Regardless of the result of validation, the validation process will try to map any address attribute to a geography of
the country, and store any mapping it could establish based on the available data. This is called  Geography Name
Referencing   and it's executed as part of validation. The result of this referencing is used in several business processes
in the application to map an address to a specific geography or zone. Therefore, Geography Name Referencing is
the process of validating and mapping address elements of existing location table records against master reference
geographies. For example, CA value in the STATE column of the HZ_LOCATIONS table is mapped to the master
reference geography of CA (California).

The Geography Dimension value in territories is derived from sell-to addresses of sales accounts. To use geography
dimensions in territories, you must validate the geography elements in the addresses, such as state, city, and postal

35

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

code. You can validate the address by enabling geography validation for each country using the Manage Geographies
task. Perform the following in the Manage Geographies task:

• Enable at least one level in the geography hierarchy for geography validation.

• Enable geography validation for all geography levels that you intend to use for territory definition for each

country.

•

If needed, enable a list of values containing specific geography elements. This will help users search and select
appropriate geography values during addresses entry and eliminate all possibilities of wrong address entry.

You can set geography validation control to Error in the Manage Geography Validation page. This ensures that users can
only use valid geography elements in addresses.

Note:  If you have already created addresses before setting up address validation for a country, you must enable
geography validation and then execute the Validate Geographies of Addresses Against Master Geographies task for
that country. This validates all your geography elements.

Related Topics

• How can I save an address that didn't pass geography validation?

• How do I validate geographies of addresses against master geographies and generate naming references?

• Setting Up Geography Validation

Change Address Style and Address Validation Settings
Use the Features by Country or Territory task to control address style and level of address validation for the countries or
territories you configure. The values you can set depend on the combination of the country or territory and the selected
country extension.

For example, for Canada, you can change the address style from its default value only when you set the country
extension to Human Resources or None. You can't change the address style from its default value when you set the
country extension to Payroll or Payroll Interface.

Address Styles
The address style you select determines which address attributes are available and maintained in the application. The
combination of address style and address validation determines the level of validation.

Depending on the country or territory and the country extension you select, you have one or both of the following
address style options. Each address style provides its own validation.

Address Style

What the Address Style Does

Postal Address

This address style provides the fundamental set of address attributes for a country or territory. In some
cases, this style adds supplemental attributes. For instance this address style might include general
address attributes that aren't relevant, such as State or Postal Code.

Supplemental Taxation and Reporting
Address

Enforces validation to attribute changes.

For example, this style may add specific validation of postal codes, such as requiring a specific number
of characters in a specific sequence.

36

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Use the Features by Country or Territory task to see what's delivered for your country. Each country has a default
address style and the choice of the country extension determines whether you can change the default address style.

Address Validation Based on Country Extension
Address validation is the validation of county, city, province, and postal code combinations.

Employees must have a valid address in order for them to receive their tax card and to ensure the accuracy of their tax
calculations.

Address validation is automatically enabled for some license and product extension combinations. For example, for
Canada, the default is Supplemental Taxation and Reporting Address. However, the address style and address validation
depends on the country extension, as shown in this table.

Extension

Style Enforced

Validation Enforced

Human Resources

Payroll Interface

Payroll

No

Yes

Yes

No

No

Yes

For Canada, if you have chosen to install Human Resources, the value for the Address Style can be modified to
either format. If you have chosen to install either Payroll Interface or Payroll, the value for the Address Style can't be
modified. It must be set to Supplemental Taxation and Reporting Address. Validations are implemented to enforce that
requirement.

Change Address Styles
For most of the predefined countries and territories, the application enforces the address style, preventing you from
making changes. However, when the address style isn't enforced, such as a customer-configured legislation, changing
address styles can affect validation rules. This might lead to address data integrity and validation issues.

For example, for Canada, if you initially implement Human Resources using the Postal Address style and then later
change the country extension to Payroll, you must also change the address style to Supplemental Taxation and
Reporting Address. As a result, you must update your existing address data to resolve validation errors.

Note:  The Supplemental Taxation and Reporting Address style, once selected, impacts both the Person and HCM
Locations address styles. Ensure to test any changes you make to address style or validation for a country or territory
before you implement them in a production environment.  If you provide data to a third party, such as a payroll or
benefit provider, statutory recipients, or financial institutions, you must test the changes. Changes to validation or
address styles may result in missing data or unrecognized data.

Tip:  Use the Manage Legal Addresses task to review and configure how addresses appear in the application.

Disable Address Validation
Disabling address validation disables any country-specific programmatic validation rules created for a specific country
or territory. You can disable address validation on the Features by Country or Territory page.

37

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

A country or territory might have rules defined using the Manage Geographies task for validating address structure,
format, or values. Disabling address validation doesn't have any impact on the validations you have set up on the
Manage Geographies page.

For some countries, the application prevents you from disabling the programmatic validation. For other countries and
territories, when you disable address validation, any existing validation rules for the selected address style, remains in
place.

Note:  For Canada, when Payroll is the selected country extension, you can't disable the address validation.

For example, suppose you have chosen Human Resources with address validation enabled. During data conversion, you
want to temporarily bypass address validation rules to load a batch of worker data. You can achieve this by deselecting
the Address Validation check box before loading your data. After loading the batch, if the address validation remains
disabled, any new address data you enter later, could be potentially invalid. Errors may occur in subsequent processes
and reports. As a result, you must re-enable address validation and update your existing address data to resolve
validation errors.

Enable Address Validation
To manually enable or disable address validation:

1. Search for and start the Features by Country or Territory task.
2. Select the Address Validation box.
3. Click Save and then Done.

CAUTION:  If you don't have address validation enabled, then you must take care when switching product extensions,
as any address you previously defined may be missing required values, such as county and tax district. There's also
the possibility of invalid address combinations, such as mismatched city and postal code combinations.

Legislation

Payroll Legislative Data
Use the Configure Legislations for Human Resources task in the Setup and Maintenance area to create and edit payroll
rules for countries or territories not initially provided by Oracle.

Objects you can configure include:

• Legislative rules

• Element classifications

• Valid payment types

• Component groups

• Balance dimensions

• Legislative data groups

Legislative Rules
Legislative rules govern how to manage employee records when you rehire employees into your organization. For
example, for some countries, a rehire continues to be associated with the earlier payroll relationship, thereby having

38

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

access to prior data, such as year-to-date balances. For some other countries, a rehire creates a new payroll relationship
record with no access to prior data. The statutory rules for your country or territory determines the selections you make,
such as the starting month of the tax year.

The legislative rules you can configure include mappings between system person types and payroll relationship types.
This mapping controls which person types you can include in payroll calculation processing, such as the Calculate Gross
Earnings process.

Note:  You can't undo payroll relationship type mapping. If you select an element entries only option for a person type
and then at a later date decide to use the Calculate Gross Earnings process, the process won't generate results for that
person type. Consider using a standard option to provide more flexibility.

Element Classifications
Element classifications are collections of related elements. You select the primary classifications you want to include
for your elements. You can provide new display names for element classifications to match the terminology that's most
appropriate for your country or territory.

Valid Payment Types
Payment types are the means by which you issue payments to workers. The predefined payment types are Check, Cash,
EFT (electronic funds transfer), and International Transfer. You can provide new display names for payment types to
match terminology that's most appropriate for your country or territory.

Component Groups
Component groups are logical sets of payroll components, which are the rates and rules that determine calculated
values for some earnings and deduction elements. You can provide new display names for the component groups you
want to support to match terminology that's most appropriate for your country or territory.

The Configure Legislations for Human Resources task creates a calculation card definition and payroll components for
each component group you enable. When you create elements in certain classifications and categories, the element
template associates the element with a payroll component and creates calculation components that you can add to
workers' calculation cards. The calculation card creates the components for the component groups you selected. The
element template then associates these components with the statutory elements you create. Ensure that you associate
these components with your employees through element eligibility for calculation to be processed.

Depending on the legislative rules, if you enable the Federal or Social Insurance component groups and set your
country extension on the Features by Country or Territory page to Payroll or Payroll Interface for your country or
territory, hiring workers automatically creates a statutory deduction calculation card for them. Ensure that you create
eligibility records for your statutory deduction elements before hiring any workers.

Balance Dimensions
Balance dimensions identify the specific value of a balance at a particular point in time, based on a combination of
criteria, including time, employee relationship level, jurisdiction, and tax reporting unit. You can provide new display
names for the balance dimensions you want to support to match terminology that's appropriate for your country or
territory.

The Configure Legislations for Human Resources task creates some predefined balances that the application uses
within the statement of earnings, such as Gross Earnings and Net Pay. Additionally, the Net Payment balance is required
to set up organization payment methods.

39

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Legislative Data Groups
Use the Manage Legislative Data Groups task in the Setup and Maintenance area to define at least one legislative data
group for each country or territory where your enterprise operates.

Related Topics

• Legislative Data Groups

Configure Legislations
Create the legislative content for a country or territory in the Setup and Maintenance area as part of implementing
Oracle Human Resources. The Installed Legislations page shows which country extensions are predefined or already
implemented or both.

This procedure outlines the steps required to configure a legislation that isn't predefined by Oracle.

When you first configure a legislation, the flow guides you through a series of setup steps for the objects necessary to
set up elements, balances, and other payroll-related data for implementations. The objects you can configure include:

• Legislative Rules

• Element Classifications

• Payment Types

• Component Groups

• Balance Dimensions

Set Legislative Rules
Legislative rules govern default values and how to manage employee records in your organization. Base your selections
on the statutory rules for your country or territory.

1.

In the Setup and Maintenance area, go to the Configure Legislations for Human Resources task.

Note:  Use the Configure Payroll Legislations task if you're implementing Global Payroll.

2. Select the country or territory from the list on the Installed Legislations page.
3. Select Legislative Rules from the left-pane and click Edit.
4. Select the month and day of the typical tax year. For example, 01 for January and 01 for the first day of the

month.

5. Select the currency to use by default for this country or territory.
6. Select a payroll relationship rule. This value determines how employment records are created when employees

are hired or rehired.

7. Review the mapping of the predefined system person types to payroll relationship types. Select appropriate

values for your country or territory.

8. Click Save.

Note:  You can't undo payroll relationship type mapping. If you select an 'element entries only' option for a
person type and decide at a later date to use a payroll calculation process, such as Calculate Gross Earnings,
the process won't generate results for that person type. If you're certain that you won't perform any type of
payroll calculation, you can select an element entries only option. Selecting a standard option provides more
flexibility.

40

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Select Objects and Modify Display Names
The flow guides you through selecting primary classifications you want to include for your elements, payment types,
balance dimensions, and component groups. For each of these objects, you can provide new display names to match
the terminology that's most appropriate for your country or territory.

1. Select Element Classifications from the left pane and click Edit. Select the primary classifications you want to

include for your elements.

2. For each primary classification you select, optionally edit the value in the Display Name column, and then click

Next.

3. Select the payment types to include, such as Check/Cheque and EFT (electronic funds transfer).

The payment types you select here are available when you create organization payment methods for your
country or territory.

4. For each payment type you select, optionally edit the value in the Display Name column, and then click Next.
5. Select the component groups to include.
6. For each component group you select, optionally edit the value in the Display Name column, and then click

Next.

7. Add any balance definitions as needed that aren't already selected. The page displays all balance dimensions

available for your country or territory.

8. For each selected balance definition, optionally edit the value in the Display Name column.
9. Click Submit.

How Legislations are Edited
If you have configured legislative content for a country or territory not already predefined by Oracle, you can edit it
using the Configure Legislations for Human Resource task.

Your ability to edit the legislative rules and objects depends on the other objects in the legislation.

Legislative Rules and Objects You Can't Edit or Delete
The following tables summarize the restrictions when you're editing legislative content for a country or territory.

Legislative Rule

Restriction

Tax Year Start Date

Can't change after running a payroll process

Currency

Can't change after initial configuration because it would impact generated balances

Payroll Relationship Type Mapping

Can change, but affects only future person records, not existing person records

Object

Restriction

Element Classification

Can't delete if you have created an element of that primary classification

Payment Type

Can't delete if you have created payment methods for that payment type

Component Group

Can't delete if you have created calculation cards for that component group

41

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Object

Restriction

Balance Dimension

Can't delete if you have created balances with that dimension

Enterprise Structures

Enterprise Structures Overview
Oracle Fusion Applications have been designed to ensure your enterprise can be modeled to meet legal and
management objectives.

The decisions about your implementation of Oracle Fusion Applications are affected by your:

•

Industry

• Business unit requirements for autonomy

• Business and accounting policies

• Business functions performed by business units and optionally, centralized in shared service centers

• Locations of facilities

Every enterprise has three fundamental structures that describe its operations and provide a basis for reporting.

• Legal

• Managerial

• Functional

In Oracle Fusion, these structures are implemented using the chart of accounts and organization hierarchies. Many
alternative hierarchies can be implemented and used for reporting. You are likely to have one primary structure that
organizes your business into:

• Divisions

• Business Units

• Departments

Align these structures with your strategic objectives.

This figure illustrates a grid with Business Axis, representing the enterprise division, Legal Axis representing the
companies, and the Functional Axis representing the business functions.

42

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Legal Structure
The figure illustrates a typical group of legal entities, operating various business and functional organizations. Your
ability to buy and sell, own, and employ comes from your charter in the legal system. A corporation is:

• A distinct legal entity from its owners and managers.

• Owned by its shareholders, who may be individuals or other corporations.

Many other kinds of legal entities exist, such as sole proprietorships, partnerships, and government agencies.

A legally recognized entity can own and trade assets and employ people in the jurisdiction in which the entity is
registered. When granted these privileges, legal entities are also assigned responsibilities to:

• Account for themselves to the public through statutory and external reporting.

43

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

• Comply with legislation and regulations.

• Pay income and transaction taxes.

Chapter 1
Let’s Get Started

• Process value added tax (VAT) collection on behalf of the taxing authority.

Many large enterprises isolate risk and optimize taxes by incorporating subsidiaries. They create legal entities to
facilitate legal compliance, segregate operations, optimize taxes, complete contractual relationships, and isolate risk.
Enterprises use legal entities to establish their enterprise's identity within the laws of each country in which their
enterprise operates.

The figure illustrates:

• A separate card represents a series of registered companies.

• Each company, including the public holding company, InFusion America, must be registered in the countries

where they do business.

• Each company contributes to various divisions created for purposes of management reporting. These are

shown as vertical columns on each card.

For example, a group might have a separate company for each business in the United States (US), but have its United
Kingdom (UK) legal entity represent all businesses in that country.

The divisions are linked across the cards so that a business can appear on some or all of the cards. For example, the
air quality monitoring systems business might be operated by the US, UK, and France companies. The list of business
divisions is on the Business Axis.

Each company's card is also horizontally striped by functional groups, such as the sales team and the finance team.
This functional list is called the Functional Axis. The overall image suggests that information might, at a minimum, be
tracked by company, business, division, and function in a group environment. In Oracle Fusion Applications, the legal
structure is implemented using legal entities.

Management Structure
Successfully managing multiple businesses requires that you segregate them by their strategic objectives, and measure
their results. Although related to your legal structure, the business organizational hierarchies don't have to be reflected
directly in the legal structure of the enterprise. The management structure can include divisions, subdivisions, lines
of business, strategic business units, profit, and cost centers. In the figure, the management structure is shown on the
Business Axis. In Oracle Fusion Applications, the management structure is implemented using divisions and business
units as well as being reflected in the chart of accounts.

Functional Structure
Straddling the legal and business organizations is a functional organization structured around people and their
competencies. For example, sales, manufacturing, and service teams are functional organizations. This functional
structure is represented by the Functional Axis in the figure. You reflect the efforts and expenses of your functional
organizations directly on the income statement. Organizations must manage and report revenues, cost of sales, and
functional expenses such as research and development and selling, general, and administrative expenses. In Oracle
Fusion Applications, the functional structure is implemented using departments and organizations, including sales,
marketing, project, cost, and inventory organizations.

Legislative Data Groups
Legislative data groups are a means of partitioning payroll and related data. At least one legislative data group is
required for each country where the enterprise operates.

44

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Each legislative data group is associated with one or more payroll statutory units. Each payroll statutory unit can belong
to only one legislative data group.

Payroll-related information, such as elements, is organized by legislative data group. Each legislative data group:

• Marks a legislation in which payroll is processed.

•

•

Is associated with a legislative code, currency, and its own cost allocation key flexfield structure.

Is a boundary that can share the same set up and still comply with the local laws.

• Can span many jurisdictions as long as they're within one country.

• Can contain many legal entities that act as payroll statutory units.

Payroll Employment Hierarchy Profile Options
You can use profile options to specify the values that you want to display for each payroll employment hierarchy level.
You can specify up to three values at each level to help identify the record.

For example, you can select payroll relationship type and payroll relationship number to identify payroll relationship
records that you will see in the payroll relationship switcher on the Payment Methods page.

Depending on the employment model used in your enterprise, you can use these levels to set up your payroll
employment hierarchy:

• Payroll relationship

• Assignments

To define profile option settings and values, select the Payroll Employment Hierarchy Profile Option Values.

Profile Options for the Payroll Relationship Level
This table lists the profile option codes and available profile values at the site level for the payroll relationship level of the
payroll employment hierarchy.

Profile Option Codes

Profile Values

PAY_EMP_HIERARCHY_REL_DESC_1

Payroll Relationship Number

PAY_EMP_HIERARCHY_REL_DESC_2

Payroll Statutory Unit Name

PAY_EMP_HIERARCHY_REL_DESC_3

Payroll Relationship Type

Profile Options for the Assignment Level
This table lists the profile option codes and available profile values at the site level for the assignment level of the payroll
employment hierarchy.

Profile Option Codes

Profile Values

PAY_EMP_HIERARCHY_ASG_DESC_1

Assignment Name

PAY_EMP_HIERARCHY_ASG_DESC_2

Assignment Number

PAY_EMP_HIERARCHY_ASG_DESC_3

Employment Category

45

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Profile Option Codes

Profile Values

Grade Name

Job Name

Legal Employer Name

Location Name

Position Name

Override Site-level Values with User-level Values
You can override site-level values at the user level. For example, you might use position as the default value. Override
the default value with job for the payroll administrator who manages records for a group of workers who aren't assigned
to positions.

Related Topics

• Overview of Implementing Payroll Relationship

Examples of HCM Organization Models for Payroll
Use these examples to understand different models for human capital management (HCM) organizations that include a
legislative data group (LDG). These examples include LDGs, which aren't an organization classification, to show how to
partition payroll data by associating them with a payroll statutory unit.

Simple Configuration
This example illustrates a simple configuration that doesn't include any tax reporting unit.

Note the following:

• The legal employer and payroll statutory units are the same, sharing the same boundaries.

• Reporting can only be done at a single level. Countries such as Saudi Arabia and the United Arab Emirates

(UAE) might use this type of model, as these countries report at the legal entity level.

46

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

This figure illustrates a simple configuration where the enterprise has only one legal entity, which is both a payroll

statutory unit and a legal employer.

Multiple Legal Employers and Tax Reporting Units
This example illustrates a more complex configuration. In this enterprise, you define one legal entity, InFusion US, as
a payroll statutory unit with two separate legal entities, which are also legal employers. This model shows multiple
legal employers that are associated with a single payroll statutory unit. Tax reporting units are always associated with a
specific legal employer (or employers) through the payroll statutory unit.

The implication is that payroll statutory reporting boundaries vary from human resources (HR) management, and you
can categorize the balances separately by one of the following:

• Payroll statutory unit

• Legal employer

• Tax reporting unit

This configuration is based on tax filing requirements, as some tax-related payments and reports are associated with a
higher level than employers. An example of a country that might use this model is the US.

47

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

This figure illustrates an enterprise that has one payroll statutory unit and multiple legal employers and tax reporting

units.

One Payroll Statutory Unit and Two Tax Reporting Units
This model makes no distinction between a legal employer and a payroll statutory unit. You define tax reporting units as
subsidiaries to the legal entity.

In this enterprise, legal entity is the highest level of aggregation for payroll calculations and reporting. Statutory
reporting boundaries are the same for both payroll and HR management. An example of a country that might use this
model is France.

48

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

This figure illustrates an example of an organization with one legal entity. The legal entity
is both a legal employer and a payroll statutory unit and has two tax reporting units.

One Payroll Statutory Unit with Several Tax Reporting Units
In this model, the enterprise has one legal entity. Legal employers and tax reporting units are independent from each
other within a payroll statutory unit, because there is no relationship from a legal perspective. Therefore, you can run
reporting on both entities independently.

Using this model, you wouldn't typically:

• Report on tax reporting unit balances within a legal employer

• Categorize balances by either or both organizations, as required

An example of a country that might use this model is India.

49

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

This figure illustrates an enterprise with one legal entity that's a payroll statutory unit
and a legal employer. The tax reporting units are independent from the legal employer.

Multiple Payroll Statutory Units with Several Tax Reporting Units
In this model, the enterprise has two legal entities. The legal employers and tax reporting units are independent from
each other within a payroll statutory unit, because there is no relationship from a legal perspective. Therefore, you can
run reporting on both entities independently.

Using this model, you wouldn't typically:

• Report on tax reporting unit balances within a legal employer

• Categorize balances by either or both organizations, as required

An example of a country that might use this model is the United Kingdom (UK).

50

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

This figure illustrates an enterprise with two legal entities, and legal employers and tax reporting units are independent

from each other.

What's a legal employer?
A legal employer is a legal entity that employs workers. You define a legal entity as a legal employer in the Oracle Fusion
Legal Entity Configurator.

The legal employer is captured at the work relationship level, and all assignments within that relationship are
automatically with that legal employer. Legal employer information for worker assignments is also used for reporting
purposes.

51

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

What's a payroll statutory unit?
Payroll statutory units are legal entities that are responsible for paying workers, including the payment of payroll tax and
social insurance.

A payroll statutory unit can pay and report on payroll tax and social insurance on behalf of one or many legal entities,
depending on the structure of your enterprise. For example, if you're a multinational, multiple company enterprise,
then you register a payroll statutory unit in each country where you employ and pay people. You can optionally register
a consolidated payroll statutory unit to pay and report on workers across multiple legal employers within the same
country. You associate a legislative data group with a payroll statutory unit to provide the correct payroll information for
workers.

What's a tax reporting unit?
Use a tax reporting unit to group workers for the purpose of tax and social insurance reporting. A tax reporting unit is
the Oracle Fusion Human Capital Management (HCM) version of the legal reporting unit in Oracle Fusion Applications.

To create a tax reporting unit, you use the Oracle Fusion Legal Entity Configurator to define a legal entity as a payroll
statutory unit. When you identify a legal entity as a payroll statutory unit, the application transfers the legal reporting
units that are associated with that legal entity to Oracle Fusion HCM as tax reporting units. You can then access the tax
reporting unit using the Manage Legal Reporting Unit HCM Information task.

If you identify a legal entity as a legal employer, and not as a payroll statutory unit, you must enter a parent payroll
statutory unit. The resulting legal reporting units are transferred to Oracle Fusion HCM as tax reporting units, but as
children of the parent payroll statutory unit that you entered, and not the legal entity that you identified as a legal
employer.

Legal Entities

Legal Entities Overview
A legal entity is a recognized party with rights and responsibilities given by legislation.

Legal entities have the following rights and responsibilities to:

• Own property

• Trade

• Repay debt

• Account for themselves to regulators, taxation authorities, and owners according to rules specified in the

relevant legislation

Their rights and responsibilities may be enforced through the judicial system. Define a legal entity for each registered
company or other entity recognized in law for which you want to record assets, liabilities, expenses and income, pay
transaction taxes, or perform intercompany trading.

A legal entity has responsibility for elements of your enterprise for the following reasons:

• Facilitating local compliance

• Minimizing the enterprise's tax liability

• Preparing for acquisitions or disposals of parts of the enterprise

52

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

•

Isolating one area of the business from risks in another area. For example, your enterprise develops property
and also leases properties. You could operate the property development business as a separate legal entity to
limit risk to your leasing business.

The Role of Your Legal Entities
In configuring your enterprise structure in Oracle Fusion Cloud Applications, the contracting party on any transaction is
always the legal entity. Individual legal entities:

• Own the assets of the enterprise

• Record sales and pay taxes on those sales

• Make purchases and incur expenses

• Perform other transactions

Legal entities must comply with the regulations of jurisdictions, in which they register. Europe now allows for companies
to register in one member country and do business in all member countries, and the US allows for companies to register
in one state and do business in all states. To support local reporting requirements, legal reporting units are created and
registered.

You are required to publish specific and periodic disclosures of your legal entities' operations based on different
jurisdictions' requirements. Certain annual or more frequent accounting reports are referred to as statutory or external
reporting. These reports must be filed with specified national and regulatory authorities. For example, in the United
States (US), your publicly owned entities (corporations) are required to file quarterly and annual reports, as well as other
periodic reports, with the Securities and Exchange Commission (SEC), which enforces statutory reporting requirements
for public corporations.

Individual entities privately held or held by public companies don't have to file separately. In other countries, your
individual entities do have to file in their own name, as well as at the public group level. Disclosure requirements are
diverse. For example, your local entities may have to file locally to comply with local regulations in a local currency, as
well as being included in your enterprise's reporting requirements in different currency.

A legal entity can represent all or part of your enterprise's management framework. For example, if you operate in a
large country such as the United Kingdom or Germany, you might incorporate each division in the country as a separate
legal entity. In a smaller country, for example Austria, you might use a single legal entity to host all of your business
operations across divisions.

Plan Legal Reporting Units
Each of your legal entities has at least one legal reporting unit. Some legal reporting units can also be referred to as
establishments. You can define either domestic or foreign establishments.

Define legal reporting units by physical location, such as sales offices. For example, set up legal reporting units to
represent your company and its offices for tax reporting.

Planning Legal Reporting Units
Plan and define your legal reporting units at both the local and national levels if you operate within the administrative
boundaries of a jurisdiction that's more granular than country. For example, your legal entity establishes operations in
a country that requires reporting of employment and sales taxes locally as well as nationally. Therefore, you need more
than one legally registered location to meet this legal entity's reporting requirements in each area. Additionally, legal
entities in Europe operate across national boundaries, and require you to set up legal reporting units for the purposes
of local registration in each country. There can be multiple registrations associated with a legal reporting unit. However,
only one identifying registration can be defined by the legal authority used for the legal entity or legal reporting unit
and associated with the legal reporting unit.

53

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Legal Entities for Global Payroll
A legal entity is an entity unequivocally identified and given rights and responsibilities under commercial law, through
registration with the territory's appropriate authority.

A legal entity can legally:

• Own property

• Trade

• Repay debt

• Account for themselves to company regulators, taxation authorities, and owners according to rules specified in
the relevant legislation (as performed through balance sheets, income statements, specified reports, and so on)

The judicial system may enforce its rights and responsibilities.

For your enterprise, a legal entity may help you with:

• Facilitating local compliance

• Minimizing your tax liability

• Preparing for acquisitions or disposals of parts of the enterprise

•

Isolating one area of the business from risks in another area

For example, your enterprise develops property and also leases properties. You could operate the property
development business as a separate legal entity to limit risk to your leasing business.

There are no predefined legal entities. You must create all legal entities that apply to the enterprise you're setting up.
Use the Legal Entity HCM Information task from your implementation project.

There are several things you need to consider when you define your legal entities.

• What roles will they play

• What types of legal entities do you need

• What registrations will they require

• Does your organization support any retirees

• How to configure them for your HR reports

Roles of Legal Entities
In configuring your enterprise structure, the contracting party on any transaction is always the legal entity. Individual
legal entities:

• Own the assets of the enterprise

• Record sales and pay taxes on those sales

• Make purchases and incur expenses

• Perform other transactions

Legal entities must comply with the regulations of their registering jurisdictions.

To support local reporting requirements, you create and register legal reporting units (LRUs) within a legal entity.

54

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

You're required to publish specific and periodic disclosures of your legal entities' operations based on the different
jurisdictions' requirements. Certain annual or more frequent accounting reports are referred to as statutory or external
reporting. You must file these reports with the specified national and regulatory authorities.

For example, your publicly owned entities (corporations) are required to file quarterly and annual reports, as well
as other periodic reports, with the Securities and Exchange Commission (SEC), which enforces statutory reporting
requirements for public corporations. Individual entities privately held or held by public companies don't have to file
separately.

Disclosure requirements are diverse. For example, your local entities may have to file locally to comply with local
regulations in US dollars, as well as being included in your enterprise's reporting requirements in different currency.

A legal entity can represent all or part of your enterprise's management framework.

Types of Legal Entities
There are two types of legal entities.

This kind

Does this

Legal employer

A legal entity that employs workers.

Payroll statutory unit (PSU)

A legal entity responsible for paying workers, including the payment of payroll tax and social insurance.
A PSU can pay and report on payroll tax and social insurance on behalf of one or many legal entities.
That choice depends on the structure of your enterprise.

When defining a legal entity, consider how you're going to use it.

•

•

If you're using the legal entity in an HCM context, designate it as a legal employer. All workers must be assigned
to a legal employer.

If you're using it in a payroll context, designate it as a PSU for payroll processing and tax reporting.
Limit your organization to one PSU for employees and one for retirees. This helps you:

◦ Control how the payroll process calculates limit taxes.
◦ Control overtime calculations between multiple TRUs.
◦ Track deferred compensation contribution limits.

For further info, see Contribution Limits for Deferred Compensation Plans in the Help Center.

◦ Issue pension payments to retirees.

• You can define a legal entity that's both a legal employer and a PSU.

• To group multiple legal employers together for tax reporting purposes, assign them to the same parent PSU. If

your legal employers represent different companies, assign them to separate PSUs.

There are no predefined legal entities. You must create all legal entities that apply to your enterprise.

Registrations
When you create a legal entity, it automatically establishes a registration with the identifying jurisdiction. For each
employer, create a registration for tax jurisdiction and specify its unique identifying number. If the legal entity has an
LRU that interacts with other legal authorities, create additional registrations as appropriate.

55

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Note:  Capture the unique identifying number, registered name, and other details using the Legal Reporting Unit
Registrations task.

If you don't define the registration, some payroll processes may not function properly.

Configuration for Retirees
If your organization includes retirees:

1. Define separate PSUs for employees and retirees. Do not assign both employees and retirees to the same PSUs

or to the same legal employers.

2. Designate these PSUs with the 2-Tier - Multiple Assignment employment model.
3. When you set up a tax reporting unit (TRU) for a retiree, specify the distribution code that it. Set up a separate

TRU for each distribution code you require.

Additional Reporting Info
When defining a legal entity, use the Legal Entity HCM Information task from your implementation project. Provide
additional info required for HR reporting.

If the legal entity is also a PSU, specify:

• Fiscal year start

• Any additional info to support electronic year-end filings
These settings apply to all LRUs attached to the PSU.

Related Topics

• Define Legal Entities for Global Payroll

How Legal Employers Work with Payroll Statutory Units and Tax Reporting Units
You can designate legal entities as legal employers and payroll statutory units, which makes them available for use in
Oracle Fusion Human Capital Management (HCM).

You can have only one legal entity that's also a payroll statutory unit and legal employer, or multiple legal entities,
payroll statutory units and legal employers. Payroll statutory units and tax reporting units share a parent child
relationship with the payroll statutory unit being a parent of a tax reporting unit

Legal Employers and Payroll Statutory Units
You can designate payroll statutory units to group legal employers to do statutory calculations at a higher level. For
example, you can use payroll statutory units for court orders, or to calculate the United Kingdom (UK) statutory sick pay.
A legal employer can exist independently of an enterprise or be a part of a payroll statutory unit. There can be many
legal employers belonging to a payroll statutory unit, but a legal employer can belong only to one payroll statutory unit.

Legal Employers and Tax Reporting Units
Tax reporting units are indirectly associated with a legal employer through the payroll statutory unit. One or more
tax reporting units can be used by a single legal employer, and a tax reporting unit can be used by one or more legal
employers.

For example, if a single tax reporting unit is linked to a payroll statutory unit and two legal employers are associated with
this payroll statutory unit, then both legal employers are associated with the tax reporting unit. Use the Manage Legal
Reporting Unit HCM Information task to designate an existing legal reporting unit as a tax reporting unit. You need to

56

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

select a parent payroll statutory unit when you create a legal reporting unit belonging to a legal employer (that isn't a
payroll statutory unit as well). Next, you need to designate the legal reporting unit as a tax reporting unit and select the
legal employer.

Related Topics

• Overview

• What's a legal employer?

• What's a payroll statutory unit?

• What's a tax reporting unit?

• Examples of HCM Organization Models

Define Legal Entities for Global Payroll
To add a legal entity to your organization, you first define it using the Legal Entities task in your implementation project.
You define separate legal entities for employees and retirees.

Defining legal entities includes doing the following.

Want you want to do

How you do it

Before you begin

Make sure you have:

1. Defined the legal address for your enterprise using the Legal Addresses task.
2. Set up your legislative data group (LDG) using the Legislative Data Groups task.

Or, it's automatically created when you define your first legal entity.

Create your legal entities

Use the Legal Entities task.

•

•

If you're using the legal entity in an HCM context, designate it as a legal employer. HCM
implementations require legal employers.

If you're using it in a payroll context, designate it as a payroll statutory unit (PSU) for payroll
processing and tax reporting.

Limit your organization to one PSU for employees and one for retirees. This helps you:

◦ Control how the payroll process calculates limit taxes.
◦ Control overtime calculations between multiple TRUs.
◦ Track deferred compensation contribution limits.

For further info, see Contribution Limits for Deferred Compensation Plans in the Help Center.

◦ Issue pension payments to retirees.
• You can define a legal entity that's both a legal employer and a PSU.

• To group multiple legal employers together for tax reporting purposes, assign them to the same

parent PSU. If your legal employers represent different companies, assign them to separate PSUs.

There are no predefined legal entities. You must create all legal entities that apply to your enterprise.

Confirm the LDG

Confirm the correct LDG is associated with your PSUs.

57

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Want you want to do

How you do it

Configure your legal entities for HR
reporting and payroll processing

After creating the legal entities, use the Legal Entity HCM Information task to configure them for the
following.

• Equal Employment Opportunity (EEO) reporting

• New Hire reporting

• Veterans' Employment & Training Service (VETS) reporting

• Payroll processing

• Third-party tax filing

Configure your legal entities and PSUs for
retirees

If you have retirees in your organization, you must create separate legal entities and PSUs for them.
Don't assign both employees and retirees to the same PSUs or to the same legal employers.

Define organization calculation cards for
your legal entities

Use the Legal Entity Calculation Cards task from your implementation project.

For further info on these steps, see the following sections.

For info about Capital Management for the United States white papers, see the United States Information Center
(2063588.2) on My Oracle Support.

Before You Begin
Be sure you have already defined any associated legal addresses through the Legal Addresses task.

Consider defining your US LDG before identifying your legal entities as PSUs. If you don't, the Legal Entities task
automatically creates the LDG for you and associates it with the PSU.

If you have already defined a US LDG, you can manually associate it with the PSU.

How You Create Legal Entities
To create a legal entity:

1. Start the Legal Entities task, and click Create.
2. On the Create Legal Entity page, provide the name, identifier, and country.
3.

If you don't designate this legal entity as a PSU, assign an existing PSU to it. Choose one from the Payroll
Statutory Unit field.

4. Provide any other required info.
5. Click Save and Close.

How to Identify the LDG
To view the LDG associated with a PSU:

1. Start the Legal Entity HCM Information task from your implementation project.
2. Search for the PSU or legal entity.
3. Select PSU. This displays general info for the PSU, including the LDG.
4.

If the LDG hasn't automatically been associated, select one from the menu.

How to Configure Your Legal Entities
Your legal entities require some configuration before you can perform HR reporting and payroll processing.

58

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Note:  Electronic year-end and quarterly filings processes aren't available in HCM. You must perform these filings
through the US Third-Party Tax Filing interfaces.

To enter this info:

1. Start the Legal Entity HCM Information task.
2. Search for and choose the legal entity you want to modify.
3.

If the legal entity is a legal employer:

a. Select Legal Employer.
b.

In the left pane, click Legal Employer Details and enter the necessary values in the Work Day
Information and Legal Employer Information sections.

For retiree legal entities, select the 2 Tier - Multiple Assignment employment model.

c. Click Federal, and define the EEO, New Hire, and VETS reporting rules.
d. Enter the company identifier.
e.
f.
g.

Indicate if the company employs more than 100 employees in a pay period.
Indicate if the employer is a government contractor.
In New Hire Reporting Rules, associate a default tax reporting unit (TRU) to a legal employer. Select one
in the TRU for the New Hire Report field.

HR reports use the employer federal employer identification number (EIN), registered name, contact
details, and registration details of the TRU associated with the legal employer.
In VETS Reporting Rules, enter the reporting name, parent company, company number, and type of
reporting organization.
In EEO and VETS Reporting Information, choose the employment categories you want to include in the
reports.

h.

i.

j. Select the Single or Multiple establishment employer type.
k.
l.
m.

Identify whether your legal entity is affiliated with an enterprise of 100 or more employees.
In United States Reporting Entity Data, identify each legal employer as either a parent or child.
In EEO and VETS Assignment Category, choose the assignment categories to include or exclude from
the EEO-1 report.
If the legal entity is also a PSU:

4.

a. Select PSU. This tab lists the associated PSU, including the LDG.
b. Enter the fiscal year start date.
c. Select Federal, and enter any additional info to support electronic year-end filings for the US.

5. Click Submit.

The details you specify apply to all legal reporting units (LRUs) associated with the PSU.

Note:  The TRU you select in the New Hire Reporting Rules requires additional EEO and VETS reporting info. Use the
Legal Reporting Unit HCM Information task to set these values for the TRU in the EEO and VETS Reporting Rules
region. For further info, see the Legal Entities for the US topic in the Help Center.

Define Organization Calculation Cards
To define a calculation card for a legal entity:

1. Start the Legal Entity Calculation Cards task from your implementation project.

59

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

2. On the Payroll Statutory Unit page, click Create.
3. Provide an effective date, and select Calculation Rules for Tax Reporting and Payroll Statutory Unit.
4. Click Continue.
5. Define the federal income tax (FIT) calculation rules for the card.

a. Select the appropriate row under Calculation Components.
b. Enter the appropriate data in Calculation Component Details, including the applicable employer self-

adjustment method.

c. Repeat to add calculation rules for Social Security, Medicare, and federal unemployment tax (FUTA).
d. Click Save.

6. Create regional calculation rules for the card.

a. Select Regional in Calculation Card Overview.
b. Under the Actions menu, select Create.
c. Select the appropriate state, and click OK.
d. Select State Unemployment in Calculation Components.
e.
f. Select State Unemployment Organization Information, and click OK.
g. Select the self-adjustment method.

In Calculation Component Details of the State Income Tax: Details section, click Add Row.

For further info, see Self-Adjustment Methods for Tax Withholding in the Help Center.

h. To define state unemployment (SUI) employer experience rates for your PSU, select Enterable

Calculation Values on Calculation Cards and click Create.

i. Repeat these steps to enter the self-adjustment method for state disability.
j. Define any appropriate courtesy tax withholding rules.

The settings you make on subordinate LRU calculation cards override values on this card.

Related Topics

• Legal Entities for Global Payroll

Employment Model

Overview of Payroll Employment Model
In the payroll employment model, each person has a payroll relationship to a payroll statutory unit (PSU), and one or
more payroll assignments and other employment structures.

Comparing the HR and Payroll Employment Models
This diagram shows the human resource (HR) employment model and the payroll employment model contrast where
two legal employers, Manufacturing and Installation belong to one PSU, Sun Power. As you can see, David Ellis has two
assignments where the HR model creates two work relationships and the payroll employment model creates one payroll
relationship.

60

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Related Topics

• Payroll Employment Hierarchy Profile Options

• Employment Level Options for Payroll Elements

• How do I diagnose payroll employment model setup issues?

How do I diagnose payroll employment model setup issues?
After creating enterprise structures, run the Payroll Employment Model Setup Validation test. This test checks whether
legal employers are associated with a legislative data group.

Select Run Diagnostic Tests from the Setting and Actions menu in the global header. You must have access to the
Diagnostic Dashboard to run this test.

61

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Payroll Relationships

Overview of Implementing Payroll Relationship
A payroll relationship is the highest level of the payroll employment model. It groups a person's assignment records for
payroll statutory calculation and reporting purposes.

The assignments grouped within a payroll relationship always belongs to the same PSU and person type such as
employee.

A payroll relationship enables you to enter information for a person in Oracle HCM Cloud that impacts their pay such as
salary, compensation, time cards, and absences.

For employees with multiple assignments, payroll relationships support tax and social insurance calculations that you
perform on earnings from all assignments grouped within the relationship. The results of payroll processes such as
Calculate Payroll are accordingly held against the payroll relationship of a person.

Payroll relationship rules and mappings control the creation of payroll relationships and define how they're processed
by Cloud Payroll for a localization. These rules and mappings are automatically available for country extensions
which are predefined by Oracle. If you're configuring a legislation that isn't predefined by Oracle, use the Configure
Legislation for Human Resources task to define the payroll relationship and mapping rules.

Related Topics

• Configure Legislations

• Overview of Administering Payroll Relationships

Payroll Relationship Switcher
Payroll relationship switcher gives you the ability to switch between payroll relationships when you have multiple payroll
relationships defined for the employee.

For example, an employee that's a contingent worker and a pending worker with element entries only, the employee
has personal payment methods: one in context of the contingent worker payroll relationship and one in context of the
pending worker payroll relationship. When this occurs, a drop-down list is available to switch views from one payroll
relationship to another.

You can define the values in the payroll relationship switcher using profile options to choose to display the Payroll
Relationship Type, Payroll Relationship Number and Payroll Statutory Unit. If these profiles aren't defined, Payroll
Relationship Type is shown by default. Use Manage Administrator Profile Options in Setup and Maintenance to define
profiles associated with the payroll relationship switcher. If defining all profile options, define them all at the same level,
such as Site level.

Related Topics

• Overview of Implementing Payroll Relationship

• Overview of Administering Payroll Relationships

Payroll Relationship Rules
Define a payroll relationship rule for each HCM Cloud legislation. The rule controls when and how payroll relationships
are created for a person. Oracle HCM Cloud delivers predefined payroll relationship rules for all country extensions.

62

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

If you're configuring a legislation that isn't predefined by Oracle, define mapping rules for all person types including
candidates that the legislation uses. The Configure Legislation for Human Resources task would create mapping rules
for person types such as employee. You can use this task to create any person type mapping rules that aren't predefined
by Oracle.

This table describes the application behavior based on the available payroll relationship rules for a legislation.

Create Employment Records Based on
Rules

Application Behavior

Last Record

When you create an assignment, the application searches for an active payroll relationship of the same
person type and for the same PSU.

•

•

If an active payroll relationship exists, the application groups the assignment under the existing
payroll relationship.

If an active payroll relationship doesn't exist, the application creates a new payroll relationship for
the assignment.

The Last Record rule is used in localizations such as the UK.

Lifetime Record

When you create an assignment, the application searches for a payroll relationship of the same person
type and for the same PSU.

•

•

If a payroll relationship exists, the application groups the assignment under the existing payroll
relationship. If the payroll relationship is terminated, the application removes the end date.

If a payroll relationship doesn't exist, the application creates a new payroll relationship for the
assignment.

New Record

When you create an assignment, the application creates a new payroll relationship. Each payroll
relationship is associated with one work assignment.

Note:  These rules apply to all new assignments, including the assignment that the application creates when a person
is rehired.

Related Topics

• Configure Legislations

• Overview of Administering Payroll Relationships

Payroll Relationship Type Mappings
Define payroll relationship type mappings for each HCM Cloud legislation. The mappings control when the application
creates payroll relationships for a specific type of person such as employee or candidate. The mappings also define if
the person type is processed by Cloud Payroll.

Oracle HCM Cloud delivers predefined payroll relationship type mappings for all the supported country extensions.
If you're configuring a legislation that isn't predefined by Oracle, define mapping rules for all person types including
candidates that the legislation uses. The Configure Legislation for Human Resources task would create mapping rules
for person types such as employee. You can use this task to create any person type mapping rules that aren’t predefined
by Oracle.

63

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

This table summarizes the behavior of the application when a person type is mapped to these payroll relationship types.

Note:  Few legislations have extended this list of payroll relationship types to meet their country specific
requirements.

Payroll Relationship Type

Application Behavior

Standard

Creates a payroll relationship and includes the person in payroll processes.

Element Entries Only

Creates a payroll relationship, but doesn't include the person in payroll processes.

Pending Worker Standard

Creates a payroll relationship and includes the person in payroll processes

Pending Worker Element Entries Only

Creates a payroll relationship, but doesn't include the person in payroll processes.

Candidate Standard

Creates a payroll relationship and includes the person in payroll processes.

Candidate Element Entries Only

Creates a payroll relationship, but doesn't include the person in payroll processes.

Note:  If a person type isn't mapped to a payroll relationship type, the application doesn't create payroll relationships.
In this scenario, you wouldn't be able to capture payroll information for the person type such as salary, element
entries, and personal payment methods.

Payroll Relationship Type Mappings Example for US Legislation
Payroll relationship types are mapped to one or more person types for each legislation.

Here's an example of the mapping rules predefined for the US legislation.

Person Type

Payroll Relationship Type

Process in Payroll

Employee

Retiree

Standard

Standard

Non-Worker

Non-Worker

Contingent Worker

Contingent Worker

Contingent Worker Candidate

Candidate Element Entries Only

Employee Candidate

Candidate Standard

Yes

Yes

No

No

No

No

64

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Here, Employee and Retiree person types are both mapped to the Standard payroll relationship type. If a US worker has
both employee and retiree assignments within the same PSU, the application will group these assignments under the
same payroll relationship.

Note:  Use the Configure Legislation for Human Resources task in My Client Groups to view the predefined rules
for your legislation.

Related Topics

• Configure Legislations

• Overview of Administering Payroll Relationships

Why can't I see candidate records on the Payroll pages?
Check the Display Candidate Records on Payroll Pages profile option setting, which controls the display of the
candidate employment records on the Payroll application pages.

The Display Candidate Records on Payroll Pages profile option controls whether the candidate records are displayed
on the Payroll pages. The default value of this profile option is No, which hides the candidate records. This setting lets
you view and select only those records that are managed within the Payroll product, such as employee. You can't select
candidate records on Payroll responsive pages such as Personal Payment Methods, Payroll Relationship, and Calculation
Entries.

To display the candidate records on the Payroll pages, set this profile option to Yes.

Why do I define payroll relationship rules for an international HR legislation?
Payroll relationships capture all types of payroll information for a person in Oracle HCM Cloud, such as salary,
compensation, personal payment methods, and time cards.

When do I change the payroll relationship rules for an international legislation?
Configure payroll relationship mapping rules for all person types when you implement an international legislation.

The Configure Legislation for Human Resources task would create mapping rules for person types such as employee.
You can use this task to create any person type mapping rules that aren't predefined by Oracle.

If employment records already exist, the best approach is to not change the payroll relationship rules. This approach
ensures that new and existing employment records have the same rules. However, if you want to update the payroll
relationship rules after employment records exist, your updates will affect only the newly created employment records
for the person type.

Related Topics

• Configure Legislations

Why doesn't the payroll region display for Candidate person type while you're
configuring international legislation?
Verify if you have created payroll relationship mapping rules for all person types including Candidate in the international
legislation.

Payroll relationship rules ensure that the application has created payroll relationship records for the person type. You
can view the payroll region for workers who have a payroll relationship record.

65

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

HCM Data Roles

Chapter 1
Let’s Get Started

Role Provisioning and Deprovisioning
You must provision roles to users. Otherwise, they have no access to data or functions and can't perform application
tasks. This topic explains how role mappings control role provisioning and deprovisioning.

Use the Manage Role Provisioning Rules or Manage HCM Role Provisioning Rules task to create role mappings.

Role Provisioning Methods
You can provision roles to users:

• Automatically

• Manually

◦ Users such as line managers can provision roles manually to other users.
◦ Users can request roles for themselves.

For both automatic and manual role provisioning, you create a role mapping to specify when a user becomes eligible for
a role.

Role Types
You can provision data roles, abstract roles, and job roles to users. However, for Oracle Fusion Cloud HCM users, you
typically include job roles in HCM data roles and provision those data roles.

Automatic Role Provisioning
Users acquire a role automatically when at least one of their assignments satisfies the conditions in the relevant role
mapping. Provisioning occurs when you create or update worker assignments. For example, when you promote a
worker to a management position, the worker acquires the line manager role automatically if an appropriate role
mapping exists. All changes to assignments cause review and update of a worker's automatically provisioned roles.

Role Deprovisioning
Users lose automatically provisioned roles when they no longer satisfy the role-mapping conditions. For example, a line
manager loses an automatically provisioned line manager role when he or she stops being a line manager. You can also
manually deprovision automatically provisioned roles at any time.

Users lose manually provisioned roles automatically only when all of their work relationships are terminated. Otherwise,
users keep manually provisioned roles until you deprovision them manually.

Roles at Termination
When you terminate a work relationship, the user automatically loses all automatically provisioned roles for which he
or she no longer qualifies. The user loses manually provisioned roles only if he or she has no other work relationships.
Otherwise, the user keeps manually provisioned roles until you remove them manually.

The user who's terminating a work relationship specifies when the user loses roles. Deprovisioning can occur:

• On the termination date

66

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

• On the day after the termination date

Chapter 1
Let’s Get Started

If you enter a future termination date, then role deprovisioning doesn't occur until that date or the day after. The Role
Requests in the Last 30 Days section on the Manage User Account page is updated only when the deprovisioning
request is created. Entries remain in that section until they're processed.

Role mappings can provision roles to users automatically at termination. For example, a terminated worker could
acquire the custom role Retiree at termination based on assignment status and person type values.

Reversal of Termination
Reversing a termination removes any roles that the user acquired automatically at termination. It also provisions roles to
the user as follows:

• Any manually provisioned roles that were lost automatically at termination are reinstated.

• As the autoprovisioning process runs automatically when a termination is reversed, roles are provisioned

automatically as specified by current role-provisioning rules.

You must reinstate manually any roles that you removed manually, if appropriate.

Date-Effective Changes to Assignments
Automatic role provisioning and deprovisioning are based on current data. For a future-dated transaction, such as a
future promotion, role provisioning occurs on the day the changes take effect. The Send Pending LDAP Requests
process identifies future-dated transactions and manages role provisioning and deprovisioning at the appropriate time.
These role-provisioning changes take effect on the system date. Therefore, a delay of up to 24 hours may occur before
users in other time zones acquire their roles.

Create HCM Data Roles for Global Payroll Implementation Users
If you've licensed the Oracle Fusion Global Payroll Cloud Service, then you create the PayrollAdmin_ViewAll and
PayrollMgr_ViewAll data roles. You create these roles using the Assign Security Profiles to Role task.

Create the PayrollAdmin_ViewAll Data Role
If you're already on the Manage Data Roles and Security Profiles page, then follow this procedure from step 2.
Otherwise, sign in as the TechAdmin user and follow these steps:

1.

In the Setup and Maintenance work area, go to the following:

◦ Functional Area: Users and Security
◦ Task: Assign Security Profiles to Role

You can also go to this page by selecting Navigator > My Client Groups  >  Workforce Structures >  Data
Roles and Security Profiles.
In the Search Results section of the Manage Data Roles and Security Profiles page, click Create.

2.
3. Complete the fields on the Create Data Role: Select Role page as shown in the following table.

Field

Value

Data Role Name

PayrollAdmin_ViewAll

Job Role

Payroll Administrator

67

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Field

Value

4. Click Next.
5.

In the sections of the Create Data Role: Security Criteria page, select the following predefined security profiles
for each drop-down list.

Section

Security Profile

Organization

View All Organizations

Position

View All Positions

Legislative Data Group

View All Legislative Data Groups

Person

View All People

Document Type

View All Document Types

Payroll

View All Payrolls

Payroll Flow

View All Flows

6. Click Review.
7. On the Create Data Role: Review page, click Submit.
8. On the Manage Data Roles and Security Profiles page, search for the PayrollAdmin_ViewAll data role to confirm

that it exists.

Create the PayrollMgr_ViewAll Data Role
Follow these steps:

In the Search Results section of the Manage Data Roles and Security Profiles page, click Create.

1.
2. Complete the fields on the Create Data Role: Select Role page as shown in the following table.

Field

Value

Data Role Name

PayrollMgr_ViewAll

Job Role

Payroll Manager

3. Click Next.

68

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

4.

In the sections of the Create Data Role: Security Criteria page, select the predefined security profiles shown in
this table.

Section

Security Profile

Organization

View All Organizations

Position

View All Positions

Legislative Data Group

View All Legislative Data Groups

Person

View All People

Document Type

View All Document Types

Payroll

View All Payrolls

Payroll Flow

View All Flows

5. Click Review.
6. On the Create Data Role: Review page, click Submit.
7. On the Manage Data Roles and Security Profiles page, search for the PayrollMgr_ViewAll data role to confirm

that it exists.

Related Topics

• Overview of HCM Data Roles for Implementation Users

Secure Elements through HCM Data Roles
Secure and limit access to elements based on your business requirements.

Perform these two actions to secure and limit access to all elements:

• Use the Element Security Profiles quick action to create an element security profile. Include or exclude elements

to this profile as per your requirements.

• Add the new security profile to an HCM Data Role to secure and limit access to the elements.

For example, you can now restrict a Benefits user to access only the voluntary and pretax deductions, but not the
regular and supplemental earnings. You can now define an element security profile to include only voluntary and pretax
deduction elements and attach it to the Benefits Administrator data role.

When you navigate to the Element Entries page, the elements you can manage is restricted to those in your element
security profile. You can enter, view, and edit certain earnings and deductions elements that are meant for your
respective usage.

69

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Features Secured by Element Security Profiles
The Element Security Profile restriction applies to these payroll features:

• Manage Element Entries (both Manage and View-only)

• Manage Calculation Entries – Standard Entries only

• Manage Elements

• Balance Adjustment

• Use REST Service – Element Entries

• Use REST Service – Element Entries Read-Only

• Payroll Element Definition List of Values REST

• Payroll Input Values List of Values REST

• HSDL – Element Entry

• HDSL – Element Entry with Costing

• QuickPay

It also applies to the following Benefits feature:

• View Payroll Info under the Enrollment section of the Benefits Summary page.

Element Security Profiles
Use the Element Security Profile task to create element security profiles. However, you can make use of any these
available updates.

• By default, all the existing data roles are automatically updated with the View All Elements element security

profile.

• When upgrading to Update 24A, the Regenerate Data Security Profiles and Grants job set will be run; you

should verify it ran successfully. You should see that the View All default value appears on your data roles after
upgrading.

• When you create or edit a Data Role on the HCM Data Roles and Security Profiles page, use the Element

Security Profile option under the Element section on the Create Data Role: Security Criteria page, to chose a
element security profile for the role.

•

If you have any automated test cases that try to edit a role or create a new data role based on impacted job
roles, you must populate the element security profile value.
From this section, you can either select an existing element security profile or create one for the data role.

• You can also use these options to view, create, or edit element security profiles for data roles.

◦ The Element sub-train stop on the Assign Security Profiles to Role page.
◦ Support for the new profile under Preview HCM Data Security page.
◦ A new parameter for the element security profile in the Regenerate Data Security Profiles and

Grantsscheduled process.

Include or Exclude Elements in a Security Profile
You can include or exclude elements to an element security profile as per your security and business requirements.

When you create an element security profile, you select a Legislative Data Group (LDG).

70

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Once you select an LDG on the Element Security Profile page, the element classifications applicable to the LDG gets
populated in the Classifications region.

Select the required primary classifications, all elements within the selected primary classifications are automatically
included in the element security profile. However, if required, you can exclude some elements from the selected
classifications, or include some elements from a classification you haven't selected.

Note:  You can include multiple LDGs within a security profile. Each LDG must have at least one classification or
element included. Consider the following when you create element security profiles and include or exclude elements:

•

•

LDG security and element security profile are independent of each other. When you implement both LDG and
element security profile, ensure that the LDG included in the element security profile is also included in the
LDG security profile.

Predefined statutory deduction elements exist for a legislation. If you have multiple LDGs within a single
legislation, if you include the statutory deduction elements for one of the LDGs, they will be available for all
LDGs within the same legislation.

• When the security profile is based on primary classifications, you can only create elements with those

primary classifications. Under Element Summary, Run Types, Balance Feeds, Status Processing Rules and
Autoindirect rules shows only the elements in your Element Security Profile. Similarly, when creating new
records, the element list of value is restricted.

QuickPay Processing
Element entries displayed on the QuickPay page are restricted based on the user element security profile. However, all
elements are processed when the user submits the QuickPay.

Access Requirements
You can use this feature only for the job roles given in this table.

Job Role Name

Job Role Code

Application Implementation Consultant

ORA_ASM_APPLICATION_IMPLEMENTATION_CONSULTANT_JOB

Benefits Administrator

ORA_BEN_BENEFITS_ADMINISTRATOR_JOB

Benefits Manager

ORA_BEN_BENEFITS_MANAGER_JOB

Benefits Specialist

ORA_BEN_BENEFITS_SPECIALIST_JOB

Compensation Administrator

ORA_CMP_COMPENSATION_ADMINISTRATOR_JOB

Human Capital Management Application

ORA_HRC_HUMAN_CAPITAL_MANAGEMENT_APPLICATION_ADMINISTRATOR_JOB

Administrator

Human Capital Management Integration

ORA_HRC_HUMAN_CAPITAL_MANAGEMENT_INTEGRATION_SPECIALIST_JOB

Specialist

Human Resource Analyst

ORA_PER_HUMAN_RESOURCE_ANALYST_JOB

Human Resource Manager

ORA_PER_HUMAN_RESOURCE_MANAGER_JOB

71

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Job Role Name

Job Role Code

Human Resource Specialist

ORA_PER_HUMAN_RESOURCE_SPECIALIST_JOB

Payroll Administrator

ORA_PAY_PAYROLL_ADMINISTRATOR_JOB

Payroll Manager

ORA_PAY_PAYROLL_MANAGER_JOB

How to Restrict Access to Elements Using Element Security Profile and HCM Data
Role
This topic shows how you can restrict and limit user access to certain elements based on your organisational needs.

Create a new Element Security Profile, include or exclude elements as per your specific requirements, and add this
profile to a specific data role.

1. Create an Element Security Profile
Complete these steps to create an element security profile.

1. Navigate to My Client Groups > Show More > Payroll and select the Element Security Profile quick action.
2. Click the Add icon to create an Element Security Profile.
3. Enter a Name for the profile and select the Enabled checkbox.
4. Select a Legislative Data Group.

Once you select an LDG, the element classifications applicable to the LDG gets populated in the Classifications
region.

5. Select the classifications you want to include in the security profile. All elements within the selected

classifications are automatically included.

2. Include or Exclude Individual Elements
Once you select an LDG on the Element Security Profile page and select the required primary classifications, all
elements within the selected primary classifications are automatically included in the element security profile.

However, if required, you can exclude some elements from the selected classifications, or include some elements from a
classification you haven't selected.

Complete these steps to include or exclude individual elements.

1. Click the Add icon in the Elements section on the Element Security Profile page.
2. Search for the elements you want to include or exclude and select the

Inclusion Status as required.

When you select an element and its primary classification, the Inclusion Status for the individual elements is
automatically displayed as follows:

◦ If the primary classification of the selected element is included in the profile, the inclusion status is set to

Exclude.

◦ If the primary classification is excluded from the profile, the inclusion status is set to Include.

72

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

3. Click Save and Close. The Element Security Profile is saved.

You can include multiple LDGs within a security profile. Each LDG must have at least one classification or
element included.

3. Add an Element Security Profile to a Data Role
After you create an Element Security Profile, add the profile to a Data Role. By default, for all existing data roles, the
Element Security Profile is populated with View All Elements. You can edit a Data Role and either add an existing
element security profile, or create a new element security profile.

1. Add an Existing Element Security Profile

Complete these steps to add an existing Element Security Profile and restrict elements for a specific data role.
a. Navigate to My Client Groups > Show More > Workforce Structures Payroll and select the Data Roles

and Security Profiles quick action.

b. Search and select the Data Role and click Edit.
c. Select an existing profile in the Element Security Profile field.

2. Edit a Data Role and Create an Element Security Profile

You can also create a new Element Security Profile and add it to the Data Role you're editing.

a. Navigate to My Client Groups > Show More > Workforce Structures Payroll and select the Data Roles

and Security Profiles quick action.

b. Search and select the Data Role and click Edit.
c. Select Create New in the Element Security Profile field.
d. Enter the name of the profile in the Name field.
e. Select the LDG and Primary Classifications, include or exclude elements as required.
f. Click Save and Close.

3. Use the Element Tab and Create an Element Security Profile

Complete these steps to create an Element Security Profile using the Element tab.

a. Navigate to My Client Groups > Show More > Workforce Structures Payroll and select the Data Roles

and Security Profiles quick action.

b. Search and select the Data Role and click Edit.
c. Click Next and select all the security profiles.
d. Click Next. Click the Element tab.
e. Select Create New in the Element Security Profile field.
f. Enter the name of the profile in the Name field.
g. Select the LDG and Primary Classifications, include or exclude elements as required.
h. Click Save and Close.

How do I provision HCM data roles to users?

On the Create Role Mapping page, create a role mapping for the role.

Select the Autoprovision option to provision the role automatically to any user whose assignment matches the
mapping attributes.

Select the Requestable option if any user whose assignment matches the mapping attributes can provision the role
manually to other users.

73

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Select the Self-Requestable option if any user whose assignment matches the mapping attributes can request the role.

Application Tools

Business Definitions

An integral part of the payroll setup is defining payroll business definitions.

Use the Define Payroll Business Definitions task in the Define Payroll tasks list to create lookups, value sets, and
descriptive flexfields that you need to support payroll.

Lookups
Lookups are lists of values in the application that provide validations or provide a list of values for a user input field in
the user interface. You define a list of values as a lookup type consisting of a set of lookup codes, each code's translated
meaning, and optionally a tag. The tags control which countries can have access to the lookup codes being defined. End
users see the list of translated meanings as the available values for an object.

Let's look at an example of a lookup type for marital status (MAR_STATUS) that has lookup codes for users to specify
the marital status as given below in this table.

Lookup Code

M

S

R

DP

Meaning

Married

Single

Registered Partner

Domestic Partner

Tag

Not applicable

Not applicable

+NL

-FR, AU

As you manage lookups, consider these.

• Using lookups in applications

• Configurable levels

• Accessing lookups

• Enabling lookups

• The three kinds of lookups: standard, common, and set enabled

Descriptive Flexfields
Use descriptive flexfields to add customer-defined attributes to business object entities, and define validation for them.

All the business object entities that you can use in the application are enabled for descriptive flexfields. However,
configuring descriptive flexfields is an optional task.

74

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Configuring descriptive flexfields involves managing the available flexfields registered with your Oracle Applications
Cloud database and configuring their flexfield-level properties, defining and managing descriptive flexfield contexts,
and configuring global and context-sensitive segments.

Extensible Flexfields
Extensible flexfields are like descriptive flexfields, with some additional features.

Unlike descriptive flexfields, the columns corresponding to extensible flexfield segments are part of specific tables,
separate from the base application table. Unlike descriptive flexfield contexts, the set of attributes in an extensible
flexfield context remains constant and doesn't differ by context value.

An extensible flexfield describes an application entity, with the run time ability to expand the database that
implementation consultants can use to define the data structure that appears in the application.

Extensible flexfields support one-to-many relationships between the entity and the modified attribute rows.

To get a list of predefined extensible flexfields, open the Setup and Maintenance area, and use the Extensible Flexfields
for Payroll task.

Here are a few aspects that are important in understanding extensible flexfields:

• Usages

• Categories

• Pages

• Security

• Protected Extensible Flexfield Data

Value Sets
A value set is a group of valid values that you assign to a flexfield segment to control the values that are stored for
business object attributes.

An end user enters a value for an attribute of a business object while using the application. The flexfield validates the
value against the set of valid values that you configured as a value set and assigned to the segment.

For example, you can define a required format, such as a five digit number, or a list of valid values, such as green, red,
and blue.

Related Topics

• Validation Type Options for Value Sets

• How Flexfields and Value Sets Work Together

• Considerations for Managing Descriptive Flexfields

• Overview of Extensible Flexfields

• Overview of Lookups

75

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Profile Options

Chapter 1
Let’s Get Started

Use profile options to manage user preferences and control the general function of applications. For example, you can
control user preferences involving language, date, time, currency, and other similar general settings.

You can create a profile option and also determine the level at which that profile option takes effect. You can also define
the profile values for the profile option. The profile values appear on the Manage Administrator Profile Values page
when you select the profile option.

Creating a Profile Option

In the Setup and Maintenance work area, go to the Manage Profile Options task.

1.
2. On the page, click Actions > New.
3. On the Create Profile Option page, fill all the fields with relevant details with specific attention to the following:

◦ Use the SQL Validation field to provide an SQL statement that displays the permissible profile values to

be used. Using an SQL statement, you can select the values from another table and display them as a list
of values.

For example, to display the values Yes and No from a lookup table, you can use the following SQL
statement:

select MEANING, LOOKUP_CODE from FND_LOOKUPS where LOOKUP_TYPE='YES_NO'

As a result, on the Manage Administrator Profile Values page, the profile values Yes and No are
available for selection for that profile option.

◦ You can specify a date range to keep the profile option active during that period. Beyond the specified
duration, the profile option automatically becomes inactive. If you no longer require the profile option,
you must manually delete it from the Manage Profile Options page.

4. Click Save and Close.
5. On the Manage Profile Options page, search for the newly created profile option and from the results, select it.
6.

In the Profile Option Levels section, do the following:

a.

In Enabled, select the levels at which you want to enable the profile option.

Note:  You can enable a profile option at multiple levels, but a higher-level profile value overrides a
lower-level value. Therefore, enable them only at the required levels.

b.

In Updatable, select the profile level at which you want implementors to have update privileges. Leave
the check box deselected if you don't want the implementors to modify the profile values (they appear in
read-only mode).

7. Click Save and Close.

To edit a profile option that you created, search for it and edit the necessary details.

76

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Note:

Chapter 1
Let’s Get Started

• While creating and editing profile options and profile categories, you can translate the details to the preferred
languages without changing the language session of the application. To specify the translations in all the
enabled language rows, use the Translation Editor option. Once the updates are made, users can view the
translated text for the specific details.

•

If you want to access the profile option using REST API, you must add it to the Authenticated User Profile
Option Values (ORA_FND_AUTH_REST_ACCESS) profile category.

Related Topics

• Hierarchy in Profile Levels

• Set Profile Option Values

• How can I enter or edit translated text in Fusion Applications?

• Profile Categories

Security Profiles

HCM Security Profiles
Security profiles identify instances of Human Capital Management (HCM) objects. For example, a person security profile
identifies one or more Person objects, and a payroll security profile identifies one or more Payroll objects.

For details, see the topic Security Profiles.

Related Topics

• Predefined Security Profiles

• Best Practices for Data Roles and Security Profiles

Payroll Security Profiles
You can use different methods to provide access to payrolls for members of the Payroll department. Use the Manage
Payroll Security Profiles task to organize your payroll definitions into appropriate payroll security profiles.

Then, use the Assign Security Profiles to Role task to select the security profiles included in an HCM data role that you
provision to a user.

Payroll Period Type
It's common to use the payroll security profile to organize payroll definitions by payroll period type. You simply create
one security profile for each payroll type, such as monthly payrolls, another for semimonthly payrolls, and so on.

Regional Assignments
You can use payroll security profiles to group payrolls by the regions of the employees' work location. For example, you
can create one for Canadian facilities and another for European facilities.

77

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Individual Contributors
If your payroll managers can access only the payroll definitions that they manage, use create payroll security profiles to
include only those payrolls.

Payroll and Payroll Flow Security Profiles
Use the Security Profile pages to restrict user access and review, create, and update security profiles for payroll and
payroll flows.

IT Security Managers can navigate to the following pages from the Quick Actions pane under My Client Groups
> Show More> Payroll on the Home page. If you've enabled the corresponding profiles, you can also access these
Redwood pages from the Setup and Maintenance area.

• Payroll Security Profiles

• Payroll Flows Security Profiles

If you've functional access to these pages, you can directly access these pages in edit mode.

Note:  Predefined security profile values are delivered as read-only and you can't edit these rows.

The enhanced pages allow you to do the following:

• View enabled security profiles by default.

• Expose audit details for each row, such as when the security profile was created and updated.

• View focused search results with less-frequently used columns hidden by default.

• Use the Columns icon to hide or show columns and modify the column order. You can also enable new columns
that allow you to view, sort, and search security profiles based on who created or updated that security object.
You can view the date it was created on or last updated, by enabling these hidden columns.

• Sort the results in ascending or descending order.

• Export search results.

• Edit a role with a single click of the role name.

• Define security criteria using a simplified page.

Payroll Security Profile
Use payroll security profiles to limit a user's access to relevant payrolls. By default, only security profiles that are enabled
are displayed in the search results. You can access disabled security profiles by removing the filter chip selection. If the
delivered View All Payroll security profile doesn't support your business requirements, create a new payroll-specific
security profile to meet your requirements.

Payroll Flow Security Profile
Payroll flow security profiles are used to limit a user's access to relevant payroll flows. By default, only security profiles
that are enabled are displayed in the search results. You can access disabled security profiles by removing the filter chip
selection.

When you add a new record, choose the relevant payroll flow. By default, the applicable legislative data group that the
payroll flow is associated with appears, unless it's a global flow. Choose the check mark to save the row, or 'x' to cancel
and delete your selection.

78

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Payroll Data Capture for Multiple Concurrent Assignments
You can restrict access to assignments based on a user's Person Security Profile, if your organization allows workers to
have multiple concurrent assignments.

Enable the assignment-level security profile to ensure that users have access to only those assignments that match the
criteria defined in their person security profile.

You can apply this behavior to a limited set of quick actions, such as Payroll Relationship, Element Entries, Calculation
Entries, and Costing for a Person. For all other payroll features, the behavior stays the same. If at least one of the
employee's assignment satisfies the criteria in the person security profile, then the application displays all assignments
on the search results page.

This table describes how the enhanced data capture applies to these Quick Action tasks:

Task

Manage Page

View-Only Page

REST

Responsive Person
Search

What's Displayed?

Payroll Relationship

Yes

Yes

Yes

Element Entries

Yes

Yes

NA

Assignment in
Security Profile

Assignment in
Security Profile

Calculation Entries

Yes

Yes

NA

Assignment in
Security Profile

Costing for a Person

Yes

Personal Payment
Method

Yes

Yes

Yes

NA

Yes

Assignment in
Security Profile

Assignment in
Security Profile

Payroll relationship
for the selected
assignment.
Assignments within
the payroll relationship
and in the security
profile.

Element entries for
the payroll relationship
for the selected
assignment.

All element entries for
assignments within
the payroll relationship
and in the security
profile.

Calculation entries for
the payroll relationship
for the selected
assignment.

All calculation entries
for assignments within
the payroll relationship
and in the security
profile.

Costing information
for the payroll
relationship for the
selected assignment.

Payroll relationships
for the assignments in
the user's assignment
security profile.

79

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Task

Manage Page

View-Only Page

REST

Responsive Person
Search

What's Displayed?

Here are some considerations that you factor in when enabling the assignment-level security profile:

• Any other page, process, or report apart from those in the table operate at the payroll relationship level. You'll

have access to all assignments if at least one of the assignments satisfies the criteria set in the Person Security
Profile.

•

If you've access to one assignment each in the manage and view-only pages for the same employee, you can
manage both assignments. The manage access takes precedence over view-only.

• Calculation entries, such as Absence and Time region don't support assignment level security.

• Quick Pay Person Search returns all assignments. Let's consider the case when you select an assignment that

you're not allowed to view. Then the application displays those element entries for the assignments that you're
allowed to view, which could be a different assignment than the one selected. If you aren't allowed to view
any assignment, then the element entry section is blank. If you submit the Quick Pay, then the application
processes all element entries.

• Quick Pay Person Search returns all assignments. Let's consider the case when you select an assignment that

you're not allowed to view. Then the application displays those element entries for the assignments that you're
allowed to view, which could be a different assignment than the one selected. If you aren't allowed to view
any assignment, then the element entry section is blank. If you submit the Quick Pay, then the application
processes all element entries.

For more information about concurrent assignments, see the Secure Access for Workers with Multiple Assignments
section of the Oracle Human Resources Cloud What's New.

Secure Access to Payroll Relationships of Employees with Multiple Assignments
Use assignment-level security to control what users can see for employees with multiple assignments.

Scenario

Person Search Behavior

Detail Page Visibility

Example

Assignment-level security disabled All assignments shown if at least

The user can see:

one assignment meets the criteria
defined in the user's person
security profile.

• All assignments

• All payroll relationships

Assignment-level security enabled
for these pages:

• Adjust Individual Balances

Only those assignments that meet
the criteria defined in the user's
person security profile are shown.

• Balance by Date

• Calculation Entries

• Event Action Notifications

• Event Notifications

• Payslips

The user can see:

• Entries for the selected

assignment

• Entries for the selected
assignment’s payroll
relationship

• Entries for all assignments

within that payroll
relationship, even if those
assignments don’t meet the

The user's person security
profile allows access to people
in the UK LDG. An employee has
assignments in UK and France.

The user can see the person, all
their assignments (UK and France),
 and all payroll relationships.

The user can access assignments
in the Sales department. An
employee has assignments in Sales
and Marketing.

Search shows only the Sales
assignment.

On the detail page, the user can
see both Sales and Marketing

80

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Scenario

Person Search Behavior

Detail Page Visibility

Example

• Person Results

• QuickPay Payments

• Simplified QuickPay

• Third-Party Person Payment

Methods

• View Process Information

Groups

Assignment-level security enabled
for other pages such as Element
Entries, Payroll Relationship, and so
on

Only those assignments that meet
the criteria defined in the user's
person security profile are shown.

criteria defined in the user's
person security profile

assignments, along with payroll
relationship details.

The user can see:

• Entries for the selected

assignment

• Entries for the selected
assignment’s payroll
relationship

The user can access assignments
in the Sales department. An
employee has assignments in Sales
and Marketing.

Search shows only the Sales
assignment.

• Entries for other assignments
only if they also meet the
criteria defined in the user's
person security profile

On the detail page, the user can
see only the Sales assignment and
payroll relationship details. The
Marketing assignment isn’t shown.

Load Objects with HCM Data Loader

Use HCM Data Loader for bulk-loading and maintaining payroll data. You can navigate to the HCM Data Loader pages
directly from the Payroll Checklist page. On the Checklist page, select the Initiate Data Loader task to open the HCM
Data Loader object status page.

You can use HCM Data Loader to load these payroll objects.

• Balance Definitions

• Element Entries

• Object Groups

• Organization Payment Method

• Payroll Consolidation Groups

• Payroll Costing

• Payroll Definitions and Time Periods

• Payroll Element Run Usage

• Payroll Elements

• Payroll Relationship

• Personal Payment Method

• Time Definitions

• User-Defined Tables

• Wage Basis Rules

81

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

For more info on how to load these business objects, refer to the Integrating with HCM guide.

Payroll Transformation Formula for HCM Data Loader
Your existing data or the data that you upload might not be in the format recognized by HCM Data Loader. In such
cases, use the Payroll Transformation formula for HCM Data Loader to transform your data into a format that's
supported by HCM Data Loader.

Payroll Transformation Formula for HCM Spreadsheet Data Loader
You can use HCM Spreadsheet Data Loader to load all payroll objects that HCM Data Loader supports. As the first step,
you create a spreadsheet template for the required object from the Data Exchange work area and further download
the template in CSV format. The Payroll Transformation Formula for HCM Spreadsheet Data Loader transforms the raw
delimited file to a format that suits the template.

Related Topics

• Example of Loading Organization Payment Methods

• Example of Loading Payroll Balance Attribute Definitions

• Overview of Loading Payroll Costing

• Overview of Loading Payroll Details

• Overview of Loading User-Defined Tables

Load Payroll Data Using Transformation Formula

Overview of Payroll Transformation Formula For HCM Data Loader
Often times, your existing data or the payroll data that you upload might not be in the format recognized by HCM Data
Loader.

In such cases, you can use a payroll transformation formula to transform your data into a format that's supported by
HCM Data Loader.

Let's consider these examples.

• An inbound file contains data that needs to be loaded using different payroll business objects in HCM Data

Loader. Here, the content of the file needs to be split across more than one HCM Data Loader file.

• You might create a transformation formula to convert an attribute value in the file to another value that you

derive using value sets.

• You want to change a person number into an assignment number. In this case, you'll use a more complex

formula to convert the attributes.

You use the Load Data From File flow to transform your data into the HCM Data Loader file format using your
transformation formula.

As this table shows, the two flow patterns are secured using these privileges:

Flow Pattern

Privileges

Submit Payroll Flow

PAY_SUBMIT_PAYROLL_FLOW_PRIV

82

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Flow Pattern

Privileges

Load HCM Data

HRC_LOAD_HCM_DATA_PRIV

Chapter 1
Let’s Get Started

This example specifies the file name in the formula as PersonalPaymentMethod, the file discriminator as
PersonalPaymentMethod, and the business operation as MERGE.

/*HDL Related Outputs*/
 FileName = 'PersonalPaymentMethod'
 BusinessOperation = 'MERGE'
 FileDiscriminator = 'PersonalPaymentMethod'

To view details about the file name, file discriminator, and a list of supported business operations, use the View
Business Objects task in the Data Exchange work area.

1. On the View Business Objects page, search for and select your business object. In this example, the business

object is Personal Payment Method.

2. On the Component Details page, you can find the name of the file, and the file discriminator and a list of

supported actions for the object.

Related Topics

• How You Transform Data Using Payroll Transformation Formula for HCM Data Loader

• How To Create A Program for Automation

• Submit the Load Data From File Flow

How You Transform Data
Use the Load Data From File flow to transform data in the source file into a format that's supported by HCM Data
Loader.

You can submit this flow independently or include it in a flow that you create for automating data loads on a periodic
basis. When you submit the flow, either manually or using a web service, you must specify a transformation formula to
transform the data, as needed.

The flow contains these two tasks that help you to transform data into a HCM Data Loader format:

• Generate Data Loader File

•

Initiate Data Loader Task

As this figure shows, the first step is to submit the Load Data From File flow. This flow takes data from the flat file and
generates an equivalent file format for the data present in the input file.

83

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Perform these steps to transform data using Payroll Transformation Formula for HCM Data Loader:

1. On the Home page, click the Submit a Flow quick action under the My Clients Groups tab. On the Flow

Submission page, search for, select, and submit the Load Data From File flow pattern.

2. The flow invokes the Payroll Transformation Formula for the Content ID. Typically, you create your

transformation formula for HCM Data Loader on the Manage Fast Formulas page. The type of the formula
should be HCM Data Loader.

3. The Generate Data Loader File task reads the data file line by line, producing an equivalent HCM Data Loader
format for each line. Finally, it creates a compressed file of all the transformed data files and uploads to the
Oracle WebCenter Content server. Also, the task records the Content ID.

4. The Initiate Data Loader task takes the Content ID for the file generated by the Generate Data Loader File
task. And it invokes HCM Data Loader. HCM Data Loader validates the data and creates valid records in the
HCM cloud.

The table shows the tasks and the privileges that they're secured with:

Task

Privilege

Submit Payroll Flow

PAY_SUBMIT_PAYROLL_FLOW_PRIV

Load HCM Data

HRC_LOAD_HCM_DATA_PRIV

84

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Related Topics

• How To Create A Program for Automation

• Submit the Load Data From File Flow

• Transformation Formula Input Variables

How To Create A Program for Automation
You can submit the Load Data from File flow by using a web service.

As this figure shows, your program uploads the source file to content server, and retrieves the content ID for the Flow
Actions Service web service. Then, the program calls the Flow Actions web service by supplying certain parameters.

When calling the web service, your program supplies these parameters.

• Name of the flow pattern, which is Load Data from File

• Content ID of the uploaded file

• Unique name to identify the flow instance being submitted

• Process configuration group ID for special processing (optional)

• Transformation formula ID (mandatory)

For more information about the Flow Actions Service web service, refer to the SOAP Web Services for Oracle HCM Cloud
guide. For examples of its usage for automating file uploads, refer to the attachment for HCM Data Loader User Guide
(1664133.1) on My Oracle Support at https://support.oracle.com.

85

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Related Topics

• Submit the Load Data From File Flow

• Transformation Formula Input Variables

• Payroll Transformation Formula Operations

• Sample Payroll Transformation Formula for HCM Data Loader

• Sample Payroll Transformation Formula for Multiple Business Objects

Submit the Load Data From File Flow
On the Home page, click the Submit a Flow quick action under the My Clients Groups tab. On the Flow Submission
page, submit the Load Data from File flow pattern to transform data in your source file into the HDL format.

Assumptions
This procedure has these assumptions.

• You have the Human Capital Management Integration Specialist role.

• You have the source file ready to upload to Oracle WebCenter Content.

•

If you have already uploaded the source file, you have the content ID handy.

Note:  To upload files to the content server, browse to the source file on your file system, check it in to the content
server, and retrieve its Content ID.  For more information, see Oracle Fusion Middleware Using Oracle WebCenter
Content guide.

Before You Begin
Before you submit the flow, ensure that you meet these prerequisites.

Characteristics

What You Should Do

Data transformation

If the data in the source file requires transformation, create and compile a transformation formula
using the HCM Data Loader formula type.

On the Home page, click the Fast Formulas quick action under the My Clients Group tab.

You can now specify the processing parameters for your process configuration group.

File encryption

Before loading encrypted files, ensure that the encryption keys exist for the secure file transfer. This
process involves creating a service request, generating PGP key pairs, and sharing the encryption keys.

Specify the Payroll Batch Loader Encryption Type  parameter value for the process configuration
group you select when running the flow or the web service. Valid values are PGPSIGNED,
 PGPUNSIGNED, and NONE.

On the Home page, click the Process Payroll Configuration quick action under the My Clients group
tab. Now, you can specify the processing parameters for your process configuration group.

Other processing parameters

Use the Payroll Process Configuration task to add parameters for the process configuration group.

Examples of processing parameters include Batch Error Mode, Logging Area, Logging Category, and
Threads.

86

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Characteristics

What You Should Do

In the Legislative Data Group option, select a legislative data group.

1. On the Home page, click the Submit a Payroll Flow quick action under the My Clients Groups tab.
2.
3. Search for and select the Load Data from File flow pattern.
4. Click Next.
5. Enter the parameters, as shown in this table.

Field

Value

Payroll Flow

Descriptive name for this specific flow process.

Content Id

Enter the Content Id. The source file must already exist on the content server.

Transformation Formula

Select the required transformation formula. The type of the formula should be HCM Data

Loader.

Process Configuration Group

Select your process configuration group.

6. On the Enter Parameters page, click Next.
7. On the Enter Flow Interaction page, click Next.
8. On the Schedule page, click Next.
9. On the Review page, click Submit.
10.
11. On the Payroll Flow page, Task Details tab you should see a green check mark in the Generate Data

In the confirmation dialog box, click OK and View Checklist.

Loader File and Initiate Data Loader rows, Task Type column. If not, on the toolbar, click the Refresh icon
intermittently until you do.

12. Close the Payroll Flow page.
13. On the Overview page, search for and click your payroll flow.
14. View the process results.
15. Check for any errors or warnings.

Related Topics

• Transformation Formula Input Variables

• Payroll Transformation Formula Operations

• Return Values for Payroll Transformation Formula for HCM Data Loader

• Sample Payroll Transformation Formula for HCM Data Loader

• Sample Payroll Transformation Formula for Multiple Business Objects

Transformation Formula Input Variables
Variables, such as FileName, FileDiscriminator and LINEREPEATNO, are available for all formulas of HCM Data Loader
Transformation formula type. Additional variables may be available depending on the selected business object.

87

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Positions
Using the transformation formula, you can assign attributes to the required position. Positions can range from 1 to N.
Depending upon the business object, the positions can be either optional or mandatory.

Example:

This figure shows the different attributes for positions 2 through 8 for Balance Adjustments.

In this example, you assign attributes to positions 2 through 8.

• POSITION2: EffectiveDate
• POSITION3: PayrollName
• POSITION4: LegislativeDataGroupName
• POSITION5: ConsolidationSetName
• POSITION6: BalAdjBatchId
• POSITION7: SourceSystemId
• POSITION8: SourceSystemOwner

FileName, FileDiscriminator, and BusinessOperation
FileName, FileDiscriminator, and BusinessOperation variables are required for all transformations.

Here are the details of these variables.

• FileName is the name of the file for the business object.
• FileDiscriminator is the file discriminator for the business object.
• BusinessOperation refers to the operation, such as Merge or Delete that are performed by the HCM Data Loader

process on the transformed file.

Here's an example of values that you can supply for the input variables: FileName, FileDiscriminator, and
BusinessOperation.

FileName = 'BalanceAdjustmentHeader'
BusinessOperation = 'MERGE'
FileDiscriminator = POSITION1

LINEREPEAT And LINEREPEATNO
LINEREPEAT allows a single line of input to be processed multiple times. And LINEREPEATNO indicates the number of
repetitions.

For example, for time entry, there might be a regular time entry wage followed by a premium time entry wage.

88

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Example: The Element Entry file contains these details.

Update|ElementEntryValue|Vision Corporation US LDG|WLM_Salary|2019/04/15|4712/12/31|E955160008191355-2|
Amount|1002|2|E
Update|ElementEntryValue|Vision Corporation US LDG|WLM_Salary|2019/04/15|4712/12/31|E955160008191355-2|
Amount|1003|3|E

The input line can be processed twice. The output file contains the element entry and element entry value as shown in
this sample code snippet.

ELSE IF OPERATION='MAP' THEN
(
 LegislativeDataGroupName=POSITION3
 ElementName=POSITION4
 EffectiveStartDate=POSITION5
 EffectiveEndDate=POSITION6
 AssignmentNumber=POSITION7
 InputValueName=POSITION8
 ScreenEntryValue=POSITION9
 MultipleEntryCount=POSITION10
 EntryType=POSITION11
IF LINEREPEATNO=1 THEN
 (
 BusinessOperation='MERGE'
 BusinessObject='Element Entry'
 FileName = 'ElementEntry'
 FileDiscriminator ='ElementEntry'
 LINEREPEAT = 'Y'
 RETURN BusinessOperation,FileDiscriminator,FileName
 )
ELSE
(
 BusinessOperation='MERGE'
 BusinessObject='Element Entry Value'
 FileName = 'ElementEntry'
 FileDiscriminator = 'ElementEntry'
 LINEREPEAT = 'N'
 RETURN BusinessOperation,FileDiscriminator,FileName
 )

Note:

• The length of a line in the incoming raw file can't be more than 1000 characters

• The length of an attribute between two delimiters can't be more than 255 characters

Related Topics

• Payroll Transformation Formula Operations

• Return Values for Payroll Transformation Formula for HCM Data Loader

• Sample Payroll Transformation Formula for HCM Data Loader

• Sample Payroll Transformation Formula for Multiple Business Objects

Payroll Transformation Formula Operations
The transformation formula is invoked several times to derive different components that are required for processing the
incoming data.

This table explains the various operations that you can do with the formula.

89

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Operation Type

Return Value

FILETYPE

DELIMITER

READ

MAP

OUTPUTVALUE

OUTPUTVALUE

OUTPUTVALUE

Business Object Attributes

NUMBEROFBUSINESSOBJECTS

OUTPUTVALUE

Example

DELIMITED

|

NONE

NA

2

METADATALINEINFORMATION

METADATAn

METADATA1

Note:  Remember that only 'Delimited' file type is supported.

Delimiter
The default delimiter that separates values is a pipe character. If your file uses a different delimiter, you must set the
delimiter you want your formula.

This example specifies a comma character as the delimiter.

/* Calculations */
IF OPERATION='FILETYPE' THEN
 OUTPUTVALUE='DELIMITED'
ELSE IF OPERATION='DELIMITER' THEN
 OUTPUTVALUE=','

Note:  Ensure that the delimiter you enter in the formula is a single non-ASCII character and not part of any of the
values to upload.

MAP
The MAP operation defines the return values related to a particular object. The return values must have the same
names as the attributes specified in the application for that object.

For example, these RETURN values can be used to generate an Element Entry dat file.

RETURN
 BusinessOperation,FileDiscriminator,FileName,AssignmentId,AssignmentNumber,CreatorType,DateEarned,EffectiveEndDate,EffectiveStartDate,ElementEntryId,ElementName,ElementTypeId,EntryType,GUID,LegislativeDataGroupId,LegislativeDataGroupName,MultipleEntryCount,Reason,SourceSystemId,SourceSystemOwner,Subpriority

Here, the BusinessOperation is set to MERGE and the BusinessObject is set to Element Entry.

METADATALINEINFORMATION
The application generates the file either with all defined attributes or with only specified attributes, depending on
whether you specify a value for METADATALINEINFORMATION or not.

1.

If you don't specify a value for METADATALINEINFORMATION, then the application generates METADATLINE in the
transformed file with all defined attributes for the business object.

90

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

2.

If you specify a value, then the transformed file will contain only the attributes that you specified.

For the METADATALINEINFORMATION operation, you specify an array per business object being processed in the formula.
The number of arrays should match the number specified in the NUMBEROFBUSINESSOBJECTS operation. The name
of the array should be METADATA with the number as suffix . For example, RETURN METADATA1, METADATA2 when the
NUMBEROFBUSINESSOBJECTS is 2.

Note: The first two entries in the array are reserved to specify the FileName and FileDiscriminator of the business object.

Additionally, for METADATALINEINFORMATION, you can specify attributes with special characters for that business objects.

Notice that in this example BalAdjBatchId(SourceSystemId) has parenthesis.

If the file contains either Flexfield or SourceSystem references, then the application can't resolve the default mapping of
output parameter names and attributes.

Let's consider this syntax: jobEffSegment1(PER_JOBS_EIT_EFF=context). To allow this construct to be generated in the
HCM Data Loader file, you define the METADATA line in the transformation formula. For each business object that appears
in the output, you must define the METADATA content in an array.

Example:

 METADATA2[1] = 'Job' /*FileName*/
 METADATA2[2] = 'JobExtraInfo' /*FileDiscriminator*/
 METADATA2[3] = 'EffectiveStartDate'
 METADATA2[4] = 'EffectiveEndDate'
 METADATA2[5] = 'JobCode'
 METADATA2[6] = 'SetCode'
 METADATA2[7] = 'FLEX:PER_JOBS_EIT_EFF'
 METADATA2[8] = 'EFF_CATEGORY_CODE'
 METADATA2[9] = 'InformationType'
 METADATA2[10] = 'JeiInformationCategory'
 METADATA2[11] = 'LegislationCode'
 METADATA2[12]= 'SequenceNumber'
 METADATA2[13]= 'jobEffSegment1(PER_JOBS_EIT_EFF=job-eff-context)'

Here's how the generated HCM Data Loader file looks like.

METADATA|JobExtraInfo|EffectiveStartDate|EffectiveEndDate|JobCode|SetCode|FLEX:PER_JOBS_EIT_EFF|
EFF_CATEGORY_CODE|InformationType|JeiInformationCategory|LegislationCode|SequenceNumber|
jobEffSegment1(PER_JOBS_EIT_EFF=job-eff-context)

NUMBEROFBUSINESSOBJECTS
This operation indicates the number of business objects being processed in the formula.

Related Topics

• Return Values for Payroll Transformation Formula for HCM Data Loader

• Sample Payroll Transformation Formula for HCM Data Loader

• Sample Payroll Transformation Formula for Multiple Business Objects

Return Values for Payroll Transformation Formula for HCM Data Loader
The return values for HCM Data loader formulas vary based on the business object and task action.

They are the same as the attribute names and must include BusinessOperation, FileName, and FileDiscriminator.

Here's an example of return values.

/*Return Values*/

91

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

RETURN BusinessOperation,FileName,FileDiscriminator,Attribute1,Attribute2,...,Attributen
/*Attributes for a particular Business Object can be found from the View Business Objects UI under the HCM
 Data Loader task in the Data Exchange Work Area */

For the NUMBEROFBUSINESSOBJECTS and METADATALINEINFORMATION operations, the RETURN statement is as follows.

/*Return Values for NUMBEROFBUSINESSOBJECTS and METADATALINEINFORMATION Operation*/
IF OPERATION='FILETYPE' THEN
 OUTPUTVALUE='DELIMITED'
ELSE IF OPERATION='DELIMITER' THEN
 OUTPUTVALUE='|'
ELSE IF OPERATION='READ' THEN
 OUTPUTVALUE='NONE'
ELSE IF OPERATION = 'NUMBEROFBUSINESSOBJECTS' THEN(
 OUTPUTVALUE = '2'
 RETURN OUTPUTVALUE
 )
ELSE IF OPERATION = 'METADATALINEINFORMATION' THEN
 (
 METADATA1[1] = 'BalanceAdjustmentHeader' /*FileName*/ /*Reserved*/
 METADATA1[2] = 'BalanceAdjustmentHeader' /*FileDiscriminator*/ /*Reserved*/
METADATA1[3] = 'LegislativeDataGroupName'
 METADATA1[4] = 'BatchName'
 METADATA1[5] = 'SourceSystemId'
 METADATA1[6] = 'SourceSystemOwner'

 METADATA2[1] = 'BalanceAdjustmentHeader' /*FileName*/ /*Reserved*/
 METADATA2[2] = 'BalanceAdjustmentGroup' /*FileDiscriminator*/ /*Reserved*/
 METADATA2[3] = 'EffectiveDate'
 METADATA2[4] = 'PayrollName'
 METADATA2[5] = 'LegislativeDataGroupName'
 METADATA2[6] = 'ConsolidationSetName'
 METADATA2[7] = 'BalAdjBatchId(SourceSystemId)'
 METADATA2[8] = 'SourceSystemId'
 METADATA2[9] = 'SourceSystemOwner'
 RETURN METADATA1, METADATA2 /*Only two as Return value for NUMBEROFBUSINESSOBJECTS is 2*/
 )

You can define variables with special characters. For example, use this structure to return the
BalAdjBatchId(SourceSystemId) Source ID.

/*Return Values for the MAP Operation*/
 FileName = 'BalanceAdjustmentHeader'
 BusinessOperation = 'MERGE'
 FileDiscriminator = POSITION1
 EffectiveDate = POSITION2
 PayrollName = POSITION3
 LegislativeDataGroupName = POSITION4
 ConsolidationSetName = POSITION5
 "BalAdjBatchId(SourceSystemId)"= POSITION6
 SourceSystemId = POSITION7
 SourceSystemOwner = POSITION8

 RETURN BusinessOperation, FileDiscriminator, FileName, EffectiveDate, PayrollName,
 LegislativeDataGroupName, ConsolidationSetName, "BalAdjBatchId(SourceSystemId)", SourceSystemId,
 SourceSystemOwner

/*Note BalAdjBatchId(SourceSystemId) is enclosed by double quotes while assigning value as well as while
 putting it in the return values list */

92

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Related Topics

Chapter 1
Let’s Get Started

• Overview of Payroll Transformation Formula For HCM Data Loader

• How You Transform Data Using Payroll Transformation Formula for HCM Data Loader

• Sample Payroll Transformation Formula for HCM Data Loader

• Sample Payroll Transformation Formula for Multiple Business Objects

Sample Payroll Transformation Formula
In this example, the transformation formula specifies the transformation mechanism for an incoming comma separated
delimited file. The formula's return values are the same as the list of attributes for the personal payment method object.

Here's the sample raw file for personal payment method, with comma as the delimiter.

2018/04/04,1,ZHRX_VS_US_TPPI_LDG_ONE,E955160008191423,ZHRX_VS_US_TPPI_Check,PPM1,M,10

And this code snippet has the formula for this example.

/******************************************************************
FORMULA NAME: Load Personal Payment Method
FORMULA TYPE: HCM Data Loader
******************************************************************/
/* Inputs */
INPUTS ARE OPERATION (text), LINENO (number), LINEREPEATNO (number),POSITION1 (text), POSITION2 (text),
 POSITION3 (text), POSITION4 (text), POSITION5 (text), POSITION6 (text), POSITION7 (text), POSITION8 (text)

DEFAULT FOR POSITION1 IS 'NO DATA'
DEFAULT FOR POSITION2 IS 'NO DATA'
DEFAULT FOR POSITION3 IS 'NO DATA'
DEFAULT FOR POSITION4 IS '2'
DEFAULT FOR POSITION5 IS '100'
DEFAULT FOR POSITION6 IS 'NO DATA'
DEFAULT FOR POSITION7 IS 'NO DATA'
DEFAULT FOR POSITION8 IS 'NO DATA'
DEFAULT FOR LINEREPEATNO IS 1

IF OPERATION='FILETYPE' THEN
 OUTPUTVALUE='DELIMITED'
ELSE IF OPERATION='DELIMITER' THEN

(
 OUTPUTVALUE=','
 RETURN OUTPUTVALUE
)
ELSE IF OPERATION='READ' THEN
 OUTPUTVALUE='NONE'
ELSE IF OPERATION='MAP' THEN
 /*HDL Related Outputs*/
 (
 FileName = 'PersonalPaymentMethod'
 BusinessOperation = 'MERGE'
 FileDiscriminator = 'PersonalPaymentMethod'
 EffectiveStartDate=POSITION1
 ProcessingOrder=POSITION2
 LegislativeDataGroupName=POSITION3
 AssignmentNumber=POSITION4
 OrganizationPaymentMethodCode=POSITION5
 PersonalPaymentMethodCode=POSITION6
 PaymentAmountType=POSITION7
 Amount=POSITION8
 RETURN
 BusinessOperation,FileName,FileDiscriminator,EffectiveStartDate,PersonalPaymentMethodCode,AssignmentNumber,Amount,ProcessingOrder,OrganizationPaymentMethodCode,PaymentAmountType,LegislativeDataGroupName

93

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

 )
ELSE
 OUTPUTVALUE='NONE'
RETURN OUTPUTVALUE
/* End Formula Text */

Related Topics

Chapter 1
Let’s Get Started

• Overview of Payroll Transformation Formula For HCM Data Loader

• How You Transform Data Using Payroll Transformation Formula for HCM Data Loader

• Sample Payroll Transformation Formula for Multiple Business Objects

Sample Payroll Transformation Formula for Multiple Business Objects
In this example, the formula uses the user defined tables and personal payment method business objects. It
converts the Person Number in the flat file into Assignment Number and uses the METADATALINEINFORMATION and
NUMBEROFBUSINESSOBJECTS operations.

Here's the sample of the raw input file.

PPM|2018/04/04|1|ZHRX_VS_US_TPPI_LDG_ONE|955160008191423|ZHRX_VS_US_TPPI_Check|PPM1|M|10
UDT|SM_UDT_4|Range|Number|Test UDT|USA LDG

And this code snippet has the formula for this example.

/**********************************************************
FORMULA NAME: Load User Defined Table and Personal Payment Method
FORMULA TYPE: HCM Data Loader
*************************************************************/
/* Inputs */
INPUTS ARE OPERATION (text), LINENO (number), LINEREPEATNO (number),POSITION1 (text), POSITION2 (text),
 POSITION3 (text), POSITION4 (text), POSITION5 (text), POSITION6 (text), POSITION7 (text), POSITION8
 (text),POSITION9 (text)
DEFAULT FOR POSITION1 IS 'NO DATA'
DEFAULT FOR POSITION2 IS 'NO DATA'
DEFAULT FOR POSITION3 IS 'NO DATA'
DEFAULT FOR POSITION4 IS '2'
DEFAULT FOR POSITION5 IS '100'
DEFAULT FOR POSITION6 IS 'NO DATA'
DEFAULT FOR POSITION7 IS 'NO DATA'
DEFAULT FOR POSITION8 IS 'NO DATA'
DEFAULT FOR POSITION9 IS 'NO DATA'
DEFAULT FOR LINEREPEATNO IS 1
IF OPERATION='FILETYPE' THEN
 OUTPUTVALUE='DELIMITED'
ELSE IF OPERATION='DELIMITER' THEN
 OUTPUTVALUE='|'
ELSE IF OPERATION='READ' THEN
 OUTPUTVALUE='NONE'
ELSE IF OPERATION = 'NUMBEROFBUSINESSOBJECTS' THEN
 (
 OUTPUTVALUE = '2'
 RETURN OUTPUTVALUE
 )
ELSE IF OPERATION = 'METADATALINEINFORMATION' THEN
 (
 METADATA1[1] = 'UserDefinedTable' /*FileName*/
 METADATA1[2] = 'UserDefinedTable' /*FileDiscriminator*/
 METADATA1[3] = 'UserTableCode'
 METADATA1[4] = 'RangeOrMatch'
 METADATA1[5] = 'UserKeyUnits'
 METADATA1[6] = 'UserRowTitle'
 METADATA1[7] = 'UserTableName'

94

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

 METADATA1[8] = 'LegislativeDataGroupName'
 METADATA2[1] = 'PersonalPaymentMethod' /*FileName*/
 METADATA2[2] = 'PersonalPaymentMethod' /*FileDiscriminator*/
 METADATA2[3] = 'EffectiveStartDate'
 METADATA2[4] = 'PersonalPaymentMethodCode'
 METADATA2[5] = 'AssignmentNumber'
 METADATA2[6] = 'Amount'
 METADATA2[7] = 'ProcessingOrder'
 METADATA2[8] = 'OrganizationPaymentMethodCode'
 METADATA2[9] = 'PaymentAmountType'
 METADATA2[10] = 'LegislativeDataGroupName'
 RETURN METADATA1, METADATA2
 )
ELSE IF OPERATION='MAP' THEN

 IF POSITION1='UDT' THEN
 (
 FileName = 'UserDefinedTable'
 BusinessOperation = 'MERGE'
 FileDiscriminator = 'UserDefinedTable'
 UserTableCode = POSITION2
 IF POSITION3='Range' THEN
 (
 RangeOrMatch = 'R'
 )
 IF POSITION4='Number' THEN
 (
 UserKeyUnits = 'N'
 )
 UserRowTitle = POSITION5
 UserTableName = POSITION2
 LegislativeDataGroupName = POSITION6
 RETURN
 BusinessOperation,FileDiscriminator,FileName,UserTableCode,RangeOrMatch,UserKeyUnits,UserRowTitle,UserTableName,LegislativeDataGroupName
 )
 IF POSITION1='PPM' THEN
 (
 FileName = 'PersonalPaymentMethod'
 BusinessOperation = 'MERGE'
 FileDiscriminator = 'PersonalPaymentMethod'
 EffectiveStartDate=POSITION2
 ProcessingOrder=POSITION3
 LegislativeDataGroupName=POSITION4
 AssignmentNumber=GET_VALUE_SET('SAMPLE_GET_ASG_NUM','|=PERSON_NUMBER='''||POSITION5||'''')
 OrganizationPaymentMethodCode=POSITION6
 PersonalPaymentMethodCode=POSITION7
 PaymentAmountType=POSITION8
 Amount=POSITION9
 RETURN
 BusinessOperation,FileName,FileDiscriminator,EffectiveStartDate,PersonalPaymentMethodCode,AssignmentNumber,Amount,ProcessingOrder,OrganizationPaymentMethodCode,PaymentAmountType,LegislativeDataGroupName
 )
ELSE
 OUTPUTVALUE='NONE'
RETURN OUTPUTVALUE
/* End Formula Text */

Note:  To debug value sets, create a BI report with this query to return the required data.

SELECT pay_ff_functions.gvs ('SAMPLE_GET_ASG_NUM','|=PERSON_ID=100000012092216') value FROM dual;

95

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Related Topics

• Overview of Payroll Transformation Formula For HCM Data Loader

• How You Transform Data Using Payroll Transformation Formula for HCM Data Loader

• How To Create A Program for Automation

Chapter 1
Let’s Get Started

Payroll Transformation Formula for HCM Spreadsheet Data Loader

Overview of Payroll Transformation Formula for HCM Spreadsheet Data Loader
You can use HCM Spreadsheet Data Loader to load all payroll objects that HCM Data Loader supports.

As the first step,you create a spreadsheet template for the required object from the Data Exchange Work area and
further download the template in CSV format. You can download CSV and XML file templates from a spreadsheet
template. The Payroll Transformation Formula for HCM Spreadsheet Data Loader transforms the raw delimited file to a
format that suits the template.

This figure summarizes the process of transforming data that's uploaded using HCM Spreadsheet Data Loader.

96

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Here's a summary of how the transformation process works.

1. On the Home page, click the Submit a Flow quick action under the My Clients Groups tab. Submit the Load

Spreadsheet Data File flow pattern.

The flow is secured using these privileges:

Flow

Privilege

Submit Payroll

PAY_SUBMIT_PAYROLL_FLOW_PRIV

Load Data using HCM Spreadsheet

Data Loader

HRC_LOAD_DATA_USING_HSDL_PRIV

2. This flow pattern invokes the transformation formula for the Content ID and has these tasks:

a. Generate Data Loader File
b.

Initiate Spreadsheet Data Loader

3. The Generate Data Loader File task reads the data file line by line, producing an equivalent HCM Spreadsheet

Data Loader format for each line. Finally, it creates a compressed file of all the transformed data files and
uploads it to Oracle WebCenter Content server.

4. The Initiate Spreadsheet Data Loader task takes the compressed file generated by the Generate Data Loader

File  task and invokes the HCM Spreadsheet Data Loader. The HCM Spreadsheet Data Loader creates the
required data in the HCM Cloud.

Related Topics

• Guidelines for Using HCM Spreadsheet Data Loader

• How Data Is Uploaded Using HCM Spreadsheet Data Loader

• HCM Spreadsheet Data Loader Templates

• Create and Edit Spreadsheet Templates

• Guidelines for Designing Spreadsheet Templates

Sample Payroll Transformation Formula for HCM Spreadsheet Data Loader
In this example, the transformation formula specifies the transformation mechanism for an incoming pipe separated
delimited file. The formula's return values are the same as the list of attributes in the template file for the User Defined
Table business object.

And this code snippet has the formula for this example.

/* Inputs */
INPUTS ARE OPERATION (text), LINENO (number), LINEREPEATNO (number),POSITION1 (text), POSITION2 (text),
 POSITION3 (text), POSITION4 (text), POSITION5 (text), POSITION6 (text), POSITION7 (text), POSITION8 (text)
DEFAULT FOR POSITION1 IS 'NO DATA'
DEFAULT FOR POSITION2 IS 'NO DATA'
DEFAULT FOR POSITION3 IS 'NO DATA'
DEFAULT FOR POSITION4 IS 'NO DATA'
DEFAULT FOR POSITION5 IS 'NO DATA'
DEFAULT FOR LINEREPEATNO IS 1
IF OPERATION='FILETYPE' THEN
OUTPUTVALUE='DELIMITED'
ELSE IF OPERATION='DELIMITER' THEN

97

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

OUTPUTVALUE='|'
ELSE IF OPERATION='READ' THEN
OUTPUTVALUE='NONE'
ELSE IF OPERATION = 'NUMBEROFBUSINESSOBJECTS' THEN
(
OUTPUTVALUE = '1'/*Always be 1*/
RETURN OUTPUTVALUE
)
ELSE IF OPERATION = 'METADATALINEINFORMATION' THEN
(
METADATA1[1] = 'SMUDT' /*TemplateCode*/
METADATA1[2] = 'UserDefinedTable' /*FileDiscriminator*/
METADATA1[3] = 'UserDefinedTable_UserTableCode'
METADATA1[4] = 'UserDefinedTable_LegislativeDataGroupName'
METADATA1[5] = 'UserDefinedTable_UserTableName'
METADATA1[6] = 'UserDefinedTable_RangeOrMatch'
METADATA1[7] = 'UserDefinedTable_UserRowTitle'
METADATA1[8]= 'UserDefinedTable_UserKeyUnits'
RETURN METADATA1 /*You can return only one METADATA for the respective template*/
)
ELSE IF OPERATION='MAP' THEN
(
FileName = 'SMUDT'
BusinessOperation = 'HSDL'
FileDiscriminator = 'UserDefinedTable'
UserDefinedTable_UserTableCode = POSITION1
UserDefinedTable_LegislativeDataGroupName = POSITION2
UserDefinedTable_UserTableName = POSITION1
UserDefinedTable_RangeOrMatch = POSITION3
UserDefinedTable_UserRowTitle = POSITION4
UserDefinedTable_UserKeyUnits = POSITION5
RETURN
 BusinessOperation,FileDiscriminator,FileName,UserDefinedTable_UserTableCode,UserDefinedTable_LegislativeDataGroupName,UserDefinedTable_UserTableName,UserDefinedTable_RangeOrMatch,UserDefinedTable_UserRowTitle,UserDefinedTable_UserKeyUnits
)
ELSE
OUTPUTVALUE='NONE'
RETURN OUTPUTVALUE
/* End Formula Text */

Note:  The template code needs to be used in the Fast Formula.

Related Topics

• Guidelines for Using HCM Spreadsheet Data Loader

• How Data Is Uploaded Using HCM Spreadsheet Data Loader

• HCM Spreadsheet Data Loader Templates

• Create and Edit Spreadsheet Templates

• Guidelines for Designing Spreadsheet Templates

User Defined Tables

Example to Create a User-Defined Table for Matched Row Values
User-defined tables store a date effective list of values that you can use in a formula. Set up your own structured tables
to hold data such as wage codes or shift differentials.

98

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

In this example, you create a user-defined table to store values for workers' schedules. To create a new table, use the
User-Defined Tables task in the My Clients Group tab.

Scenario
Your organization works on a 10 hour a day, four day a week rotating schedule. The employees work for four
consecutive days, 10 hours a day.

User-Defined Table Components
These are the main components of the user-defined table.

• Basic details

• Columns

• Rows

• Values

As this figure shows, the user-defined table contains the schedules available in your organization.

Resulting User-Defined Table Components
This table shows the resulting user-defined table components for this scenario.

Component

Basic Details

In This Example

The Unit of measure is a text because the row values are Days of the Week.

The row title is Days of the Week.

Rows

Contain the name of a day of the week.

99

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Component

Columns

In This Example

These are the schedules, such as Monday - Thursday. The data type for each column is number
because they hold a count of hours.

Values

Represent the number of hours to work each day in each schedule.

Related Topics

• User Table Validation Formula Type

Example to Create a User-Defined Table for a Range of Row Values
Click the User-Defined Tables quick action under the My Clients Groups table to create a user-defined table to store
values for stock option allocations.

Scenario
Each year, your organization offers stock options to its employees. The amount of options depends on years of service
and job category of the employee receiving them.

User-Defined Table Components
The main components of the user-defined table are the definition, columns, rows, and values.

• Basic details

• Columns

• Rows

• Values

As this image shows, the user-defined table contains stock option allocations by job category and years of service.

100

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Resulting User-Defined Table Components
This table shows the resulting user-defined table components for this scenario.

Component

Basic Details

Rows

Columns

Values

In This Example

The unit of measure is a number since the row values are years. The row title is Years of Service.

Represent a range of years of service during which employees receive the same number of stock
options.

Represent job categories and the data type of each column is number because they hold a number of
stock options.

Represent the number of stock options awarded to the specified job category during the specified
years of service.

Related Topics

• User Table Validation Formula Type

Create a User-Defined Table
In this example, you create a user-defined table to hold the bonus percentages based on a person's years of service and
department.

101

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

This table shows the various user-defined table components and values for those components:

• Rows represent the years of service.

• Columns represent the department.

Years of Service

Accounting

Payroll

1-5

6-10

11-99

.10

.20

.30

Step 1: Create a User-Defined Table

.08

.16

.24

1. On the Home page, click the User-Defined Tables quick action under the My Clients tab.
2. On the User-Defined Tables page in the Search Results area, click Create.
3. On the Create User-Defined Table dialog box, in the Legislative Data Group field, select US Legislative Data

Group.
In the Effective As-of Date field, enter 1/1/2016.

4.
5. Click Continue.
6. On the Create: User-Defined Table page in the Basic Details section in the Name field, enter Bonus_Percent.
7.
8.

In the Range or Match field, select Range.
In the Row Title field, enter Years of Service.

Step 2: Define the Accounting and Payroll Columns

1.

In the User-Defined Columns section, click Create.

◦ In the Column Name field, enter Accounting.
◦ In the Data Type  field, select Number.
In the User-Defined Columns section, click Create.

2.

◦ In the Column Name field, enter Payroll.
◦ In the Data Type field, select Number.

Specify the Bonus Percent Range

1.

In the User-Defined Rows section, click Create.

◦ In the Sequence field, enter 10.
◦ In the Low Range field, enter 1 as the low range.
◦ In the High Range field, enter 5 as the high range.

2.

In the User-Defined Rows section, click Create.

◦ In the Sequence field, enter 20.

102

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

◦ In the Low Range field, enter 6 as the low range.
◦ In the High Range field, enter 10 as the high range.

3.

In the User-Defined Rows section, click Create.

◦ In the Sequence field, enter 30.
◦ In the Low Range field, enter 11 as the low range.
◦ In the High Range field, enter 99 as the high range.

Step 4: Add Table Values for the Accounting Column

In the User-Defined Columns section, click Accounting.

1.
2. Click Next.
3. On the Create User-Defined Table: User-Defined Table Values page in the User-Defined Table Values section,

click Create.

◦ On the Add User-Defined Table Values dialog box, select the first row, and then click OK.
◦ In the Value field, enter .10.

4. Click Create.

◦ On the Add User-Defined Table Values dialog box, select the second row, and then click OK.
◦ In the Value field, enter .20.

5. Click Create.

◦ On the Add User-Defined Table Values dialog box, select the third row and click OK.
◦ In the Value field, enter .30.

Step 5: Add Table Values for the Payroll column.

In the User-Defined Columns section, click Payroll.

1. Click Back.
2.
3. Click Next.
4. On the Create User-Defined Table: User-Defined Table Values page in the User-Defined Table Values area, click

Create.

◦ On the Add User-Defined Table Values dialog box, select the first row, and then click OK.
◦ In the Value field, enter .08.

5. Click Create.

◦ On the Add User-Defined Table Values dialog box, select the second row, and then click OK.
◦ In the Value field, enter .16.

6. Click Create.

◦ On the Add User-Defined Table Values window, select the last row, and then click OK.
◦ In the Value field, enter .24.

7. Click Submit.
8. On the User-Defined Tables page, click Done.

103

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

User Table Validation Formula Type
The User Table Validation formula type validates entries in user-defined tables. When you create or edit user-defined
tables, select the formula in the Formula field for the user-defined columns.

You can use this formula type to ensure that entries are:

• Between a specified range

• Don’t contain a negative value

You can use the EFFECTIVE_DATE (text) context for formulas of this type.

You must use one input variable called ENTRY_VALUE of data type text.

These return values are available to formulas of this type:

Return Value

Data Type

Required

Description

FORMULA_MESSAGE

Text

FORMULA_STATUS

Text

N

Y

Returns a text message for either
or both statuses. The message
is displayed on the Create User-
Defined Table: User-Defined Table
Values page.

Returns the value S (success) or E
(error).

This formula checks whether the deduction value entered in the Union A column of the Union Dues table is between
10.00 and 20.00:

/* Formula Name: Union A Dues Validation */
/* Formula Type: User Table Validation */
INPUTS ARE entry_value (text)
IF TO_NUMBER(entry_value) < 10.00 OR
TO_NUMBER(entry_value) > 20.00
THEN
(
formula_status = 'e'
formula_message = 'Error: Union A dues must be between $10.00 and $20.00.'
)
ELSE
(
formula_status = 's'
formula_message = ' '
)
RETURN formula_status, formula_message

Fast Formulas

Overview of Using Fast Formulas
Fast Formula is a simple way to write formulas using English words and basic mathematical functions. You can use
information from your database in formulas without learning the database structure or a programming language.

104

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

The Elements task generates standard element skip and calculation formulas, and you can modify these formulas
based on your requirements. Use the Fast Formulas task to use formulas corresponding to one or more formula types,
requiring specific formula inputs and outputs.

Uses of formula in payroll include:

• Control Processing

◦ Payroll flow patterns: Control the repetition of a payroll flow.
◦ Element skip: Control when elements are processed in a payroll run.
◦ Work or payroll relationship groups: Define a set of people for payroll processing, data entry, or reporting.

• Configuration

◦ Configure payment method preferences. For example, you can limit the number and types of payment

methods.

• Validation

◦ Element entry validation: Validate one or more element entry values. Provide a default value for an
element entry value, or calculate entry values based on the user's entries in other entry values.

◦ User table validation: Validate entries in user-defined tables.

• Calculation

◦ Proration formulas control how payroll runs prorate element entries when they encounter an event such

as a mid-period change in an element entry value.

◦ Associate more than one payroll formula with each element to perform different processing for employee

assignments with different statuses.

• Data Loading

◦ Transformation formulas convert inbound data into a format that HCM Data Loader understands.

Note:   Refer Using Fast Formula guide for more information about the general formula concepts.

Example of Writing a Fast Formula Using Formula Text
In this example, you use the text editor to create a fast formula.

Here are the key decisions when deciding on which formula to create:

Key Decisions

In This Example

Is the formula for a specific legislative data
group?

No, this is a global formula that can be used by any legislative data group.

Are there any contexts used in this
formula?

No

Are there any database item defaults?

Yes, PER_ASG_JOB_NAME

105

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Key Decisions

In This Example

Are there any input value defaults?

No

What are the return values?

MIN_HOURS, MAX_HOURS, FREQUENCY

Creating a Fast Formula Using the Text Editor to Determine a Manager's Scheduled Hours

1. Search for and select Fast Formulas in My Client Groups.
2. Click Create.
3. Complete these fields:

Fields for the Fast Formula

Values for the Fast Formula

Formula Name

Manager Range of Scheduled Hours

Formula Type

Range of Scheduled Hours

Description

Manager's Range of Hours

Effective Start Date

1-Jan-2010

4. Click Continue.
5. Enter these formula details in the Formula Text section:

/* DATABASE ITEM DEFAULTS BEGIN */
DEFAULT FOR per_asg_job_name IS ' '
/* DATABASE ITEM DEFAULTS END */
JOB_1 = PER_ASG_JOB_NAME
IF JOB_1 = 'Manager' then
(MIN_HOURS = 25
MAX_HOURS = 40
FREQUENCY = 'H')
else
(MIN_HOURS = 20
MAX_HOURS = 35
FREQUENCY = 'H')
return MIN_HOURS, MAX_HOURS, FREQUENCY

6. Click Compile.
7. Click Save.

Example of Writing a Fast Formula Using Expression Editor
In this example, you create a fast formula that groups executive workers for reporting and processing. All executive
workers are in department EXECT_10000.

After you create the formula, you need to add it to the object group parameters, so that only the workers that belong to
the EXECT_10000 department are used in processing.

106

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Here are the key decisions when deciding on which formula to create.

Key Decisions

In This Example

Is the formula for a specific legislative data
group?

Yes, InVision

What's the formula type for this formula?

Payroll Relationship Group

Creating a Fast Formula Using the Expression Editor

1. On the Home page, click the Fast Formulas quick action under the My Client Groups tab.
2. Click Create.
3. Complete these fields:

Fields for Fast Formula

Values for Fast Formula

Formula Name

Executive Payroll Relationship Group

Type

Payroll Relationship Group

Description

Executive Workers

Legislative Data Group

Vision LDG

Effective As-of Date

1-Jan-2010

Type of Editor

Expression Builder

Note:

For more complex conditions to create a group, you can select Text. However, after you save

the formula, you can't change the type of editor.

4. Click Continue.
5.

In the Formula Details section, click Add After to add a row and complete these fields:

Conjunction

Database Item Name

Data Type

Operand

Literal Value

None applicable

DEPARTMENT

Character

And

SELECT_EMP

Character

=

=

'EXECT_10000'

'YES'

107

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Conjunction

Database Item Name

Data Type

Operand

Literal Value

6. Click Compile.
7. Click Save.

When do I run the Compile Formula process?
When you create or update multiple fast formulas simultaneously, run the Compile Formula process on the Submit a
Process or Report page.

Payroll Flows

Overview of Payroll Flows
Use payroll flows to streamline and optimize your payroll operations. They help you ensure smooth and seamless end-
to-end execution of the processes that address all of your payroll business requirements.

Use payroll flows to manage, effectively and efficiently, all your payroll tasks, such as calculating payrolls, running
reconciliation reports, and making payroll payments.

For example, to ensure your payroll cycles are accurate, you can design a flow that includes manual tasks that request
validation at each step in the process. In this way, your Financial Director can verify the payroll costing results before the
flow transfers the payroll costs to the general ledger.

Predefined flow patterns are automatically available for you to submit all types of payroll processes and reports. A flow
pattern can consist of a single task such as the Calculate Payroll flow, or multiple tasks, such as the Payroll Cycle flow.
The Payroll Cycle flow includes all tasks for a payroll period in a best practice flow.

You can run the predefined flows directly, or you can use them as templates to create your own. You can even copy a
predefined flow pattern and edit it to meet your business requirements, such as adding, deleting, or moving a task in
the schedule.

There are also features to help you to design flows that address other complex business requirements, such as the
task iterator, that automates repetitive tasks with a single flow submission. For example, use the task iterator option to
generate a report for multiple payroll statutory units within your organization.

Similarly, use the flow connectors feature to isolate and review off-cycle and on-cycle payroll runs and subsequently
combine the run results for downstream processing.

This workflow diagram gives you an understanding of how payroll flows work. It shows the navigation path from
the pages that provide high-level flows information, such as the View Flows page, to the pages that provide detailed
employee-level information, such as the Checklist and Process Results Details pages.

108

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

This table gives you a list of the payroll flow pages and a high-level description of the ongoing tasks you can perform to
submit and monitor your flows.

Page Name

Submit a Flow

Tasks You Can Do On the Page

After you have created the flow pattern, use the Submit a Flow page to submit the flow. Navigate to
Submit a Flow task from Quick Actions or under Payroll in My Client Groups.

Use the filter options and search for the flow you want to submit. Enter a unique name for the flow and
use the appropriate sections on the page to enter flow parameters, schedule your flow, and link flows if
required.

109

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Page Name

Checklist

Tasks You Can Do On the Page

A Checklist is generated for each submitted flow. The Checklist page provides a central point to
monitor and manage all tasks within the flow. Use the Checklist to easily identify areas that require
your attention, such as any tasks within your flow that have error messages.

Perform actions on the Checklist page, such as roll back a task or mark a manual task as complete. To
view further information for a specific task, select the task and navigate to the Process Results Details
page.

Process Results Details

Use the Process Results Details page to view more detailed information for a flow task, such as errors
and warning messages, report output, and log files.

Errors and Warnings

Use the Errors and Warnings page to view messages pertaining to persons or processes. You can also
access this page from the Process Results Summary.

View Flows

Once you resolve all issues, navigate back to the Checklist page to continue processing any remaining
tasks within your flow.

Use the View Flows page to get an overall status of all submitted flows. Use the filter options on
the page to identify flows that require your attention, such as a flow that includes tasks with error
messages. Drill down on a flow to go to the Checklist page, to get more detailed information for the
tasks within the flow.

Navigate to View Flows task from Quick Actions or under Payroll in My Client Groups.

For more information on payroll flows, refer to the Administering Payroll Flows guide on the Oracle Help Center.

Related Topics

• Flow Pattern Components

• Payroll Flow Patterns

Flow Pattern Components
Before you begin to use flow patterns, let's walk you through a delivered flow pattern to understand flow components.

Use the Payroll Flow Patterns task under Payroll in My Client Groups to search and select a flow pattern.

For example, search for the predefined Calculate Payroll flow and click Edit. While creating your own flow pattern, select
field options or values based on the information in this table.

Field

Flow Status

Description

Use this field to define how you can submit the flow. Select one of these options:

• Active flow, to submit the flow from the flow submission page or to include the flow in automated

flow submissions.

•

Inactive flow, to submit the flow through automated flow submissions. The flow isn't available for
submission on the flow submission page.

• Hidden flows aren't available for submission.

Connector Status

Use this field to decide what you want to include in the flow results. Select either of these options:

110

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Field

Description

Connector Name

LDG Required

• Task Flow, to consolidate results generated from tasks within the current flow and those from

other connected flows.

• Parameters Only flow, to include results generated from tasks within the flow. It doesn't include

results from any additional flows.

Use this field to identify the flow pattern for the purpose of flow connector rules. This field is defaulted
to the name of your flow pattern.

Use this field to determine availability of the flow to other legislative data groups (LDGs). Select either
of these options:

• Yes, to restrict the flow to a single LDG.

• No, to indicate that the flow is available to all other LDGs.

Use these tabs on the Payroll Flow Patterns page to define more flow components and tasks within the flow.

Flow Connectors
Use the Connector tab to link flows at the flow pattern level and consolidate flow results for downstream processing.
Use the Connected Flows field to select flows you want to connect to consolidate payroll results. The rules are
automatically applied to all instances of the flow and you don't have to manually define connector rules each time you
submit the flow.

For more information, refer to Considerations to Configure Flow Connectors topic in the Help Center.

Tasks
Review the task list, and if necessary, add new tasks to the flow pattern. You can edit the task name, description, and its
placement in an activity or task group.

The Activity and Task Group define how the submitted flow instance is viewed hierarchically in the Checklist. In this
example, the activity is 'Calculate' and the task group is 'Calculate and Validate Payroll'.

Edit the task to update the task parameters, owner and checklist information, and which notifications to send the task
owner.

Optionally, select the Process after Error check box against a task, to allow a subsequent task to process, even if an
immediately preceding task is in error. This ensures continuation of the flow.

For example if you have a flow with tasks, A ->B -> C, task B can't run if task A is in error, unless you select Process
after Error for task B. Similarly, task C will run irrespective of the status of task B, if you select Process after Error for
task C. After you complete the flow, you can view the errors, make corrections, roll back the errors, and resubmit the
flow, if required.

Task Sequence
Since there is only one task for this flow, the sequence of the flow tasks is Start Flow > Calculate Payroll > End Flow.

For more complex multi-task flows, use the Task Sequence tab to review the task sequence and reorder, add or delete
tasks, as required. Some tasks within the flow use and build upon the results of a previous task.

111

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Parameters
Use the Parameters tab to define flow parameters, some of which you manually enter while submitting the flow, and the
others are default or derived values. Define the properties of the parameters here. For example, indicate if a parameter
is mandatory or optional, display the parameter on the UI or not, display format, and so on.

For more information, refer to Flow Pattern Parameters topic in the Help Center.

Outbound Integration
Use the Outbound Integration tab to configure an outbound notification with the payroll flows outbound API
notifications feature. Once a task in a flow completes, it sends a completion message to an external downstream
server. The server gets an automatic notification once the task completes, and it then triggers downstream non-payroll
processes.

Review
Use the Review tab to preview how the flow is organized and displayed on the Checklist page.

Related Topics

• Considerations to Configure Flow Connectors

• Flow Pattern Parameters

• Sequencing Rules for Flows and Locked Tasks

Payroll Background Logging and Monitoring Flow
Use the Payroll Background Logging and Monitoring flow to identify and help resolve payroll queries for features that
use the payroll background flow.

This flow helps you track the status of a process and troubleshoot issues. It's useful for those who manage customer
environments, test payroll processes, and troubleshoot issues with payroll processes. For example, your system
administer can use this flow to generate log files for features that uses the payroll background flow such as Anytime Pay.

Note:  These are the payroll features that use the payroll background flow:

• Anytime Pay

• Event Notification Processing that has rate events enabled

The payroll background process is an ESS process that runs continuously in the background to improve the
performance of payroll features. Since it runs continuously, it’s not required for the ESS server to start or stop whenever
you submit a process, such as the submission of the QuickPay process for Anytime Pay.

When you submit the flow, leave the Legislative Data Group field blank.

Use the Action field to perform any of these actions on the flow.

• Start Process: When called by a feature, the background payroll ESS process starts automatically and will

continue to run. Use this option to override this default behavior and manually start the process.

• Stop Process: Use this option to stop the background payroll ESS process. Any process that's already running

using the payroll background process will complete, but the next process in queue will not start.

• Report: Use this option to report on the status of the background payroll ESS process.

112

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

• Resubmit Process: Use this option to resubmit a process submitted using the background payroll ESS process

and is in error.

Use the Job Identifier field to identify a process that’s submitted using the payroll background and that needs a log file
or must be resubmitted. Each background process has a job ID number, similar to an ESS job number.

Use the Report Type field to select the type of report you want to generate using this flow. You can use these reports to
identify the root cause of an issue. The types of reports you can generate are:

• Processing Report: This report displays all processes that are currently running or are in the payroll

background queue for the day. For example, a QuickPay has been submitted for Anytime Pay but no results are
generated for the employee. Use this report to check if the QuickPay is stuck in a queue of processes waiting to
be completed by the payroll background process.

• Scheduled Report: This report identifies all pending processes in the payroll background queue for the

specified date range.

• Error Report: This report identifies all error messages for the payroll background process. For example, you
have submitted a QuickPay for Anytime Pay but no results are generated for the employee. Use this report to
check if the payroll background process has hit an error that stopped the submission.

• Log File: Use this option to enable detailed logging information for a process submitted using the payroll

background process.

Prerequisite Tasks

You'll find most of the setup tasks required for payroll processing in the Define Payroll task list in the Setup and
Maintenance work area.

There are required common application configuration tasks you may have already done because other HCM
applications require them. You may want to revisit tasks to address payroll-specific requirements,such as when you
create tax reporting units, to verify.

If these prerequisite tasks haven't been completed, you can find them within Define Common Applications
Configuration for Human Capital Management:

• Define Features by Country or Territory

• Define Geographies for HCM

• Define Enterprise Structures for HCM

Define Geographies for HCM
Verify predefined geographies, and define any other required local geographies.

For further information, see these topics in the Help Center:

• Geography Structures: Explained

• Geography Validation: Explained

Define Enterprise Structures for HCM
Complete tasks in the task lists shown in this table.

113

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Task List

Action

Chapter 1
Let’s Get Started

Define Legal Jurisdictions and Authorities
for HCM

• Create a legal jurisdiction if not already created or predefined for your country or territory.

• Create a legal authority for each government body you interact with.

• Create addresses for legal entities and legal authorities.

Define Legal Entities for HCM

• Create a legislative data group for each country or territory you operate in, to partition your

payroll data.

• Create at least one legal entity designated as a payroll statutory unit (PSU) for each legislative

data group.

• Associate each PSU with a legislative data group.

• Create calculation cards for statutory deductions for each PSU, if supported for your country or

territory.

Define Legal Reporting Units for HCM

• Create any other legal reporting units that you need under a PSU and designate them as tax

reporting units (TRUs).

• Define the TRUs as reporting establishments as needed.

• Optionally, create calculation cards for statutory deductions for each TRU, if supported for your

country or territory.

Define Business Units for HCM

Create business units that you can use to perform one or more business functions.

Define Chart of Accounts for Enterprise
Structures

Create business units that you can use to perform one or more business functions.

Define Accounting Configurations for HCM

Create charts of accounts, ledgers, and accounting calendars. When you create a bank for a payment
source, you must select a legal entity that's assigned to a ledger for the associated legislative data
group. Payroll costing also requires these financial components.

Define Features by Country or Territory
Review and update the selected features for your countries and territories of operation. These settings control the
availability of payroll-related features, such as element templates, and address style and address validation rules used in
processes and reports.

Related Topics

• How Legal Employers Work with Payroll Statutory Units and Tax Reporting Units

• Legislative Data Groups

• Payroll Setup Tasks for Financials

• How Country Extensions are Selected

Setup Task List for HCM

To start an implementation of Oracle HCM Cloud Service, you must have an application implementation consultant role.
Select an offering to implement and generate the setup tasks.

114

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

The Service Administrator creates this user. Instructions for how to create this user are included in the post-provisioning
notification.

Payroll Managers and Application Implementation Consultants use the Setup and Maintenance work area to open the
setup pages associated with the Oracle HCM Cloud Service features. The Setup and Maintenance work area is also
known as the Functional Setup Manager.

Generate the Setup Task List
This figure illustrates the offering in which each HCM feature is located.

Here's how you can generate the setup tasks. The documentation in this list is in the Oracle Applications Cloud Using
Functional Setup Manager guide.

1. Sign in to Oracle Cloud Services.

◦ Using the Oracle Cloud Services URL, sign in to Oracle Cloud Services as a user with the application

implementation consultant role.

The Welcome page appears.
2. Go to the Setup and Maintenance work area.

◦ Select Setup and Maintenance under the Tools category in the Navigator to go to the Setup and

Maintenance work area.

3. Browse offerings on the Getting Started page.

◦ On the Getting Started with Oracle Fusion Applications page, view all Oracle Fusion Applications

offerings.

115

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

4. Analyze implementation requirements of the offerings.

◦ Drill down on the Oracle HCM offering of your choice to view a description, documents, and reports

related to the offering on the Documents page.

5. Configure the offerings.

◦ On the Configure Offerings page, configure the offerings of your choice to fit your business

requirements.

Expand any offering to find its optional offerings, called Optional Functional Areas. Select all that apply to
your organization.

Use the Select Feature Choices page to review optional or alternative business processes. Select all
that apply to your enterprise. If you select the Payroll functional area, you must select the appropriate
countries as feature choices.

Note:  To use the Enterprise Structures Configurator, you must Select the Enterprise Structures Guided
Flow feature on the Configure Offerings page. This feature is selected by default. Use the feature to set
up enterprise structures.

6. Generate setup tasks.

◦ Create a new implementation project on the Manage Implementation Projects page to generate setup

tasks for a selected offering.

7. Review the generated setup task list.

◦ The task list includes the tasks that are relevant to the offerings and optional functional areas that you
selected. The most common requirements across all offerings are listed first. Next, the common tasks
across product families are shown, and then the common tasks across product offerings. Tasks that are
specific to product functionality are listed last.

You can expand the task lists to see the tasks that they contain. For more information about the
Functional Setup Manager, see the Oracle Applications Cloud Using Functional Setup Manager guide.

Implementation Tasks
This table lists the task areas and their associated roles.

Task Area

Role

Work Area

Define Geographies for Human Capital
Management

Application Implementation Consultant

Setup and Maintenance

Defining Enterprise Structures

Application Implementation Consultant

Setup and Maintenance

Defining Features by Country or Territory

Application Implementation Consultant

Setup and Maintenance

Manage Currencies

Application Implementation Consultant

Setup and Maintenance

Defining Elements, Balances, and Formulas

Application Implementation Consultant

Setup and Maintenance

116

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Task Area

Role

Work Area

Managing Data Security

IT Security Manager

Setup and Maintenance

Define Payroll Business Definitions

Application Implementation Consultant

Setup and Maintenance

Define Pay Frequency

Application Implementation Consultant

Setup and Maintenance

Define Earnings and Deductions Definitions

Application Implementation Consultant

Setup and Maintenance

Define Events

Application Implementation Consultant

Setup and Maintenance

Define Payment Methods

Application Implementation Consultant

Setup and Maintenance

Define Payroll Costing

Application Implementation Consultant

Setup and Maintenance

Define Object Groups

Application Implementation Consultant

Setup and Maintenance

Define Payroll Flow Patterns

Application Implementation Consultant

Setup and Maintenance

Setup Task List for Financials

Because payroll and payroll costing rely on and integrate with components of other applications, you must set up the
components in Financials, such as charts of accounts and ledgers.

Set up the financial components before you set up components in Payroll, such as banks to process payments, associate
a ledger to a payroll definition, and run processes to distribute costing results.

Complete these setup tasks to create the chart of accounts and ledgers. You can perform these tasks with the
application implementation consultant job role can perform these tasks.

Chart of Account Setup
Complete these tasks to set up your chart of accounts information. Later, you associate the chart of accounts to a
ledger.

Task

Value Sets

Structures

Action

Create new or review existing value sets, which you will associate with a key flexfield segment.

Create account structures that specify the segments to include, their order, and the value sets that will
validate the data entered in the segments.

General Ledger predefines the Accounting key flexfield.

117

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Task

Action

Chapter 1
Let’s Get Started

Structure Instances

Create account structure instances, which you will use to record transactions and maintain account
balances.

Value Set Values

Create groups of values, which you will assign to a key flexfield segment.

Account Hierarchies

Search, create, and edit hierarchical groupings of accounts.

Accounting Calendars

Set up accounting calendar period details. Determine the total number, frequency, and duration of the
accounting periods.

Account Combinations

1. Create account combinations if the structure instance of your chart of accounts flexfield doesn't

allow dynamically created account combinations

2. Create accounts for each account combination used in payroll. As a best practice, use the same

3.

account numbers for your payroll and general ledger accounts.
If you reconcile payments in Cash Management, create an account combination for reconciliation
differences.

Ledger Setup
You perform these tasks as part of the accounting configuration setup for Global Payroll.

Task

Action

Primary Ledgers

Create a ledger with a chart of accounts, accounting calendar, currency and subledger accounting
method.

Note:
If you're creating bank information, you must create a primary ledger.

Legal Entities

Add the legal entities that use the ledger.

The Legal Entity HCM Information task associates the payroll statutory units for legal entities to the
legislative data group.

Ledger Options

1. Complete all the fields for the General Information and Accounting Calendar, and Subledger

2.
3.

Accounting sections.
In the Period Close section, select the Retained Earnings Account you will use for payroll.
In the Journal Processing Intercompany subsection, select the option to launch AutoReverse after
the open period.

Balancing Segment Values to Legal
Entities

Assign specific balancing segment values to each legal entity before assigning values to the ledgers.

By specifying this information, you can more easily identify legal entities during transaction processing
and reporting

Balancing Segment Values to Ledger

Optionally, assign specific primary balancing segment values to the primary and secondary ledgers to
represent transactions for nonlegal entities, such as adjustments.

118

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Task

Action

Chapter 1
Let’s Get Started

Reporting Currencies

Review and update reporting currencies.

Reporting currencies maintain and record subledger and general ledger journal entries in additional
currencies.

Review and Submit Accounting
Configuration

Submit your configuration.

Open First Period

Open the first period when you're ready to process transactions for the ledger.

After you open the first period, use the Accounting Periods task in General Ledger to open and close
periods, and to specify the target period that concludes the series of calendar periods.

Related Topics

• How Payroll Costing Components Integrate with Other Applications

• Primary Ledgers, Secondary Ledgers, and Reporting Currencies

• Payroll Setup Tasks for Subledger Accounting

• Assign Legal Entities and Balancing Segments

• Chart of Accounts Structures and Instances

Setup Task List for Payment Reconciliation

Global Payroll integrates with Cash Management and General Ledger. This integration facilitates the setup of banks,
branches, and bank accounts, and the reconciliation of bank statements with payment transactions.

An administrator or implementor with the appropriate privileges performs the tasks shown in this table:

Application

General Ledger

Cash Management

Setup Steps

Task

Create an account combination for the
reconciliation differences account.

• Account Combinations

Set up transaction codes that map to the
payment method transaction codes used in
payroll.

• Cash Transaction Type Mapping

• Bank Statement Transaction Codes

Cash Management

Create reconciliation rules.

• Bank Statement Reconciliation Tolerance

Rules

• Bank Statement Reconciliation Matching

Rules

• Bank Statement Reconciliation Rule Sets

119

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

Application

Payroll

Setup Steps

Task

Create liability, cash clearing, and cash accounts
for your payment sources.

• Costing of Payment Sources

Specify the option Transfer to General Ledger.

Reconciliation Differences Account Setup
If you reconcile payment costs before posting the costing results to General Ledger, set up a reconciliation differences
account in General Ledger using Account Combinations. The reconciliation differences accounts in Cash Management
records discrepancies between the bank statement and the transferred payment files, such as over and under
payments.

Payroll Transactions Codes Setup
If you cost your payments, set up and map transaction codes in Cash Management for the organization payment
methods.

Task

Action

Bank Statement Transaction Codes

1. Review the transaction and statement codes that your enterprise currently uses
2. Create transaction codes for the transaction types that support your organization payment

methods

Cash Transaction Type Mapping

1. Map transaction types to payment types used for the organization payment methods that

2.

support costing of payments.
Identify the organization payment methods for payroll accounts, such as payroll liability, cash, and
cash clearing accounts.

Reconciliation Rules Setup
Payroll processes transfer your payment entries to Cash Management for manual or automatic reconciliation with bank
statements, and cost the unreconciled and reconciled payments to the appropriate account, such as the cash clearing
and cash accounts.

If you reconcile transactions automatically, in Cash Management complete the tasks listed in this table.

Task

Action

Bank Statement Reconciliation Tolerance
Rules

Create tolerance rules based on date, amount, or percentage that prevent or warn you when
reconciliation exceeds a defined tolerance.

Bank Statement Reconciliation Matching
Rules

Define bank statement automatic reconciliation matching rules.

Bank Statement Reconciliation Rule Sets

Assign a group of matching rules and tolerance rules to a bank account for reconciling bank statement
lines with transactions.

Bank Accounts

Specify the Reconciliation Differences account you set up in General Ledger..

120

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Task

Action

Chapter 1
Let’s Get Started

Payroll Accounts Setup
Create a liability and cash account. Use Costing of Payments to create a cash clearing account to track payments such
as checks/cheques, where a delay exists between the date the payment is issued and the date it clears.

Note:  When you set up the accounts, it's best practice to enter the same account information that you use for the
cash and cash clearing account that you created in General Ledger.

Related Topics

• Payroll Setup Tasks for Financials

• Considerations When You Create Accounts

• Payroll Setup Tasks for Subledger Accounting

• Reconcile Payroll Payments

121

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 1
Let’s Get Started

122

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

2  Elements, Earnings and Deductions

Payroll Elements

Overview of Payroll Elements

Some elements are predefined. You can also create other elements to match your requirements. Each element belongs
to a primary classification, according to its purpose, which determines the template you use to create it.

For information on how to secure and limit access to elements based on your business requirements, see Secure
Elements through HCM Data Roles and How to Restrict Access to Elements Using Element Security Profile and HCM Data
Role.

Use the template to create the elements and depending on your country extension, you create the associated items
required for payroll processing.

Use the elements to represent these components:

• Earnings, such as salary, wages, and bonuses

• Compensation, such as employee stock purchase and insurance plans

• Absences from work

• Tangible items distributed to persons, such as tools, uniforms, mobile phones, or computers

• Statutory deductions, such as taxes, voluntary deductions, contributions to charities or savings plans, and

involuntary deductions, such as court orders and pretax deductions

• Employer taxes and other employer liabilities

Note:  You can associate a time card with a results element that has the costing definition. On the Element Summary
page, you can use the base element attribute to directly link a time element to the result element.

Use Predefined Elements
The predefined elements are specific to your country or territory. They typically include deductions for tax and wage
attachments. You can't make any changes to these predefined elements. However, you must create eligibility records for
them.

Create Element
You can create as many earnings and deduction elements as you require using the Elements task. Let's assume that,
effective 6th March, you create an element entry for a worker. In this case, the element entry has a start and end date of
6th March.

You select the element classification and category that determine the template of questions. You answer the questions
to specify the details of the element you want to create. The items that the template generates can include multiple
elements, input values, formulas, balances, and other items.

123

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Note:  The template you use to create elements also depends on the configuration selected for your country or
territory on the Features by Country or Territory page. For example, if the country extension is set to Payroll, you
use a template that generates all the items required for payroll processing. If the country extension is set to Human
Resources or None, you use a basic template that generates the elements only. However, if you select an element
classification, such as Standard Earnings, Supplemental Earnings, Direct Payments and Taxable Benefits, the basis
template creates input values for Amount, Periodicity, and Full-Time Equivalent.

You can configure any of the generated items to match your specific business requirements. For example, you can
add input values, edit the formulas, or add a status processing rule to use a different formula for certain assignment
statuses. You must also create element eligibility records for the elements.

This table explains the purpose of the items that you use when creating element.

Items

Input Values

Purpose

Defines the entry values available on each entry of this element, such as hours worked or amount.

Element Eligibility Records

Defines the eligibility criteria a worker's employment record must meet to be eligible for the element.
For example you can use grade, payroll, salary basis, or organization as eligibility criteria.

Status Processing Rules

Identifies the formula the payroll run uses to process the element, and how to handle the formula
results.

Related Formulas and Related Elements

Identifies additional elements and formulas created by the template for payroll processing.

Related Balances

Identifies the balances created by the element template for this element.

Related Topics

• Maintain Elements

• Formula Result Rules for Elements

• Payroll Element Input Values

• Create Earnings Elements for Payroll

• Payroll Element Eligibility

Maintain Elements

After you create and use an element, you're limited on the updates you can make to it. This ensures the integrity of the
element for retroactive processing and the balances of the input values.

You can't remove existing input values or add new ones if you've created entries for the element. To add an input value
to an element before you create any element entries, set your effective date to the element's start date.

You can make these changes to an element that has been processed before:

• Change a required input value to be optional.

124

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

• Alter the sequence in which input values appear on the Element Entries page.

• Change the input value validation rules for minimum, maximum, lookup, or formula.

• Change your specification of which input values create database items.

• Change the reporting name. However, the database items created for the element continue to use the original

name.

• Delete elements that are in In Progress status.

For existing elements you can now make updates to these attributes in the correction mode if the element meets the
specified criteria rules for the attribute.

• Allow multiple entries in same period

• Latest Entry Date

• Output Currency

• Process once per period

Let's assume you correct the Allow multiple entries in same period attribute, all date effective records would get
updated with the change.

Example:

An element has these two date-effective records:

• 01-Jan-2010 to 31-Dec-2017

• 01-Jan-2018 to 31-Dec-4712

And for that element, the value of Allow multiple entries in same period option is N. Effective 15-Jun-2018, you
change the value of this option from N to Y. Then, as the figure shows, the application updates both the records with
the value Y.

125

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Allow Multiple Entries
Edit the Allow multiple entries in same period option from N to Y even if element entries and run results exist for that
element.

However, you can't edit this option in these scenarios:

•

•

•

If the element is target of Stop Entry rules.

If the value of the Standard Link option is Y.

If the element is a target of indirect formula result rules.

As this figure shows, you can't change the value from Y to N. This is because such an action invalidates the existing
entries and possibly could impact retroactive processing.

Update Termination Rule
You can update the termination rule of an element even if element entries or run results exist for that element. Such
updates don't affect the existing element entries, but impact only new element entries.

In the Latest Entry Date field, you can change the element duration option so that entries have a later end date. You
can't select an element duration option that will result in entries having an earlier end date.

For example, you can update the dates as follows:

• Last Standard Earning Date to Last Standard Process Date

• Last Standard Process Date to Final Close

• Last Standard Earning Date to Final Close

This change isn't applicable to the time definitions that you define.

Update Output Currency
The output currency for an element is defaulted based on the currency defined for the legislative data group. You can
update the Output Currency field to a required currency under these circumstances.

•

If it's a newly created element

• There isn't element eligibility for that element

• No balances exist for this element

Note:  If you calculate statutory deductions such as tax, you should not change the element output currency. All
predefined tax calculations are performed using the currency of the legislative data group. All reports including
payslips are also generated using the currency of the legislative data group.

126

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Your company might have a requirement to change the element output currency for payroll calculations that don't
include legislative taxes. For example, a British national who works in the USA might be paid on an expat payroll which
isn't subject to US taxes.

Process Once Per Period
Use the Process once per period option to check if the element entry has been processed or not.

As this figure shows, change this field both from Y to N and N to Y even if element entries or run results exists.

If the value of the option is Y and the element entry is already processed in the period, then the application doesn't
process it again.

If the value of the option is N, then the application processes the element entry even if it's already processed in the run.

As this figure shows, depending upon the value of the option, the application processes the element entry.

Search for Elements Using the Element Code
You can now search and view elements using the element code.

• Use the Add Fields option in the Advanced Search region to search the element using element code.

• Select View > Columns > Element Code to view the element code attribute with other element details.

• The element code attribute is displayed under the Element Name attribute in the Element Summary page.

Delete In Progress Status Elements
On the Element Search page, you can delete those elements that are in the In Progress status. However, you can delete
only those elements for which the corresponding element creation scheduled process has failed.

127

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Add New Input Values to Existing Elements
You can add new input values to an element using the HCM Data Loader (HDL), when the element has entry values
created or processed in the payroll run. The new input value must meet the following criteria:

•

Input value isn't required

• Default at runtime isn't enabled

• Default value isn't provided

• Default formula isn't attached

•

Input value with the same name doesn't exist already for the same element

When you create a new input value for an element using the PayrollElementDefinition HDL object, a new flow, Perform
Post Processing of Element with task Create Element Entry Values will automatically assign this value to all element
entries. After the entry values are created for all impacted employees, you can change the entry value.

During the entry creation process, if the Perform Post Processing of Element flow errors out for any reason, you can
retry or resubmit the process to create the remaining entry values. You also have the option to rollback the process,
which deletes all entry values. When you delete the entry values, you must also delete the input values that were created
using HDL.

Validations are provided to ensure the input and entry values are created successfully. When the Perform Post
Processing of Element process is running, or being rolled back, the following validations will be applied:

• The element will be locked for any modification.

• The Calculate Payroll, Adjust Multiple Balances, Calculate Gross Earning, Load Initial Balances, Reverse Payroll
Calculation, and Recalculate Payroll for Retroactive Changes payroll processes will be blocked from running
when the postprocessing of element is being run.

• The element will continue to be in locked status if the element postprocess is rolled back but newly created
input values aren't deleted. During this time, the Calculate Payroll, Adjust Multiple Balances, Calculate Gross
Earning, Load Initial Balances, Reverse Payroll Calculation, and Recalculate Payroll for Retroactive Changes
payroll processes will error out till the newly created input values are deleted.

• The Quickpay submission and Retry process are prevented from submission.

• The input value can't be created while a payroll process is being run.

Note:  The payroll processes that are running beyond 3 days will be ignored while doing the above validation check.
This feature isn't intended to upgrade the existing elements with any other objects, such as upgrading the element
that was created using the HR or Payroll Interface license to an element to use in Payroll processing with Payroll
license. It's only for adding new input values when the above conditions are met. Consider when's the best time to
create any new input values, to avoid the impact on your payroll cycle, such as overnight or weekend. Ensure that
the add new input value functionality isn't planned to be run when any of the above payroll processes are running,
waiting, or planned to be run, as it will impact the regular payroll cycle.

Related Topics

• Payroll Element Input Values

128

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Earnings and Deductions

Overview of Define Earning and Deduction Definitions

The Define Earning and Deduction Definitions task list in Setup and Maintenance contains the tasks required to set up
elements and payroll components.

Your implementation may include a few predefined elements, usually for legislative tax deductions. Use the Elements
task to create additional elements and the associated objects required to support their processing. The objects vary
depending on the element classification and category.

Manage Element Classifications
Elements are grouped into primary classifications that control their sequence of processing and the balances they feed.
Secondary classifications are subsets of the primary classifications, which you may use to manage wage basis rules for
deductions and taxes.

The primary classifications and some secondary classifications are predefined. You can't remove or change predefined
classifications.

What you can do:

• Create additional balances that the primary classifications feed.

• Create secondary classifications, if required.

• Specify costing setup options and frequency rules for element classifications. The default frequency rule is

always each period.

Manage Elements
Use the Elements task to review elements and to add new ones. When you create an element, your selection of the
element classification and category determines the questions on a predefined template. Submitting the template
generates an element, which you can edit, as required.

You must create at least one element eligibility record for all predefined and newly created elements.

The following figure shows the tasks involved.

129

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Note:  Make sure you set the country extension to Payroll using the Features by Country or Territory task before you
create elements for payroll processing. This setting ensures that you use the appropriate element templates.

Creating certain elements also creates component groups, calculation value definitions, and other calculation
information. For example, creating involuntary deductions and pension deductions may create these additional objects.
Use the relevant tasks in the Define Earning and Deduction Definitions task list to review the objects generated for each
element.

Payroll components are associated with a set of rates and rules used for calculation or reporting. These components
conform to manage calculation value definitions

What you can do:

• Review the tables that hold the rates and other values used to calculate deduction and exemption amounts.

• Modify some value definitions. For example, you might enter a default payee for pension payments.

• Add new calculation ranges, if required

Manage the calculation information for elements that generate payroll components, such as involuntary deductions and
statutory deductions.

What you can do:

• Review the calculation information supplied for your country or territory, such as the wage basis rules and

calculation factors

• Add new calculation factors, if required.

Component groups are predefined categories of calculation components managed by component group rules.

What you can do:

• View rules for component groups.

130

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

• Modify the rules, such as wage basis rules, for some deductions

After setup, you add calculation components to personal calculation cards by loading data, such as time cards, or using
the Calculation Cards task. Usually, hiring a worker creates a statutory deduction card automatically.

Add Eligibility Rules For Predefined Elements
The task list includes this task as a reminder. Use the Elements task to define at least one element eligibility record for
every predefined and newly created element.

Note:  Make sure you create an eligibility record for the statutory deduction elements like Tax, before you start hiring
workers.

Element eligibility determines who can receive entries of the element. Do the following:

1. Create a name for the element eligibility record. Use a naming convention similar to the element's to easily

identify the record, for example, when you set up costing for the element's eligibility record.

2. Restrict who can receive entries of the element by specifying eligibility criteria. For elements applicable to all

workers, create eligibility without specifying any criteria.

Manage Rate Definitions
Define any rates that are based on calculated payroll balances, such as an employee's average salary during the last
three months. You can use rate definitions in absence plans and formulas.

You can define rates to be:

• Monetary, such as a pay rate, or non monetary, such as an absence accrual rate defined in days or hours

• Based on a combination of elements, or a single element

Related Topics

• Overview of Payroll Elements

• Define Voluntary and Prestatutory Deductions

• Payroll Calculation Information

• Payroll Element Eligibility

• Create Earnings Elements for Payroll

How Payroll Elements Hold Information for Multiple Features

Use Payroll Elements to determine the payment of base pay, benefits, absences, and other earnings and deductions.
Associate payroll elements with salary bases, absence plans, and the benefits object hierarchy to determine how you will
use those elements.

This table provides some examples of how you can use payroll elements.

Payroll Element Usage

Examples of Payroll Elements

Base Pay Management

Annual Salary Basis

131

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Payroll Element Usage

Examples of Payroll Elements

Monthly Salary Basis

Hourly Salary Basis

Absence Management

Absence Payment

Benefits

Leave Liability

Discretionary Disbursement

Final Disbursement

Health Care Deduction

Savings Plan Deduction

Employee Stock Purchase Deduction

Time and Labor

Regular Hourly Earnings

Overtime Earnings

Shift Earnings

Payroll

Regular Standard Earnings

Bonus Earnings

Tax Deduction

Involuntary Deduction

Base Pay Management
To manage base pay, you attach an earnings element to each salary basis (hourly, monthly or annual) for each worker.
When a manager or compensation specialist enters a base pay amount for a worker, the application writes the amount
to an element entry. The application does this by using the element input value associated with the worker's salary
basis. Payroll processing uses the element entry to generate payment amounts.

Absence Management
You can manage worker absences and corresponding entitlements. You can create absence types based on predefined
absence patterns, and associate them with absence plans. You can associate an absence element with an absence plan
to transfer this information for payroll processing:

• Payments for absent time, for example, during maternity or long term sickness.

• Accrual disbursement at the end of absence plan year

• Accrual disbursement when plan enrollment ends

• Absence liability amounts

132

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

You can process the payments in Oracle Fusion Global Payroll or use HCM extracts to transfer the information to a third-
party payroll application for processing.

Benefits
Attach payroll elements at various levels in the benefits object hierarchy to create deductions and earnings that you can
process in a payroll run to calculate net pay.

Time and Labor
Create payroll elements for use in time cards, and calculate payroll or gross earnings based on the time card entries
transferred to payroll. For example, for Oracle Fusion Time and Labor, you run processes that create dependent payroll
attributes and time card fields for element input values. You can automate the routine import of time card entries to
payroll using predefined flows.

Payroll
For Oracle Fusion Global Payroll, you define earnings and deduction elements, such as bonus and overtime earnings
and involuntary deductions. These elements incorporate all components required for payroll processing, including
formulas, balances, and formula result rules.

Define Elements, Balances, and Formulas

The Define Elements, Balances, and Formulas task list contains the tasks required for creating payroll elements for
compensation, absences, time and labor, and HR management.

You can also use this task list if you're recording earnings, deductions, and other payroll data for reporting,
compensation and benefits calculations, or transferring data to a third-party payroll provider.

Note:  If you're using Oracle Global Payroll, use the Define Payroll task list instead. The Define Payroll task list includes
other tasks required to set up payroll processing.

Required Tasks
Your business requirements and product usage decide which required tasks you need to complete. The required tasks
include:

• Elements

• Payroll Definitions, which is usually required to support elements

• Consolidation Groups, which is required for creating payroll definitions

If you use predefined Payroll Interface extracts to transfer data to a third-party payroll provider, you might need to
create element subclassifications, balances, organization payment methods, and object groups. See the Global Payroll
Interface documentation for more information.

Before You Begin
Before you start the Define Elements, Balances, and Formulas task list, complete the tasks these offerings contain.

133

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Task

Use To

Why It's Important

Manage Legal Entities

Create payroll statutory units.

Ensures that hiring employees automatically
creates payroll relationship records.

Manage Legal Entity HCM Information

Associate a legislative data group with each
payroll statutory unit.

Ensures that hiring employees automatically
creates payroll relationship records.

Manage Features by Country or Territory

Select Payroll Interface as the extension for any
countries or territories where you extract HR
data to send to a third-party payroll provider.

Ensures that you use the appropriate element
templates to create earnings.

Configure Legislations for Human Resources
Use this task to create and edit legislative data for a country or territory that doesn't have a predefined country
extension. It guides you through configuring some payroll objects and values required for creating elements, including:

• Tax year start date

• Period of service on rehire rules

• Default currency

• Element classifications

• Component groups

• Payment types

Note:  Complete this task before the other tasks in this task list.

Elements
Use elements to communicate payment and distribution information to payroll applications from the source
applications listed in the following table.

Source Application

Element Purpose

Compensation

• Earnings and deduction elements, such as bonuses, overtime earnings, and voluntary

deductions.

•

Information elements to load user-defined data to use during a workforce compensation cycle.

Benefits

• Deduction elements to record activity rate calculation results, such as:
◦ Employee contributions and employer distributions for medical options
◦ Flex credits for flex benefits
• Earnings elements to disburse unused credits as cash.

Time and Labor

Time card details such as salary, overtime hours, and shift unit payments.

Absence Management

Absence details such as number of hours, days absent, or accrual absence balance details.

134

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Payroll Definitions
The payroll definition supplies the payroll period frequency and dates, which some applications use for payroll
calculations. A payroll is assigned to the assignment record of an employee, it indicates the payroll frequency for the
assignment such as weekly. This table shows which applications require payroll definitions.

Application

Payroll Definition Required?

Usage Conditions

Global Payroll Interface

Yes, optional

Compensation

Yes, optional

Benefits

Time and Labor

Absence Management

Optional

Optional

Optional

Required if you run the Calculate Gross
Earnings process

Required if you capture salary with a frequency
of payroll period

Required to use the payroll period frequency to
calculate communicated rates or values passed
to payroll.

NA

NA

Consolidation Groups
You must have at least one consolidation group for each legislative data group where you create elements. Payroll
definitions require a consolidation group.

Other Payroll-Related Setup Tasks
Your implementation might require other tasks from My Client Groups.

Task

Requirements

Organization Payment Methods

To record personal payment methods for your employees, you need to create organization payment
methods and associate them with your payroll definitions. Organization payment methods define the
combination of payment type and currency to use for payments to employees or external parties.

Element Classifications

Primary element classifications are predefined. If you run the Calculate Gross Earnings process
(provided with Global Payroll Interface), you might create subclassifications to feed user-defined
balances.

Fast Formulas

The Elements task provides predefined payroll formulas for payroll interface users. You can also write
formulas for several uses, including:

• Validating user entries into element input values

• Configuring compensation, benefit, and accrual plan rules

• Calculating periodic values for gross earnings and defining element skip rules for the Calculate

Gross Earnings process (provided with Global Payroll Interface)

Balance Definitions

If you're using Global Payroll Interface, creating earnings elements creates balances automatically. You
can edit these generated balance definitions.
If you're using the Calculate Gross Earnings process, you might want to create other balances for
extracts or reporting.

135

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Task

Object Groups

Requirements

You can create object groups to specify subsets of elements or payroll relationships to include in a
report or process, such as the Calculate Gross Earnings process.

Related Topics

• Payroll Definitions

• Payroll Balance Definitions

• How Payroll Elements Hold Information for Multiple Features

• Overview of Using Formulas

Define Voluntary Deductions Using Reference Codes

Maintain voluntary deduction balances for each reference number provided. For example, when an employee has two
loan deductions, you can maintain separate balances for each loan by specifying a unique reference for each loan.

Specify a Deduction Reference Code for each element entry that has arrears and total owed options enabled for the
newly created element. The element template for voluntary deductions is modified by replacing the existing template
questions for arrears and total owed.

These are the new template questions:

Template Question

Options

What should happen when there are
insufficient funds to cover the deductions?
If you enable arrears, a reference is
required for each deduction entry.

• Don't take partial deduction or create arrears.

• Don't take partial deduction, place all in arrears.

• Take partial deduction, but don't create arrears.

• Take a partial deduction, place remaining in arrears.

Do you want to stop processing when the
total owed is reached? If you enable total
owed, a reference is required for each
deduction entry.

• No

• Yes

If you enable the arrears option or the total owed in the above questions, the application creates a required input value
named "Deduction Reference". The application uses this reference number to maintain deduction accruals and arrears.
Enter the reference number while creating an element entry, such as Loan Account Number given by the bank or a
financial institution when a loan is disbursed

Get Reference Code Formula
Use this formula to generate a unique reference number using a database sequence for each element entry.

You can link this formula to the Default Formula attribute in Default Entry Values and Validation Section at element level,
when you don't have a reference number provided by a respective authority such as a Loan Reference Number provided
by banks. For example, if an employee is contributing an amount to two different unions without receiving a reference
number, but you have a requirement to capture the arrears separately for each union. You can then use the delivered

136

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

fast formula Get Reference Code from the Database Sequence, which generates a unique reference number for each
union element entry.

The starting value returned by this formula is 100 and increments by 1 for each new element entry. You can also write
your own fast formula, such as Person Number as the reference number.

Note:  Using the same reference number across entries of the same element will combine the balances.

For the elements using a Benefits module that meets one of the above conditions, you must use a Default reference
value for all entries or use a formula to create a reference based on the Person Number of the employee or Benefits Plan
name. This is because, when an employee is enrolled into a benefits plan, an element entry is created. When there is a
subsequent life event and enrollments, it end-dates the previous element entry and creates a new entry. If you use the
above delivered default formula, the balances will be re-initiated.

Related Topics

• Payroll Balance Definitions

Security Requirements to Access Earnings and Deductions Data

The Earnings and Deductions page offers you a single, centralized location to manage all employee earnings and
deductions. Use this page to quickly review all earnings and deductions for an employee for a specific date range,
however, the date range can be a single date.

To access the Earnings and Deductions page, grant this functional privilege to a custom role:

• Manage Payroll Calculation Entries (PAY_MANAGE_CALCULATION_ENTRIES)

This table lists the aggregate privileges you can assign to the relevant custom roles to enable view or manage privileges
to records on a page.

Security Privileges

Type of Entries

View Only Access

Manage Access

Standard Entries

Time Entries

Absence Entries

Calculation Cards

View Payroll Element Entries – ORA_PAY_VIEW_
PAYROLL_ELEMENT_ENTRY

Manage Payroll Element Entries – ORA_PAY_
MANAGE_PAYROLL_ELEMENT_ENTRY

View Payroll Time Entries – ORA_PAY_VIEW_
PAYROLL_TIME_ENTRIES

Time entries must be managed using the
source time product.

View Payroll Absence Entries – ORA_PAY_VIEW_
PAYROLL_TIME_ENTRIES

Absence entries must be managed using the
source absence product.

View Payroll Calculation Cards -
ORA_PAY_VIEW_PAYROLL_CALCULATION_CARDS

Manage Payroll Calculation Cards – ORA_PAY_
MANAGE_PAYROLL_CALCULATION_CARDS

Data Security
This table lists the applicable data security privileges within the Earnings and Deduction page and it's dependent on the
type of entries.

137

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Data Security

Chapter 2
Elements, Earnings and Deductions

Type of Entries

Person Security

Support for Element Type

Support for Assignment Level Security

Standard Entries

Yes

Yes

Yes

Users can view element
entries with their element
security profile

Users can view entries for:

• Assignments within the person and assignment

security profile

• Payroll relationship for those assignments

Time Entries

Yes

No

Yes

Users can view entries for:

• Assignments within the person and assignment

security profile

• Payroll relationship for those assignments

• All other assignments within those payroll

relationships.

This is different from the earlier Calculation Entries
page.

Absence Entries

Yes

No

Yes

Users can view entries for:

• Assignments within the person and assignment

security profile

• Payroll relationship for those assignments

• All other assignments within those payroll

relationship.

This is different from the earlier Calculation Entries
page.

Calculation Cards

Yes

No

Yes

Users can view entries for:

• Assignments within the person and assignment

security profile

• Payroll relationship for those assignments

• All other assignments within those payroll

relationships

138

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Element Classifications

Primary Element Classifications

Primary element classifications are defined by Oracle Fusion to meet legislative requirements, and are supplied to users
with the product.

Primary Classifications
Elements are grouped into primary classifications, such as Earnings and Voluntary Deductions. In a human resources
department, you can use the primary classifications to identify groups of elements for information and analysis
purposes. In a payroll department, the classifications control processing, including the sequence in which elements are
processed and the balances they feed. Oracle Fusion provides primary classifications and some balances, mainly to
reflect tax legislation. They are designed to meet the legislative requirements of your country, so you can't change or
delete them. You can create additional balances to be fed by any of the primary classifications.

For example, in a human resources department, you can use them to identify groups of elements for information and
analysis purposes.

Element Templates

You use an element template to create an element, based on the element's purpose, and the primary classification to
which the element belongs.

The exact scope of each element template, including the questions displayed on the Elements page, is controlled by
many factors, such as, the country extension and payroll license status of the user.

Here's a list of the primary classifications supported by the global payroll element templates:

Note:  The element classification name and calculation rules may vary by country because they're based on the
legislation rules. For example, the Days * Rate calculation rule isn't applicable for the US legislation. For more
information, see the Implementing Payroll guide for the respective country.

Primary Classification

Description

Category

Calculation Rules Supported

Absences

Use for elements that calculate

Absence

You can select the unit of measure

absence payments and deductions

for an employee.

You must select this option for

absences managed in Oracle

Absences or a third-party absence

product.

for Absence reporting:

• Hours

• Days

139

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Primary Classification

Description

Category

Calculation Rules Supported

Balance Initialization

Use to load initial balance values.

Standard

NA

You'd mainly use these elements

when transferring balances from a

legacy payroll application as part of

your payroll implementation.

Direct Payments

Use for payments that are made

Standard

directly to employees, and aren't

subject to payroll taxation, such as

expense reimbursements.

• Flat Amount

• Factor

• Percentage of Earnings

• Days * Rate

• Hours * Rate

Direct Payments

Use for payments that are made

Time card

You can select the unit of measure

directly to employees, and aren't

subject to payroll taxation, such as

expense reimbursements.

You must select this option for

direct payments captured on a time

card in Oracle Time and Labor or a

third-party time product.

Employee Tax Credits

Use to capture excess tax amounts

Standard

that should be deducted as part of

payroll processing.

Employer Charges

Use to calculate taxes that are paid

Standard

by employers in accordance with

their employees’ gross wages and

compensation.

Employer Pretax Charges

Use to calculate employer

Standard

matching contributions that

must be processed in alignment

with corresponding employee

pretax deductions. These

amounts are processed after

prestatutory deductions, but before

employee tax deductions, ensuring

compliance with local taxation

rules.

for time reporting:

• Hours

• Other Units

• Days

• Fixed amount deduction

• Percentage deduction

• Fixed amount deduction

• Percentage deduction

• Fixed amount deduction

• Percentage deduction

140

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Primary Classification

Description

Category

Calculation Rules Supported

Note:  Balances for Employer

Pretax Charges are included

within the existing Employer

Charges balance group.

Employer Taxes

Use to calculate taxes that are paid

Standard

by employers in accordance with

their employees’ gross wages and

compensation.

• Fixed amount deduction

• Percentage deduction

Information

Use to capture information that's

Standard

NA

required for the calculation of other

elements or formulas. For example,

 this type of element may capture

details to cost the hours worked

to a different natural account from

the regular earnings account.

Involuntary Deductions

An example of an involuntary

Involuntary Deduction

NA

deduction is a court ordered

payment taken from the

employee's pay and paid to a court

or an individual person.

Prestatutory Deductions

Pretax deductions are deductions

Standard

made from a person's gross

income. They reduce the total

taxable income of the person and

the tax withheld.

Severance Pay

Severance is a type of discretionary

Standard

payment that can be made to an

employee when their employment

is terminated.

Standard Earnings

Use for the payment of regular

Standard

earnings, such as salary.

• Fixed amount deduction

• Percentage deduction

• Flat Amount

• Factor

• Days * Rate

• Hours * Rate

• Flat Amount

• Factor

• Percentage of earnings

• Days * Rate

• Hours * Rate

Standard Earnings

Use for the payment of regular

Time card

You can select the unit of measure

earnings, such as salary.

for time reporting:

141

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Primary Classification

Description

Category

Calculation Rules Supported

Select this option for standard time

captured on a time card in Oracle

Time and Labor or a third-party

time product.

Supplemental Earnings

Use to define an augment payment

Standard

to an employee, such as bonus,

 incentive.

• Hours

• Other Units

• Days

• Flat Amount

• Factor

• Percentage of earnings

• Days * Rate

• Hours * Rate

Supplemental Earnings

Use to define augment payment

Time card

You can select the unit of measure

to an employee, such as bonus,

 incentive.

Select this option for supplemental

earnings captured on a time card in

Oracle Time and Labor or a third-

party time product.

for time reporting:

• Hours

• Other Units

• Days

Tax Deductions

Use for legal tax deductions such

Standard

NA

as income tax, resident tax, and

special tax. Many elements with

this classification are predefined

for your legislation.

Taxable Benefits

Use for elements that aren't

Standard

applied to a payment balance.

The difference between earnings

and taxable benefits is whether the

elements are applied to a payment

balance or not.

• Flat Amount

• Factor

• Percentage of earnings

• Days * Rate

• Hours * Rate

Taxable Benefits

Use for elements that aren't

Time card

You can select the unit of measure

applied to a payment balance.

The difference between earnings

and taxable benefits is whether the

elements are applied to a payment

balance or not.

You must select this option for

taxable benefits captured on a time

card in Oracle Time and Labor or a

third-party time product.

for time reporting:

• Hours

• Other Units

• Days

142

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Primary Classification

Description

Category

Calculation Rules Supported

Voluntary Deductions

Use these elements for deductions

Standard

such as union dues, which

the employee authorizes the

employer to make voluntarily on

the employee's behalf, after tax

deductions.

• Fixed amount deduction

• Percentage deduction

Element Category
The element category indicates whether the element is maintained using the standard element feature or the payroll
calculation solution.

When you create an element, either a default value is selected in the Category field, based on the selected primary
classification, or you can select a category from a list of values that are decided by the primary classification.

You need to select the appropriate category for each of your elements. For example, you must select the Timecard
category when you create an element that will be used to capture time card information in Oracle Time and Labor or a
third-party time product.

Note:  The element category is now stored in the PAY_ELEMENT_TYPES_F table, instead of template internal tables,
as part of the element creation from 23C onward. The existing elements have been updated with the corresponding
element category values used at the time of element creation.

Here's how you use the element categories:

• Standard: The information required to calculate a standard element, such as number of hours, is captured

through element input values. You can view the entry details for this element on the Standard Element Entries
region of the Calculation Entries page for an employee.

• Calculation Information: The information required to calculate this type of element, such as number of hours,

is captured through value definitions within the calculation information repository. You can view the entry
details for an employee on the Calculation Entries page. For example, absence entry details can be viewed on
the Absence page and tax information can be displayed on the Tax page for the employee.

Here's a list of all element categories and the model used by each category:

Category

Absence

Element Model

Calculation Information

Involuntary Deduction

Calculation Information

Standard

Standard

143

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Category

Time card

Element Model

Calculation Information

Calculation Rules
Select the calculation appropriate for your element, to control which input values or value definitions are created for the
element, the predefined formula associated with the element, and so on. For example, when you create an allowance
element that's based on a percentage of earnings, select the Percentage calculation rule.

Here's a list of the calculation rules supported by the element template:

Name

Days * Rate

Description

The element formula multiplies the number of absence days by the applicable rate. This rule is

commonly used for absence payments that are paid based on the number of days an employee is

(including Days rule)

absent.

Flat Amount

Select this option when the payment or deduction amount is entered for an employee. The element

formula can convert the entered amount, based on the payroll frequency of the employee. For

example, you can enter an annual allowance amount of $6,000 for an employee and the element will

calculate $500 as payable in each monthly payroll period.

Factor

Select this option for earnings or deductions that are calculated based on a factor, using rates. For

example, a company pays shift payments that are calculated as a factor of 0.05% of the employee's

salary.

Hours * Rate

The element formula multiplies the number of hours entered for the employee by the applicable rate.

This rule is commonly used for employees that are paid based on the number of hours submitted on a

(including Hours rule)

time card.

Percentage of Earnings / Percentage of

Select this option for earnings or deductions that are calculated based on a percentage. For example, a

Deductions

company pays car allowance payments that are calculated as 5% of the employee's salary.

This type of element creates a balance called <ELEMENT_NAME> Eligible Comp. The predefined

element formula uses this balance for the percentage calculation. Add balance feeds to this balance

to meet your business requirements. For example, apply the salary element to this balance when the

percentage calculation is based on the salary of the employee.

Other Units

This option supports payment rates that are based on units such as mileage or piecework rates. The

element formula multiplies the number of units entered for the employee by the applicable rate.

144

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Secondary Element Classifications

You can define secondary classifications to feed your own user defined balances.

Secondary classifications are subsets of the primary classifications. In some legislations, secondary classifications are
predefined. As with primary classifications, you can't remove or change any predefined secondary classifications, and
you can't disable any of the predefined balance feeds created for them.

How Element Classification Components Work Together

When you create an element, you select a primary classification, such as Involuntary Deductions, and optionally a
secondary classification, such as Child Support.

The classifications, which vary by country or territory, control the element template questions you answer to define the
element. An element may automatically inherit subclassifications from its primary classification. You can optionally
select more subclassifications for an element to control the balances it feeds.

Primary Classifications
Primary classifications meet the legislative requirements of your country or territory, so you can't change them.

In a payroll department, the classifications control processing, including the sequence in which elements are processed
and the balances they feed.

Secondary Classifications
Use secondary calculations to manage wage basis rules for deductions and taxes. You can't remove or change any
predefined secondary classifications. In some countries or territories, you can create your own secondary classifications.

Subclassifications
Subclassifications provide a way to feed balances. Elements can have only one primary and secondary classification,
but multiple subclassifications. You can create subclassifications or use predefined ones. You can specify that a
subclassification automatically applies to every element in the primary classification.

Tip:  Each subclassification belongs to one primary classification only. If you reuse a subclassification name under
different primary classifications, it's treated as a separate subclassification. And you must create separate balance
feeds for each subclassification.

Costing
Each primary classification includes these costing rules:

Rule

What It Does

Allow Costing

If set to Yes, you can select any costing option for element eligibility records.

145

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Rule

What It Does

Allow Distribution

If set to Yes, you can create distribution groups with elements in this classification. For example,
 you can create a distribution group with all the earnings elements. And prorate tax expenses
proportionately over the cost centers in which the wages were earned.

Frequency Rules
If frequency rules are enabled for a primary classification, you can use them on an element if you don't want to process
it each period. For example, you can set frequency rules to process element entries on the first and third weekly payroll
periods of each month. The default frequency rule is to process each period.

Related Topics

• How Element Processing Sequence is Determined

• Payroll Balance Definitions

How Element Processing Sequence is Determined

You can set a predefined sequence in which a payroll run processes elements. An element's primary classification
defines a default processing priority for the element in payroll runs. Lower priority numbers process first.

Most classifications also have a priority range. You can override the default processing priority. To set the priority,
edit the element on the Element Summary page. Setting a specific priority establishes the order in which the element
processes with respect to other elements in the classification.

Sometimes you must prioritize the processing of certain element entries for an individual person. For example, you may
need to determine the precise order in which deductions taken for wage attachments process for a person. In this case,
enter a subpriority number for element entries.

Element Employment Level

Employment Level Options for Payroll Elements

Your enterprise uses an employment model. When you create elements, you select the employment level at which to
attach the element. If you select a level below payroll relationship, each assignment record can have separate element
entries.

Payroll Relationship Level
This level is the highest level for accumulating balances. Every payroll run processes payroll relationship elements.

146

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Here are the typical elements to define at payroll relationship level:

• Tax deductions

• Pension

• Child support

• Medical care

• Union dues

• Benefits activity rate calculations, such as employee contributions and flex credits

Assignment Level
Use this lowest level for elements that require different entries for different assignments, or when the element applies
only to specific assignments.

Here are the typical elements to define at assignment level:

• Assignment salary

• Regular hours

• Overtime

• Sales bonus

• Profit-sharing bonus

Element Configurations

Create Earnings Elements for Payroll

For information on creating a payroll element, see Create a payroll element.

For information on upgrading an existing payroll element, see Upgrade a payroll element.

Payroll Elements for Time Card Attributes

To process pay according to time card entries, such as regular and overtime, you can create elements with the Time
Card category.

Time card elements support hours-based and units-based quantities. You use the hours-based quantifies to assign
people a flat payment amount through associated rates. For example, you pay people a meal allowance according to
the number of meals they take daily. The related payroll elements, balances, formulas, and calculation components are
automatically generated when you create a time card element.

Time cards with retroactive changes include the Expedite to payroll option that lets managers transfer the changes for
expedited processing and payment.

147

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Create Time Card Elements for Time Entries

Time card elements support hours-based and units-based quantities. You use the units-based quantities to assign
people a flat payment amount through associated rates. For example, you pay people a meal allowance according to the
number of meals they take daily.

When you create a time card element, you also create the related payroll elements, balances, formulas, and calculation
components.

Tip:  If people report regular and straight time portions of overtime separately, create two elements, such as Overtime
and Overtime Premium. If they report the portions together, you might use straight time instead of regular time, and
create a separate element for the overtime premium.

1. Go to Setup and Maintenance > Workforce Deployment > Elements and Formulas > Elements.
2. Create the payroll element.

a. On the Create Element dialog box, complete these steps:

i. Select the legislative data group, such as FR LDG, Hong Kong LDG, or US LDG.
ii. Select the primary classification, such as Regular Earnings or Earnings.
iii. When available, select the secondary classification.
iv. Select the Time Card category.
v. Click Continue.

3. On the Create Element: Basic Information page, complete these steps:

a. Enter a descriptive name, such as Regular, Straight Time, Overtime, or Shift Pay.
b. Enter the name that you want to display on reports containing this payroll element.
c. Select the effective date January 1, 1951. The early date ensures that the element attributes are
immediately available to use with shifts, time cards, web clock, and time collection devices.

d. Accept the remaining default values by clicking Next.

4. On the Create Element: Additional Details page, complete these steps:

a. Select Hours or Other Units as the calculation units for reporting.
b. Select the Work Units conversion rule. For the calculation used by each conversion rule, see Conversion Rule

Options for Configuring Additional Details of Payroll Elements.

c. Accept the remaining default values by clicking Next.

5. On the Create Element: Review page, complete these steps:

a. Review the element configuration to ensure that everything is correct.
b. Create the element and automatically generate all the related elements, balances, formulas, and calculation

components by clicking Submit.

By default, the Time Card category elements already have the appropriate value definition configurations required to
support location overrides. You don't have to make any edits.

148

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

6. On the Element Summary page, configure element eligibility by completing these steps:

In the Elements Overview section, select Element Eligibility.

a.
b. On the Actions menu, select Create Element Eligibility.
c.

In the Information section, enter an element eligibility name with a suffix that identifies the criteria. For
example, for the regular element with open eligibility--no selected criteria--the name would be Regular
Open.

d. Select the eligibility criteria. To leave eligibility open on the element and control it with HCM groups and

time processing profiles, skip this step.

e. Click Done.

7. Configure element eligibility for each of the related elements, which share the same name as this element and have

suffixes. Suffixes include Earnings Calculator, Earnings Distributor, Earnings Results, Retro, and Retro Results.

a. On the Manage Elements page, search for the element that you just created.
b. Click the related element name.
c. On the element summary page, complete these steps:

In the Elements Overview section, select Element Eligibility.

i.
ii. On the Actions menu, select Create Element Eligibility.
iii.
iv. Click Submit.
v. Click Done.

In the Information section, configure the same eligibility criteria as the original element.

Related Topics

• Time Card Required Option

• Process Time Entries in Payroll

• Create the Units-Based Meals Taken Element for Time Entries

• Time Card Updates to Payroll

• Calculate Time Based on a User-Defined Value

Time Element Value Definitions

The time element value definition captures and calculates time in cloud payrolls. The elements in this category create
value definitions used in time cards. The calculation steps are associated with the calculation element that's created by
the time template.

Value Definition - Name

Value Definition -Calculation
Type

Description

Calculation Step-Name

<Element Name> Element Rate
and Payment Rate

Rate Definition

Time Element Rate and Payment
Rate

You can calculate time using a
rate definition. The rate definition
details will be captured on the
element rate. A default rate
definition can be defined when
you create a time element.
Alternatively, a rate definition
can be captured on the time
card and passed to payroll from
your time product. The payment

149

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Value Definition - Name

Value Definition -Calculation
Type

Description

Calculation Step-Name

<Element Name> Rate Amount

Flat Amount

<Element Name> Conversion
Formula

Text

<Element Name> Reporting UOM

Text

<Element Name> Time Factor

Flat Rate

Rate Amount

Time Card Rate Conversion
Formula

rate identifies if there's no rate
definition for the time.

You can calculate time using a
flat amount such as 22 USD per
hour or 0.75 USD per mile. The
amount can be entered on the time
card. Alternatively, if the value is a
fixed amount it can be entered as
a default on the rate amount value
definition.

When you create a time element
you must specify a conversion
formula. This formula converts a
rate amount to the appropriate
periodicity. For example, if an
annual amount is captured for an
hourly element this formula would
convert the annual amount into an
hourly amount.

Note:
This <Element Name>
Conversion Formula isn't
created for elements with a unit
of measure.

-

The reporting value definition
captures the unit of measure of the
time element. This is derived based
on the calculation unit selected
for the element and will be either
hours, days or units.

Time Factor

Optionally you can apply a
percentage to the time calculation.
For example, the time calculation
could be based on 22 USD * 50
percent. The factor value can be
entered on the time card or entered
as a default on the value definition.

Note:
If the percentage varies based
on criteria, such as the worker's
location, then the details should
be captured on values defined
by the criteria.

Time

Flat Amount

The predefined time value
definition captures the number of

Time Card Unit

150

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Value Definition - Name

Value Definition -Calculation
Type

Description

Calculation Step-Name

Expedite

Text

Override Pay Method

Text

Override Check Printer

Identifier

time units worked. For example, '8'
hours or '2' units.

The predefined expedite value
definition identifies if the time has
been marked for inclusion in an
expedited payroll run.

Expedite

The predefined override check
payment method captures the
organization payment method for
expedited time.

Override Pay Method

The predefined override check
printer captures printer details for
an expedited time.

Override Check Printer

Generate Time Attributes and Time Card Fields for Your Elements

After you create or edit earnings elements for time entries, such as Regular, Overtime, and Shift Pay, you generate time
attributes for the data dictionary. Optionally, you can also generate time card fields for them.

Go to Setup and Maintenance > Workforce Deployment > Time and Labor and complete these processes:

Step

Process

Description

Comments

1

2

Generate Data Dictionary
Time Attributes, required

Creates dependent payroll
attributes for all element input
values, such as hours and rate

You must run the Generate Data Dictionary Time Attributes
process after making any changes to time elements. Such
changes include adding or deleting elements, editing input
values, or editing element eligibility records.

CAUTION:  Failure to run the process might negatively
affect the setup of fields, validation of payroll time types,
 or transfers of time data to payroll.

Generate Time Card Fields,
 optional

Creates time card fields using time
attributes from the data dictionary
for the specified legislative data
group

Instead of running this process, use the Time Entry Layout
Components task to create time card fields and web clock
buttons.

If you’re using a third-party time provider, create an HCM extract for the time entry elements. The extract includes the
element mapping ID that you specify in the XML file when you transfer the time entries to payroll.

151

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Related Topics

• Time Attributes

• How Time Entry Profile Components Work Together

Set Up Overrides

You can override the default value or formula for a specific group of employees identified by an element eligibility
record. Override the default value for specific employees on their element entries.

Set Up Area Overrides

Some countries or territories create time card elements with area input values for use as overrides. The overrides enable
employers to tax employees based on where they work. For example, employees specify the area information where
they worked on temporary assignment while away from their normal work location. These area entries are then included
in the time card records transferred to payroll by the Load Time Card Batches process.

Set Up Costing Overrides

You can specify additional attributes in Time and Labor to enter costing segment values on time cards. The segments
must match the segments that you can enter on element entries. Use the Element Entries task to search a person's
record. View the available segments on the Costing tab of the Person Details page. Costing is defined on the element
eligibility record of the results element. When you transfer time entries, the transfer process displays the costing on the
calculation element.

As an example, the structure of your cost allocation key flexfield might specify that the department segment is entered
at the element entry level. You could specify this additional attribute on the time card. Your employees can then specify
the department to charge for overtime hours worked while on loan to a different department. After you transfer the
time entries, the payroll calculation uses the department specified for the overtime hours to derive the costing results.

To view the results of the costing overrides transferred to payroll, perform these steps:

1. On the Home page, click the Process Results Summary quick action under the My Client Groups tab.
2. You can find a list of payrolls which have been processed on the View Person Process Results page. Select the

correct payroll before you search for a person, then select a person on this page.

3. Click the down arrow in the Process Results tab.
4. Go into that person's statement of earnings.
5. Select Costing Results.

Related Topics

• Time Card Required Option

• Process Time Entries in Payroll

Define Payroll Elements for an Absence Accrual Plan

This example shows how to define an absence element for a vacation accrual absence plan.

152

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Based on your setup decisions, this procedure configures these additional elements:

• Accrual element to process absence liability amounts

• Entitlement element to process payments for absence during vacation

• Discretionary Disbursement element to process disbursement of partial time accruals

• Final Disbursement element to process accrual disbursement when the absence plan enrollment ends

The name of the element is prefixed to each additional element.

Note:  Each absence accrual plan will have its own, specific payroll element defined. The element you define for an
absence accrual plan shouldn't be used across multiple plans. You can't map one element to multiple absence accrual
plans.

This table summarizes key decisions for this scenario.

Decisions to Consider

In This Example

What type of an absence are you
transferring to payroll?

Accrual balances

Who's eligible to receive this element?

All workers

What units do you want to use for
reporting calculations?

Do you want the element to calculate
absence liability?

Days

Yes

Which rate should the calculate absence
liability use?

Liability Rate

Does your absence plan enable balance
payments when enrollment ends?

Yes

Which rate should the final disbursement
payment use?

Final Disbursement Rate

Does your absence plan enable payment
of partial accrual balances?

Yes

Which rate should the partial
disbursement payment use?

Partial Disbursement Rate

How do you want to calculate deductions
for paid absences for employees not
requiring a time card?

• Reduce regular earnings by the

amount of the absence payment

Reduce regular earnings by absence payment

153

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Decisions to Consider

In This Example

so that the worker doesn't get paid
twice?

• Select a rate to determine the
absence deduction amount?

Before You Begin
Ensure that you configured a rate definition to determine the monetary value of a unit of absence. And depending on
your enterprise separate rates to calculate liability, discretionary disbursement, and final disbursement payments. You
configure a rate definition using the Rate Definitions  task.

Define an Absence Element

1. On the Elements page, click Create.
2.

In the Create Element window, complete the fields as shown in this table.

Field

Value

Legislative Data Group

Select your legislative data group.

Primary Classification

Absences

Secondary Classification

Select an appropriate value for your legislation, such as Vacation.

3. Click Continue.
4. On the Create Element: Basic Information page, enter Vacation Payment in the Name and Reporting Name

5.

fields.
In the Absence Plan Details section, complete the fields as shown in this table. Use default values for fields
unless the steps specify other values.

Field

Value

What calculation units are used for

Days

reporting?

Work Units Conversion Rule

Standard Rate Daily

What type of absence information do

Accrual Balances and Absences

you want transferred to payroll?

6. Click Next.
7. On the Create Elements: Additional Details page, in the Accrual Liability and Balance Payments section,

complete the fields as shown in this table. Use default values for fields unless the steps specify other values.

154

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Field

Value

Calculate absence liability?

Yes

Which rate should the liability

Liability rate.

balance calculation use?

Does this plan enable balance

Yes

payments when enrollment ends?

Which rate should the final balance

Final disbursement rate.

payment calculation use?

How do you want Payout Amount to

Supplemental

be taxed?

Absence Payout Process Mode

Process and pay with other earnings

Does this plan enable partial

Yes

payments of absences?

Which rate should the discretionary

Discretionary disbursement rate.

disbursement use?

How do you want Cash out amount to

Regular

be taxed?

8. On the Create Elements: Additional Details page, in the Absence Payments section, complete the fields as

shown in this table. Use default values for fields unless the steps specify other values. For the purposes of this
worked example, all fields are being entered, however, only required fields must be entered and others may be
blank.

Field

Value

How do you want to reduce earnings

Reduce regular earnings by absence payment.

for employees not requiring a time

card?

Which rate should the absence

Absence payment.

payment calculation use?

155

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Field

Value

9. Click Next.
10. On the Create Element: Review page, review the information that you entered so far.
11. Click Submit to open the Element Summary page.

The template generates all the related elements, balances, and formulas.

Define Element Eligibility

In the Element Overview section of the Element Summary page, click the Element Eligibility node.

1.
2. Click Create Element Eligibility from the Actions menu.
3.

In the Element Eligibility section, enter Vacation Payment Open in the Element Eligibility Name text box.
Leave the rest of the fields on the page blank.

4. Click Submit.
5. Click Done.
6. On the Elements page, search for the other elements prefixed with your absence element name.
7. Select each element in turn and repeat the steps on the Element Summary page to define eligibility for each

element.

Define Payroll Elements to Process Absences

You define elements to calculate and process absence payments in Oracle cloud. When you define an absence element,
your responses to the element template questions determine which elements, balances, formulas, and calculation
components the template generates.

Defining an absence element involves these steps:

• Define an absence element

• Complete absence detail questions

• Complete accrual liability and balance payment questions

• Complete absence payment questions

• Submit the element

• Define element eligibility records and cost distributions

Define an Absence Element
Use the Elements task to define an absence element, selecting a primary classification of Absence, and a secondary
classification. Typically, the predefined values include vacation, maternity, and sickness.

Complete Absence Detail Questions
The questions you complete in the Absence Details section determine which subsequent questions the template
displays. You enter this information in the Absence Details section:

1. Specify the calculation units to use when reporting the absence, for example that's shown on the payslip, and

statement of earnings. Typically, you select Days or Hours for your reports that correspond to the units for your
absence plan. When creating an absence element, select the work calculation rule to calculate the absence rate.

156

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

2. Select the absence information to transfer to payroll based on the type of absence management plan.

Absence Management Plan Type

Absence Information to Transfer

Accrual

Accrual Balances

Accrual, Leave Donation,

Accrual Balances and Absences

 Compensatory

Qualification

Qualification Absences

No Entitlement

No Entitlement Absences

Complete Accrual Liability and Balance Payment Questions
If you transfer accrual balances, complete these questions.

Question

Steps

Calculate absence liability?

1. Select Yes, if you calculate liability.
2. Select a liability rate.

Usually the rate is the same as the absence payment rate. You might select a different rate when
estimating liability for billing purposes.

Does this plan enable balance payments
when enrollment ends?

1. Select Yes to configure a final disbursement element and to maintain balances for the

disbursement hours and payments.

2. Optionally, select a rate to use for the calculation.

Does this plan enable partial payment of
balance?

1. Select Yes to configure a discretionary disbursement element and to maintain balances for

disbursement hours and payments.

2. Optionally, select a rate to use for the calculation.

Complete Absence Payment Questions
Complete these questions:

1. Select a method to reduce regular earnings if employees don't complete a time card.:

◦ Reduce regular earnings by absence payment (entitlement payment balance)
◦ Select rate to determine absence deduction amount (entitlement deduction balance)

You might select one of these options:

- The Reduce regular earnings option to reduce regular earnings by the absence payment. This

means that the employee is paid the same net amount as if they weren't absent.

- The Select rate to determine deduction amount option when the employee isn't due to be paid
for the absence at the same rate as their regular earnings. In this case, the absence deduction rate

157

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

that you select will be a rate that deducts 100% of the regular earnings. However, the absence
payment rate would be a different rate, for example 50%.

2. Optionally, select a rate to calculate the absence payment.

If you have standard earnings and absence elements in the same payroll run that reduce regular earnings, the
payroll calculation reduces earnings in this sequence:

a. Using absence element entries
b. Using any standard earnings elements that reduce regular earnings

The salary balance isn't reduced beyond zero.

3. You can now ensure that absence entitlement payments are made to employees after terminations. Use the

Does this plan enable entitlement payments after termination?  question on the absence element template
to set the entitlement element to Final Close.

Example: Amelia is due to be paid maternity payments after her termination. Select Yes in this question to set
the latest entry date of the entitlement elements to final close. With this, the absence entitlement payments are
made to Amelia after her termination. When Amelia is terminated, change her employment assignment status
to Process When Earning. Also, set the TERM_INCLUDE_PR_LEVEL action parameter to Y, so that payroll
relationship level entries are considered for processing.

Submit the Element
When you submit the element, the template automatically configures a base pay element, balances, formulas, and
calculation components.

The template also configures additional elements, depending on the options selected in the template to transfer
absence information, as shown in this table.

Type of Absence Information to Transfer

Optional Balance Payments Selected

Additional Elements Configured

Accrual Balances

• Discretionary Disbursements

• Accrual

• Final Disbursements

• Discretionary Disbursement

• Final Disbursement

Accrual Balances and Absences

• Discretionary Disbursements

• Accrual

• Final Disbursements

• Entitlement

Qualification Absences

No Entitlement Absences

none

none

• Discretionary Disbursement

• Final Disbursement

Entitlement

Entitlement

Define Element Eligibility Records and Cost Distributions
Define element eligibility records for all elements generated by the template, for example for your accrual, entitlement,
discretionary and final disbursement elements.

158

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

If your enterprise calculates cost distributions, specify costing for all the element eligibility records. For example, for an
accrual element, you do these steps

1. Define element eligibility records for the accrual, accrual results, accrual retroactive, and accrual retroactive

results elements.

2. Specify costing for the accrual results and retroactive results elements.

The costing process costs the change in the liability balance since the last payroll period, debits the expense account
and credits the liability account.

Related Topics

• Define Elements, Balances, and Formulas

• How Payroll Elements Hold Information for Multiple Features

• Rates Used to Calculate Absences in Payroll

• Element Costing Options

•

Import Absence Entries to Payroll

Absence Elements for Compensatory and Leave Donation Plans

You can make absence payments for compensatory absence plans based on the date that the compensatory time was
accrued. The Absence application passes the accrued date to the Global Payroll application so that it uses the correct
rate of pay for absence.

For example, an employee is hired on 1/1/17 and is paid at a rate of 10 per hour. On 8/1/17, the employee receives a pay
rise and is now paid at a rate of 12 per hour. The employee takes 3 days of leave from 10/5/17 to 10/7/17.

The employee accrued this leave as time off in lieu (TOIL) in July 2017 when they were earning 10 per hour. The
application pays the employee for the 3 days leave at a rate of 10 per hour.

Compensatory Plans
When creating a rate definition to use for compensatory absence plans, in the Reference Date field, select the Absence
Accrued Date value. The rate calculator calculates the rate as of the absence accrued date that's passed from the
Absence application.

In the Setup and Maintenance work area, use the Element task to create absence elements for compensatory absence
plans.

When creating such plans, in the type of absence information to transfer to payroll option, select Accrual Balances and
Absences.

Leave Donation Plans
Workers can initiate requests to donate some or all of their accrual plan balances to coworkers who need additional time
off. Administrators and managers can initiate this donation request on behalf of the worker. You can donate vacation
only from Accrual and Compensatory plan types. Also, you can only donate in day or hours.

For example, Employee A is diagnosed with a long term illness and will be absent from work for a long time. You can
enroll the employee into a leave donation plan. Employee B has a vacation accrual balance of 100 hours and wants to
donate 10 hours to Employee A.

159

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Now, instead of the stipulated 100 hours, Employee B will have an accrual balance of 90 hours. Employee A will have an
accrual balance of 10 hours against the leave donation plan.

To use this balance, Employee A can do one of these actions:

• Enter a leave in the Absence application. The Global Payroll application receives an entitlement record for the

number of hours or days that they requested.

• Take the balance as a Cash out or Payout.

Note: If Employee B earns 20 per hour and Employee A earns 10 per hour, then the application pays Employee B at 10
per hour.

When creating absence elements for leave donation plans, in the type of absence information to transfer to payroll
option, select Accrual Balances and Absences.

Absence Elements for Payments after Termination
For absence plans that support payments after termination, set the entitlement element to Final Close. When creating
absence element template, select Yes in the enable entitlement payments after termination option. Then, set each of
the entitlement elements to the Final Close value.

On the Payroll Process Configuration page, set the Absence and Time Calculation Entries During Payroll parameter to
one of these values:

Value

Yes

No

What The Application Does

Includes the absence and time calculation entries in the payroll run for those active employees that
have these assignment statuses:

• Process When Earning

• Process When One Time Entry

Further, the application includes the terminated employees in the payroll run only if they have an
earning or an assignment level nonrecurring element entry.

Does not include the absence and time calculation entries in the payroll run for those employees that
these assignment statuses:

• Process When Earning

• Process When One Time Entry

And the application includes the terminated workers in the payroll run only if they have an assignment
level nonrecurring element entry.

Related Topics

• Absence Elements for Compensatory and Leave Donation Plans

• Options to Define Compensatory Plans

• Options to Define Donation Plans

160

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Overview of Donation Pool Plans

Donation pool plans enable employees to donate their accrued leave to a central pool, and eligible employees can then
claim leave from that pool.

Donation pool elements are created so that Payroll calculates the monetary value of those employee donations and
claims, and maintains the total monetary value of the donation pool. The donation pool value is credited or debited
based on the donations and claims.

You can create absence accrual elements and enable them for donating to donation pools. When an employee donates
leave from an accrual-based absence plan to a donation pool, the plan's element processes the donation in the payroll
run, where it calculates the monetary value of the donations, and transfers that value to the nominated donation pool.

You can create donation pool elements that are associated with a donation pool plan. When an employee's claim from
a donation pool is approved in Absences, the donation pool element processes the claim in the payroll run, where it
calculates the monetary value of the claims, and transfers that value out of the nominated donation pool.

You can review the donations and claims that are processed in a payroll run by using the Balance by Date task with the
Absence Donation for Employee Balance Report balance group usage.

For more information, see How do I configure payroll to set up absence donation pools?

Related Topics

• Overview of Donation

• Options to Define Donation Plans

• Create a Donation Plan

• Enroll a Worker in a Donation Plan

Donation Pool Setup for International Payroll

International Payroll customers must enable the rate definition and balance dimensions for the installed legislations of
the Configure Legislations for Human Resources task.

Enable the Rate Definition and Balance Dimensions
The Absences Donation Pool rate definition returns a payroll balance that shows the total monetary value of a
donation pool, calculated as of the last payroll run. This rate definition is used in Absences to display the total monetary
value of the donation pool for the HR Administrator, when reviewing an employee's request to claim leave from a
donation pool.

Here’s how you enable the rate definition and balance dimensions:

1. Navigate to the Configure Legislations for Human Resources task.
2. On the Installed Legislations page, select your legislation from the list.

161

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

3. To enable the rate definition:

Chapter 2
Elements, Earnings and Deductions

In the Overview pane of your legislation page, click Legislative Rules.

a.
b. Click Edit and then click Save.

4. To enable the balance dimensions:

In the Overview pane of your legislation page, click Balance Dimensions.

a.
b. Click Edit.
c. Select the Base Name checkbox to select all balance dimensions.
d. Click Save.

5. Click Done.

Frequency Rules

Use frequency rules to process a recurring element at a frequency other than the one you defined for the payroll.

For example, you can use a frequency rule to process a monthly deduction in the third payroll period of the month
for employees that are paid on a weekly basis. For employees that are paid on a semimonthly payroll, you can use
a frequency rule to process the monthly deduction in the second period of the month only. In these cases, define a
different frequency rule for each element.

Column headers dynamically display on the Element Summary page based on the frequency period. For example, if
the payroll period is weekly, the column headers are Week 1, Week 2, and so on. To control how often to process the
element, select the periods you want.

Controlling the Processing of Recurring Elements
The Date field on the Element Summary page provides three values. This table explains the three options you can use to
control the processing of recurring elements.

Field Value

Date Earned

Effective Date

In this context the effective date is the date on
which the payments are processed.

Description

How Pay Periods are Derived

Date on which the application processes
element entries for the payroll run.

Uses the pay period end date of the period that
contains the date earned to identify the number
of pay periods in the month.

Usually this is the date between the first day
and last day of the payroll period.

Uses the pay period end date of the period
that contains the effective date to identify the
number of pay periods in the month.

162

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Field Value

Description

How Pay Periods are Derived

Note:
For offset payrolls, where the effective date
isn't within the start and end dates of the
current period, the end date of the period
that contains the effective date is used.

For example, you have an offset payroll
where the period start date is 01-February,
the end date is 14-February, and the effective
date for the process is 16-February. In
this case the actual period end date is 28-
February because the effective date (16-
February) is between 15-February and 28-
February.

Payroll Run Date

Date used by the payroll calculation process
to retrieve effective values such as employee
details.

Uses the payroll run date to identify the number
of pay periods in the month.

Note:
While the payroll run date is essentially the
same as the effective date, the frequency
rules process uses a different method to
identify the number of the period in the
month.

Example of Using the Payroll Run Date Option
Let's say you deduct pre-tax medical insurance payments twice a month for all employees on your biweekly payroll.
In this scenario, you should select the Payroll Run Date option. Selecting this option ensures your payroll application
doesn't process more than two deductions for the month.

The pay period dates listed in this table are for a biweekly payroll.

Pay Period

Pay Period Start Date

Pay Period End Date

Payroll Run Date

1

2

3

19-December-2015

1-January-2016

6-January-2016

2-January-2016

15-January-2016

20-January-2016

16-January-2016

29-January-2016

3-February-2016

This table describes how the process identifies the number of deductions taken for each of the date values when you
process your January payroll.

163

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Field Value

Date Used to Derive the Number of Pay
Periods

Number of Deductions Taken for January

Date Earned

Pay period end date

Effective Date

Pay period end date

Payroll Run Date

Payroll run date

3

3

2

Note:
Deductions would be taken out for the first
two pay periods only because the payroll run
date for the third pay period is in February.

Element Frequency Rules for Terminated Employees
When you terminate the employment of an employee, the application normally ends the payment of recurring elements
such as salary, therefore frequency rules can't be applied. The application processes frequency rules in the payroll
period in which the employee terminates but these rules aren't processed in subsequent payroll periods. You can use
element entry start and end dates to control the frequency of recurring elements for terminated employees.

Related Topics

• Restrict Payroll Processing

Rate Conversion Rules

You can select specific formula rules when you create an element to manage rate conversions. Conversion rules apply to
earnings classification elements, including standard, supplemental, absence, and time elements.

Use one of these approaches to specify these conversion rules.

• Periodicity, if you select a calculation rule for flat amount, hours multiplied by rate, or days multiplied by rate

• Work Units, if you select flat amount calculation rule for a standard or supplemental earnings element

• Proration, if the element is subject to proration

Note:  Unlike earning elements, Absence and Time Card elements don't have element input for conversion rules. To
edit the conversion rules for such elements after they're created, do these steps:

1. On the Calculation Value Definitions page, search for and select the time card element.
2. Change the default value for the rate conversion rule from Standard Rate Annualized to Periodic Work Schedule

Rate Annualized.

Conversion Rules
This table describes the predefined formula rules.

164

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Conversion Rule

Calculation

Example

Standard Rate Annualized

1. Converts the source amount and

periodicity to an annual value using
default values of 2080 hours, 260 working
days.

2. Converts the amount to the required

periodicity and rate.

Standard Rate Daily

1. Calculates a daily rate using default value

260 working days.

2. Converts the amount to the required

output periodicity and rate.

Standard Working Hours Rate Annualized

1. Converts the source amount and working

hours to an annual value, using the
employee's standard working hours.

2. Calculates the rate.

Assignment Working Hours Rate Annualized

1. Converts the source amount and working

hours to an annual value, using the
employee's working hours.

2. Calculates the rate.

Employee works 40 hours a week with a
monthly salary of 1000 pounds:

((1000*12) / (40.00*52) = 5.77 an hour

Employee works 40 hours a week, with a 37.5
standard working hours a week, and a monthly
salary of 1000 pounds:

((1000*12) / (37.50*52) = 6.15 an hour

Periodic Work Schedule Rate Annualized

1. Converts the monetary value and work
schedule to an annual value, using the
employee's work schedule for the payroll
period for daily and hourly conversions.

2. Calculates the rate.

Employee assigned a payroll:

Employee has a monthly salary of 1000 pounds,
 and is assigned a monthly payroll. The formula
checks the work schedule details for the month.

For a daily conversion:

1000 a month / 20 days in the month = 50

Employee not assigned a payroll:

1. Rate is calculated using the weekly rate

calculation.

2. The amount is converted to an annual

amount.

3. The amount is divided by the number of
days or hours in that week based on the
work schedule.

Work Schedule Calculations
For the Periodic Work Schedule Rate Annualized rule, the formula determines whether a work schedule exists for a
person. The calculation begins at the assignment level and continues in the mentioned order until it finds a schedule.

1. Assignment
2. Position
3. Job
4. Department
5. Location
6. Legal Employer
7. Enterprise

165

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Consider these conditions to accurately calculate elements for a payroll period:

• Confirm that a work schedule assigned to a person exists at the start date of the payroll period in which you're

paying the person.

•

If a person has multiple assignments for a term, create the work schedule at terms or assignment level, but not
at both levels. You could find calculation errors while setting up schedules at both levels.

Related Topics

• Calculation Value Definitions

• Calculation Types in Calculation Value Definitions

Element Input Values

Overview of Element Input Values

An element's input values define the entry values available on each entry of an element. Each input value has a unit of
measure, such as money or date.

Input values can include validations and conditions to control the data entry of the element entry assigned to a person.
For example, an earnings element may have an input value for hours worked that's required and has a unit of measure
of number.

When you create an element, some input values are created automatically depending on your country extension and
the element classification. You can create more input values for any element, as needed.

Note:  You can't add an input value to the element if any payroll process were run after the element was created. This
behavior holds good irrespective of whether the payroll run included this element or not. To add input values, rollback
all processes that were ran after the element creation date.

Input Value Options
For each input value created, you can change these attributes:

Field Value

What You Do

Display Sequence

Enter a number to control the display order of the entry value on element entries.

Special Purpose

Select how the input value is to be used. For example, you can indicate that it holds a percentage value,
a rate, or third-party payee details. This value helps with processing the input value based on what type
of information it holds.

Unit of Measure

Select the value that describes the type of value the entry value can hold, such as number or character.

Displayed

Select to display the input value on the element entry.

166

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Field Value

What You Do

Allow User Entry

Select to enter values on element entries.

Required

Select to make the input value a required entry value on the element entry. If you select Required, you
must also select Displayed and Allow User Entry.

Create a Database Item

Select to make the values available for formulas or HCM extract.

Rate Formula

Select a rate calculation formula, for example to return a value from a user-defined table. This option
only applies to the Primary input value for elements associated with rate definitions that have the
Element method and a contributor type of Amount. If you select a formula, you must not select Allow
User Entry.

Default

Enter a value that appears as the default value for this entry value in element entries, if needed.

Apply default at runtime

Select to apply the default value when you run the payroll process, rather than when you create the
element entry. This selection ensures you use the latest value on the date of the payroll run. You can
manually override the default value on the element entry.

Minimum

Maximum

Enter a minimum value, if needed.

Enter a maximum value, if needed.

Validation Formula

Enter a formula that validates the entry value entered on element entries, if needed.

Validation Source

Lookup Type

Warning or Error

Use with the other input value options to select the valid validation method, such as lookups or
formulas.

Specify a lookup type to provide a list of values for an entry value. This option is available for input
values of type Character only.

Use when you're validating the input value or entering a minimum or maximum value. It specifies
whether a warning or an error displays if the entry fails the validation condition or doesn't meet the
minimum or maximum value indicated.

Reference

Use to associate a balance context with the run result.

For example, you can associate a context, such as jurisdiction, with an element. Create an input value
for jurisdiction and select the jurisdiction context in the Reference field. Then the run result value of
the input value works as a context value when updating the balance.

If you select a reference, then the lookup type and validation source values should be automatically set
to the reference context. You must provide the Reference field first for the validation source value to
be automatically populated.

Value Set

Specify a value set to provide a dynamic list of values for an entry value. This option is available for
input values of type Character only.

167

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

CAUTION:  Once an element is processed, you can't update certain input value attributes, such as unit of measure.
This restriction ensures that you can't change attributes that would invalidate prior results.

This table provides examples of the allowable formats, depending on the unit of measure (UOM) specified for the entry
value.

Unit of Measure

Sample Entry Value

Display in Application

Character

Integer

Number

Day

Money

Hours in decimal format, 1 place

Hours in decimal format, 2 places

Hours in decimal format, 3 places

C

12345

12345.6789

0.123456789

123

0.123

12345

-12345.67

12345

12345

12345

Hours expressed as a numeric value

12345

Hours and minutes expressed as numeric
values

Hours, minutes, and seconds expressed as
numeric values

Date

Time

12345

12345

2016-06-21

13:05

Complete

12,345

12,345.6789

0.123456789

123

0.123

12345.00

<12345.67>

12345.0

12345.00

12345.000

12345

12345:00

12345:00:00

21-Jun-2016

1:05 PM

Note:  Display values can be derived from the meaning attribute of the view object. For example if you enter C as a
value for the Character UOM, it displays as Complete. Conversion to display formats is based on the profile option
value and locale.

168

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Related Topics

• Overview of Payroll Elements

• Create and Edit Profile Options

• How Element Setup Affects Standard Entries and Their Values

• Use a Value Set for an Element Input Value

Use a Value Set for an Element Input Value

You can use value sets to provide a dynamic list of values for an element input value. Use a value set for lists containing
values that already exist in tables.

For example, person name or number, legislative data group, or payroll statutory unit. The benefit of this approach is
that you don't have to create and maintain a lookup type. Using value sets helps maintain consistency and accuracy in
your data.

Note:  The only type of value set supported for element input values is the table-based value set. Oracle Fusion Global
Payroll doesn't support other value set types, such as Independent or Format Only.

Use the Manage Value Sets task in the Setup and Maintenance work area.

Create value sets using the Manage Value Sets task. You select the Table validation type to define a value set that filters
values from an existing table using a SQL statement.

This table provides the required values that you enter when you create a value set for use on the Manage Elements
page.

Field

Module

Value

Global Payroll

Validation Type

Table

Value Data Type

Character

Note:  To enable the Value Set field on the Manage Elements page you must select Character as the Unit of Measure
for the input value.

To improve the performance of your value set queries, use these contexts to filter the value set records:

• PayrollRelationshipId

• PersonId

• PayrollTermId

• PayrollAssignmentId

• LegDataGroupId

169

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

• LegCode

• SysEffectiveDate

Chapter 2
Elements, Earnings and Deductions

WHERE Clause example: pay_pay_relationships_dn.payroll_relationship_id = :{PARAMETER.PayrollRelationshipId}

Note:  If you use these contexts in your value set SQL, make sure the WHERE clause parameter name matches the
context name.

In this example, an element contains input values for legislative data group and element name. The list of values for
element name depends on the selected legislative data group. As part of setup, you can select a default legislative data
group for the element, or for a specific element eligibility record.

In summary, here are the steps:

• Create a value set to return a list of all legislative data groups

• Create a value set that returns all elements in the legislative data group

• Add the value set codes to the Manage Elements page

Create a Value Set to Return a List of all Legislative Data Groups

1. From the Setup and Maintenance work area, search for and select the Manage Value Sets task.
2. Click Create.
3. Complete the fields, as shown in this table.

Field

Value Set Code

Value

LDG_VS

Description

Retrieve Legislative Data Groups

Module

Global Payroll

Validation Type

Table

Value Data Type

Character

FROM Clause

PER_LEGISLATIVE_DATA_GROUPS_vl

Value Column Name

NAME

ID Column Name

WHERE Clause

LEGISLATIVE_DATA_GROUP_ID

business_group_id=202

170

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Field

Value

Tip:

Chapter 2
Elements, Earnings and Deductions

To avoid failure of the value set, use IDs instead of names in case the display name changes

in the future.

ORDER BY Clause

NAME

4. Click Save.

Create a Value Set that Returns all Elements in the Legislative Data Group

1. On the Manage Value Sets page, click Create.
2. Complete the fields, as shown in this table.

Field

Value Set Code

Value

ELE_VS

Description

Elements

Module

Global Payroll

Validation Type

Table

Value Data Type

Character

FROM Clause

pay_element_types_f

Value Column Name

base_element_name

ID Column Name

element_type_id

WHERE Clause

LEGISLATIVE_DATA_GROUP_id=:{PARAMETER.LDG_IP}

Note:

LDG_IP is the input value name.

ORDER BY Clause

base_element_name

171

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Field

Value

3. Click Save.

Add the Value Set Codes to the Elements Page

1. On the Home page, click the Elements quick action under the My Clients Groups tab.
2. Create a new element to meet your requirements and then click Submit.
3. When the Element Summary page displays, click the Input Values folder.
4. Click Actions and then select Create Input Values.
5. Enter the name LDG_IP and the display sequence for the input value.
6. Select Character as the Unit of Measure.
7. Enter LDG_VS in the Value Set field.
8. Go to the Default field and select a legislative data group.
9. Click Save.
10. Click Submit.
11. Repeat these steps to create an element input value using the ELE_VS value set.

You can override the default values on the Element Eligibility - Input Values page for a specific eligibility record.

Standard Element Entries

Enable Automatic, Multiple, or Additional Standard Element
Entries Options

You can select one of these options for an element to define how you can update its element entries:

• Automatic entry

• Allow multiple entries in same period

Automatic Entry
When you create an element, you can select Yes for the question: Should every person eligible for the element
automatically receive it? This setting selects the Automatic entry option by default for all eligibility records you create
for that element. However, you can override the selection for any specific eligibility record before you save it.

When you select this option, saving the eligibility record initiates a payroll flow to create element entries for all eligible
workers. To monitor this flow, you do these tasks:

• View the progress of the process in the Automatic Entry Status field. If the status shows that an error

occurred, you can save the eligibility record again to resubmit the flow.

• Monitor the progress of the Generate Automatic Element Entries flow on the Processes and Reports tab.

Any updates to the employment records of eligible workers, including hires and terminations, automatically update,
create, or end the element entries, as appropriate.

172

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Tip:  If you select the Automatic entry option, you can't also select Allow multiple entries in same period.

Allow Multiple Entries in Same Period
This option enables you to give a person more than one entry of the element in the same pay period. Let's consider the
scenario when you enter overtime hours on a weekly basis for a person that's paid monthly. In this case, you might need
to enter five entries on an overtime element in each period.

If you're creating a net-to-gross element, you must select Allow multiple entries in same period.

Note:  An element with the Automatic entry option selected can't allow multiple entries in the same period.

Related Topics

• Default Values for Standard Element Entries

• Standard Entry Methods

• Status of Flow Tasks

Options to Determine an Element's Latest Entry Date

An element's latest entry date determines how element entries process after a person is terminated or transferred to
another payroll.

The options include: final close, last standard earning date, and last standard process date. These are the predefined
options. You can create others that fit your business needs.

Final Close
Use this option to let the element stay open for entries beyond a person's last day worked. For example, you may want
the element to stay open to pay a severance package.

Last Standard Earning Date
Use this option to stop all element entries on the date the person leaves. You can use this option for recurring entries,
such as salary.

Tip:  If you select the last standard earning date option, also select proration for the element. This ensures that the
element is processed up to this date, even if it isn't active at the end of a payroll period.

Last Standard Process Date
The application sets the value for the last standard process date to the last day of the pay period in which the person is
terminated. However, you can set it to a later period when you terminate the person. The application stops all element
entries on the last standard process date or on the date the assignment ends, if it's earlier.

173

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Related Topics

• Overview of Payroll Elements

• How Element Setup Affects Standard Entries and Their Values

Default Values for Standard Element Entries

Specify default values for element entries using the Elements task. Your element setup controls when the default value
affects element entries.

You can apply the default value in any of these scenarios

• When you create an element entry

• At run time

• When you use a formula to define default values on one or more entry values

You can do these actions:

• Set a default value for an input value, or select a defaulting formula for the element.

• Override the default value or formula for a specific group of employees that an element eligibility record

identifies.

• Override the default value for specific employees on their element entries.

Define Default Values at Element Entry Creation
When you create or edit input values, you can specify a default value. If you don't select the Apply default at runtime
option, subsequent updates to the default value have no effect on existing element entries. Users can override or
change the default value at any time.

Define Default Values at Runtime
To use this method, enter the default value and select the Apply default at runtime option for the input value. If
the element entry value is left blank, the payroll process uses the current default value from the element or element
eligibility record. If you enter a value, the manual entry overrides the default value and updates to the default value don't
affect that entry. If you want to restore the default value, clear the entry.

Use a Formula to Provide Default Values
You can create a formula of type element input validation to provide default values for one or more entry values. Select
this formula in the Defaulting Formula field for an element or element eligibility record.

Here's the order of precedence:

1. A formula at the element eligibility level overrides a formula at the element level.
2.

If you enter a default value for the input value and select a defaulting formula, the formula overrides the default
value.

Related Topics

• How Element Setup Affects Standard Entries and Their Values

174

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Element Input Validation Formula Type

You can use an element input validation formula to validate one or more element entry values. You can also use this
formula type to provide a default value for an element entry value.

Also, you can calculate entry values based on the user's entries in other entry values.

You select the formula on the Element Summary page in these fields:

Page Section

Field

Purpose

When Does the Formula Run?

Element Details or Element
Eligibility

Validation Formula

Validates one or more entry values
for the element based on entries in
other entry values.

When you save the element entry.

Element Details or Element
Eligibility

Calculation Formula

Provides values for one or more
entry values using a calculation
formula that takes input from these
entry values or other entry values.

When you save the element entry.

Element Details or Element
Eligibility

Defaulting Formula

Provides default values for one or
more entry values.

When you create the element
entry.

Input Value

Validation Formula

Validates one entry value
independent of others.

When you enter a value.

Note:  A formula at the element eligibility level always overrides an equivalent formula at the element level.

Here are the contexts that are available to all formulas of this type:

• LEGISLATIVE_DATA_GROUP_ID

• DATE_EARNED

• EFFECTIVE_DATE

These contexts are available to formulas only at element or element eligibility level; they aren’t available to validation
formulas at the input value level:

• PERSON_ID

• PAYROLL_RELATIONSHIP_ID

• PAYROLL_TERM_ID

• PAYROLL_ASSIGNMENT_ID

• HR_RELATIONSHIP_ID

• HR_TERM_ID

• HR_ASSIGNMENT_ID

Here are the input variables that are available to formulas of this type.

175

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Formula Usage

Input Variables

Comments

Validation formula at input value level

entry_value

Passes the value to be validated. You must
declare the input variable as the appropriate
type for the element input value.

Validation formula at element or element
eligibility level

Any element input value name that
corresponds to an entry value.

Replace spaces in the input value name with
underscores in the input variable name.

It doesn't matter whether you use uppercase or
lowercase for the name.

Defaulting formula

None

Use database items or other logic instead.

Calculation formula

Any element input value name of an entry
value.

Replace spaces with underscores.

You need not provide all the available entry
values.

Here are the return values that are available to formulas of this type.

Formula Usage

Return Values

Comments

Validation formula at any level.

formula_status

Must be either 'S' (success) or 'E' (error).
Required.

Validation formula at any level.

formula_message

The text of the message is passed to the user if
the validation fails. Optional.

Defaulting formula

Any element input value name of an entry
value.

A return value overrides any default value that’s
provided on the input value in the element or
element eligibility record.

Calculation formula

Any element input value name of an entry
value.

You don't need to return all the available entry
values. You can return the entry values that
were passed as input variables or other entry
values.

Here are a few sample formula that you can use:

• Validation formula at input value level

• Validation formula at element or element eligibility level

• Calculation formula at element or element eligibility level

• Defaulting formula at element or element eligibility level

Validation formula at input value level:

inputs are entry_value(date)
if(entry_value = '01-APR-2008' (date)) then
(
formula_message = 'Valid date'

176

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

formula_status = 'S'
)
else(formula_message = 'Invalid date'
formula_status = 'E'
)
return formula_message, formula_status

Validation formula at element or element eligibility level:

inputs are hours_worked, rate, earning_date(date), comment(text)
if(hours_worked > 80) then
(
formula_message = 'You are within the working limit.
'formula_status = 'S'
)
else
(
formula_message = 'You have worked too many hours.
'formula_status = 'E'
)
return formula_message, formula_status

Calculation formula at element or element eligibility level:

inputs are hours_worked, rate, comment(text)
if(hours_worked > 80) then
(
rate = rate * 1.2
comment = 'Your rate has been increased'
)
return rate, comment

Defaulting formula at element or element eligibility level:

if(CATEGORY = 'S') then
(
rate = 20
)
else
(
rate = 30
)
rate_code = 'B'
return rate, rate_code

Formula Result Rules for Elements

An element's status processing rule identifies the formula that the payroll run uses to process the element for workers
with a specified assignment status. For each status processing rule, formula result rules determine what happens to
each result that the formula returns.

Status Processing Rules
An element can have one status processing rule for all assignment statuses, or a different rule for each status. For
example, you could have two rules for a Wages element: Standard Wages and Paid Training Leave.

177

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Formula Result Rules
Formulas return formula results, such as the amount to be paid, or a message. Results can update the current element
entry or another element entry with a lower processing priority.

This table explains the available result rules.

Results Rule

Direct Result

Indirect Result

Message

What's Its Use

The element's run result, or a direct result updating one of the element's input values.

An entry to a nonrecurring element that has a lower processing priority. The target element must be at
the same employment level as the source element.

A message issued by the formula under certain conditions. For example, a formula can check a loan
repayment balance and, if the balance is zero, issue the message Loan is repaid.

There are three severity levels for a message rule:

• Error - Causes the run to roll back all processing for the employment record.

• Warning - Doesn't affect payroll processing but warns you of a possible problem.

•

Information - Doesn't affect payroll processing.

Order Indirect

Updates the subpriority of the element you select in the Target Element Name field.

Stop

Uses the Date Earned of the payroll run to stop the processing of a recurring entry. A stop rule can be
based upon reaching a specified accumulator, such as a balance owed of zero. The date upon which
the total owed is reached appears on the Element Entries page as Settlement Date. The entries aren't
actually end dated but stopped from future processing. This rule supports retroactive processes which
impact the total owed balance.

You should define the target element with Allow Multiple Entries selected. This option enables you
to allocate a new entry once the value of an existing entry has reached zero. For example, once an
employee has repaid a loan you can add a new loan entry for the employee. If you add a new stop entry
for the same element type, use balance contexts to differentiate between the owed balances.

Note:
Let's assume you don't select Allow Multiple Entries and you add a second loan after the first loan
has been stopped by a payroll run. In this case, end date the first loan before creating the second
loan.

Target Indirect

An entry to a nonrecurring element that has a lower processing priority. Here, the target element is
defined at a different employment level than the element being processed. For example, you could use
a Target Indirect rule to update the input value of an assignment-level element from the processing of
a payroll relationship element.

178

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Element Eligibility

Element Eligibility

Use element eligibility to determine which people are eligible for an element. To determine eligibility,select the criteria
that people must receive entries of the element.

These examples show how you can define element eligibility and restrict who can receive an element entry.

• Your enterprise provides company cars only to people in the sales or customer support departments. Create

two eligibility records and use the Department field to specify the eligibility criteria. Select Sales Department for
one record and Customer Support for the second record.

• Your enterprise offers a production bonus to people who work full-time in production and are on the weekly

payroll. You create one eligibility record and select Full-time regular in the Employment Category field,
Production in the Department field, and Weekly in the Payroll field.

Define at least one element eligibility record for every predefined element and each element you create.

Note:  Create an eligibility record for the statutory deduction elements like Tax before you start hiring workers.

Eligibility Criteria
This table lists the criteria you can use to define element eligibility rules.

Element Eligibility Criteria

Level

Available Criteria

Payroll Relationship

Payroll Statutory Unit

Relationship Type

Assignment

Legal Employer

Department in which the person works

Job, for example, associate professor or secretary

Grade

Employment Category

People Group

Note:  You set up all the people groups appropriate for your enterprise. For example, you could

group people by company within a multicompany enterprise or by union membership.

179

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Level

Available Criteria

Location of person's office

Position

Payroll

All Payrolls Eligible

Note:

Define eligibility rules based on the payroll criteria for all assignment elements such as salary. Select

the 'All Payroll Eligible' option if your company doesn't have eligibility rules based on an employee's

payroll. The 'All Payroll Eligible' option ensures all employees who are assigned to a payroll will be

eligible for the element.

Bargaining Unit

Collective Agreement

Union Member

Define element eligibility for every element, including predefined elements and indirect elements. If you want the
element to be available to all workers, add an eligibility name and save the element eligibility record with no additional
criteria selected. This is the usual practice for compensation and benefit elements where you decide eligibility using
eligibility profiles.

Multiple Rules of Eligibility
You can define more than one eligibility record for each element, but there must be no overlap between them.

For example, you can create one record for the combination of grade A and the job of accountant. However, you can't
create one record for grade A and a second for the job of accountant. These rules would imply that an accountant on
grade A is eligible for the same element twice.

If you have more than one element eligibility record, you can enter different default values and costing information for
each eligibility group.

Maintain Element Eligibility

After saving an element eligibility record, you can only make certain changes. You can't update the eligibility criteria.

This table summarizes the actions you can take.

180

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Action

What's The Result

Change the input value default values and
validation

These changes affect all new entries, and updates to existing entries. Changes to runtime defaults
affect existing entries too.

Delete the element eligibility record

The application automatically ends all existing recurring entries when you end the element's eligibility.

Note:
You can't delete the element eligibility record if any nonrecurring entries exist at the date you want
to end the record. You must delete existing entries before you end the element's eligibility.

Related Topics

• Payroll Element Eligibility

Add Eligibility Rules for Predefined Elements

If the country extension on the Manage Features by Country or Territory page is set to Payroll or Payroll Interface, you
must add element eligibility records for predefined statutory deduction elements before you hire any workers.

Here's how you can search for the predefined elements:

1. Go to the Elements task.
2. Click Go to Task.
3. Search for these predefined elements:

Country or Territory

Predefined Element

US, Canada, Mexico

US Taxation, CA Taxation, MX Taxation

Australia, India, Singapore

Statutory Deductions

Kuwait, Saudi Arabia, United Arab
Emirates, Bahrain, Qatar and Oman

Social Insurance

China

UK

Gratuity

GOSI

Aggregation Information

Tax and NI

Pensions Automatic Enrollment

Netherlands

Tax and Social Insurance Calculations

France

French Payroll Processing

181

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Country or Territory

Predefined Element

Note:  There are no predefined elements that require eligibility rules for Germany, Ireland, Switzerland, or Hong Kong.

Here's how you can add eligibility rules:

1. Click the element name to open the Element Summary page.
2. Enter a date in the Effective As-of Date field.

Use the start date of the element, which is 1/1/1901.

3. Enter a name for the eligibility rule and click Submit. Since you haven't selected any eligibility criteria, all

employees are eligible for the element.

4. Click Done.

Voluntary Deductions

Define Voluntary and Pre-statutory Deductions

Use the Elements task to define voluntary and prestatutory deductions, such as pensions. You can manage pension
deductions through calculation cards or element entries, depending on country-specific rules.

You can also manage other voluntary deductions, such as gym membership, union membership, and charity donations,
through element entries.

Use these steps to set up deductions:

1. Define the elements.
2. Define the third-party payees.
3. Define a third-party payment method for each third-party payee.
4. Enter the deduction details for each person. Do this in the following ways, depending on the deduction type

and your setup:

◦ Configure a Benefits and Pensions calculation card.
◦ Define element entry.
◦ Load benefit batches.

Define Elements
When you define a pension plan deduction, if you select the Benefit category, or it's selected for you, the element
template defines a calculation component. You add this component to Benefits and Pensions calculation cards to assign
it to your workers.

To define other voluntary deductions:

• Select the Standard category.

This selection means you manage these deductions using the Element Entries task.

182

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

• After defining the element, you must add a Payee input value and select Third-Party Payee as the special

purpose for it.

If appropriate, enter a default value on the element or element eligibility record to populate the third-party
payee details.

Note:  You can streamline the creation of Voluntary Deduction and Pretax Deduction elements by reducing
the number of rules created. The application creates stop rules only if you had selected the total owned
option when you created the element.   If you had selected No for the template question Processing Stop
when the Total is Reached, the application doesn't create the stop rule for the element.

Define Third-Party Payees
To define third-party payees, use the Third Parties page in the Administration section.

For pensions, select the Organization payee type and select the Pension Provider party usage code.

Define Third-Party Payment Methods
To define payment methods for all external payees, you can use the Third-Party Payment Methods task in the Person
Information section.

Enter Deduction Details for Each Person
For pensions using the Benefit category:

1. Configure a Benefits and Pensions calculation card for the worker.
2. Add your new pension calculation component to the card.
3. Enter the payee and other details.

If you load your pension information using the Load Benefit Batches process, the payroll application configures the
calculation card automatically. Before running this process, you must generate an XML file that contains the data you
want to transfer to payroll.

For other voluntary deductions, you must define element entries. If the payee isn't defaulted from the element or
eligibility record, enter the payee on the element entry.

Related Topics

• Third-Party Payment Methods

• Considerations to Enter Calculation Values for Pensions

• Create Elements for Pension Deductions

Create Elements for Pension Deductions

This example shows you how to create a pension deduction element using an element template. Follow these steps:

1. Create a pension deduction element
2. Create an eligibility record for the deduction

183

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Creating a Pension Element

1. On the Home page, click the Elements quick action under the My Client Groups tab.
2. Click Create.
3. Complete the fields, as shown in this table.

Field

Value

Legislative Data Group

Your Legislative Data Group

Primary Classification

Voluntary Deductions or Pre-statutory Deduction

Secondary Classification

Appropriate classification for your country or territory, such as Pension Plan After Tax

4. Click Continue.
5. Complete the Basic Information page. For the latest entry date:

◦ Select Last Standard Earning Date if you enable proration for the element.
◦ Otherwise, select Last Standard Process Date.

6. Click Next.
7. On the Additional Details page, enter the calculation rules and limits for the deduction. This table summarizes

your choices.

Rules

What You Can Enter

Calculation rule

Fixed amount or percentage

Age limits

Minimum and maximum age

Maximum contribution amount

Any numeric value

Pensionable earnings limit

Minimum and maximum amount

Additional contributions allowed

Yes, or no. If yes, select calculation rule.

Employer contributions allowed

Yes, or no. If yes, select calculation rule, age limits, and amount limits

Overrides allowed

Yes, or no

Element subject to proration

Yes, or no

184

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

8. Click Next.
9. Verify the information is correct.
10. Click Submit.

The template creates a recurring element at the payroll relationship level. It also creates a calculation
component with the same name as the element. You add this component to workers' calculation cards.

Creating an Eligibility Record for the Deduction
On the Element Summary page, you can create as many eligibility records as you require:

In the Element Overview section, click the Element Eligibility link.

1.
2. Select Create Element Eligibility from the Actions menu.
3. Enter a name for the eligibility record.
4. Select any criteria if you want to restrict who can pay this deduction.
5. Click Submit.
6. Click Done.

Related Topics

• Considerations to Enter Calculation Values for Pensions

Overview of Deduction Reference

Deduction Reference maintains voluntary deduction balances for each reference number provided.

The deduction reference is a mandatory input value and must be entered to maintain the balances. It should not be
made non-mandatory and left blank to avoid the incorrect balance calculations.

This input value gets created in specific scenarios, as mentioned below, and there by the arrears and accrued balances
are tracked with respect to a specific reference entered using Deduction Reference input value.

There are 2 element template questions in Voluntary Deductions that control the creation of deduction reference and
the corresponding defined balances. You can track and report the arrears / total owed (loan) balances with respect to a
specific reference and it does not combine with another entry either during the same time or even in future.

1. What should happen when there are insufficient funds to cover the deductions? If you enable arrears, a

reference is required for each deduction entry. Available Options:

a. Do not take a partial deduction or create arrears
b. Do not take partial deduction, place all in arrears
c. Take a partial deduction, but do not create arrears
d. Take a partial deduction, place remaining in arrears

Scenario 1: If you select either (b) or (d) options, mandatory Deduction Reference input value and the
corresponding "reference" related dimensions, such as Relationship Tax Unit, Reference Run are created.

Scenario 2: If you select (a) or (c), Deduction Reference input value is not created and the non-reference
related defined balances, such as Relationship Tax Unit, Run is created. Reference related dimensions are
not created.

2. Do you want to stop processing when the total owed is reached? If you enable total owed, a reference is

required for each deduction entry.

185

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

If you select "Yes" for the above template question, mandatory Deduction Reference input value and the corresponding
"reference" related dimensions, such as Relationship Tax Unit, Reference Run are created.

Note:  Get Reference Code from Database Sequence is a default formula that generates a unique reference number
for each element entry. You could also write the formula, such as using Person Number as the Deduction Reference, if
you would like to continue the balances across entries for an employee.

Prerequisites
Review the below points before using the deduction reference functionality:

•

If you would like to have the compatibility of the previous functionality prior to 21C such that the balances will
be maintained across element entries, you can choose any one of the below:

◦ Use the default formula to default the person number as suggested in this document.
◦ Write the default formula to default the payroll relationship number as suggested in the release

documentation.

◦ Default a constant value.

• You should not add or delete the defined balances in balance dimensions of the primary balance of the element

or balance group. Otherwise, it will cause duplicate records in the reports and in the archive.

•

If you would like to maintain the balances separately for each element entry, you can use the delivered default
formula, Get Reference Code from Database Sequence, that generates the unique sequence number as the
reference number for each element entry.

• For the elements using a Benefits module that meets one of the above conditions, we suggest you use a

Default reference value for all entries or use a formula to create a reference based on the Person Number of the
employee or Benefits Plan name. This is because, when an employee is enrolled into a benefits plan, an element
entry is created. When there is a subsequent life event and enrollments, it end-dates the previous element entry
and creates a new entry. If you use the above delivered default formula, the balances will be re-initiated which is
not expected.

Note:  You need to attach the default formula at element level while using the Person Number as the default.
If you are using benefits plan name as the default, you need to define the formula using extra input type and
associate it at Extra Inputs section of benefits plan for deduction reference input value.

• The deduction reference input value is mandatory. Oracle does not recommend making it optional. The

validation formula ensures that the element entry is not created without the deduction reference even if the
deduction reference input value is made optional.

Create Fast Formula
You need to create 2 fast formulas of type “Element Input Validation” to populate the default value in deduction
reference input value and raise an error exception when no value is entered in deduction reference input value.

186

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Note:  Use the delivered default formula, Get Reference Code from Database Sequence, for elements such as Loans to
maintain balances with respect to each entry.
1. Formula to return the person number

Below is the sample formula that returns the person number. Attach this formula to the Default Formula
attribute in element in Default Entry Values and Validation Section.

/* Sample Formula Begins – Defaulting Person Number */
 DEFAULT FOR PER_PER_PERSON_NUMBER is '-1'
 Inputs are Deduction_Reference (text)
 l_person_number = PER_PER_PERSON_NUMBER
 Deduction_Reference = l_person_number
 Return Deduction_Reference
 /* End of Sample Formula – Defaulting Person Number */

2. Formula to validate the element entry

Below is the sample formula that validates the element entry when no value is entered for Deduction Reference
input value. Attach this formula to the Validation Formula attribute for Deduction Reference input value in
Default Entry Values and Validation Section.

/* Sample Formula Begins – Validate required attribution of Deduction Reference input value */
 DEFAULT FOR ENTRY_VALUE IS 'NO VALUE'
 INPUTS ARE ENTRY_VALUE (text)
 IF ENTRY_VALUE WAS DEFAULTED then
 (
 FORMULA_MESSAGE = 'The deduction reference cannot be null. You must enter a value.'
 FORMULA_STATUS = 'E'
 )
 RETURN FORMULA_STATUS, FORMULA_MESSAGE
 /* End of Sample Formula – Validate required attribution of Deduction Reference input value */

Attach Formulas to Element

1. Attach the default formula to Default Formula attribute in Default Entry Values and Validation Section at

element level.

187

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

2. Attach the validation formula to Validation Formula attribute for Deduction Reference input value in Default

Entry Values and Validation Section.

Note:

◦ You need to date track to the start date of the element.
◦ If you have any date effective update record of the element, ensure that the formulas are

associated to all date effective records.

◦ Once you attach these formulas, the default value will be populated while creating the element

entry and validation will be performed.

Calculation example with and without reference
Let's examine two common examples: calculations with reference and calculations without reference.

• Deductions with Arrears only enabled

• Arrears Enabled but no Total Owed – Without Reference

Deductions with only Arrears enabled

1. Arrears Enabled but no Total Owed – Without Reference

You create an element entry with every pay period deduction of $100. The entry starts from 01-Sep-2020.
Below are the sample calculation results:

Element Name

Pay Period

Deduction (RUN)

Arrears (RUN)

Total Deduction

Arrears (ITD)

Deduction1

30-Sep-2020

31-Oct-2020

30-Nov-2020

31-Dec-2020

100

100

70

80

0

0

30

20

(ITD)

100

200

270

350

0

0

30

50

In Nov and Dec, the employee does not have sufficient earnings and hence partial deduction has happened. At
the end of the Dec-2020 period, the accrued arrears were 50.

Now, you have end dated the entry.

You create a new element entry of the same element in the month of Apr-2021 with every pay period deduction
as $70. Below are the sample calculation results. Assume that there is a cap of $100 as maximum amount.

Element Name

Pay Period

Deduction (RUN)

Arrears (RUN)

Total Deduction

Arrears (ITD)

(ITD)

188

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Deduction1

30-Apr-2021

100 (70+30 from

-30 (from previous

450 (ideally, it

20 (from previous

previous arrears)

arrears. ideally,

should be 70 for this

arrears. Ideally, it

should be 0)

entry)

should be 0)

31-May-2021

90 (70+20 from

-20 (from previous

540 (ideally, it

0

previous arrears)

arrears. ideally,

should be 140)

should be 0)

2. Arrears Enabled but no Total Owed – With same Reference such as Person Number

If you use the same reference number (such as Person Number) as the Deduction Reference after 21C, then the
calculations would be the same as the results without reference prior to 21C.

3. Arrears Enabled but no Total Owed – With Unique Reference

You create an element entry with every pay period deduction of $100. The entry starts from 01-Sep-2020.
Below are the sample calculation results. The arrears are maintained using the reference PLN2020.

Element Name

Pay Period

Deduction (RUN) Arrears (RUN)

Total Deduction

Arrears (ITD)

Deduction1

30-Sep-2020

31-Oct-2020

30-Nov-2020

31-Dec-2020

100

100

70

80

0

0

30

20

(ITD)

100

200

270

350

0

0

30

50

Deduction

Reference

PLN2020

PLN2020

PLN2020

PLN2020

In Nov and Dec, the employee does not have sufficient earnings and hence partial deduction has happened. At
the end of the Dec-2020 period, the accrued arrears were 50.Now, the user has end dated the entry.

You create a new element entry of the same element in the month of Apr-2021 with every pay period deduction
as $70. Below are the sample calculation results. Assume that there is a cap of $100 as maximum amount. The
entry is maintained with reference PLN2021.

Element Name

Pay Period

Deduction (RUN) Arrears (RUN)

Total Deduction

Arrears (ITD)

Deduction1

30-Apr-2021

31-May-2021

70

70

0

0

(ITD)

70

140

0

0

Deduction

Reference

PLN2021

PLN2021

Note:  Here PLN2020 and PLN2021 are user entered unique reference numbers. You can use the delivered
default formula, Get Reference Code from Database Sequence, that generates the unique reference number
from database sequence that starts with 1.

189

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Deductions with Arrears and Total Owed enabled

1. Arrears Enabled with Total Owed – Without Reference

You create an element entry with every pay period deduction of $100 and with Total Owed as $400. The entry
starts from 01-Jan-2020. Below are the sample calculation results:

Element Name

Pay Period

Deduction (RUN) Arrears (RUN)

Total Deduction

Arrears (ITD)

Remaining

Deduction2

31-Jan-2020

29-Feb-2020

31-Mar-2020

30-Apr-2020

100

100

70

80

0

0

30

20

(ITD)

100

200

270

350

0

0

30

50

Balance

300

200

130

50

You have end dated the entry after 30-Apr-2020. Loan is not cleared. Arrears is left over and remaining balance
is also left over.

a. Total Owed in the 2nd entry is less than Total Accrued in the 1st Entry.

You create a new element entry of the same element in the month of Aug-2020 with every pay period
deduction as $70 and Total Owed as 280. Below are the sample calculation results.

It gets end dated immediately in the 1st run as the accrued deduction from the previous entry is already
350 and the current total owed is 280. It returns the amount 70 with the assumption that it has deducted
additional. It gets end dated in the 1st pay period itself.

Element Name

Pay Period

Deduction

Arrears (RUN)

Total

Arrears (ITD)

Remaining

(RUN)

Deduction (ITD)

Balance

Deduction2

31-Aug-2020

-70

-50

280

0

0

b. Total Owed in the 2nd entry is greater than Total Accrued in the 1st Entry.

You create a new element entry of the same element in the month of Aug-2020 with every pay period
deduction as $70 and Total Owed as 410. Below are the sample calculation results.

It gets end dated immediately in the 1st run after deducting the 60 with the calculation of subtracting
total accrued deduction of previous period from total owed of current period.

Element Name

Pay Period

Deduction

Arrears (RUN)

Total

Arrears (ITD)

Remaining

(RUN)

Deduction (ITD)

Balance

Deduction2

31-Aug-2020

60

-50

410

0

0

2. Arrears Enabled with Total Owed – With same Reference such as Person Number

If you use the same reference number (such as Person Number) as the Deduction Reference in the 2nd entry
also after 21C, then the calculations would be same as the results without reference prior to 21C.

190

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

3. Arrears Enabled with Total Owed – With Unique Reference

You create an element entry with every pay period deduction of $100 and with Total Owed as $400. The entry
starts from 01-Jan-2020. Below are the sample calculation results:

Element

Name

Pay Period

Deduction

Arrears (RUN) Total

Arrears (ITD)

Remaining

(RUN)

Deduction

(ITD)

Deduction2

31-Jan-2020

100

29-Feb-2020

100

31-Mar-2020

70

30-Apr-2020

80

0

0

30

20

100

200

270

350

0

0

30

50

Balance

300

200

130

50

Deduction

Reference

LOAN1

LOAN1

LOAN1

LOAN1

You have end dated the entry after 30-Apr-2020. Loan is not cleared. Arrears is left over, and the remaining
balance is also left over.

You create a new element entry of the same element in the month of Aug-2020 with every pay period
deduction as $70 and Total Owed as 350. Below are the sample calculation results.

It gets calculated correctly and the deduction balances are maintained correctly.

Element

Name

Pay Period

Deduction

Arrears (RUN) Total

Arrears (ITD)

Remaining

(RUN)

Deduction

(ITD)

Balance

Deduction2

31-Aug-2020

70

30-Sep-2020

70

31-Oct-2020

70

30-Nov-2020

70

31-Dec-2020

70

0

0

0

0

0

70

140

210

280

350

0

0

0

0

0

280

210

140

70

0

Deduction

Reference

LOAN2

LOAN2

LOAN2

LOAN2

LOAN2

Note:  Here LOAN1 and LOAN2 are user entered unique reference numbers. You can use the delivered default
formula, Get Reference Code from Database Sequence, that generates the unique reference number from
database sequence that starts with 100.

191

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Involuntary Deductions

Add Involuntary Deductions to a Calculation Card

You use element templates to create the involuntary deduction elements supported for your legislation, such as
bankruptcy orders, garnishments, child support payments, tax levies, and educational loans.

The templates also create calculation components, which you can add to a personal calculation card, so the deductions
are processed during a payroll run.

This figure shows the steps involved in creating an involuntary deduction and adding it to a personal calculation card:

Prerequisites
Before you can add an involuntary deduction to a personal calculation card, you must first:

• Create a third party to receive the payment.

• Create a third-party payment method.

• Create an involuntary deduction element.

You can create multiple elements for the same involuntary deduction type if processing information or other
details vary. For example, each jurisdiction you deal with may have different processing rules for court orders.

192

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Create an Involuntary Deduction Calculation Card
Follow these steps:

In the Payroll section of My Client Groups, click the Calculation Cards task.

1.
2. Search for and select the payroll relationship.
3.
4. Enter a start date for the card and select the involuntary deduction card type.
5. Click Continue.

If the person doesn't already have an involuntary deduction calculation card, click Create.

Add the Calculation Component to the Calculation Card
You can add multiple calculation components for the same or different involuntary deduction types. For example, you
could add two child support components and one garnishment component to the same calculation card.

On the Calculation Cards page:

In the Calculation Components section, click Add Row.

1.
2. Select the calculation component with the same name as the involuntary deduction element.
3. Optionally, enter a number in the Subprocessing Order field if the calculation card will include more than one

calculation component.

By default, the payroll run processes these element entries in order by date received, starting with the oldest
entry.

4. Enter a reference code to uniquely identify this deduction, such as a court order number, case number, or other

identifier provided by the issuing authority.

5. Complete the fields on the Calculation Component Details tab.

◦ In the Involuntary Deduction Payment Details section, select all payees for the deduction.

The payee fields display all third-party person payees associated with this payroll relationship and all
external payees defined for your legislative data group.

◦ In the Involuntary Deduction Rules section, specify the information you require, including:

- The date the involuntary deduction order was received
- The issuing authority (such as a court)
- The frequency of the deduction such as monthly or weekly, regardless of the payroll frequency. If

you leave the Frequency field blank, the application uses the payroll frequency.

Enter Values for the Deduction Amounts
You enter the order amount, fee, or other amounts used in the calculation on the calculation card. The values you
enter replace any default values defined in calculation value definitions. The default order amount for an involuntary
deduction is typically zero.

To create overrides on the Enterable Calculation Values on the Calculation Cards task, complete the fields as shown in
the following table. The values you enter may vary by country or territory, but typically include the items described in
the table below.

Note:  For most values, you can enter either an amount or a rate. Enter a rate if you want the application to calculate
the amount as a percentage of available pay. For example, to define a rate of 20 percent for the order amount, create
an Order Amount (Rate) value. Then enter 20 in the Rate field.

193

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Calculation Value

Description

Order Amount

Rate or amount paid to the Order Amount Payee based on the frequency you specified.

For example, if you specified a frequency of monthly in the component details, enter the amount
to deduct each month, regardless of the payroll period. The application automatically calculates the
correct amount to deduct in each payroll period.

If you leave the Frequency field blank, this amount is deducted at the payroll frequency defined at the
assignment level.

Organization Fee

Rate or amount paid to the Organization Fee Payee each time the deduction is processed.

Person Fee

Rate or amount paid to the Person Fee Payee each time the deduction is processed.

Processing Fee

Rate or amount paid to the Processing Fee Payee each time the deduction is processed.

Initial Fee

Rate or amount paid to Processing Fee Payee the first time this deduction is processed.

Maximum Withholding Amount and
Minimum Withholding Amount

Maximum and minimum rates or amounts that can be withheld in one payroll period for this
deduction.

Maximum Withholding Duration

The number of days after the Date Received that the order is valid. For example, a court order might
only be valid for 90 days after the date issued.

Protected Pay Amount

Amount of the employee's pay that's exempt from this deduction. Only pay exceeding this amount is
included in the deductible amount (available for the deduction).

Exemption Percentage

Percentage of the employee's pay that's exempt from this deduction.

Related Topics

• Examples of Involuntary Deduction Processing

• Third Parties Overview

• Fee and Proration Rules for Involuntary Deductions

• Third-Party Payment Methods

Fee and Proration Rules for Involuntary Deductions

Creating an involuntary deduction creates calculation value definitions that include predefined fee and proration rules.
These rules vary by country and territory.

The following table describes the global rules:

194

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Rule

Fee

Processing

Deduct the fee first, before calculating and paying the deduction amount.

Proration

Use the first come, first serve method.

If a person has multiple orders and there is insufficient money to pay them all, pay the deductions in
the order in which they were received. Start with the oldest.

You can override these predefined fees and proration rules. For details, see the topic Involuntary Deduction Calculation
Value Override Details for the US in the Help Portal.

Related Topics

• Add Involuntary Deductions to a Calculation Card

Examples of Involuntary Deduction Processing

Processing rules may vary by the legislation or the legal authority issuing the order for an involuntary deduction. Let's
look at some examples that illustrate the processing of fees, protected pay amounts, and when employees have multiple
assignments and payrolls.

Payroll processing first calculates disposable income using the disposable income rules. Then it looks at the exemption
rules to calculate the amount exempt from withholding. Using these amounts, it can calculate the amount available to
deduct.

Note:  The payroll process calculates disposable income once, based on the highest processing priority card
component. The exception is regional tax levies, which have a separate disposable income calculation.

You can use these examples to understand how involuntary deductions are processed in different scenarios:

•

Involuntary deduction has initial fee and processing fee

• Deduction amount exceeds protected pay amount

• Employee has multiple assignments and payrolls

• Multiple orders exist with different protected pay amounts

Involuntary Deduction Has Initial Fee and Processing Fee
Scenario: An employee in Country 1 is issued a court order for a monthly garnishment of 500. The order is subject to
two fees. Both fees are paid to the agency responsible for administering the account. The agency then forwards the
payments to the recipients:

• A one time initial fee of 10

• A monthly processing fee of 10

On the involuntary deduction calculation card:

1. Add a calculation component for a garnishment.
2.

In the Calculation Component Details tab:

195

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

◦ Select the Order Amount Payee and the Processing Fee Payee. The processing fee payee is also the

initial fee payee.

◦ Select Monthly in the Frequency field.

3.

In the Enterable Calculation Values tab, enter the following values:

Field

Order Amount

Processing Fee

Initial Fee

Payroll Run Results:

Value

500

10

10

• The amount of the employee's pay subject to deduction is 1000.

• During the first monthly payroll after the court order is received, both the initial fee amount and the processing

fee are deducted. The total deduction amount is 520.

•

In subsequent payroll runs, the order amount and the processing fee are deducted. The total deduction amount
is 510.

Deduction Amount Exceeds Protected Pay Amount
Scenario: An employee in Country 2 is issued a court order for the amount of 100 per month. However, protected pay
rules defined for the deduction require that the employee take home at least 700, after all deductions.

On the involuntary deduction calculation card:

1. Add a calculation component for a court order.
In the Calculation Component Details tab:
2.

◦ Select the Order Amount Payee and the Processing Fee Payee.
◦ Select Monthly in the Frequency field.

3.

In the Enterable Calculation Values tab, enter the following values:

Field

Order Amount

Protected Pay

Value

100

700

196

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Payroll Run Results:

Chapter 2
Elements, Earnings and Deductions

• The amount of the employee's pay subject to the deduction is 750.

• A deduction amount of 100 would leave only 650 for the final pay amount. Therefore, only 50 is deducted for

the month.

• The remaining balance of 50 isn't placed in arrears, based on processing rules defined for this deduction.

Employee Has Multiple Assignments and Payrolls
Scenario: An employee has one payroll relationship with two assignments. They receive paychecks from two different
payrolls. One payroll is run on a weekly basis. The other is run on a monthly basis.

The employer receives a court order to deduct 200 per month from the employee's wages. The court order amount
must be deducted from all available money, regardless of the payroll. If the total order amount can't be deducted from
the first payroll run, then the following occurs. The remaining balance must be deducted from one or more subsequent
runs during the month, until the full amount is paid.

On the involuntary deduction calculation card:

1. Add a calculation component for a court order.
In the Calculation Component Details tab:
2.
◦ Select the Order Amount Payee.
◦ Select Monthly in the Frequency field.

3.

In the Enterable Calculation Values tab, enter the following value:

Field

Order Amount

Value

200

Payroll Run Results:

• During the first weekly payroll run, only the amount of 50 can be deducted, leaving an amount owed of 150 for

the month.

• When the next weekly payroll is run, the deduction can't be taken due to insufficient pay; the balance for the

month remains 150.

• The monthly payroll runs before the next weekly payroll is run. The remaining amount of 150 owed for the

deduction is taken during the monthly payroll run.

• No money is deducted during the subsequent weekly payroll runs for this month.

Note:  If a person has two assignments for different payroll relationships, they would typically be issued two different
court orders, one for each employment. In this case, you would add each court order to a different calculation card.

Multiple Orders Exist with Different Protected Pay Amounts
Scenario: An employee in Country 2 has three court orders. Each court order has a different protected pay amount.

1. On the involuntary deduction calculation card add three calculation components for child support.

197

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

2. For each calculation component, select Monthly in the Frequency field.
3. Define the protected pay and order amount values for each deduction as shown in the following table:

Involuntary Deduction

Protected Pay Amount

Order Amount

Date Received

Child Support 1

Child Support 2

500

600

Child Support 3

1000

1000

1100

1200

23 January 2012

2 February 2012

2 February 2012

Payroll Run Results:

The net amount available for involuntary deductions in the payroll run is 2000 GBP. Based on the processing priority
defined for child support payments, the payroll run processes the involuntary deductions in order by date received.

Here's the result:

• Child Support 1 is paid in full, leaving 1000 available for other deductions.

• Child Support 2 is paid an amount of 400 (1000 less protected pay of 600).

• Child Support 3 isn't paid. The total amount is placed in arrears, based on processing rules defined for the

deduction.

Related Topics

• Add Involuntary Deductions to a Calculation Card

Net-to-Gross Earnings

Calculate Net-to-Gross Earnings

When you create an earnings element, you can indicate that it pays a specified net amount.

Use this feature, if you need to pay a person:

• Guaranteed take-home pay (net) per payroll period

• Bonus of a specified net amount

To create an earnings element, use the Elements quick action under the My Clients Groups tab.

You can create a net-to-gross (gross-up) element for any recurring or nonrecurring earnings element using these
primary classifications:

• Standard Earnings

• Supplemental Earnings

198

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

• Taxable Benefits (Imputed Earnings)

Settings That Affect Net-to-Gross Processing
Define the deductions that are used to calculate the gross amount from the specified net amount.

Answer Yes to the Use this element to calculate a gross amount from a specified net amount? prompt in the
element template to create the element as a gross-up element.

In each element entry, specify the limits of the gross-up processing as follows:

•

•

In the Net value, enter the value you want the employee to receive.

In the To Within value, enter the allowed difference between the desired amount and the actual amount. This
limit can't be 0.

Note:   If these values are the same across most entries, you can enter a default value on the element eligibility record.

How Formulas Calculate the Gross Amount
The formulas for net-to-gross processing perform these actions:

1. The predefined GLB_EARN_GROSSUP iterative formula takes as input the desired net amount (Net input value)

and the amount by which net can differ from the desired amount (To Within input value).
In the first run, the formula performs these actions:

2.

a. Sets the lower gross limit to the desired net amount, and the higher gross limit to twice the desired

amount.

b. Runs a function to provide the first guess of the gross.
c. Returns three values to the element's input values: low gross, high gross, and additional amount.

3. The element's payroll formula runs. The formula adds the additional amount to the desired amount for creating

4.

the gross amount. The formula returns this value to the element's pay value for the payroll run to process.
In the next iteration, the iterative formula compares the additional amount to the total value of the balances
that are available for gross-up for this element entry. The additional amount must not differ from this balance
total by more than the amount you specified in the To Within field.

◦ If the additional amount equals the balance total, the iterative processing ends.
◦ If the additional amount is higher or lower than the balance total by an acceptable margin, the processing
ends. The formula returns the remainder (additional amount minus balance) to the element's Remainder
input value.

◦ Otherwise, the formula runs the function to generate a better estimate for gross, using the remainder to

determine by how much to change the guess. The formula checks the results in another iteration.

Related Topics

• Payroll Element Input Values

• Payroll Element Eligibility

• Overview of Using Fast Formula Components

• Create a Net-to-Gross Earnings Element

199

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Create a Net-to-Gross Earnings Element

This example demonstrates how to create a net-to-gross (gross-up) earnings element when an organization wants to
pay a person a specific net amount on a bonus.

Before you create your earnings element, you may want to consider these decisions:

Decisions to Consider

In This Example

What is the primary classification of this
earning?

Supplemental Earnings

Is the element recurring or nonrecurring?

Nonrecurring

Who is the bonus recipient?

Linda Swift

How much is the bonus?

1000

What is the allowed difference between
the specified bonus and the actual amount
paid?

.05

What is the calculation rule?

Flat amount

Create the Earnings Element

1. On the Home page, click the Elements quick action under the My Client Groups tab.
2. Click Create and then in the Create Element dialog box, select the values as shown in this table.

Field

Legislative Data Group

Value

LDG1

Primary Classification

Supplemental Earnings

Secondary Classification

Bonus

Category

Standard

3. Click Continue.

200

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

4. On the Create Element: Basic Information page, select the values as shown in this table.

Field or Question

Name

Reporting Name

Value

Bonus

Bonus

Effective Date

01/01/2013

Should every person eligible for the

No

element automatically receive it?

What is the earliest entry date for

First Standard Earning Date

this element?

What is the latest entry date for the

Last Standard Earning Date

element?

At which employment level should this

Assignment Level

element be attached?

Does the element recur each payroll

Nonrecurring

period, or does it require explicit

entry?

Process the element only once in

Yes

each payroll period?

Can a person have more than one entry

Yes

of this element in a payroll period?

Process and pay element separately or

Process separately and pay separately

with other earnings elements?

Tax this earning across multiple pay

No

periods?

Prorate this earning across all periods

No

during which it was earned, and

consider it for FLSA calculations,

 such as for commissions, bonuses,

201

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Field or Question

Value

 incentives, and other nondiscretionary

earnings?

5. Click Next.
6. On the Create Element: Additional Details page select the values shown in the table.

Field or Question

Value

What is the calculation rule?

Flat Amount

Note:

The default value is Flat Amount. Do not change this value. All gross-up earnings must have

a calculation rule of Flat Amount.

What is the default periodicity of this

Periodically

element?

Periodicity Conversion Rule

Periodic Work Schedule Rate Annualized

How do you want the work units to be

None

reported?

Is this element subject to retroactive

No

changes?

Use this element to calculate a gross

Yes

amount from a specified net amount?

Should this element be included in

No

the earnings calculation of the FLSA

overtime base rate?

Should this element be included in the

No

hours calculation of the FLSA overtime

base rate?

7. Click Next.
8. Click Submit.

202

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

9.

In the Element Overview pane, select and review each input value, as shown in the table.

Input Value

Description

Pay Value

The gross pay value to be processed in the payroll run, entered by the iterative formula when it

completes gross-up calculations.

Net

The user-entered flat amount, which provides the iterative formula with the desired net pay.

Low Gross

Used by the iterative formula to hold the lower gross pay guess, which feeds into the next

iteration of the formula.

High Gross

Used by the iterative formula to hold the higher gross pay guess, which feeds into the next

iteration of the formula.

Remainder

The amount by which the additional pay to be paid by the employer (gross minus desired net)

differs from the total of the balances that are eligible for net-to-gross processing. This amount

is returned by the iterative formula.

To Within

The amount by which actual net can differ from desired net after normal processing. This

amount must not be zero but can be a nominal amount such as 0.01.

Additional Amount

The amount to add to the desired net to calculate gross pay. This amount is returned by the

iterative formula.

Note:  Not all input values are visible by default.

Create Eligibility Rules

In the Element Overview pane, click Element Eligibility.
1.
2. Select Create Element Eligibility from the Actions menu.
3.
4. Click Save.

In the Element Eligibility Name field, enter Bonus.

Review Iterative Processing Order

1.
2.

In the Element Overview pane, click Bonus.
In the Advanced Rules section, review the iterative order.

Note:  The default value is 1000. If you have more than one iterative element that may be processed in the
same payroll flow, it's important to adjust the iterative order to indicate which should be processed first.
Iterative order must be in the reverse sequence of the processing priority numbers. The element with the
lowest iterative priority number is reduced first.

203

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

Include Balances in the Net-to-Gross Processing
Perform the following steps to include balances:

In the Element Overview pane, click Balance Feeds.
1.
2. Review the balances to which the bonus contributes.
3.
4. Add any balances that have been set to exclude by default if you want to include it on this specific earnings.
5. Click Submit.

In the Element Overview pane, click Gross Balance Exclusions.

Create an Element Entry
In this example, create the element entry for the bonus for Linda Swift.

In the Search Results, select Linda Swift.

In the Name field, enter Swift, Linda.
In the Legislative Data Group field, select LDG1.
In the Effective As-of Date field, enter 01/01/2013.

1. On the Search page, search and select Swift, Linda.
2.
3.
4.
5. Click Search.
6.
7. Click Create.
8.
9.
10.
11. Click Continue.
12.
13.
14. Click Submit.

In the Effective Date field, enter 01/01/2013.
In the Element Name field, select Bonus.
In the Assignment field, select E1026.

In the Net Value field, enter 1000.00.
In the To Within field, enter .05.

Related Topics

• How Net-to-Gross Earnings are Calculated

• Balances in Net-to-Gross Calculations

FAQs for Elements

What's the difference between a recurring and nonrecurring
element?

A recurring element has an entry that applies in every pay period until the entry ends.

A nonrecurring element has an entry that applies in one pay period only. It's only processed once per pay period. The
assigned payroll determines the dates of the person's pay period.

Note:  A base pay element associated with a salary basis must be recurring.

204

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

When does an element get processed with a processing option of
process once per period?

The first payroll run of each period processes the element entries. If this option isn't available for your country or
territory, you can select a skip rule to process the element once each period.

Related Topics

• What's an element's skip rule?

What's an element's skip rule?

A skip rule is an optional formula that determines the circumstances in which an element is processed.

If you specify a skip rule for the element, payroll runs process the element only when the conditions of the formula are
met. Otherwise, it skips the element. You select skip rules on the Manage Elements page.

Related Topics

• Overview of Using Fast Formula Components

• Element Skip Formula Type

What happens if I select the Closed for Entry option for an
element?

The Closed for Entry option prevents the creation of all new element entries for the element. However, it doesn't affect
any existing element entries.

CAUTION:  When hiring, terminating, or updating assignments, this option prevents all element entry creation for the
element, including automatic entries.

Related Topics

• Standard Entry Methods

How can I create an element for retroactive processing?

When you create the element, specify that it's subject to retroactive changes. Select the predefined retroactive event
group for the element or create your own to select.

205

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

When an element is subject to retroactive changes, many of the components for the retroactive element are created
automatically. This includes adding the element to the retroactive event group and proration group; however you
must set up the retroactive components. To process an element in a retroactive payroll run, the element must have
a retroactive component that defines the processing rules. Create your own retroactive event group, proration event
group and change the default values for elements in the Element page.

How can I create offset entries instead of deleting retroactive
entries and notifications?

Retroactive payroll is an automated process that generates notifications automatically. If you're sure you have
retroactive entries that aren't wanted, run retroactive payroll, let these retroactive entries generate and offset them with
balancing amounts with the same retroactive elements added.

It is important that you don’t delete the notifications. Run the retroactive process to generate the retroactive entries.
Using the same retroactive elements, create retroactive entries with negative amounts to offset. You can upload the
respective entries via HCM Data Loader. For example, if the retro process has created a retro entry for $100 of retro
overtime, create a new retro overtime entry of -$100 to offset.

It is important to remember not to remove or delete the retroactive notifications. Deleting will just delay the process
and those employees won't be picked up in the next retroactive process. Also, if there are any other retroactive changes
in the period where the delete notification was raised, a new retroactive notification will be created and processed
accordingly. For example, in the scenario above, if you deleted the notification for the $100 of retro overtime without it
being processed and any other changes are made to that period, this unprocessed $100 retro overtime will be picked up
in the recalculation and a retro overtime element entry is created. However, a new notification is not regenerated.

Related Topics

• How Retroactive Pay Is Calculated

• Overview of Retroactive Pay

• Retroactive Notification Report

What happens if I manually enter a value in a standard element
entry value that has a runtime default value?

Any subsequent changes to the default value on the element or element eligibility record won't affect the element entry.
To clear your entry, you can restore the default value.

Related Topics

• Default Values for Standard Element Entries

206

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

How can I use normal elements for a retroactive element to
distribute costing?

The process uses normal elements from the current period when there are no retroactive elements to distribute or the
sum of retroactive group members is zero.

The process configuration parameter Distributed costing for a retroactive element uses normal elements because
the default is Y. If you don't want to distribute on the current period elements, you can set the parameter value to N in
the Default Group.

How do I change the number of decimal places used in element
input values?

Monetary input values use the number of decimal places defined for the currency, such as two for USD. If your
calculations require more decimal places, select a numeric unit of measure for the input value.

The level of decimal precision that you specify must match the precision value set on the Manage Currency page for the
country. This ensures that the payroll processes and reports used for reconciliation and legislative reporting produce the
expected results.

How can I Edit the Date for a Frequency Rule?

The date field on the Frequency Rules page is made read-only when the frequency rule is saved with at least one of the
periods.

To edit the date field, clear all periods and click Submit. Now, you can edit the Date field. Remember to select your
periods again. Note: You will have to clear all periods every time you want to edit the Date field.

Why can't I add a secondary element classification to process a
new deduction or tax?

Primary element classifications are predefined, can vary by country or territory, and are often based on specific rules
and legislative requirements. These rules and requirements can limit the types of secondary classifications that you can
add to primary element classifications.

To manage your element classifications, see the setup documentation for the specific country or territory.

207

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 2
Elements, Earnings and Deductions

How do I capture information on a time card that's required by my
company for payroll calculations?

You need to create a value definition to capture the information in Payroll and associate this to your time element.

If you're using Oracle Time and Labor, you also need to run the Generate Data Dictionary Time Attributes process. This
process creates the attributes that are required to capture the information on the time card and pass this information to
Payroll.

Related Topics

• Calculate Time Based on a User-Defined Value

208

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

3  Calculation Cards and Calculation Values

Payroll Calculation Information

Overview of Payroll Calculation

When you create an element, the application generates the rules and definitions required to calculate earnings or
deduction amount. For all types of elements, these rules and definitions include elements, formulas, and processing
rules.

This topic explains the payroll calculation information rules and definitions generated for user-defined elements with
one of the following categories:

• Absence

• Benefit

•

Involuntary Deductions

• Time card

All predefined tax and social insurance elements also include payroll calculation information rules and definitions.

Note:  Elements that use calculation information definitions don't capture the values required for the calculation on
element input values.

Task Summary
The following table summarizes the purpose of each type of calculation information and the task you can use to view or
edit it.

Calculation Information

Description

Task

Payroll calculation information

Use the Payroll Calculation Information task.

The payroll calculation information task groups
rates and rules used by the payroll run to
calculate values for user-defined earnings, and
deductions.

Predefined elements such as tax and social
insurance rules also use the payroll calculation
feature to provide a group of rates and rules
which vary by country or territory.

Payroll components

A payroll component is a group of rates and
rules that the payroll run uses to calculate
values for earnings and deductions.

Use the Payroll Calculation Information task to
view payroll components and their associated
rules.

When you create elements in certain
classifications and categories, such as
involuntary deductions, the element template

209

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Calculation Information

Description

Task

Wage basis rules

creates a payroll component with the same
name.

You can manage payroll components using
predefined component groups, which vary
by country or territory but may include social
insurance, taxes, retirement plans, involuntary
deductions, and benefits.

Wage basis rules determine the earnings
that contribute to a deductible amount or,
 for exemptions, the elements that reduce the
amount subject to deduction.

For example, wage basis rules might define
which secondary classifications of standard
and supplemental earnings are subject to a
particular tax.

Rules may vary based on reference criteria such
as a worker's place of residence.

Use the Component Group Rules task to define
the rules and references.

Use the Calculation Cards task to enter
reference values for workers.

Calculation value definitions

Calculation value definitions store calculation
rates and rules, which may vary based on other
criteria.

Use the Calculation Value Definitions task to
view predefined definitions and the definitions
that element templates create.

For example you can use calculation value
definitions to calculate regional income tax
rates for employees, which vary based on their
income levels.

The calculation value definition controls which
calculation values are enterable on a calculation
card.

Note:
You can edit definitions that element
templates create, such as adding default
calculation values.

Calculation factors

Calculation factors indicate which calculation
value definition to use when calculating the
amount.

Use the Elements, Element Overview task to
access calculation factors.

Calculation components

For example, a calculation factor might identify
which set of tax rates to use based on the tax
code of the employee.

If tax rates vary based on a factor such as
a person's filing status, then filing status is
defined as a calculation factor reference. Thus,
 an element may have multiple calculation
factors, one for each unique set of rules and
references values.

When an element template creates a payroll
component, it also creates calculation
components that you can enter on personal
calculation cards to enter specific details for the
person.

Use the Payroll Calculation Information task to
create new calculation factors. Normally, you
don't need to create new factors, but if you do,
you must also edit the element's payroll formula
to use the new calculation factors.

Use the Calculation Cards task to enter
calculation components for a person.

210

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Calculation Information

Description

Task

Calculation types

A calculation type describes a way of calculating
a value. For example, calculating a value as a
Flat Amount or by applying a Rate to a value.

Use the Calculation Value Definitions task to
view calculation types.

There's a predefined set of Calculation Types.

Calculation steps

A Calculation Step is a name or label that
denotes part of a payroll calculation.

Use the Payroll Calculation Information task.

For example, a time calculation can consist of
the following parts:

• Calculate hours worked

• Calculate hourly rate

A regional tax calculation can consist of the
following parts:

• Calculate Exemptions

• Calculate Allowances

• Calculate Tax

Each one of these is a calculation step in a fast
formula.

Calculation methods

Predefined calculation methods are a way of
performing a payroll calculation.

Use the Payroll Calculation Information task.

Calculation factors

Use the Elements, Element Overview task.

For example, a tax could be calculated using a
cumulative year-to-date payroll balance or a
periodic payroll value.

Calculation factors create an association
between an element, calculation step, and a
calculation value definition.

Calculation factors indicate which calculation
value definition to use when calculating the
amount.

Calculation factors can support complex
calculations such as tax rates. For example, if
a tax rate varies based on a factor such as a
person's filing status the filing status can be
defined as a calculation factor reference thus,
 an element may have multiple calculation
factors, one for each unique set of rules and
references values.

Related Topics

• Calculation Factors

• Add Involuntary Deductions to a Calculation Card

• Wage Basis Rules

211

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Examples of Payroll Calculation Information at the Legislative
Level

To understand how the rules and definitions for calculating payroll components work together, let's examine two
common examples: income tax deductions and social insurance deductions.

Each example provides sample values for the following rules and definitions:

• Component group

• References for wage basis rules

• References for calculation factors

• Wage basis rules

• Related elements

• Calculation factors for elements

• Associations for tax reporting

Individual Income Tax Deduction
A particular country or territory has a statutory deduction for an individual income tax. The exemption amount for the
tax varies based on the person's residential status. The earnings classifications included in the wage basis for the tax
vary by geographical region. Therefore, references are defined for both the wage basis rules and the calculation factors.

The calculation is a two-step process that calculates the exemption and then calculates the tax amount based on the
reduced deductible amount.

• Component group: Taxes

• Component name: Individual Income Tax Deduction

• References for wage basis rules:

Reference Name

Reference Value

Geographical Region

Mainland

Geographical Region

Territory

• References for calculation factors:

Reference Name

Reference Value

Residential Status

Resident

Residential Status

Nonresident

212

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Reference Name

Reference Value

• Wage basis rules:

Geographical Region

Primary Classification

Secondary Classification

Use in Wage Basis?

Reference Value

Mainland

Standard Earnings

All secondary classifications

selected

Territory

Standard Earnings

All secondary classifications

selected

Mainland

Supplemental Earnings

Commission

Territory

Supplemental Earnings

Commission

Y

Y

Y

N

Mainland

Supplemental Earnings

Personal Use of Company Car

Y

Territory

Supplemental Earnings

Personal Use of Company Car

N

• Related element: Individual Income Tax Processor

The processing rule (a fast formula) associated with this element drives the income tax calculation. It accesses
the appropriate calculation factor, based on the resident status reference value and the current step in the
calculation process.

• Calculation factors for Individual Income Tax Processor element:

Resident Status

Reference Value

Calculation Step

Calculation Method

Calculation Value

Values

Definition

Nonresident

Calculate exemption

None

Tax Exemption Amount

4800

amount

for Nonresident

Resident

Calculate exemption

None

Tax Exemption for

2000

amount

Resident

(None)

Calculate individual

None

Individual Income Tax

0-50000: 3%

income tax

Rate

50000-100000: 4%

213

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Resident Status

Reference Value

Calculation Step

Calculation Method

Calculation Value

Values

Definition

Over 10000: 5%

• Tax reporting units: All tax reporting units defined for this payroll statutory unit can report this calculation

component. You associate calculation components with a specific tax reporting unit on the personal calculation
card.

Social Insurance Deduction
The same country has a statutory deduction for a social insurance tax. Both the employer and the employee contribute
to the social insurance tax, but their contribution rates are different. Calculation of the deduction includes several steps:

1. Calculate the base amount for the employee's contribution.
2. Calculate the base amount for the employer's contribution.
3. Calculate the employee's contribution amount.
4. Calculate the employer's contribution amount.

The following rules and definitions apply to this calculation at the legislative level:

• Component group: Social Insurance

• Component name: Medical Insurance Deduction

• References for wage basis rules: None

• References for calculation factors:

Reference Name

Reference Value

Contribution Level

Employee

Contribution Level

Employer

• Wage basis rules:

Primary Classification

Secondary Classification

Use in Wage Basis?

Standard Earnings

All secondary classifications selected

Supplemental Earnings

All secondary classifications selected

Y

Y

• Related elements: Medical Insurance Calculation element

The processing rule (fast formula) associated with this element drives the social insurance calculation. It
accesses the appropriate calculation factor, based on the contribution level reference value and the current step
in the calculation process.

214

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

• Calculation factors for Medical Insurance Calculation element:

Contribution Level

Calculation Step

Calculation Method

Calculation Value

Values

Reference Value

Definition

Employee

Calculate Employee Base

None

Employee Contribution

8000

Amount

Upper Limit

Employee

Calculate Employer Base

None

Employer Contribution

5000

Amount

Upper Limit

Employer

Calculate Employee

None

Employee Contribution

4%

Contribution Amount

Amount

Employer

Calculate Employer

None

Employer Contribution

3%

Contribution Amount

Amount

• Tax reporting units: All tax reporting units defined for this payroll statutory unit can report this calculation

component. You associate calculation components with a specific tax reporting unit on the personal calculation
card.

Related Topics

• Calculation Factors

• Calculation Value Definitions

• Wage Basis Rules

Payroll Calculation Information Formulas

Overview of Payroll Calculation Information Formulas

When you create an element, the application generates the rules and definitions required to calculate the earnings or
deduction amount. This includes elements, formulas, and processing rules.

Use the predefined calculation formulas to calculate and access calculation information in a payroll run. Here are the
formulas that contain specific rules for each calculation type:

• CALL_CALC_VALUE (Fast Formula)
• CALC_DIR_EXISTS (Fast Formula Function)
• GET_CALC_DETAIL (Fast Formula)
• CALC_DIR_GET_OVERRIDE_LEVEL (Fast Formula)
• CALL_CALC_VALUE_DETAILS (Fast Formula)

215

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

The element associated with these formulas calculates the value definitions. For example, the time element template
creates multiple value definitions to capture time-related information, such as number of units, rate information, and
accrual date. The formula that the time elements template generates includes multiple calls to the CALL_CALC_VALUE
formula, one call for each value definition.

You can also use the predefined CALL_CALC_VALUE formula to calculate rates based on a rate definition or values defined
by criteria in the payroll run. In a scenario where we calculate a bonus, we can do so using a rate definition or a car
allowance value based on criteria of the worker's location.

• CALL_CALC_VALUE (Fast Formula)

You can use this formula to access payroll calculation information. This formula evaluates the calculation
factors required to identify the value definition to be calculated. After the formula identifies the value definition,
the corresponding value is calculated.

• CALC_DIR_EXISTS (Fast Formula Function)

You can use this function to identify if a value definition exists for the current contextual settings. If this
function returns Y, a value definition does exist. If the function returns N, no value definition was found.

• GET_CALC_DETAIL

This Formula returns the details of the prior call to CALL_CALC_VALUE. For example, the value definition was
for these incremental rates:

From

0

1001

10001

To

1000

10000

999999999

Rate

1%

10%

20%

CALL_CALC_VALUE formula would return an amount of 2910 for a base of 20000. Then, GET_CALC_DETAIL would return
these values:

Base

1000

9000

10000

Rate

1%

10%

20%

Amount

10

900

2000

The formula also returns these override types and the details that this call uses.

216

Chapter 3
Calculation Cards and Calculation Values

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Override Type

R

T

A

B

C

AA

AR

RT

RD

F

M

D

1

Meaning

Rate

Total Amount/Value to be returned.

Value A

Value B

Value C

Additional Amount

Additional Rate

Range Table (Override the complete Range Items)

Rate Definition

Flat Amount

Multiplier

Date

String

CALC DIR GET OVERRIDE LEVEL
This formula calls the CALC_DIR_GET_OVERRIDE_LEVEL function which determines the level at which the override value is
used for the qualifying Calculation Unit.

For example, if the function determines the Calculation Factor, the Value Definition is used for the calculation.

The formula takes an input Parameter of override type, and then determines the level where the override type is
overridden. The available override types vary based on the calculation type.

Override Type

R

T

A

Meaning

Rate

Total Amount/Value to be returned.

Value A

217

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Override Type

Meaning

B

C

AA

AR

RT

RD

F

M

D

1

Value B

Value C

Additional Amount

Additional Rate

Range Table (Override the complete Range Items)

Rate Definition

Flat Amount

Multiplier

Date

String

It would determine where the value for the override type is retrieved.

Return

NO_VALUE

NONE

PREL

TRU

PSU

Purpose

The Value Definition (no range items) calculates no value.

There are no overrides, but the Value Definition has range items that may perform the calculation.

There's an override on the Payroll Relationship Card.

There's an override on the TRU Card.

There's an override on the PSU Card.

You can get the Rate Override level by calling the formula with an override type of 'R'.

CALL_CALC_VALUE_DETAIL
This formula is a combination of CALL_CALC_VALUE and GET_CALC_DETAIL and returns the details of both calls.

218

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Related Topics

• Time Element Value Definitions

• Calculate Time Element Rate Using Values Defined by Criteria

• Calculate Standard Earnings Rate Using Values Defined by Criteria

Parameters for Calculation Information Payroll Formulas

Parameters for Calculation Information Payroll Formulas

Input and Output Parameters for the Calculation Information Payroll Formulas

1. CALL_CALC_VALUE (Fast Formula)

◦ Inputs

Name

Base

Data Type

Number

Range_Value

Number

Calculation_factor

Number

Range_offset

Number

Use To

Mandatory. The amount that the

calculation would be based on. For

example, if the calculation is a Flat Rate,

 the Rate is applied to Base for calculating

the return value.

Optional. Defaulted to Base when no

value is specified. Range Value is used

with the From and To values on the

Range Items for identifying the Range

Item to use for the calculation. For

example, an Allowance could be based

on the Number of Children and Employee

has. The Range Value could be the

Number of Children, but the Base could

be Gross Earnings (as the Allowance is a

factor of the Gross Earnings).

Optional. Default Value 1. Some

Calculation Types use a factor (z). For

example, Standard Formula 1, using this

parameter the caller can specify the

factor to use.

Optional. Default 0. This is similar

to the Range Value. In this case, it

defines the amount that has previously

been considered. For example, when

calculating an Incremental Rate for a

219

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Name

Data Type

Use To

Range_low_override

Array of Numbers

Payroll Period, a previous Payroll Run

may have calculated on a base/range of

$2000. So there's a $2000 offset for the

current Payroll Run.

Optional. Default Empty Array. The low

and high overrides work in combination,

 the number of rows in the arrays must

match the number of Range Items in the

Value Definition to be processed. Certain

statutory Value Definitions are allowed

to override the Ranges (From and To

values).

Range_high_override

Array of Numbers

Optional. Default Empty Array. See

Value_name

Array of Strings

Range_low_override.

Optional. Default Empty Array. Some

Calculation Types allow parts of the

Calculation to be overridden. This is

performed by the value_* parameters,

 these arrays must have equal numbers of

entries. Value_name contains the Name

of the attribute (typically a DB Item) to

be overridden. Value_Value contains the

override value and Value_datatype is the

data type of the override.

Value_value

Array of Strings

Optional. Default Empty Array. See

Override_name.

Value_datatype

Array of Strings

Optional. Default Empty Array. See

Override_name.

◦ Outputs

Name

Ded_amount

Data Type

Number

Periodicity

String

Use To

This amount is the returned calculated

value.

Some Calculation Types return the

frequency of the Amount returned. For

220

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Name

Data Type

Use To

example, 'YEAR' meaning Annually,

 hence a calculated amount of $50000

with a periodicity of Year (annually).

Out_uom

String

The Unit of Measure of the calculated

2. CALC_DIR_EXISTS (Formula Function)

◦ Outputs

Name

Exists

3. GET_CALC_DETAILS (Fast Formula)

◦ Outputs

Name

Ded_amount

Data Type

String

Data Type

Number

Periodicity

String

Value.

Use To

Y or N.

Use To

This amount is the returned calculated

value.

Some Calculation Types return the

frequency of the Amount returned. For

example, 'YEAR' meaning Annually,

 hence a calculated amount of $50000

with a periodicity of Year (annually).

Out_uom

String

The Unit of Measure of the calculated

Value.

High_value

Array of Number

Range Item High Value

Base

Rate

Array of Number

Base used for this portion of the

calculation.

Array of Number

Rate Used for this portion of the

calculation.

221

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Name

Data Type

Use To

Flat_amount

Array of Number

Flat Amount used for this portion of the

calculation.

Multiplier

Array of Number

The multiplier used for this portion of the

calculation.

Parameter

Array of String

The parameter used for this portion of

the calculation.

Value_a

Array of Number

Value A used for this portion of the

Calculation.

Value_b

Array of Number

Value B used for this portion of the

Calculation.

Value_c

Array of Number

Value C used for this portion of the

Calculation.

Val_def_name

Array of String

Name of the Value Definition used.

Override_flags

Array of String

Override Types used for this portion of

the calculation.

4. CALC_DIR__GET_OVERRIDE_LEVEL (Fast Formula)

◦ Inputs

Name

Data Type

Use To

Override_type

String

Type of Override to look for.

◦ Outputs

Name

Level

Data Type

String

Use To

The level at which the override was

found.

222

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

•

Calculation Cards

Calculation Entries

The Calculation Entries page consolidates all the payroll entries for an employee within a single page.

You can view element categories such as Standard Entries, Time, and Absence. Click an entry to view the earnings and
deductions processed for an employee for a payroll period and the enabled calculation cards.

To view a calculation card, you must configure them as per your localization. These additional cards are accessible
depending on whether data has been transferred or localizations have enabled them such as Time and Absence related
information.

View the following additional reserved input values in the Standard Entries section of the Calculation Entries page:

• Primary Input

• Percentage

• Hours

• Days

• Units

• Rate

You can create an entry, or update, correct, or delete entries from the Standard Entries page. You can also add and
amend costing information from this page and view the history of an element entry. There are also date range options
available to change the selection of element entries that are viewable.

Use the Creator Type field to identify the origin of an element entry on the collapsed Standard Entries page. For
example, an entry displayed on the page can be a Salary Proposal, Element Entry, Balance Adjustment, and so on. View
the Time and Absence Entries region to identify if an entry has been processed or not processed by a QuickPay or
Payroll process.

Calculation card information such as taxation and involuntary deductions can be accessed with the provided links.
Some Calculation Cards such as Absence and Time, are read-only, while other calculation cards such as taxation
are editable. You can also create a new card from the Calculation Entries page using the Actions drop-down list. For
example, in the UK localization, you can create a new Court Order entry from the Calculation Entries page.

Security Info for the Calculation Entries Page
The following table shows the function privilege that secure access to the Calculation Entries Quick Action:

Page

Privileges

Job Roles

Calculation Entries

Manage Payroll Calculation Entries PAY_
MANAGE_CALCULATION_ENTRIES

• Payroll Manager

• Payroll Administrator

223

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Page

Privileges

Job Roles

• Payroll Interface Coordinator

• Human Resource Manager

• Human Resource Specialist

• Human Resource Analyst

Calculation Entries and the Earnings and
Deductions pages

View Payroll Calculation Cards ORA_PAY_VIEW_
PAYROLL_CALCULATION_CARDS

• Payroll Administrator

Note:  If a calculation card doesn’t support this view-only privilege, you won’t be able to open the Redwood
Calculation Card page and access will not be available.

The view-only access is provided by default to the Payroll Administrator role, and you can also assign it to other
predefined roles.

Within the Calculation Entries UI, you've access to various types of Calculation Entries, such as Standard Entries,
Absences, and Time Cards. Access to those type of entries are secured independently by the following aggregate
privileges:

Entry Type

Aggregate Privileges

Job Roles

Standard Entries

Manage Payroll Element Entry

• Payroll Manager

ORA_PAY_ELEMENT_ENTRY_MANAGEMENT_
DUTY

• Payroll Administrator

• Payroll Interface Coordinator

• Human Resource Manager

• Human Resource Specialist

Standard Entries (View Only)

View Payroll Element Entry

• Human Resource Analyst

ORA_PAY_ELEMENT_ENTRY_VIEW_DUTY

Absences

View Payroll Absence Entries

• Payroll Manager

ORA_PAY_VIEW_PAYROLL_ABSENCE_ENTRIES

• Payroll Administrator

• Payroll Interface Coordinator

Time Cards

View Payroll Time Entries (NEW)

• Payroll Manager

ORA_PAY_VIEW_PAYROLL_TIME_ENTRIES

• Payroll Administrator

• Payroll Interface Coordinator

Other Entries held in Calculation Cards

Manage Payroll Calculation Cards

• Payroll Manager

ORA_PAY_PERSONAL_DEDUCTION_
MANAGEMENT_DUTY

• Payroll Administrator

• Payroll Interface Coordinator

If you’re using predefined roles, ensure you generate your data roles. If you’re using custom roles, add the new privilege
and aggregate privileges depending on what types of Calculation Entries users should have access to.

224

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Note:  To have access to the Calculation Entries Quick Action, you need the new function privilege (Manage Payroll
Calculation Entries) and at least one of the aggregate privileges above-mentioned.

Note:  Access isn't secured independently for Calculation Entries held in Calculation Cards (such as Benefits and
Pension or Involuntary Deductions).

Support for Assignment Level Security
The application supports Assignment-level security for the following calculation entry types:

1. Standard Entries (in both Manage and Read-only mode)
2. Absences
3. Time Cards

When you enable assignment-level security, the Person Search will only return those assignments in the user’s person
security profile.

When navigating to any of those Calculation Entries types, the following entries are displayed:

1. Entries for the selected assignment
2. Entries for the select assignment's payroll relationship
3. Entries for other assignments in the user's person security profile

Change Hire Date Support
You can change the hire date backward when an employee has a Time and Absence card entry with the element
creation date later than the hire date. Changing the hire date has the following impact on the calculation entry:

• When the hire date changes to a backward date, the calculation entries are deleted from the Payroll calculation
card. However, this data will be available after running the Evaluate Absence scheduled process. This data will
always be available in the Absence application.

• When the hire date is moved to a forward date, the Absence and Time Card calculation entries with the creation

date earlier than the new hire date, will be deleted from the Payroll and Absence applications.

For example, an employee is hired on 22 January 2024 and has an absence that has a start date of 22 January 2024, and
an end date of 28 January 2024. When the hire date is changed to 29 January 2024, the time entries before 29 January
2024 are deleted from the Payroll application.

Here’s how this feature works in the Absence application:

• All absences that are before the new hire date or spanning the new hire date will be deleted.

• Absences that are after the new hire date will be marked for reevaluation.

• Absences that are marked for reevaluation (processing status = unprocessed) will have only header. The

absence type entries data, plan entries, and Payroll calculation card entries will be deleted. Later, when the
Evaluate Absence scheduled process picks up these absences, the corresponding entries will be created.

Related Topics

• Add a Payroll and Make Payroll a Mandatory Attribute

225

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

How Entries of Personal Calculation Cards Fit Together

Personal payroll calculation cards capture information specific to a particular payroll relationship. Payroll runs use this
information to calculate earnings and deductions. Actions such as hiring a person or loading data may create some
cards automatically.

Otherwise, you can create the card manually. You can also add components to cards and enter calculation values, which
may override default values. Additionally, you can associate the card with a tax reporting unit.

To view and manage calculation cards, use the Calculation Cards task from the Payroll section.

Card Types
The types of calculation cards you can create and the type of information captured on a card vary by country or
territory. Examples include cards for:

• Statutory deductions

•

Involuntary deductions

• Time card entries

• Absences

• Benefits and pensions

Additional cards may be available to capture information for reporting purposes.

Card Creation
In countries where all employees are subject to the same set of statutory deductions, the application automatically
creates one or more statutory deduction calculation cards. These cards are created when you hire a new employee. In
other countries, you must create calculation cards manually.

For other card types, you create calculation cards as needed for each employee. If you load absence, time card, or
pension data from another application, the application automatically creates the calculation cards.

Calculation Components and Component Groups
The Calculation Card Overview pane shows a hierarchy of calculation components within component groups. For
example, child support, education loan, and alimony are calculation components in the US involuntary deduction
component group.

Each component relates to an element, such as an income tax deduction. Adding a calculation component to the card
creates an entry for the related element.

A calculation component may have one or more references that define its context, such as the employee's place of
residence or tax filing status.

Click a row in the Calculation Components table to see component details. Use the Component Details section to enter
additional values used to calculate the component.

Note:  For some countries, the Calculation Cards page doesn't include the Calculation Components and Component
Details sections. Instead, the layout of the page is specific to the data items required for the country.

226

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Enterable Calculation Values
When you select a calculation component, you may see the Enterable Calculation Values on the Calculation Card tab.
Here you can enter specific rates or other values for the person, which may override default values held on a calculation
value definition. For example, if an employee qualifies for a special reduced tax rate, you enter the rate as an enterable
value on their personal calculation card.

You can't override values loaded from another application, but you may be able to add values, such as adding additional
contributions to a pension deduction.

Tax Reporting Unit Associations
Click the Associations node in the Calculation Card Overview pane to associate a tax reporting unit with the card.
Associations determine:

• Which rates and rules held at tax reporting unit level apply to the calculation of the components

• How the calculations are aggregated for tax reporting

Rules about what you can enter here vary by country:

• Typically, all components on a calculation card are associated with the same tax reporting unit by default.

• You may be able to associate individual components with different tax reporting units.

•

If a person has multiple assignments, you may be able to associate specific assignments with calculation
components.

Related Topics

• Enterable Values on Calculation Cards

Examples of Creating Calculation Cards for Deductions at Different
Levels

You can create and manage calculation cards at several different levels, from an individual person to a payroll statutory
unit.

Use the cards to capture information specific to a person or organization, such as an employee's tax filing status or
an employer's tax identification number. Calculation card entries override default values defined at other levels. The
priority of information, from highest to lowest, is as follows:

1. Personal calculation card (payroll relationship level)
2. Tax reporting unit calculation card
3. Payroll statutory unit calculation card
4. Calculation value definitions (legislative data group level)

Note:  Not all countries or territories support creating calculation cards for payroll statutory units and tax reporting
units. The enterable values at each level also vary by country or territory. The basic steps to create and manage
calculation cards are the same at all levels.

Use these examples to understand when you might define calculation cards at each level.

227

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Personal Calculation Card
Scenario: An employee qualifies for a special reduced tax rate.

Task: Calculation Cards task in the Payroll section under My Client Groups.

Tax Reporting Unit Card
Scenario: The income tax exemption amount is 2000 at the legislative data group level, but a tax reporting unit in a
particular state or province uses an exemption amount of 2500. Enter this default value for the tax reporting unit, which
can be overridden on personal calculation cards.

Task: Manage Legal Reporting Unit Calculation Cards task in the Setup and Maintenance section.

Payroll Statutory Unit Card
Scenario: During application setup, the implementation team defines default contribution rates for the payroll statutory
unit.

Task: Manage Legal Entity Calculation Cards task in the Setup and Maintenance section.

Calculation Value Definition
Scenario: You can view the predefined income tax rates for your country, but you can't edit them.

Task: Calculation Value Definitions task in the Payroll section.

If an employer qualifies for a special tax rate, enter these values on a calculation card at the appropriate level.

Calculation Value Definitions

Overview of Calculation Value Definitions

A calculation value definition specifies how a value is provided or calculated.

The value isn't necessarily monetary. Typically, it's a flat amount or rate, but it could be a date or a text value, such as a
tax code, depending on the calculation type. Some definitions hold the values in a table, so that different values apply to
different employees.

For example, a graduated tax varies depending on the employee's earnings balance. The calculation value definition for
this tax might contain two rows where you define the tax rate for:

• Earnings under $50,000

• Earnings above $50,000

Calculation Value Definitions Provided
Each localization provides a set of predefined calculation value definitions used to calculate statutory and involuntary
deductions. You can't edit the predefined calculation value definitions.

228

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

In addition, when you create the following element types, the element template creates calculation value definitions
based on your selections:

• Pensions

•

Involuntary deductions

• Absences

• Time cards

Create or Edit Calculation Value Definitions
The element template creates calculation value definitions when you create elements with a certain category such as
benefits, absences, and time card elements.

You can also create or edit calculation value definitions using the Calculation Value Definitions task in the Payroll
section. For example, you can create value definitions to capture additional attributes that are required for your
company's absence or time calculations.

You can also create value definitions to calculate a rate derived from a rate definition or values defined by criteria.

Value Definition Groups
When you create a calculation value definition, either select an existing group or create a new one. The group
categorizes related calculation value definitions. The predefined set of standard groups is available to all countries or
territories.

Examples of predefined value definition groups include Time and Absences. You must select these when creating value
definitions for elements with the corresponding element category.

Calculation Factors
Some elements, such as statutory deductions, require a large number of calculation value definitions. They use
calculation factors to determine when and how to apply each calculation value definition, based on a reference value.

For example, a calculation factor may direct the payroll process to:

• Use a calculation value definition only if the person lives in Region B.

• Annualize the calculated result to produce the final amount

Use the Payroll Calculation Information task to view and manage calculation factors.

Related Topics

• Calculation Factors

• Calculation Value Definitions Examples

Calculation Types in Calculation Value Definitions

The calculation type determines which values you must provide in the Calculation Values section of the Create or Edit
Calculation Value Definition page.

229

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

For example, if you select Flat Amount as the calculation type, then you must provide a flat amount value. You specify a
default calculation type for the definition, which you can override on individual rows in the Calculation Values section.

Predefined Calculation Types
Predefined calculation types are available for each type of calculation. These work in conjunction with the predefined
payroll formulas that contain specific rules for each calculation type, such as the CALL_CALC_VALUE formula.

This table describes the predefined calculation types, and indicates whether a calculation type is available for selection
when you create a new value definition.

Calculation Type

Description

Flat Amount

Uses the specified flat amount as
the total amount.

Flat Amount Times Multiplier

Multiplies a flat amount by a
multiplier value. If you select
this option, you must specify a
database item that provides the
value of the multiplier.

UOM

Money

Money

Rate Definition

Retrieves a value by calling a rate
definition.

Money

Number

Flat Rate

Uses the number entered on the
value definition as the calculated
value.

Number

Applies the specified percentage
rate to the balance.

Number

For example, to apply a rate of 10
percent, enter 10.

Incremental Rate

Applies a different percentage rate
to portions of the balance.

Number

For example, assuming that the
balance is 80,000, you could apply
a 1 percent rate for the first 20,000
of the balance. A 3 percent rate for
the next 30,000, and a 5 percent
rate to the next 30,000. This is also
referred to as a blended rate.

Applies the percentage rate to
a value. This value type derives
the value from another value
definition.

Number

A new calculation type is required
to support identifiers. For example,
 the value definition could capture
a job ID and the value set feature

Number

Flat Rate by Derived Base

Identifier

Available in Create Flow

Yes

Yes

Yes

Yes

Yes

Yes

Yes

Yes

230

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Calculation Type

Description

UOM

Available in Create Flow

Text

Date

Conditional Flat Amount

Flat Calculation Total

Incremental Calculation (Graded)

would enable the user to display
the name of the job on the page.

Uses the specified character string
as the calculated value.

Text

Yes

Uses the date entered as the
calculated value.

Text (YY-MM-DATE, HOURS MINS
SECS)

Yes

Uses the specified flat amount
if the condition defined in the
Calculation section is met.

For example, if a person's filing
status is married or head of
household, that person qualifies
for an exemption. In such a
scenario, you specify a flat amount
value in the value definition and
the condition database item
returns the person's filing status.

This calculation type supports
predefined calculations, such as
tax and social insurance.

Supports retrieving value
definitions for different range
value criteria, including predefined
calculations, such as tax and social
insurance.

Supports retrieving value
definitions for different range
value criteria, including predefined
calculations, such as tax and social
insurance.

Money

No

Money or Number

No

Money or Number

No

Standard Formula 1

Calculates the total amount based
on the following formula:

Money or Number

No

y = Ax - Bz

Where:

• y is the deducted amount.
• x is the calculated amount.
• A and B are specified values.
• z is a factor from a predefined
formula. The value defaults to
1.

Standard Formula 2

Calculates the value based on the
following formula:

Money or Number

No

231

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Calculation Type

Description

UOM

Available in Create Flow

y = (x - A) x B + Cz

Where:

• y is the deducted amount.
• x is the calculated amount.
• A, B, and C are specified

values.

• z is a factor from a predefined
formula. The value defaults to
1.

Specify View Objects
A view object is a query result set. You can specify a view object to define the valid values that are available to the
selected calculation type.

Note:

• The view objects you can specify vary depending on the calculation type. For example, if the calculation type is

Conditional Flat Amount, then specify view objects for the condition and flat amount values.

• When you specify a view object, include the fully qualified path name, such as:

oracle.apps.hcm.locUS.payrollSetup.details.publicView.UsStatePVO

Related Topics

• How Entries of Personal Calculation Cards Fit Together

• Calculation Value Definitions Examples

• Calculation Value Definitions

Enterable Values on Calculation Cards

Some values entered on a calculation card override values defined in a calculation value definition.

For example, you might set a default tax rate for the legislative data group, and allow the rate to be overridden by a flat
amount entered on a personal calculation card.

The following table explains where you can enter override values on calculation cards. It also provides the order in which
the Calculate Payroll process checks for values entered on calculation cards. When the process finds an entered value, it
stops checking and uses the values defined at that level.

Order

1

Type of Values

Task

Values for a payroll relationship on any type of
calculation card

Calculation Cards

232

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Order

2

3

Type of Values

Task

Values for a tax reporting unit for certain
deductions, which vary by country or territory

Legal Reporting Unit Calculation Cards

Values for a payroll statutory unit for certain
deductions, which vary by country or territory

Legal Entity Calculation Cards

Allowing Enterable Values on Calculation Cards
The ability to enter values on calculation cards is controlled by the Enterable Calculation Values on Calculation Cards
section of the calculation value definition. Here you can set calculation values, such as specific rates or other values for
the person, which could override default values held on a calculation value definition.

For example, if an employee qualifies for a special reduced tax rate, you enter the rate as an enterable value on their tax
card.

• For user defined calculation value definitions, you can specify an enterable calculation value in this section. You

provide:

◦ The display name to appear on the calculation card.
◦ The value type, such as total amount or additional amount.

• Enterable values for statutory and involuntary deductions are predefined. You can't allow new enterable values

for predefined calculation value definitions.

• You can't override values loaded from another application, but you can add values, such as adding additional

contributions to a pension deduction.

Enterable Value Types
The list of value types available for entry depends on the calculation type. For example, you can enter the percentage
value for a flat rate calculation or the monetary value for a flat amount calculation.

The following value types are available for all calculation types except text:

Value Type

Description

Calculation value definition

Uses the calculation value definition entered on a calculation card to calculate the amount.

Total amount

Uses the amount entered on the calculation card as the total amount.

Additional amount

Adds the amount entered on the calculation card to the calculated amount.

233

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Managing Data Display on Calculation Cards
Some calculation cards support large volumes of data. Use these options to improve usability and reduce the large
amount of data displaed on high-volume calculation cards.

• Use the Entered Values switch on the page to only display information entered by you. This is the default

behavior.

• Use the All Attributes option to display all component attributes, including those with default values and blank

values.

• Use the Create and Edit options to view all components and add new components or edit existing components.

• Expand collapsed regions to view details of regions that are collapsed by default to limit the displayed

information when the card first loads.

Related Topics

• Calculation Value Definitions Examples

• Creating Calculation Cards for Deductions at Different Levels for the US

Considerations to Enter Calculation Values for Pensions

Create a Benefits and Pensions calculation card for each worker who pays a pension deduction. On the card, select the
calculation component that was created automatically for your pension element, and enter the required contribution
amounts and limits.

If you use the Load Benefit Batches process to transfer values, this process creates the calculation cards and enters the
contribution amounts and limits.

Default Contribution Amounts and Limits
Enter default contribution amounts and limits when you create the pension element. These default values are stored as
calculation value definitions. You can edit the default values using the Calculation Value Definitions page. You can also
add a default payee or a separate payee for each employee by entering the payee ID in the Enterable Calculation Values
area.

Enterable Calculation Values for Pensions
To enter or override a calculation value for one worker, perform these steps:

1. Open the worker's Benefits and Pension calculation card on the Calculation Cards page.
2. Add the calculation component for the pension, if it isn't already on the card.
3. With this calculation component selected, click the Enterable Calculation Values on Calculation Cards tab.
4. Click Create.
5. Select the value you want to enter. Typically, you will enter a payee, reference number, and any additional

contributions. You can also override any default contribution amounts or limits.

The following table lists the calculation values you can enter.

Note:  If the calculation component was created by running the Load Benefit Batches process, you can only enter or
override the following values: Payee, Reference Number, and Employee Additional Contribution.

234

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Field

Payee

Required

Y

Reference Number

Y or N

Employee Contributions

Y

Additional Employee Contributions

N

Minimum Age

Maximum Age

Maximum Contribution Amount

Minimum Pensionable Earnings

Maximum Pensionable Earnings

Partial Deduction Allowed

N

N

N

N

N

Y

Default Provided at Element
Setup

Values

N

N

Y

N

Y

Y

Y

Y

Y

Y

Enter the ID of an organization with
the usage of Pension Provider.

Free text

Depending on the localization
rules this field may or may not be
required.

Percent or flat amount as per
element setup. Enter percentages
as decimal values.

Percentage or flat amount as
per element setup, if additional
contributions are allowed.

Numeric age

Numeric age

Numeric amount

Numeric amount

Numeric amount

Values = Y or N

If the element was set up to allow an employer contribution, you will also see these enterable values:

Calculation Value

Required

Default Provided at Element
Setup

Values

Employer Contribution

Minimum Age Limit for Employer
Contribution

Maximum Age Limit for Employer
Contribution

Maximum Contribution Amount for
Employer Contribution

Y

N

N

N

Y

Y

Y

Y

Percentage or flat amount as per
element setup

Numeric entry

Numeric entry

Numeric amount

235

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Calculation Value

Required

Default Provided at Element
Setup

Values

Minimum Pensionable Earnings
Limit for Employer Contribution

Maximum Pensionable Earnings
Limit for Employer Contribution

N

N

Y

Y

Numeric amount

Numeric amount

Calculation Value Definitions Examples

In these deduction examples, the calculation value depends on where the employee falls in an earnings range.

The From and To values of the range can be static or dynamic. Dynamic values are a fraction of the value of a database
item, such as gross earnings. These examples also illustrate how to override the default calculation type for selected
values in the range.

Static Values
The calculation value definition for a regional income tax uses a default calculation type of Flat Rate. However, for the
lowest and highest incomes, a flat amount applies. For these two values, the Flat Amount calculation type overrides the
default type, and uses a monetary value rather than a percentage. The Basis of Calculation Values field is blank, so the
values are static.

The following table shows sample static values for this calculation value definition.

From Value

To Value

Calculation Type Override

Rate or Amount

0

200

1000

2000

199

999

1999

Flat Amount

0

_

_

4 (percent)

6 (percent)

999,999,999

Flat Amount

300

Dynamic Values
The calculation value definition for a tax exemption uses a default calculation type of Incremental Rate. The first and
last values specify the Flat Amount calculation type, which overrides the default type. The Basis of Calculation Values
field specifies the Gross Earnings YTD database item. This means the From and To values represent a percentage of
year-to-date gross earnings.

The following table shows sample dynamic values for this calculation value definition.

236

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

From Value

To Value

Calculation Type Override

Rate or Amount

0

.1

.2

.9

.1

.2

.9

1

Flat Amount

300

_

_

10 (percent)

30 (percent)

Flat Amount

0

The first row defines a flat amount of 300 that applies to the first 10 percent of gross earnings. The second row defines
a 10 percent rate that applies to the next 10 percent of gross earnings. The third row defines a 30 percent rate that
applies to between 20 and 90 percent of gross earnings. The final row defines a flat amount of 0 between 90 and 100
percent.

Calculation Factors

Overview of Calculation Factors

Calculation factors define data-driven rules for calculating complex payroll elements, such as statutory deductions.
Some elements may have a large number of calculation factors, one for each unique set of rules, ranges, and references
values.

Calculation factors create an association between an element, a calculation step, and a calculation value definition.

The payroll run determines which calculation factor to use based on the reference values and calculation rules of the
element being processed.

For example, a calculation factor for a tax deduction element might define:

• A context reference, such as a city or state

• The calculation value definition, such as a 4 percent tax rate on balances under 50,000

• Optionally a calculation method and calculation step

Navigate to the Element task and select an element to view and manage calculation factors.

Note:  Calculation factors are predefined for statutory and involuntary deductions, and should not be changed.

To view and manage calculation factors, follow these steps:

1. Select the Payroll Calculation Information task from Quick Actions list of the Payroll section.
2. Select the calculation component.
3.
4. Expand the Calculation Factors node to display a list of all calculation factors associated with the element.
5. Create new calculation factors and edit existing ones that have an update status of Unlocked.

In the Calculation Overview section, expand the Related Elements node.

237

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Note:  You can't edit predefined calculation factors or their reference values. If you create a new calculation factor, you
must edit the element's formula to use the new factor.

Aspects of a calculation factor are shown in the following figure:

Reference Values
A calculation factor may be associated with up to six references that define its context. For example, the calculation of a
social insurance deduction might vary based on a person's age and employment status.

Each reference has a reference number that determines the order in which it's evaluated for processing relative to other
references.

Navigate to the Calculation Information task and search for a payroll component to view and manage calculation factor
reference information.

Calculation Value Definition
Calculation factors create an association between an element, calculation step and a calculation value definition. The
calculation value definition defines the calculation type, such as flat amount or flat rate. The calculation rates and rules
may vary based on the amount subject to calculation. Predefined calculation value definitions are provided for statutory
and involuntary deductions.

Navigate to the Payroll Calculation Value Definition task to view and manage value definitions.

Calculation Step
A calculation step is a name or a label assigned to a calculation factor to identify its role in a complex payroll calculation.

For example, a time calculation can consist of several parts, such as:

• Calculate hourly worked

• Calculate hourly rate

And when calculating an income tax deduction, the payroll run can do the following:

• Calculate allowance

• Calculate exemptions

• Calculate tax

238

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

This tax deduction might be defined as a single element with multiple calculation steps, each defined in a separate
calculation factor. You can assign the same calculation step to more than one calculation factor. Calculation steps are
optional.

Navigate to the Payroll Calculation Information task to view and manage calculation steps.

Range Values
Range values capture values required for the calculation. The type of information captured is controlled by the
calculation type of the value definition such as flat amount, rate (percentage) or date.

Navigate to the Payroll Calculation Value Definition task to view and manage range values.

Calculation Methods
A calculation method references a single fast formula. It's an optional component of a calculation factor. Calculation
methods operate at a higher level than the calculation types defined in the calculation value definition. They provide
a wrapper around the calculation of a deduction by retrieving values from a calculation value definition, applying a
formula, and returning the final deduction amount for the current run.

For example, if the calculation method is set to Cumulative, which references the Core Cumulative fast formula, then the
calculation process returns the total deduction amount as a cumulative year-to-date amount. Accrual calculations for
payroll balance calculations typically restart at the beginning of each calendar year. This is another type of calculation
method. In this case the plan rule for the accrual term start date is January 1.

Navigate to the Payroll Calculation Information task to view and manage calculation methods.

Related Topics

• Payroll Calculation Information

• Examples of Payroll Calculation Information at the Legislative Level

• Calculation Value Definitions

Examples of Calculation Factors for Payroll Deductions

To illustrate how the payroll run uses calculation factors to calculate different types of deductions, let's look at a social
insurance deduction and a national income tax deduction using calculation steps.

Social Insurance Deduction
Employers in many countries or territories deduct social insurance payments from employees and also make
contributions. Employee and employer rates are typically different. Such deductions often have wage limits.

The social insurance deduction processor element for this type of calculation might have the following calculation
factors:

Employer or Employee
Code (Reference Value)

Calculation Method

Calculation Step

Calculation Value
Definition

Values

Employee

None

Calculate Social Insurance
Employee Rate

Social Insurance Employee
Rate

4 percent flat rate

239

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 3
Calculation Cards and Calculation Values

Employer or Employee
Code (Reference Value)

Calculation Method

Calculation Step

Calculation Value
Definition

Values

Employer

None

Calculate Social Insurance
Employer Rate

Social Insurance Employer
Rate

2 percent flat rate

Employee

None

Calculate Social Insurance
Employee Wage Limit

Social Insurance Employee
Wage Limit

100,000 flat amount

Employer

None

Calculate Social Insurance
Employer Wage Limit

Social Insurance Employer
Wage Limit

100,000 flat amount

National Income Tax Deduction Using Calculation Steps
A national income tax calculation involves multiple steps. First, it calculates the allowance, then any exemption amount,
and then it applies the tax rate.

The following table shows a subset of calculation factors that might be associated with a tax processor element.

Filing Status (Reference
Value)

Calculation Method

Calculation Steps

Calculation Value
Definition

Values

Single

Single

Single

Married

Married

None

None

None

None

None

Calculate Region A
Allowance - Single

Region A Allowance -
Single

10,000 flat amount

Calculate Region A
Exemption Amount - Single

Region A Exemption -
Single

0 flat amount

Calculate Region A Regular
Rate - Single

Region A Rate - Single

7 percent flat rate

Calculate Region A
Allowance - Married

Region A Allowance -
Married

10,000 flat amount

Calculate Region A
Exemption Amount -
Married

Region A Exemption -
Married

1,000 flat amount

Married

None

Calculate Region A Regular
Rate - Married

Region A Rate - Married

6 percent flat rate

Related Topics

• Calculation Value Definitions

240

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

4  Rates and Values by Criteria

Rate Definitions

Overview of Rate Definitions

Use rate definitions to create rates such as salary rates, absence rates, time card rates, and other types of payroll rates.

Further, you can use a rate definition for different types of rate calculations. For example, use a salary rate definition to
display an employee's salary on the salary page. You can also use it to display the employee's salary rate on the time
card and to pay the employee's salary in Cloud Payroll.

Here are some rate types that you can create:

• Compensation rates, such as a base salary or car allowance rate.

• Rates based on a set of criteria and conditions. For example, a union rate that's based on the job and location of

an employee.

• Rates with multiple rate contributors, such as an overall salary rate, which is the sum of multiple salary

components.

• Rates derived on the grade of an employee, such as a base salary rate and payroll balance rates, such as

pension reporting rate.

• Rates calculated based on other rates. For example, a shift allowance rate that's calculated based on a

percentage of the employee's salary rate.

You can define minimum and maximum validation rules for your rate definition. For example, define a minimum rate
rule to ensure that an employee isn't paid less than the minimum hourly rate for their job.

When you create a rate definition, you can define a frequency for the rate returned by the calculation, such as 50,000
annually, or 7.25 hourly. Alternatively, you can define a rate that's calculated for a unit of work, such as a shift rate, or a
mileage rate. You can control if the application calculates the rate values live or retrieves it based on the results of the
Generate HCM Rates process. For example, it's a common practice for salary rates to be calculated live when you enter
the salary page for an employee.

As a cloud payroll user, you can calculate most rate calculations live in the payroll run. However, you'll need to perform
some complex rate calculations using the Generate HCM Rates process. In this scenario, Cloud Payroll retrieves the
stored rate value directly from the rates reporting table for an employee. You can use the rates generated by the
Generate HCM rates process for generating reports, such as pension reports.

Use the Rate Definitions task to define and manage rate definitions.

Categories
To create a new rate, select a category from this table.

241

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Category

Derived Rate

Element

What it Does

Retrieves values from one or more payroll balances or other rate definitions, including rates that
retrieve element entry values. Use this option to create a rate that retrieves a value from one or more
rate contributors.

Retrieves rate information from an element input value. When using salary rates, use this type of rate
definition to create and update entries, such as create or update a salary element entry.

Select a storage type of Amount or Factor and then select the name of a corresponding element.

You can select one of these storage types:

• Amount: Retrieves a value from or posts to the element input value with a special purpose of

Primary Input Value. For example, 'Amount' is the primary input value for elements created with
the flat amount calculation rule, such as salary. If you associate a flat amount salary element with
a rate, the application retrieves or posts to the salary amount for an employee.

• Factor: Retrieves a value from or posts to the element input value with a special purpose of

Factor. The 'Factor' is the primary input value for elements created with the Factor calculation
rule.

Use this rate definition to apply the factor held on an element entry to a payroll balance. You can also
use it to apply it to another rate definition including base rates or an overall salary rate.

For example, the application calculates your company's car allowance rate based on a factor of salary.
The application captures the factor value, such as 0.05 at the employee level on their car allowance
element entry. When creating the car allowance rate definition, select your car allowance element to
enable the rate to retrieve the factor value for an employee.

In the rate contributor region, select your salary rate definition. This selection ensures that the
application calculates the car allowance rate based on a factor value of the employee's salary rate.

Note:
The element rate doesn't support the input value information that's held on Hours x Rate elements.
It's a common practice for the payment rate for this type of element to be based on a recurring flat
amount element, such as salary.

Note:
Salary rates supports Factor, but the payroll run doesn't. Use the Generate HCM Rates process to
calculate this type of rate. Also, you can use the process to retrieve the stored value in the payroll run
using the predefined CALL_CALC_VALUE formula.

Value by Criteria

Retrieves values from a single value by criteria definition. A value by criteria definition specifies one or
more evaluation conditions that determine a particular value or rate. You can specify the conditions as
a tree structure to define the evaluation sequence.

For example, you can define a value-by-criteria to capture car allowance and housing allowance values
based on an employee's job. Define a rate definition to retrieve car allowance rates and another rate
definition to retrieve housing allowance rates. Both rate definitions refer to the same value-by-criteria
and use the criteria of job to retrieve the appropriate rate values for an employee.

Grade Rate

Formula

Retrieves values based on an employee's grade details.

Retrieves values from a rate definition formula. The Generate HCM Rates process supports the
calculation of most formula-based rates. However, rates that include complex payroll formula contexts
or use balances calculated within the payroll run, are calculated by the payroll run.

242

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Category

What it Does

Note:
Formula-based rates are only supported for rate calculations in the payroll run.

Related Topics

• Options to Configure Rate Definitions

• Rate Contributors for Derived Rates

• Configure Elements Used by Rate Definitions

• Overview of Values Defined by Criteria

• Calculate Values Defined by Criteria

Options to Configure Rate Definitions

To configure rate definitions to get your desired rates, you should know how to use the various rate definition options.
For rates based on a single element entry value, you can also apply override and defaulting rules.

Note:  Use the HCM Generate Rates process to calculate factor based element rates.

This table describes the fields that you can configure for the Derived Rate, Element, and Value by Criteria category
types.

Field

Storage Type

Category

Element

Element Name

Element

Derived Rate

Description

If you select the Element category to define a
rate, you must select a storage type of Amount
or Percentage. For example, you can configure
a rate definition using the Salary element. If
the salary is held as a monetary value, select
Amount. If the salary is a factor of another
value, such as a balance, select Percentage.

Note:
This field is hidden for all rate definition
categories other than Element.

For the Element category, the field is enabled
only when you select the storage type.

If you select the Element category to define a
rate, you must select an element name. This is
required if you're configuring a primary rate.
This is a rate that retrieves a value from a single
element, such as salary.

243

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Field

Category

Description

Employment Level

Derived Rate

Value by Criteria

Status

Element

Derived Rate

Value by Criteria

Base Rate

Element

Overall Salary

Reporting Required

Element

Derived Rate

Element

Derived Rate

Value by Criteria

For the Derived Rate category, the field is
enabled when you access the page.

Select either Payroll Relationship, Term,
 or Assignment. This field is mandatory for
all derived rates and value by criteria rate
definitions. It controls which employment ID the
rates process uses when calling a rate.

If the employee has multiple assignments,
 the rates process uses the assignment ID to
identify the correct assignment record for the
employee.

Sometimes the contributor value is held at a
different level to the employment level defined
on the rate. In such cases, the rate process uses
the employment ID to locate the correct record.

Set the status of a rate to active or inactive. You
can't assign an inactive rate to an employee.
Employees that are allocated a rate while it was
active aren't impacted by a change in status to
inactive.

Select this option if the rate represents a base
rate that another rate uses in its calculation. For
example, you might have day shift employees
and night shift employees, with different base
pay rates.

If each set of employees receives an allowance
that's a percentage of the base rate, define one
allowance rate. And that rate is calculated based
on the two rates that have the Base Rate option
selected.

If you're defining rates for use on the Salary
page, use the derived rate category and define
an Overall Salary. To do this, you must associate
a salary element to the rate. Define an Overall
Salary Information element for this purpose.

Select this option to indicate if the calculated
rate value should be stored on the rate table for
reporting purposes.

If you're defining rates for use on the Salary
page, you must select this option.

Rate definitions with this option selected are
included when the Generate HCM Rates batch
process is run. Use this feature to report on
primary rates and not derived rates. HCM
extracts use this report to send data to third
parties.

244

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Field

Category

Description

Value by Criteria Name

Value by Criteria

If you select the Value by Criteria category
to define a rate, you must select a Value by
Criteria name. A value by criteria definition
specifies one or more evaluation conditions
that determine a particular value or rate.

Returned Rate Details
You can specify the periodicity of the returned rate, factor rules, currency, decimal display, rounding rules, and minimum
and maximum rules. If the process returns a rate that's outside the minimum and maximum range, you can do one of
these actions.

• Set up an action that enforces the rule, displays a warning

• Forces the user to fix the error

Select the Return FTE Rate check box to instruct the rate definition process to return a part-time value by applying an
employee's FTE to the rate value.

Periodicities
You must specify a periodicity, such as hourly or weekly, for the returned rate and each rate contributor. However, when
you use the rate in a formula, you can override the default periodicity.

The rate calculation converts each contributor to the periodicity specified on the rate contributor. It then adds or
subtracts the rate contributors, even if the periodicities are different. In most cases, they will be the same. Once the rate
contributors are summed up, the rate calculation then converts them into the return periodicity and currency.

For example, for a rate with a periodicity of weekly using the Standard Rate Annualized conversion formula, the rate
calculation does these actions.

1. Calculates an annual figure from the value and periodicity of each contributing earning and deduction.
2. Converts the annual figure into a weekly value.

By default, rates are converted using these predefined rate conversion formulas.

• Standard Rate Annualized

• Standard Rate Daily

• Standard Working Hours Rate Annualized

• Assignment Working Hours Rate Annualized

• Periodic Work Schedule Rate Annualized

If the values in the predefined conversion rules don't meet your requirements, you can define your own.

Factor Rules
You can apply a factor or multiplier to a calculated rate, or to an individual rate contributor. To apply a factor rule, do
these steps.

• Select Value as the factor rule.

•

In the Factor field, enter the number by which you want to multiply the rate.

245

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

• Add the contributor.

Chapter 4
Rates and Values by Criteria

You can apply a factor rule to the rate definition, rate contributors, or both. For example, you can define rate
contributors to calculate hourly values based on salary and bonus. You can then apply a factor of 1.0 or 100 percent
to the salary balance contributor and a factor of 0.5 or 50 percent to the bonus balance contributor. The factor rule is
applied to the rate before the periodicity conversion is applied.

Minimum and Maximum Values
You can define minimum and maximum values for the returned rate, and for individual rate contributors.

Use the Limit Violation Action field to display an error, warning, or enforce the application to use minimum or
maximum value that you enter. For example, you can enter 500 as the minimum value and then select Enforce Rules. If
the returned value comes back as 400, the application uses 500 as the value.

This table explains the options for the minimum and maximum rate values.

Value

Null

Comments

No minimum or maximum value

A specified value

Example: 2000

Based on another rate

Uses the calculated value of the rate definition that you select.

Be careful that you don't create a loop. For example, Rate A has minimum value that's based on Rate B,
 which has a minimum value based on Rate A. This situation would result in a runtime error.

Value by Criteria

Minimum or maximum value based on a value by criteria definition.

Override and Defaulting Rules
You can set override and default rules only if you select Element as the category when you define rate definitions. Set
up override rules for the element associated with your rate definition. If you select the Override Allowed check box, you
can enter rate values on the Salary page.

If an element input validation formula has been defined for the rate contributor input value, you can view it in the
Override and Defaulting Rules section.

Note:  You can't define override and defaulting rules if you select the Values by Criteria category to define a rate. But
you can select a formula to validate any rate that's returned and also use formulas to create default values.

For example, you can use the HCM Rates Default Value formula type to define the number of workdays in a year for your
organization.

workday = 250
periodicity = YEAR
return workday, periodicity, currency

In addition, you can use a value by criteria definition as the default type. Here, the process uses the value for the first
record created and carries that value forward in subsequent records, unless it's manually overridden. The rate engine
reevaluates the rate that the value by criteria method creates for each subsequent record. So, this rate could change. For

246

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

example you could use a value by criteria definition to enable a default value of 10 percent for bonuses that are targeted
to all eligible employees.

Contributor Rules
You can specify the periodicity for the contributor total. To process contributor totals as full-time equivalency amounts,
select Yes in the Process Contributor Total as FTE Amount field. The final rate value is converted from this status to
the Return Rate FTE status.

Information
In this section, enter text that explains the purpose of the rate, how the rate is calculated, or provides further details for
the rate. This section isn't available for rate definitions using the Value by Criteria categories.

Related Topics

• Rate Contributors for Derived Rates

• Configure Elements Used by Rate Definitions

• Configure Periodicity Conversion Rules

• Element Input Validation Formula Type

Configure Elements Used by Rate Definitions

If you create rate definitions that reference element input values, you must configure them for the different calculation
rules, such as Flat Amount and Factor.

This ensures that the values calculated by the rate are consistent with the values processed through payroll.

Elements use the predefined CALL_CALC_VALUES formula to calculate rate values in Calculate Payroll and Generate
HCM Rates. Each element also requires the necessary payroll calculation information is defined such as values
definitions, calculation steps and calculation factors.

When you create elements with a category such as Time Card or Absence, you can associate a default rate definition
and the application generates all the rules and definitions required to calculate the rate.

When you create elements with a category of Standard, you need to update the element formula to use
CALL_CALC_VALUE and create the payroll calculation information required to associate the rate definition to the
element and calculate the rate.

Do these element configuration steps if you're using this element for a rate definition with the category element.

1. Create an element of type Recurring or Assignment level.
2. Don't select the Multiple Entries Allowed  check box.
3. Select a special purpose for each element input value.

a. Primary Input Value for an Amount value.
b. Factor for a Factor value.
c. Periodicity for a Periodicity value.

Note:  When creating elements for use in rate definitions, don't select Periodically. The Rate Definition
process is unable to convert rates with a periodicity of periodically to different frequencies such as annual,
weekly, and daily.

247

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

4.

If the flat amount is a full-time equivalent value, you must select Yes in the Default field for the Full-Time
Equivalent input value.
5. Create element eligibility.

Configure Elements to Create Rate Definitions for Flat Amount Calculations

1. On the Home page, click the Elements quick action under the My Client Groups tab.
2. Click Create.
3. Enter these values.

Field

Value

Legislative Data Group

Select your legislative data group

Primary Classification

Standard Earnings

Category

Standard

4. Click Continue.
5. Enter a name, reporting name, and description.
6. Enter the effective date.
7. Answer the questions in the Duration and Standard Rules sections.

Note:  Multiple entries aren't allowed.

8. For the question, At which employment level should this element be attached?, select Assignment Level.
9. For the question, Does this element recur each payroll period, or does it require explicit entry? select Recurring.
10. Click Next.
11.
12. Click Submit.
13. On the Element Summary page under the Input Values folder, select Full-Time Equivalent.
14. Check that these values exist.

In the Calculation Rules section, select Flat Amount and then click Next.

Field

Name

Value or Check Box Status

Full-Time Equivalent

Special Purpose

Full-Time Equivalent

Unit of Measure

Character

Displayed

Selected

Allow User Entry

Selected

248

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Field

Required

Value or Check Box Status

Deselected

Create a Database Item

Selected

Default

No

Lookup Type

PAY_TMPLT_YES_NO

Configure Elements to Create Rate Definitions for Factor Calculations

In the Calculation Rules section, select Factor and then click Next.

1. Repeat steps 1 through 9 in the first procedure.
2.
3. Click Submit.
4. On the Element Summary page under the Input Values folder, select Pay Value.
5. Check that these values exist.

Field

Name

Value or Check Box Status

Pay Value

Special Purpose

Primary output value

Unit of Measure

Money

Displayed

Selected

Allow User Entry

Selected

Required

Deselected

Create a Database Item

Selected

6. On the Element Summary page under the Input Values folder, select Factor.

249

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

7. Check that the following fields and values exist.

Field

Name

Special Purpose

Value or Check Box Status

Factor

Factor

Unit of Measure

Number

Displayed

Selected

Allow User Entry

Selected

Required

Deselected

Create a Database Item

Selected

Test Your Element Configuration
You're almost done. Now, to test your element configuration, follow these steps.

Note:  These procedures are for payroll users only.

Step

Page

Do This Action

1

2

3

4

5

My Client Groups

Elements

Element Entries

Find a payroll and an employee that you can
use for testing purposes.

For the Flat Amount element, use the Pay Value
balance feed to enter an Eligible Compensation
balance for the Percentage element.

Add the Flat Amount and Percentage elements
to the employee as element entries and enter
input values.

Submit a Process or Report

Enter a suitable period for the payroll you
selected in step 1.

Submit a Process or Report

Run the payroll.

250

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Step

6

Page

Do This Action

View Payroll Process Results

Check if the payroll results are correct.

Related Topics

• Overview of Rate Definitions

• Options to Configure Rate Definitions

• Rate Contributors for Derived Rates

• Calculate Standard Earnings Rate Using Values Defined by Criteria

• Payroll Calculation Information

• Overview of Payroll Calculation Information Formulas

Example to Calculate a Standard Earnings Rate

Let's look at an example that shows how to calculate a standard earnings rate. This example doesn't cover the payroll
calculation. But it does support the configuration to calculate a rate for a standard element.

1. Create a Rate Definition: Use the Rates Definitions task to create a bonus rate definition.

2. Create the Element: Use the Elements task to create a flat amount bonus element.

a.
b.

In the Primary Classification field, select Standard Earnings.
In the Category field, select Standard.

3. Create a Value Definition:Use the Calculation Value Definitions task to create a bonus value definition. This is

required to associate the rate definition with the bonus element.

a. Click Create for a new value definition group and provide a name such as standard earnings.
b.
c.

In the Calculation Type field, select Rate Definition.
In the Calculation Values region:

i. Enter values from 0 to 99999.9
ii. Select the bonus rate definition.

4. Create Calculation Step: Use the Payroll Calculation Information task to create a bonus calculation step.

a. Search for time cards in the component group field and navigate to the Calculation overview page.
b. Navigate to all calculation steps tasks.
c. Create a calculation step and provide a unique name such as a bonus.

5. Create Calculation Factor on Element: Use the Elements task to create a calculation factor.

a. Search and select the bonus element.
b. Select the calculation factor page.
c.
d.

In the calculation step field, select the bonus calculation step.
In the value definition, select the bonus value definition field.

251

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

6. Edit Formula on Bonus Element: Use the Elements task to edit the element formula.

a. Edit the bonus element formula to calculate a bonus rate using the CALL_CALC_VALUES formula.

Note:  You can refer to the element status processing rules page to identify which formula to edit.

Related Topics

• Payroll Calculation Information

• Overview of Payroll Calculation Information Formulas

• Calculate Standard Earnings Rate Using Values Defined by Criteria

Rates Defined by Formula

You can define rates based on Fast Formula.

Let's consider an example where an employee can work in a job at a higher grade than their normal job. The rate paid to
that employee is based on different criteria and includes rules, such as the minimum rate must be at least 1.00. You can
use a formula to step up the grade to the next level and to return the rate assigned to that higher grade.

On the Rate Definition page, Calculation Formula field, select the HCM Rates Calculate Value formula type. The
formula type supports contexts, such as assignment, payroll relationship, and job. You can select and create the correct
formula for rate definitions from all standard database items.

Write a Formula
You can write your own formula when the formula type is HCM Rates Calculate Value.

The formula has certain inputs and return value, but the rate always returns these values:

• Monetary Amount

• Currency

• Periodicity

Note:  Formula-based rates are only supported for rate calculations in the payroll run.

Examples
In this formula, the return values set to 65.23, but you can add the required logic to calculate the rate return values.

Default for value_name is EMPTY_TEXT_NUMBER
default for value_value is EMPTY_TEXT_NUMBER
default for value_datatype is EMPTY_TEXT_NUMBER

inputs are

 value_name (text_number),
 value_value (text_number),
 value_datatype (text_number),

AMOUNT = 65.23
CURRENCY = 'USD'
PERIODICITY = 'YEAR'

252

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

 return AMOUNT, CURRENCY, PERIODICITY

Chapter 4
Rates and Values by Criteria

Let's consider another example where the formula returns a rate based on a job. You can use this formula to calculate a
rate value when an employee works in a job at a higher grade than at their normal job.

default for value_name is EMPTY_TEXT_NUMBER
default for value_value is EMPTY_TEXT_NUMBER
default for value_datatype is EMPTY_TEXT_NUMBER

default for PER_ASG_ELIG_JOBS_CURRENCY is 'UNKNOW'
default for PER_ASG_ELIG_JOBS_END_DATE is '0001/01/01 00:00:00' (date)
default for PER_ASG_ELIG_JOBS_FREQUECY is 'YEARLY'
default for PER_ASG_ELIG_JOBS_FROM_DATE is '0001/01/01 00:00:00' (date)
default for PER_ASG_ELIG_JOBS_JOB_CODE is 'UNKNOW'
default for PER_ASG_ELIG_JOBS_JOB_ID is 0
default for PER_ASG_ELIG_JOBS_JOB_NAME is 'UNKNOWN'
default for PER_ASG_ELIG_JOBS_MANUAL_RATE is 0
default for PER_ASG_JOB_ID is 0

inputs are
 value_name (text_number),
 value_value (text_number),
 value_datatype (text_number)

 AMOUNT = 0
 PERIODICITY = 'YEARLY'
 CURRENCY = 'USD'

 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - count is : ' || to_char(value_name.count))
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - count2 is : ' || to_char(value_value.count))
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - count3 is : ' || to_char(value_datatype.count))

 l_job_id = PER_ASG_JOB_ID
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - l_job_id is : ' || to_char(l_job_id))

 i = 0
 while (i < value_name.count) loop
 (
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - name is : ' || value_name[i])
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - value is : ' || value_value[i])
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - datatype is : ' || value_datatype[i])

 if(value_name[i] = 'PER_ASG_JOB_ID') then
 (
 l_job_id = to_num(value_value[i])
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - l_job_id has been set with : ' || to_char(l_job_id))
 )

 i = i + 1
 )

 CHANGE_CONTEXTS(JOB_ID = l_job_id)
 (
 l_t_dummy = PER_ASG_ELIG_JOBS_CURRENCY
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - l_t_dummy is : ' || l_t_dummy)
 if(l_t_dummy != 'UNKNOW') then
 (
 CURRENCY = l_t_dummy
 )

 l_dt_dummy = PER_ASG_ELIG_JOBS_END_DATE
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - l_dt_dummy is : ' || to_char(l_dt_dummy))

 l_t_dummy = PER_ASG_ELIG_JOBS_FREQUECY
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - l_t_dummy is : ' || l_t_dummy)
 if(l_t_dummy != 'UNKNOW') then

253

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

 (
 PERIODICITY = l_t_dummy
 )

Chapter 4
Rates and Values by Criteria

 l_dt_dummy = PER_ASG_ELIG_JOBS_FROM_DATE
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - l_dt_dummy is : ' || to_char(l_dt_dummy))

 l_t_dummy = PER_ASG_ELIG_JOBS_JOB_CODE
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - l_t_dummy is : ' || l_t_dummy)

 l_n_dummy = PER_ASG_ELIG_JOBS_JOB_ID
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - l_n_dummy is : '||to_char(l_n_dummy))

 l_t_dummy = PER_ASG_ELIG_JOBS_JOB_NAME
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - l_t_dummy is : ' || l_t_dummy)

 l_n_dummy = PER_ASG_ELIG_JOBS_MANUAL_RATE
 l_log = PAY_INTERNAL_LOG_WRITE('[RATE_FML] - l_n_dummy is : '||to_char(l_n_dummy))
 if(l_n_dummy > 0) then
 (
 AMOUNT = l_n_dummy
 )
 )

return AMOUNT, PERIODICITY, CURRENCY

Related Topics

• Overview of Rate Definitions

Rates Based on Values Defined by Criteria

Use a value defined by criteria definition to specify one or more evaluation conditions that determine a particular value
or rate.

You can specify the conditions as a tree structure to define the evaluation sequence. You can calculate rates based on
a specific value defined by criteria value. For example, you define a value defined by criteria to capture car allowance,
housing allowance and market supplement values based on an employee's job.

In this example, you define these criteria details for Jobs A and B.

This table describes the various criteria details for Job A

Criteria

Car Allowance

Housing Allowance

Market Supplement

Value

1000

2500

300

This table describes the various criteria details for Job B.

254

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Criteria

Car Allowance

Housing Allowance

Market Supplement

Value

2000

3500

375

Now, you can define these three rates that are associated with the same value defined by criteria.

1. Rate 1 to retrieve car allowance values for employees based on their job.
2. Rate 2 to retrieve housing allowance values for employees based on their job.
3. Rate 3 to retrieve market supplement values for employees based on their job.

Value by Criteria Defined by Units
Typically, Value Defined by Criteria values are based on a period of time, such as 10 per hour or 25000 per year. But you
can also define values which are calculated based on a unit.

Let's consider these examples where you need unit-based rates.

• A worker is paid 3.50 for each screw that he manufactures.

• A worker is paid mileage allowance where the rate paid varies based on the number of miles traveled and the

type of vehicle.

In this example, when you create values defined by criteria, in the Period or Unit field, select Unit.

Related Topics

• Overview of Rate Definitions

• Options to Configure Rate Definitions

• Configure Elements Used by Rate Definitions

• Rates Defined by Formula

Rate Contributors for Derived Rates

You can add four different types of rate contributors to your rate definitions. These rate contributes include, Balance,
Base Rate, Overall Salary, and Rate Definitions.

You can add rate contributors when you define a rate using the Derived Rate category. You can also manually add rate
contributors for the Element category when the storage type is Factor.

For example, if you define a bonus rate which is 0.1 (10 percent) of average earnings, then you do these steps.

• Enter 0.1 as the factor on the element.

• Define a rate contributor based on your average earnings balance.

Rate Contributor Types
This table lists the types of rate contributors, descriptions, and the additional fields that display for each type.

255

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Type

Balance

What it Contains

Additional Fields

Value calculated by these payroll processes.

Balance Name

• An employee's average salary rate over

their last three months of salary payments

• Taxable earnings for the last tax year

• Commissions paid in the last quarter

Balance Dimension

Divisional Balance

Base Rate

Value from the employee's Base Rate

Employment Level

Overall Salary

Value from the employee's Overall Salary rate

Employment Level

Note:
Each overall salary element must be
associated with only one overall salary rate.
In addition, if the rate definition is an overall
salary rate, you can't select Overall Salary as
the Contributor Type.

Rate Definition

Other rate definitions that contribute to the rate
definition you're creating.

Rate Name

For example you can add regular salary, car
allowance, and bonus pay rate contributors
together to create an overall salary definition.

Reference Dates
You can select a reference date, which is the date the application uses to retrieve rate contributor information for the
rate calculation. The reference date specifies the context for the balance dimension.

For example, to retrieve a rate as of the actual start of an absence, select Absence Start Date. To retrieve a rate as of a
specific time period, select a specific time period.

The Reference Date field lists only these types of time definitions:

• Time Span - a period of time, such as three months

• Retrieval Date - a type of time definition that's based on a database item

Selecting a value for the Reference Date field is optional.

Note:  If you don't select a reference date, the application uses the effective as-of date that's used by the rate engine
to calculate the rate.

Single or Multiple Rate Contributors
If the rate definition is based on multiple values, you may need to create multiple rate contributors, as explained in this
table.

256

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Rate

Number of Rate Contributors

A single earning or deduction, such as
salary

One

A combination of earnings, such as the
sum of salary and car allowance payments

Multiple, if salary and car allowance are stored as separate rate definitions

Note:  All balances and element entries that contribute to a rate must use the same currency.

Example: Using multiple rate contributors, an hourly holiday pay rate could be based on adding together these values,
which are all paid at the end of the previous year.

• Salary

•

Incentive bonus

• Seniority bonus

• Other changeable components of remuneration

Related Topics

• Configure Elements Used by Rate Definitions

• Create Rate Definitions for Leave

• Create a Rate Definition for Basic Salary

• Create Rate Definitions for Overall Salary

Rates Based on Grades Details

You can calculate rates based on employee's grade details. For example, you can calculate the annual salary rate based
on the grade ladder, grade, and grade step information defined for an employee.

When you define a rate definition, you can select a grade rate as a basis for the rate calculation and specify the
employment level. The default employment level is Payroll Assignment. The application retrieves the grade ladder
details based on assigned grade that's held on an employee's assignment record.

In your rate definition, you add either a rate contributor of type Grade Ladder or Retained Grade.

Calculate Rates Based on Grades
Follow these steps to calculate rates based on grades.

1. Set up grades, grade ladder, and rates for the given job to record the level of compensation for the employees.
2. Create a rate definition based on grade details. Add a rate contributor of type Grade Ladder.
3. Hire the employee and provide the required grade and step details.
4. Run the Generate HCM Rates process to calculate the rates based on the information held in the grade tables.

This flowchart describes the overall steps to calculate rates based on grade details.

257

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Related Topics

• Example to Calculate Rates Based on Grades With Steps

• Example to Calculate Rates Based on Grades Without Steps

• Example to Calculate Rates Based on Grade Ladder With Multiple Assignments

Example to Calculate Rates Based on Grades With Steps

Scenario: You hire Sherry Callaway as a Pharmacy Technician with grade 3 and step 2. You calculate grade rate values
for her annual salary payments based on grades, grade ladder, and step details.

Configuration:

1. Set up grades, grade ladder, and rates for the Pharmacy Technician  job to record the level of compensation for

the technicians.

2. Create a rate definition based on grade details. Add a rate contributor of type Grade Ladder.
3. Hire Sherry in the grade 3 with Step 2.
4. Run the Generate HCM Rates Process to calculate the rates based on the information held in the grade tables.

Step 1: Grades, Grade Rates, and Grade Ladders
To set up the grade structure for the Pharmacy Technician job, perform these tasks:

1. Set up five different grades and add five steps for each grade.
◦ Use the Manage Grades task to set up the grades, 1 to 5.

258

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

◦ On the Grade Steps page, add the five grade steps, Step 1 through Step 5, to each of the grades as shown

in this illustration.

2. Use the Progression Grade Ladders task to create a grade ladder Pharmacy Technicians Salary with these

details:

Option

Grade Set

Name

Value

Common Set

Pharmacy Technicians Salary

259

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Option

Value

Legislative Data Group

US Legislative Data Group

Frequency

Annually

Assignment Action

Automated Grade Step Progression

◦ On the Grades and Steps page, add the grades with steps in the sequence in which your employees

typically progress in your organization. Enter the sequence for the place of the grade on the grade ladder,
with 1 being the lowest grade. The employee can move up till the grade 5.

Grade

1

2

3

4

5

Step 1

17803

Step 2

18398

Step 3

18990

Step 4

Step 5

19579

20171

20017

20493

21155

21717

21961

21840

22568

23296

24024

24752

24518

25335

26152

26969

27786

27431

28345

29259

30173

31087

Step 2: Rate Definition
Use the Rate Definition task to create a rate definition of category type Grade Rate. Include these details in the Return
Rate tab.

Option

Periodicity

Value

Annually

Periodicity Formula

Standard Rate Annualized

Currency

US Dollar

Add a rate contributor of type Grade Ladder.

260

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Step 3: Grade Details During Employee Hire
When you're hiring a new employee, add these grade ladder and grade details on the Employment Information page.

Option

Value

Grade Ladder

Pharmacy Technician Salary

Grade

Step

3

Step 2

Step 4: HCM Rates Process
On the Home page, click My Clients Groups and click the Payroll tile. Click the Submit a Flow task. After selecting a
legislative data group, search for and submit the Generate HCM Rates flow.

Result: As shown in this illustration, the application returns a rate value of 22568.

261

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Related Topics

• Rates Based on Grades Details

• Example to Calculate Rates Based on Grades Without Steps

• Example to Calculate Rates Based on Grade Ladder With Multiple Assignments

Example to Calculate Rates Based on Grades Without Steps

You can calculate rate based on grades without steps. In this example, you calculate grade rate values for annual salary
payments.

262

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Scenario
You hire Mathew as a grade 5 Developer and calculate grade rate values for his annual salary payments based on grades
without steps.

Configuration
Follow these steps to calculate grade rate values for Mathew:

1. Set up grades, grade ladder, and rates for the Developer job to record the level of compensation for developers

in your organization.

Perform these steps:

◦ Use the Manage Grades task to set up eight separate grades, 1 to 8.
◦ For each grade, enter the annual salary as shown in this table.

Grade

Annual Salary Amount

1

2

3

4

5

6

7

8

103900

111800

119900

127800

135900

143700

151800

155500

◦ Use the Progression Grade Ladders  task to set up a grade ladder, Developer Salary, with Grades type.

Add all eight grades to the ladder.

2. Create a rate definition of category Grade Rate based on grade details.

Option

Periodicity

Value

Annually

263

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Option

Value

Periodicity Formula

Standard Rate Annualized

Currency

US Dollar

Add a rate contributor of type Grade Ladder.

3. When hiring Mathew, on the Employment Information page, add the grade ladder and grade details as shown

in this table.

Option

Value

Grade Ladder

Developer Salary

Grade

5

4. Run the Generate HCM Rates  process to calculate the rates based on the information held in the grade tables.
Click the Submit a Flow task. After selecting a legislative data group, search for and submit the Generate HCM
Rates process.

Results
The application returns a rate value of 135900.

Example to Calculate Rate Based on Grades Without Steps and Periodicity Conversion
In this example, you want to calculate rate values for Mathew's monthly salary based on grades without steps. To do this
calculation, when creating a rate definition, you change the Standard Rate Annualized formula to a Monthly amount.

Use the steps outlined in the previous scenario to set up grades, grade ladder, and rates for the Developer job.

Create the rate definition based on grade details.

Option

Periodicity

Value

Calendar Month

Periodicity Formula

Standard Rate Annualized

Currency

US Dollar

Complete steps 3 and 4 in the previous scenario.

The application returns a rate value of 11325 (135900 / 12).

264

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Note:  For a rate with a periodicity of monthly using the Standard Rate Annualized conversion formula, the rate
calculation does these actions.

• Calculates an annual figure from the value and periodicity of each contributing earning and deduction.

• Converts the annual figure into a monthly value.

Related Topics

• Rates Based on Grades Details

• Example to Calculate Rates Based on Grades With Steps

• Example to Calculate Rates Based on Grade Ladder With Multiple Assignments

Example to Calculate Rates Based on Grade Ladder With Multiple
Assignments

In this example, you calculate grade rate values for monthly salary payments for an employee with multiple
assignments.

Scenario
Priya Krishnan has these two assignments in the Teacher Salary grade ladder:

•

In her primary assignment, she's a Mathematics teacher in grade 3.

• She holds a temporary assignment as the replacement teacher for the Science teacher who's on maternity

leave. On this temporary assignment, she teaches Science in grade 1 in the same grade ladder.

Follow these steps to calculate grade rate values for Priya Krishnan's primary assignment.

1. Set up grades, grade ladder, and rates for the Teacher job to record the level of compensation for all teachers in

your school.
Perform these tasks:

◦ Use the Manage Grades task to set up five separate grades, 1 to 5.
◦ For each grade, enter the rates as shown in this table.

Grade

Annual Salary Amount

1

2

3

4

16600

19840

20016

23231

265

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Grade

5

Annual Salary Amount

27650

◦ Use the Progression Grade Ladders task to set up a grade ladder, Teachers Salary, with Grades type. Add

all five grades to the ladder.

2. Create a rate definition of category Grade Rate.

Option

Periodicity

Value

Monthly

Periodicity Formula

Standard Rate Annualized

Currency

US Dollar

Add a rate contributor of type Grade Ladder.

3. When hiring an employee, on the Employment Information page, add the grade ladder and grade details as

shown in these tables.

Primary Assignment

Option

Value

Grade Ladder

Teacher Salary

Grade

3

Temporary Assignment

Option

Value

Grade Ladder

Teacher Salary

Grade

1

4. Run the Generate HCM Rates process to calculate rates for employee's Primary Assignment. On the Home

page, click the Submit a Flow quick action under the My Client Groups tab. After selecting a legislative data
group, search for and submit the Generate HCM Rates process.

266

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Result
The application returns a monthly rate value of 1668 (20016/12).

Related Topics

• Rates Based on Grades Details

• Example to Calculate Rates Based on Grades With Steps

• Example to Calculate Rates Based on Grades Without Steps

Rates Based on Retained Grades

You can calculate rates based on an employee's retained grade rate details.

In certain organizations, an employee is entitled to retain their previous grade even after moving to a position of lower
responsibility. The grade is retained for a fixed time beginning on the date the employee is placed in the lower-graded
position, until grade retention is terminated.

For example, an organization restructure moves an employee from grade 13 to grade 12. They are placed on the retained
grade of 13 for a period of time, such as two years. During such time, the employee should be paid at a higher of their
assignment grade and retained grade.

If the assignment grade exceeds the retained grade, then the retained grade should be ended even if it's within the
retained grade period.

It's possible that a company has multiple organization structures and therefore multiple retained grades. In such a
scenario, the employee should be paid on the retained grade with the most recent date.

Related Topics

• Example to Calculate Rates Based on a Retained Grade Rate

• Example to Calculate Rates Based on Multiple Retained Grade Rates

• Create Grade Retention Page and Associate With Retained Grade Context

Example to Calculate Rates Based on a Retained Grade Rate

In this example, you calculate grade rate values for annual salary payments based on a retained grade rate without
steps.

Scenario
Julianna is a Product Manager at grade 5 in the Product Manager grade ladder. As part of a company reorganization,
she's moved from grade 5 to grade 4. The company put her on a retained grade of 5 for a period of 2 years. During this
retained period, she will be paid the higher of her assignment grade.

In this example, you calculate grade rate values for her annual salary payments based on retained grades.

267

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Configuration
Follow these steps to calculate rate values for Julianna:

1. Set up grades, grade ladder, and rates for the Product Manager job to record the level of compensation for

product managers.

◦ Use the Manage Grade task to set up separate grades 1 to 8.
◦ For each grade, enter the annual salary as shown in this table.

Grade

Annual Salary

1

2

3

4

5

6

7

8

103900

111800

119900

127800

135900

143700

151800

155500

2. Create a rate definition based on grade rate details. Add a rate contributor of type Retained Grade Ladder.

Option

Periodicity

Value

Annually

Periodicity Formula

Standard Rate Annualized

Currency

US Dollar

3. Associate a context with the Grade Retention Info page. You must associate a context for the assignment
extensible flexfield to record the retained grade information. You can either associate this context with an

268

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

existing page or you could create a new page based on your requirements. For more information on how to set
up contexts, refer to the topic: Create Grade Retention Page and Associate With Retained Grade Context.
4. On the Additional Info page, set the Primary Indicator. Use the Additional Assignment Info task to set up the

retained grade details.

◦ On the Additional Assignment Info page, search for and select the employee.
◦ In the Info Group field, select Grade Retained Info.
◦ In the Retained Grade section, click Add.
◦ In the Primary Indicator field, select Yes.

Note: If you select the value as No, the application doesn't return any rate.

◦ In the Grade Ladder field, select your grade ladder.
◦ In the Grade field, select Grade 5.

5. Run the Generate HCM Rates process to calculate the rates based on the information held in the grade tables.

Results
The application returns a rate value of 135900.

Related Topics

• Example to Calculate Rates Based on Multiple Retained Grade Rates

• Create Grade Retention Page and Associate With Retained Grade Context

Example to Calculate Rates Based on Multiple Retained Grade
Rates

In this example, you calculate grade rate values for annual salary payments based on multiple retained grade rates
without steps.

Scenario
Prasad is a Technical Writer at grade 3 in the Technical Writer grade ladder. As part of a company reorganization, he's
moved from grade 3 to grade 2. The company put him on a retained grade of 3 from 01-JAN to 31-MAR.

During this retained period, he will be paid the higher of his assignment grade. In this example, you calculate grade rate
values for his annual salary payments based on retained grades.

269

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Configuration
Follow these steps to calculate rate values for Prasad:

1. Set up grades, grade ladder, and rates for the Technical Writer job to record the level of compensation for

technical writers.

◦ Use the Manage Grade task to set up separate grades 1 to 5.
◦ For each grade, enter the annual salary as shown in this table:

Grade

Annual Salary

1

2

3

4

5

101300

287800

310700

392100

401200

2. Create a rate definition based on grade rate details. Add a rate contributor of type Retained Grade Ladder.

Option

Periodicity

Value

Annually

Periodicity Formula

Standard Rate Annualized

Currency

US Dollar

3. Associate a context with the Grade Retention Info page. You must associate a context for the assignment

extensible flexfield to record the retained grade information. You can associate this context with an existing
page or you could create a new page based on your requirements.

For more information on how to set up contexts, refer to the topic: Create Grade Retention Page and Associate
With Retained Grade Context.

4. Use the Additional Assignment Info task to set up the retained grade details, such as Primary Indicator.

◦ On the Additional Assignment Info page, search for and select the employee.
◦ In the Info Group field, select Grade Retained Info.
◦ In the Retained Grade section, click Add.

270

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

◦ In the Start Date field, select 1-Jan.
◦ In the End Date field, select 31-Mar.
◦ In the Primary Indicator field, select Yes.
◦ In the Grade Ladder field, select your grade ladder.
◦ In the Grade field, select 3.
◦ In the Retained Grade section, click Add.
◦ In the Start Date field, select 1-Apr.
◦ In the End Date field, select the end date.
◦ In the Primary Indicator field, select Yes.
◦ In the Grade Ladder field, select your grade ladder.
◦ In the Grade field, select 2.

5. Run the Generate HCM Rates process to calculate the rates based on the information held in the grade tables.

Results
On 15-April, the compensation user updates the employee's salary rate from the retained grade rate to the grade rate.
As shown in the table and illustration, the application returns these rate values.

Period

1-Jan to 31-Mar

15-April 2020

Rate

310700

287800

As shown in the illustration, depending upon the effective start and end dates, the application returns the
corresponding rate value.

271

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Related Topics

• Example to Calculate Rates Based on a Retained Grade Rate

• How do I compare rate definitions to ensure the highest rate is paid?

• Create Grade Retention Page and Associate With Retained Grade Context

Create a Rate Definition for Basic Salary

In this example, you create a primary rate for a basic salary. After you run the rate engine, the Element Entries - Person
Details page displays the values for eligible employees.

Before you begin, create the salary element at the assignment level. This element contains the salary information to be
retrieved by the rate definition. You can create it using the flat amount or factor calculation rule.

1. On the Home page, click the Rate Definitions quick action under the My Clients Groups tab.
2. Click Create.
3. Enter these values.

Field

Category

Value

Element

Effective Start Date

Enter the current date.

272

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Field

Value

Legislative Data Group

Enter your legislative data group.

Storage Type

Amount

Element Name

Regular Salary

4. Click OK.
5.

In the Returned Rate Details section, complete the fields, as shown in this table.

Field

Periodicity

Value

Annually

Periodicity Conversion Formula

Standard Rate Annualized

Currency

LDG Currency

6. Click Submit.

Related Topics

• Overview of Rate Definitions

• Options to Configure Rate Definitions

• Configure Elements Used by Rate Definitions

• Generate HCM Rates

Create Rate Definitions for Overall Salary

In this example, you create a rate definition for overall salary that includes multiple rate contributors.

You do these actions.

• Create the overall salary rate definition

• Add the regular salary rate contributor

• Add the car allowance rate contributor

This table summarizes the key decisions for your scenario.

273

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Decisions to Consider

In This Example

What components of pay should be
included in an employee's overall salary?

• Regular Salary

• Car Allowance

Should I include all pay for car allowance in
the overall salary?

No. Only include 50 percent of the amount paid for car allowance.

Note:  The overall salary rate definition is a derived rate. To populate the Overall Salary check box, select a salary
element in the Element name field. You then add the regular salary rate and car allowance rate contributors to the
rate definition. The rate contributors that you add should be elements that you select from the Rate Name field on the
Create Rate Contributor page.

Create the Overall Salary Rate Definition

1. On the Home page, click the Rate Definitions quick action under the My Clients Groups tab.
2. Click Create.
3. Enter these values.

Field

Category

Value

Derived Rate

Effective Start Date

Enter the current date.

Legislative Data Group

Select your legislative data group.

4. Click OK.
5. Enter these values.

Field

Name

Value

Overall Salary

Short Name

OVERALL_SAL

Element Name

Salary

274

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

6.

In the Returned Rate Details section, enter these values.

Field

Periodicity

Value

Weekly

Periodicity Conversion Formula

Standard Rate Annualized

Currency

LDG Currency

Add the Regular Salary Rate Contributor

In the Calculation section, click Create.
In the Create Rate Contributor dialog box, Contributor Type field, select Base Rate.

1.
2.
3. Enter these values.

Field

Add or Subtract

Value

Add

Employment Level

Payroll Assignment

Periodicity

Weekly

4. Click Save and Continue.

Add the Car Allowance Rate Contributor

In the Calculation section, click Create.
In the Create Rate Contributor dialog box, Contributor Type field, select Rate Definition and click OK.

1.
2.
3. Enter these values.

Field

Add or Subtract

Value

Add

Rate Name

Car Allowance

Periodicity

Factor Rule

Weekly

Value

275

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Field

Factor Value

Value

0.5

4. Click Save and Continue.
5. Click Submit.

Related Topics

• Overview of Rate Definitions

• Options to Configure Rate Definitions

• Rate Contributors for Derived Rates

• Generate HCM Rates

Create Rate Definitions for Leave

In this example, let's calculate an employee's absence rate as of a particular date.

The rate includes a combination of average salary and car allowance. The employee has an annual year-to-date salary
of 26,000. The employee also receives an annual car allowance payment of 2,000. The absence rate is 26,000 + 2,000 =
28,000. To provide a daily absence rate, you convert this rate into a daily rate.

This table summarizes the key information you use in the example.

What You Need To Consider

For This Example

What elements do I need to create before I
define the rate?

• Salary (assignment level) - This element contains the salary value to be retrieved by the rate

definition. You must create it using the Flat Amount calculation rule.

• Car Allowance (assignment level) - This element contains the car allowance value to be retrieved

by the rate definition. You must create it using the Flat Amount calculation rule.

• Absence - Use the Absence template to create the element. Enter Sickness as the classification

and Absence as the category.

Which balances hold the contributing
values?

• Salary is fed by the Salary element.

• Car Allowance is fed by the Car Allowance element.

Should I process contributor totals as full-
time equivalent amounts?

Yes

Create the Rate Definition

1. On the Home page, click the Rate Definitions quick action under the My Client Groups tab.
2.

In the Search Results section, click Create.

276

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

3. Enter these values.

Field

Category

What You Select

Derived Rate

Chapter 4
Rates and Values by Criteria

Effective Start Date

A date that's after the creation date of the objects that you're referencing

Legislative Data Group

Your legislative data group

4. Click OK.
5.

In the Basic Details section, enter these values.

Field

Name

Value

Absence Rate - Salary and Car Allowance

Short Name

ABS RATE - SAL/CAR ALLOW

In the Returned Rate Details section, Periodicity field, select Daily.

6.
7. Click the Contributor Rules tab and in the Process Contributor Total as FTE Amount select, Yes.

The balances referenced need to be populated using payroll runs for the periods covered by the balance
dimension or the rate definition won't generate a meaningful value.

Create Rate Contributors

In the Rate Contributors section, click Create.
1.
In the Contributor Type field, select Balance and click OK.
2.
3. On the Create Rate Contributors page, enter these values.

Field

What You Enter

Add or Subtract

Add

Balance Name

Regular Salary

Balance Dimension

Assignment State Period to Date

Periodicity

Daily

4. Click Save and Continue.
5.

In the Rate Contributor section, click Create.

277

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

In the Contributor Type field, select Balance and click OK.

6.
7. On the Create Rate Contributor page, enter these values.

Field

What You Enter

Add or Subtract

Add

Balance Name

Car Allowance

Balance Dimension

Assignment State Period to Date

Periodicity

Daily

8. Click Save and Continue.
9. Click Submit.
10. Assign an Absence element entry to the employee's assignment. You will then need to pass the absence entry

to payroll using the absence interface.

Related Topics

• Options to Configure Rate Definitions

• Rate Contributors for Derived Rates

• Generate HCM Rates

•

Integrate Absence Management with Global Payroll

Generate HCM Rates

Submit the Generate HCM Rates process to calculate and store most types of rate definitions.

You can use the stored rate values for reporting payroll calculations. Run this batch process frequently to ensure the
stored rate values are accurate. After you run this process, you can report on the rates using extracts. The user entity
includes the database items that you can use in reports.

Use this flow to calculate and store most types of rate definitions in these scenarios.

• Rates that are associated with an element. For example, a salary rate definition is associated with a salary

element. The process calculates a salary rate value for all workers with a salary element entry.

• Rates values for factor based element rates. Use the Generate HCM Rates process to calculate and store rate

values for factor based element rates. You can retrieve this value in the payroll run.

• Rates that are associated with a value definition. Certain types of elements, such as time elements, use payroll
calculation information rules and definitions. For example, a value definition is generated for an overtime
element and this is associated with an overtime rate definition. The process calculates an overtime rate value
for all workers with an overtime element entry.

• Rates that are based on a value-by-criteria defined for an assignment level criteria, such as a worker's grade or

location.

278

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

• Rates that are based on a formula. However, such rates are calculated in a payroll run.

• Rates that are derived. For example, a rate that's derived based on the sum of car and housing allowance rates.
In this case, the Generate HCM Rates process calculates the car allowance rate, the housing allowance rate, and
the derived rate.

The stored rate values can be used for reporting or retrieving for payroll calculation purposes.

The application provides database items to support the rate batch process. These array database items return all rates
associated with a payroll relationship record as of a specific date.

Note:  The REPORTING_RATE_VALUES and REPORTING_RATE_PERIODICITIES database items return values
based on the return rate details defined on the rate definition. The other periodicity database items, such as
REPORTING_RATE_QUARTERLY, return a rate that's converted to the specified periodicity.

The Generate HCM Rates process supports the database items listed in this table.

Database Items

Description

REPORTING_RATE_NAMES

Name of the rate

REPORTING_RATE_VALUES

Value of the rate

REPORTING_RATE_PERIODICITIES

Periodicity of the rate

REPORTING_RATE_FTE_FLAGS

Full-time status of the rate

REPORTING_RATE_TERM_NUMBERS

Term number associated to the rate values

REPORTING_RATE_ASG_NUMBERS

Assignment number associated to the rate values

REPORTING_RATE_WEEKLY

Weekly rate value

REPORTING_RATE_MONTHLY

Monthly rate value

REPORTING_RATE_QUARTERLY

Quarterly rate value.

REPORTING_RATE_YEARLY

Annual rate value

REPORTING_RATE_PT_WEEKLY

Part-time weekly rate value

REPORTING_RATE_PT_MONTHLY

Part-time monthly rate value

REPORTING_RATE_PT_QUARTERLY

Part-time quarterly rate value

REPORTING_RATE_PT_YEARLY

Part-time annual rate value

279

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Database Items

Description

REPORTING_RATE_FT_WEEKLY

Full-time weekly rate value

REPORTING_RATE_FT_MONTHLY

Full-time monthly rate value

REPORTING_RATE_FT_QUARTERLY

Full-time quarterly rate value

REPORTING_RATE_FT_YEARLY

Full-time annual rate value

PER_ASG_ESTABLISHMENT_ID

Establishment

PER_ASG_UNION_ID

Worker Union ID

PER_ASG_UNION_NAME

Worker Union Name

PER_ASG_JOB_MANAGER_LEVEL

Job Manager Level

PER_ASG_JOB_MANAGER_LEVEL_NAME

Job Manager Level Name

CMP_ASSIGNMENT_SALARY_BASIS_
NAME

Salary Basis

PER_ASG_COLLECTIVE_AGREEMENT_ID

Collective Agreement

PER_ASG_BARGAINING_UNIT_CODE_
NAME

Bargaining Unit Name

PER_ASG_BARGAINING_UNIT_CODE

Bargaining Unit Code

PER_ASG_ACTION_CODE

Action Code

PER_ASG_ACTION_REASON_CODE

Action Reason

Run the process if these conditions apply.

• Changes to the data referenced by the rate, which may include element entries, grade rates, and values defined
by criteria. This process only reports the rate values. It doesn't update, delete, create, or have any impact on the
underlying objects.

• Updates to rate definitions, such as when a new rate contributor is added or removed, or the rate is made

inactive.

• Changes to employee records that impact their salary rates, such as changes to job or grade.

Note:  You should run the process before any operation that depends on the values that are stored in the table. For
example, if you have a rate based on seniority, values could change simply by the passage of time.

280

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Let's look at the steps to run the process.

Chapter 4
Rates and Values by Criteria

1. On the Home page, click the Submit a Flow quick action under the My Clients group.
2. Select your legislative data group.
3. Select the Generate HCM Rates flow pattern.
4. Enter these values for the Process Mode field:

Note:  Review how your company uses the information generated by the Generate HCM Rates process and
ensure that you're selecting the appropriate process mode parameter. The mode controls the frequency of
rate calculations performed for each employee. The higher the frequency and number of rate calculations,
the more accurate the rates, but this will be reflected in the overall performance of the Generate HCM Rates
process. For more information, see "Control the Start and End Date of the Rate Calculation Period".

Mode

Fast

Description

Accuracy

Uses the start and end date specified to

This is the quickest but least accurate

calculate the rate value. If the rate value

method to calculate rate values. It misses

is the same for both dates, it determines

any changes if a rate value goes up and

that the rate value is the same over the

then back down to the same value that's

entire period. If the start and end values are

calculated at the start and end dates.

different, this method then determines a

value in the middle, and compares it with

Select this option when you need detailed

the start and finish values to see where

rate details for reporting purposes, but you

the change occurred. This process repeats

don't require 100% accuracy. As the name

until the date of the change is found. This is

suggests, this option will deliver the best

known as a binary chop algorithm.

performance for the Generate HCM Rates

process.

Full

Performs separate rate calculations for

Slowest but most accurate method.

every day within the rate calculation period.

This mode ensures that rates are 100%

accurate, but the volume of calculations per

employee is very high. It's recommended

you only select this option if you are using

the rates stored by the Generate HCM Rates

process for payroll calculation purposes.

Periodic

This method works the same as Fast, except

The accuracy of this method is half-way

that you can specify the number of days the

between the Fast and Full modes.

process calculates rates between the start

and end dates.

Select this option when you need more

precise rate details for reporting purposes.

The number of days you enter will control

the accuracy and performance of the

Generate HCM Rates process.

For example, when you select a 7-day

period, the process will calculate the rate for

an employee at the start and end of each 7-

day period. If these rates are the same, the

281

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Mode

Description

Accuracy

process will assume that the employee rate

did not change. and will move on to the next

7-day period. If the rates are different, the

process will calculate daily rates within the

7-day period to identify the date on which

the rate changed.

When you select a 14-day period, the

process will work in the same manner,

but the rates will be calculated at the start

and end of each 14-day period. In this

example, the 7-day option is more accurate,

but the Generate HCM Rates process will

take longer because it's performing more

calculations than the 14-day option.

So, the lower the number you enter in the

Number of Days parameter, the more

accurate is the rate calculation of the

Generate HCM Rates process.

5. Click Next.
6. Select a flow submission.

Note:  If you select Using a schedule, you must also select a frequency, such as once, weekly or daily.

Note:  Use the Payroll Relationship Group parameter to reduce the number of employees included in the
Generate HCM rates process. The Payroll Relationship Group parameter supports these relationship groups:

a. Static and dynamic payroll relationship groups.
b. Groups that include assignment or payroll relationship records.

7. Click Next and then Submit.

Control the Start and End Date of the Rate Calculation Period
It's essential that you understand the HCM rates configuration for your organization in detail, so that you know what
type of updates can result in a rate change, and who makes those changes. You can then define the start and end date
of rate calculations to meet the business requirements of your company. The shorter the time span, the fewer rate
calculations will be performed, and this is reflected in the performance of the Generate HCM Rates process.

Use the Generate HCM Rates Start Date parameter to set an earliest start date for rate calculations. For example, set
this parameter to 2020-01-01 (YYYY-MM-DD), and the Generate HCM Rates process will only recalculate rates from this
date.

Note:  This parameter applies only when you're using the Full or Periodic modes.

The rates process automatically calculates the rate changes that occur up to 2 years in the future. If this rate information
is not required, use the "Set the default end date limit for the rate" batch process to stop the calculation of future dated

282

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

rates. This parameter captures the number of years in advance the rates are calculated. Set to 0 to ensure that the rates
are only calculated up to the process end date you entered while submitting the Generate HCM Rates process.

Related Topics

• Overview of Rate Definitions

• Options to Configure Rate Definitions

• Rate Contributors for Derived Rates

• Create Rate Definitions for Overall Salary

Rates Used to Calculate Absences in Payroll

You can specify a rate for use in calculating an absence in an absence plan or an absence element.

When processing absence entries in a payroll run, the formula associated with the absence element uses the Rate
Converter global formula to convert rates. The formula checks for a rate in this sequence.

1. Absence plan
2. Absence element
3. Compensation salary element

Absence Plan
In Oracle Fusion Absence Management, you can select a rate rule on the Entries and Balances tab of the Create
Absence Plan page. The rate rule calculates the units passed to payroll when you record an absence. You can select rate
rules for the absence payment, final disbursement, discretionary disbursement, and liability balance calculation.

For third-party absence providers, the application transfers the rate information and override rates in the HCM Data
Loader file attached to the Load Absence Batch process.

Absence Element
If you don't specify rates in the absence plan, you can specify a rate when you create the absence elements. The type
of absence information determines the rates you can select. For example, for plans where you transfer accrual balances
and absences, you can select different rates for these calculations.

• Absence payments

• Discretionary disbursement

• Final disbursement

• Liability balance rate

As best practice, specify a rate in either the plan or the element. If you specify in both, ensure the rate for the element is
same as the rate you selected in the corresponding plan.

Compensation Salary Element
If the formula doesn't find a rate specified in the plan or the element, it uses the compensation salary element.

When you associate a payroll element to a salary basis, you specify an input value that holds the base pay on a worker's
element entry. The monetary amount or rate recorded in the element entry is the salary value in the worker's salary

283

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

information held on the assignment. If you specify a rate, the formula uses this rate if it doesn't find one defined in the
absence plan or absence element.

Related Topics

• Define Payroll Elements for Processing Absences for the US

FAQs for Rate Definitions

How does periodicity conversion work when there are multiple contributors with
different periodicities?
Sometimes, you may need to add a base salary, which is an annual figure, to a 13th month salary. This 13th month salary
is a monthly figure that's calculated from the annual base salary.

The base salary in this example is held as an annual amount on an element entry as 24,000. The 13th month salary
is 2,000 (24000 / 12). If you add each of these contributors together, the sum of the contributors is 26,000 (24,000 +
2,000).

At this point you've added an annual figure to a monthly figure, but you haven't indicated what the periodicity of the
total is. On the Create Rate Definitions page, if you select Annual in the Contributor Total Periodicity field, the sum of the
contributors is 26,000. If you select Monthly, the application converts the contributors to 312,000 (26,000 * 12), which is
now the annual figure.

Note:  When the formula is called to calculate the rate, there's an option to override the return periodicity of the rate.

Related Topics

• Options to Configure Rate Definitions

• Rate Contributors for Derived Rates

How do I use the base rate feature to calculate a rate based on multiple salary
elements?
Create a rate definition for each your salary elements. And ensure that you select the Base Rate check box in the Basic
Details section of the Create Rate Definition page.

For example, if you have three salary elements, you need to create three rate definitions and associate each rate
definition to one of your salary elements. All of your salary rate definitions must have the Base Rate check box selected.
Create an absence rate definition that has a category of Derived Rate. In the Rate Contributors section, click Create.
On the Create Rate Contributor page, select Base Rate from the Contributor Type drop-down list. This rate definition
calculates a rate based on all of your salary rates. And all rate definitions are identified as a base rate.

You can use the base rate to identify each of your company's salary rate definitions. You can then use the derived
rate to calculate a salary rate derived from all of the salary elements. You can use the base rate and the derived rate in
scenarios where your company has multiple salary elements and needs to calculate an hourly absence rate based on the
salary rate of an employee.

284

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

How do I compare rate definitions to ensure the highest rate is paid?
Create a rate definition for your salary rate. Create a rate definition for your special pay rate, and then navigate to the
Returned Rate Details section.

From the Minimum Rate Rule list, select Rate Definition. Then, from the Minimum Value list, select the salary rate that
you created.

You can use the Minimum Rate Rule option in the Returned Rate Details section in scenarios where your company
needs to pay an employee either the salary rate or the special pay rate, whichever is greater.

How can I calculate factor based element rates?
You can use the Generate HCM Rates process to calculate and store rate values for factor based element rates. You can
retrieve these values in the payroll run.

How do I ensure the Generate HCM Rates process only recalculates rates when an
employee has a rate change?
You can generate HCM rates for any employee who has an event that impacts rate amounts.

Let’s consider an example where the location and element entry changes can impact the rates. You can configure
events to track these changes. Rate event notifications will be generated for any employee with this type of change. The
Generate HCM Rates process will only include employees who have an unprocessed rate event notification. For more
information, see Calculate Rates Based on Events.

How do I include an employee with a retroactive rate change calculated by the
Generate HCM Rates process, in Retropay?
You can track retroactive rate changes for an employee, and include the employee in the Retropay process.

The Generate HCM Rates process calculates rates for employees. In some instances, the rate change can be due to a
retrospective change such as a backdated salary award for an employee, or a late change to a values defined by criteria.
You can use events to track all employees who have a retrospective rate change calculated by the Generate HCM Rates
and raise retro event notifications. To set up this feature, you need to add the Pay Rates Event entity to a retroactive
event group.

Note:  Only a single element per employee is required to track the retroactive rate changes for each payroll period.
For this reason, it's recommended that you add the event group that includes the Pay Rates Event entity to a limited
number of recurring elements, such as salary elements.

For more information, see Calculate Rates Based on Events and Generate HCM Rates.

Values Defined by Criteria

Overview of Values Defined by Criteria

Each value defined by criteria requires you to specify one or more evaluation conditions that identify a particular value
or rate.

285

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

In cases where you specify many conditions, each condition is defined as a separate level and placed in priority order to
produce a tree structure.

You control the criteria that you enter and the resulting tree structure. In each branch of the tree, you can have multiple
evaluation conditions. If the conditions that you've set don't meet your requirements, the payroll process uses the value
established for the default criteria that you set up. Each criterion and value, and the parent criteria definition, is stored
as a calculation value definition. You can define a rate definition to retrieve a rate based on values defined by criteria.

You can also search for criteria and value records, on a value defined by criteria, to quickly select a record you want to
view or update. For more information, see Search for Values Defined by Criteria.

Criteria and Evaluation Conditions
Within the tree structure, you create the criteria rules. For example, you can define criteria rules based on the location of
an employee. You can select or enter the specific location for each criterion, such as London, from a value set or on the
criteria page.

You can also define a default criterion if an employee doesn't meet any other condition. Defining a default also includes
a situation in which the application hasn't captured criteria information on the employee record, such as location. If
you know the criteria definitions you set up cover all the conditions for all employees, then you don't need a default
criterion.

Each criterion is stored as a calculation value definition. You must enter a name for the calculation value definition that's
unique within a legislative data group. With a unique name, you can identify the record while you create the values
defined by criteria hierarchy through HCM Data Loader.

You must also select a value definition group for each criterion. The group enables you to manage the value definitions
within your legislative data group; it doesn't impact the behavior of the criterion. Use the Retrieval Date to identify
whether the criterion uses the date earned or effective date to retrieve information. The default value is the effective
date.

Once you've created a criterion, you can enter these condition details:

• Sequence: Define the priority of each criterion using the sequence. The application uses the sequence order to
produce a tree structure, which affects processing and the value that's returned. For example, the first criteria
definition has a condition of age greater than 0 years, and the next criteria definition in the sequence has
the condition of age greater than 55 years. In this scenario, all employees would meet the first condition and
there would be no results for the second condition. To fix this situation, you'd reverse the order of the criteria
definitions where the condition greater than 55 years is first in the sequence.

• Database Item Name: Select a database item to identify the type of criteria. For example, if your criterion is the

location of an employee you could select PER_ASG_LOCATION_NAME.

Note:  If you're defining values by criteria for Salary Rates, select one of the database items that are
supported by HR flows such as new hire and promotion.

• Display Name: You've the option to enter a name for the criteria. This name doesn't need to be unique and
is displayed in the value by criteria hierarchy record. If you don't enter a display name, the database item
description or name gets displayed.

• Operand: You use operands when you're creating criteria. You can specify whether the value defined by the
database item should be equal to, greater than, less than, greater than or equal to, or less than or equal to
the literal value. To capture multiple values for the same criteria, use the In operand. For example, to give
employees that work in City 1 and City 2 the same bonus, you can create a single evaluation condition for both
cities using the In operand.

286

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

• Value Sets: Specify a value set to provide a dynamic list of values from which you can select an entry. This

option is available for input values that provide text only.

• Literal Value: If you specify a value set, you can select an entry from a list of values you've chosen. If you leave
the Value Set field blank, you can enter any information that's appropriate for the value definition that you're
creating.

Values
Create one or more value records for each criterion. Here you enter the calculation types and rates. For example, you
can enter the bonus values for each location.

Each value record gets stored as a calculation value definition. You must enter a name for the calculation value
definition that's unique within a legislative data group. With a unique name, you can identify the record while you create
the values defined by criteria hierarchy through HCM Data Loader.

You must enter a value identifier when you define multiple value records for a criterion. This identifier enables you
to define which value record should be calculated. For example, your company calculates car allowance and housing
allowance rates for an employee based on their job. The job criteria details and the allowance values are captured in a
Values Defined by Criteria. You can indicate which of the values captured on the Values Defined by Criteria should be
calculated when processing an element in the payroll run.

If you don't enter a value identifier, the name of the calculation value definition gets displayed for the value on the
hierarchy. You must select a value definition group for each value record. The group enables you to manage the value
definitions within your legislative data group; it doesn't impact the behavior of the value. Use the Retrieval Date to
identify whether the date earned or effective date retrieves the information of the value. The default is the effective
date.

If you select a Default Calculation Type while creating the values defined by criteria, it gets displayed on each value
record. Or, you can enter a calculation type. You've the option to select a different calculation type for each value within
the values defined by criteria depending on your business requirements.

The supported calculation types include:

• Flat Amount Times Multiplier

• Flat Calculation

• Flat Rate

• Grade Rate

•

Incremental Rate

• Number

• Rate Definition

• Standard Formula 1

• Standard Formula 2

Database Items for Values Defined by Criteria
Each condition refers to a database item to identify where the value is used. It also identify the data type of the value,
such as text, number, or date. Define conditions using predefined database items or the dynamically created database
items when the application creates data, such as balances and elements.

You can see any static or dynamic database items that support these contexts:

• HR_ASSIGNMENT_ID

287

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

• HR_TERM_ID

• PAYROLL_ASSIGNMENT_ID

• PAYROLL_TERM_ID

• PAYROLL_RELATIONSHIP_ID

• PERSON_ID

• CALC_BREAKDOWN_ID

• PAYROLL_ID

• EFFECTIVE_DATE

• DATE_EARNED

• LEGISLATIVE_DATA_GROUP_ID

Database Items for Salary Rates
Perform rate calculations before information such as job and grade is submitted for the employee. While using salary
rates, you can only define values by criteria that use the database items supported by HR flows such as new hire and
promotion. If you see other types of database items, the process either returns zero or uses the default criteria.

For the complete list of database items to define values by criteria while using salary rates, see What database items are
supported for rates based salary calculations?

Related Topics

• Options to Configure Rate Definitions

• Calculation Types in Calculation Value Definitions

• Generate HCM Rates

• Pay Bonuses at Different Rates

• Limit Pension Contributions

Search for Values Defined by Criteria
You can search for criteria and value records, on a value defined by criteria, to quickly select a record you want to view or
update.

Here's how you can search the records:

1. Navigate to the Values Defined by Criteria page and select a record, such as the values defined by criteria for

Allowances.

Use the Search section to search for specific criteria and value records within the selected value defined by
criteria.

For example, you can search for a specific criteria or value on the Allowances value defined by criteria.

2. Enter any of the following attributes and click Search:

◦ Criteria Name
◦ Criteria Display Name
◦ Value Name
◦ Value Identifier

288

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Note:  Click the Reset button to expand all records after you have performed the search.

3. To view the details of the record, click the name of the value defined by criteria (for example, Allowances).

The Criteria and Values section (collapsed initially) displays all the top-level criteria records.

4. Use either of these methods to view and edit the records returned by the search:

◦ Expand each criteria record to view the next level of criteria and value records.
◦ Select View > Expand All to view all criteria and value records.

Note:  The Expand All option is designed for smaller values defined by criteria that do not exceed the
page display limits.

Calculate Values Defined by Criteria

Use the Values Defined by Criteria task to calculate or retrieve values based on one or more conditions. You can use
values defined by criteria in rate definitions. You can also use value by criteria definitions in any formula used for
validation.

If you use a third-party payroll product and want to extract the salary rate details, use the Generate HCM Rates process
to calculate rate values. The Generate HCM Rates process is primarily used to calculate derived rate values, such as
those which sum multiple salary components. However, it's also used to process primary rates, as you may define rate
definitions which calculate values that are different from those stored on an element entry.

Note:  The values that the Generate HCM Rates process creates are stored on a rates table. You can extract this
information using the HCM Extract tool to send to your third-party payroll providers.

Use these examples to understand how you can calculate values defined by criteria for these elements of payroll.

Annual Salaries
You can calculate annual salaries for employees based on their jobs. For example:

•

•

•

If the employee is a Consultant, pay 45,000.

If the employee is a Senior Consultant, pay 55,000.

If the employee is a Principal Consultant, pay 65,000.

Note:  If the criteria that you have set up doesn't cover all the conditions, define a default criteria condition.

289

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Bonus Payments
You can choose to calculate bonus payments for employees that are weighted by their location. A more complicated
scenario would be to pay bonuses based on an employee's department and years of service.

• To weight a bonus payment by location, you could set up these criteria:

◦ For employees working in London, pay a 15 percent bonus.
◦ For employees working in Manchester, pay a 13 percent bonus.
◦ For employees working in Southampton, pay a 9 percent bonus.
◦ For all other employees, pay a 5 percent bonus.

• To pay a bonus based on department and years of service, you could set up these criteria:

◦ If an employee working in sales has less than or equal to 5 years of service, pay a 2,000 bonus.
◦ If an employee working in sales has less than or equal to 10 years of service, pay a 5,000 bonus.
◦ If an employee working in sales has greater than 10 years of service, pay a 9,000 bonus.
◦ For all other employees working in sales, pay a 7 percent bonus.

Pension Contributions
Your pension plan may have rules that limit contributions based on an employee's job. For example, in this scenario you
could set up these criteria:

•

•

•

•

If an employee is a Consultant, limit maximum contributions to 2,500.

If an employee is a Senior Consultant, limit maximum contributions to 7,500.

If an employee is a Principal Consultant, limit maximum contributions to 12,500.

If an employee is a Manager or higher, limit maximum contributions to 14 percent of pay.

Hourly Rates
In the United States, labor law mandates to pay a higher rate when a locality's minimum wage is greater than the state
or federal minimum wage. To fulfill this requirement, use the Values Defined by Criteria task to set up pay rates that a
worker's state, county, and profession determines.

In this example, you could set up criteria for these scenarios:

• Pay carpenters working in City 1 in County 1 greater than or equal to the rate of 15 per hour.

• Pay carpenters working in City 1 in County 2 greater than or equal to the rate of 17 per hour.

• Pay carpenters working in City 1 in County 3 greater than or equal to the rate of 19 per hour.

• For all other workers, pay rate of 12 USD per hour, the prevailing state wage for laborers.

Related Topics

• Overview of Values Defined by Criteria

• Generate HCM Rates

• Overview of Rate Definitions

290

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Calculate Time Based on a Default Amount

Let's look at an example that shows how to calculate time based on a default amount.

This example doesn't cover the payroll calculation. But it does support the configuration to calculate a unit of time-
based on a fixed amount.

• Create Time Element: Use the Elements task to create a shift element payable at a rate of 35 per shift worked:

◦ In the Primary Classification field, select Standard Earnings.
◦ In the Category field, select a time card.
◦ Click to select other units as the calculation unit.

• Add Default Amount: You can navigate to the Value Definitions page:

◦ Click to select the rate amount value definition for your shift element. For example, Shift Rate Amount.
◦ Click the Correct mode, to update the value from 0 to 35.

Calculate Time

Let's look at an example that shows how to calculate a percentage-based time rate when the percentage is based on
criteria, such as the worker's location.

This example doesn't cover the payroll calculation, but it supports the configuration to calculate time rates based on
values defined by criteria.

You can choose to calculate allowance payments that are based on a percentage of salary. The percentage rate is based
on a condition such as a worker's location. Here's some criteria you could use:

• Create Values Defined by Criteria: You can calculate allowance payments that are based on a percentage of

salary. The percentage rate is based on a condition such as a worker's location. Here's some criteria you could
use:

◦ For workers at location A, apply a percentage of 25% (0.25)
◦ For workers at the location B, apply a percentage of 50% (0.50)
◦ For workers at the location C, apply a percentage of 75% (0.75)
◦ For workers at all other locations, apply a percentage of 30% (0.30)

Note:  You must set the default calculation type as Number.

• Create Salary Rate Definition: Use the Rate Definitions task to create a salary rate definition to return a worker's

salary rate:

a.

In the Category list, select Element.

291

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

b.
c.

In the Storage Type list, select Amount.
In the Element Name list, search for and select a value.

• Create Allowance Rate Definition: Use the Rate Definitions task to create an allowance definition that's

calculated based on a percentage of the salary rate:

In the Category list, select Derived Rate.
In the Factor Rule field, select a value by criteria.

a.
b.
c. Select the name of your percentage based values defined by criteria.
d. Create a Rate Contributor:

i. Select the name of your salary rate.
ii. Select a contributor type of rate definition.

• Create Time Element: Use the Elements task to create an allowance element.

In the Primary Classification list, select Standard Earnings.
a.
b.
In the Category list, select Time Card.
c. Select other hours as the calculation unit.
d. For the question, Does this element have a default rate definition? Select Yes.
e.

In the rate name field, select the allowance rate definition.

Calculate Time Element Rate

Let's look at an example that shows how to calculate a time rate based on a set of conditions held in values defined by
criteria.

This example doesn't cover the payroll calculation. But supports configuration to calculate a rate based on a set of
conditions for a time element in the payroll run.

• Create Values Defined by Criteria: You can choose to calculate shift payments by the employee's location. Use

the Values Defined by Criteria task to define the shift conditions. Here are few criteria that you can use:

◦ For employees working in location A, pay is 10.
◦ For employees working in location B, pay is 20.
◦ For employees working in all other locations, pay is 0.

• Create Rate Definition: Use the Rate Definitions task to create a rate definition and associate it with the values

defined by criteria.

a. From the Category drop-down list, select Value by Criteria.
b. From the Criteria Name drop-down list, select Shift Value by Criteria.

• Create Time Element: Use the Elements task to create a shift element:

a. From the Primary Classification drop-down list, select Standard Earnings.
b. From the Category drop-down list, select Time Card.
c. For the question, Does this element have a default rate definition? Select Yes.

292

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

d. From the Rate Name drop-down list, select Shift Rate Definition.

Now you can navigate to the Calculation Factors task on the Element Overview page and see the shift calculation steps
and value definitions created by the element template.

Calculate a Rate Using Multiple Values Defined by Criteria

You can calculate a rate using a Values Defined by Criteria by referencing another Values Defined by Criteria.

In this example you'll calculate a rate using a Values Defined by Criteria referencing another Values Defined by Criteria.
Let's assume you need to calculate housing and car allowance payments based on a condition such as a worker's job.
You'll have to create separate Values Defined by Criteria to capture the different levels of the allowance rates. Let's name
them Standard Allowance Rates, Special Allowance Rates and TRU Allowance Rates. Here are some criteria you could
use:

1. Create a Values Defined by Criteria and name it Standard Allowance Rates

For workers on Job A

◦ Pay Housing Allowance 250
◦ Pay Car Allowance 400

For workers on Job B

◦ Pay Housing Allowance 650
◦ Pay Car Allowance 900

2. Create a Values Defined by Criteria and name it Special Allowance Rates

For workers on Job A

◦ Pay Housing Allowance 500
◦ Pay Car Allowance 750

For workers on Job B

◦ Pay Housing Allowance 350
◦ Pay Car Allowance 750

293

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

3. Create a Values Defined by Criteria with calculation type as Values Defined by Criteria and name it TRU

Allowance Rates.

Note:  You can create a Values Defined by Criteria based on conditions that indicate whether the ‘Standard
Allowance Rates’ and ‘Special Allowance Rates’ are applicable. In this example, the conditions are based on
the worker's TRU.

For workers on TRU 1

◦ Pay Housing Allowance using the ‘Standard Allowance Rates’ Values Defined by Criteria
◦ Pay Car Allowance using the ‘Standard Allowance Rates’ Values Defined by Criteria

For workers on TRU 2

◦ Pay Housing Allowance using the ‘Special Allowance Rates’ Values Defined by Criteria
◦ Pay Car Allowance using the ‘Special Allowance Rates’ Values Defined by Criteria

4. Once you've defined the Values Defined by Criteria, create Rate Definitions for each type of value such as

Housing Allowance and Car Allowance.

Rate Definition: Housing Allowance

◦ Select the Value by Criteria category
◦ Select the Value by Criteria Name ‘TRU Allowance Rates'
◦ Select the Value 'Housing Allowance'

Rate Definition: Car Allowance

◦ Select the Value by Criteria category
◦ Select the Value by Criteria Name ‘TRU Allowance Rates'
◦ Select the Value 'Car Allowance'

With this type of configuration, the Housing Allowance rate for an employee on TRU 2 and Job B is calculated as 350.

Enable Overrides for Time Elements

Let's look at an example that shows how to calculate a rate for a worker based on an override condition. Use values
defined by criteria to calculate rates based on a condition such as location.

In this example, let's calculate a rate for a worker who lives in New York City but works in Boston.

294

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

This example doesn't cover the payroll calculation. But it does support the configuration to calculate a rate based on a
set of conditions using an override value for a time element in the payroll run.

• Create Value by Criteria: You can choose to calculate bonus rates based on an override condition such as an

override location. Here's some criteria you could use:

◦ For workers on location A, pay 300.
◦ For workers on location B, pay 450.
◦ For workers on location C, pay 575.
◦ For workers on all other locations, pay 600.

• Create Rate Definition: Use the Rate Definitions task to create a rate definition and associate to the bonus

values defined by criteria.

a.
b.

In the category field, select a value by criteria.
In the value by the criteria name field, select the bonus values by criteria.

• Create Time Element: Use the Elements task to create a bonus element.

In the category field, select time card.

a. Select standard earnings as the primary classification.
b.
c. Select Yes to the question, does this element have a default rate definition?
d.

In the rate name field, select the bonus rate definition.

• Value Definition: Use the Calculation Value Definition task to create a location value definition. When a worker
performs their role at a different location, the override location code can be captured on the worker's time card
and passed to payroll for calculation purposes.

a. Select time in the value definition group field.
b. Select an identifier in the calculation type field.
c.

In the overriding rate identifier field, select the assignment location database items.

Note:  This should be the same database items as you used for the values defined by criteria condition.

d. Create Usage Rules.

In the calculation card field, select time cards.

i.
ii. Select your bonus calculation component.
iii. Select the value set for location if appropriate.

e.

In the Calculation Values region:

i. Enter values from 0 through 99999.9.
ii. Enter a default location code value.

Calculate Time Based on a User-Defined Value

Let's look at an example that shows how to calculate time using a business-specific attribute such as company code.

295

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

This example doesn't cover the payroll calculation. But it does support the configuration to calculate a rate based on a
user-defined value for a time element in the payroll run.

Create Element
You can choose to calculate relief allowance payments based on a worker's company code. Use the Elements task to
create an hours rate element for relief allowance.

1.
2.

In the Primary Classification field, select Standard Earnings.
In the Category field, select Time.

Create Value Definition
Use the Calculation Value Definitions task to create a company code value definition. You can capture the company code
on the worker's time card and pass it to payroll for calculation purposes.

In the Value Definition Group field, select Time.
In the Calculation Type field, select Identifier.

1.
2.
3. Select Enterable Calculation Values on the calculation card and complete these steps:

a. Select Identifier as the value type.
b. Enter a display value, such as Company.

Note:  Ensure that you select the total amount.

4. Create Usage Rules by completing these steps:

a.
In the Calculation Card field, select Time Cards.
b. Select your relief allowance calculation component.
c. Select a value set, if appropriate.

Create Calculation Step
Use the Payroll Calculation Information task to create a company code calculation step.

In the Component Group field, navigate to the Calculation Overview page, and search for time.

1.
2. Navigate through all the calculation steps tasks.
3. Create a calculation step and enter a name, such as Company Code.

Create Calculation Factor on Element
Use the Elements task to create a calculation factor.

1. Search for your relief allowance element.
2. Navigate to the Calculation Factor page.
3.
4.

In the Calculation Step field, select the company code calculation step.
In the Value Definition field, select the company code value definition.

Edit Formula on Element
Use the Elements task to edit the element formula.

1. Edit the appropriate relief allowance element formula to use the company code value using the

CALL_CALC_VALUES formula.

296

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Note:  Remember to run the Generate Data Dictionary Time Attributes process in the Oracle Time and Labor
application after you've created the value definitions. This process creates the attributes necessary to capture the
information, such as company code, on a time card and pass these details to Payroll.

Related Topics

• Generate Time Attributes and Time Card Fields for Your Elements

• Generate Data Dictionary Time Attributes

Calculate Standard Earnings Rate

Let's look at an example that shows how to calculate a standard earnings rate based on a set of conditions held in
values defined by criteria.

This example doesn't cover the payroll calculation. But it does support the configuration to calculate a rate based on a
set of conditions for a standard element in the payroll run.

• Create Values Defined by Criteria: You can choose to calculate bonus payments based on a condition such as a

worker's grade. Here's some criteria you could use:

◦ For workers on grade A, pay 5,000
◦ For workers in grade B, pay 5,500
◦ For workers in grade C, pay 6,250
◦ For workers in all other grades, pay 7,650

• Create Rate Definition: Use the Rate Definitions task to create a bonus rate definition and associate this with the

values defined by criteria:

a.
b.

In the Category field, select value by criteria.
In the Value by the Criteria Name field, select the bonus value by criteria.

• Create Element: Use the Elements task to create a flat amount bonus element.

a.
b.

In the Primary Classification field, select Standard Earnings.
In the Category field, select Standard.

• Create Value Definition: Use the Calculation Value Definitions task to create a bonus value definition. This is

required to associate the rate definition with the bonus element.

a. Click Create for a new value definition group and provide a name such as standard earnings.
b.
c.

In the Calculation Type field, select Rate Definition.
In the Calculation Values region:

i. Enter values from 0 to 99999.9.
ii. Select the bonus rate definition.

• Create Calculation Step: Use the Payroll Calculation Information task to create a bonus calculation step.

a. Search for time cards in the component group field and navigate to the Calculation overview page.
b. Navigate to all calculation steps tasks.
c. Create a calculation step and provide a unique name such as a bonus.

297

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

• Create Calculation Factor on Element: Use the Elements task to create a calculation factor.

a. Search and select the bonus element.
b. Select the calculation factor page.
c.
d.

In the calculation step field, select the bonus calculation step.
In the value definition, select the bonus value definition field.

• Edit Formula on Bonus Element: Use the Elements task to edit the element formula.

a. Edit the bonus element formula to calculate a bonus rate using the CALL_CALC_VALUES formula.

Note:  You can refer to the element status processing rules page to identify which formula to edit.

Related Topics

• Payroll Calculation Information

• Overview of Payroll Calculation Information Formulas

Pay Bonuses at Different Rates

This example demonstrates how to create criteria to pay employee bonuses at different rates based on age and location.
This table summarizes the key decisions for this scenario:

Decisions to Consider

In this Example

What ages and rates should be used?

• Age 25 or less, pay 10 percent

• Age greater than 25, pay 14 percent to City 1 employees

• Age greater than 25, pay 16 percent to City 2 employees

What locations should be used to
determine bonus rates?

• City 1

• City 2

Are there any special conditions that
should be added?

Yes. In City 2 the general manager wants to pay a flat amount of 15,000 for all employees over the age
of 25 who make over 100,000 per year.

In this example, we would perform these actions:

• Create the bonus rate criteria definition

• Create age criteria

• Create location criteria for age group 2

• Create a calculation value definition for age group 1

• Create calculation value definitions for locations

• Modify evaluation conditions

298

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Before You Start
In this example, HRX_US_REP_LOCATION is used as the value set for the entry of different locations. If you don't have
an equivalent value set, you may need to create one.

Create the Bonus Rate Criteria Definition

1. On the Home page, click the Values Defined by Criteria quick action under the My Client Groups tab.
2. Click Create.
3. Complete these fields as shown in this table.

Field

Name

Value

Bonus Rate

Effective Start Date

1/1/15

Legislative Data Group

Select your legislative data group.

4. Select Create new value definition group.
5. Enter Bonus in the New Value Definition Group field.
6. Enter Flat Rate in the Default Calculation Type field.
7. Click OK.

Create Age Criteria

1. Select the row with the Bonus Rate criteria definition.
2. Click New.
3. Select Criteria and click OK.
4. For each criteria definition you create, complete these fields.

Field

Age 25 or less

Age greater than 25

Calculation Value Definition Name

Bonus Rate Age Group 1

Bonus Rate Age Group 2

Value Definition Group

Bonus

Bonus

Retrieval Date

Date Earned

Date Earned

Sequence

1

2

Database Item Name

PER_PER_PERSON_AGE

PER_PER_PERSON_AGE

Operand

<=

>

299

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Field

Age 25 or less

Age greater than 25

Literal Value

25

25

5. Click OK each time you create a criteria definition.
6. To create a default group for the age criteria, repeat steps 1 through 3.
7. Complete these fields:

Field

Value

Calculation Value Definition Name

Bonus Rate Age Group Default

Value Definition Group

Bonus

Retrieval Date

Date Earned

8. Select the Default Criteria check box and click OK.

Create the Location Criteria for Age Group 2

1. Select the row with the Person Age > 25 criteria definition.
2. Click New.
3. Select Criteria and click OK.
4. For each criteria definition you create, complete these fields.

Field

City 1

City 2

Calculation Value Definition Name

Bonus Range Age Group 2 Location 1

Bonus Range Age Group 2 Location 2

Value Definition Group

Bonus

Bonus

Retrieval Date

Date Earned

Date Earned

Sequence

1

2

Database Item Name

PER_ASG_LOCATION_ID

PER_ASG_LOCATION_ID

Display Name

Location

Operand

=

Location

=

300

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Field

City 1

City 2

Value Set

HRX_US_REP_LOCATION

HRX_US_REP_LOCATION

Literal Value

City 1

City 2

5. Click OK each time you create a criteria definition.
6. To create a default group for the location criteria, repeat steps 1 through 3.
7. Complete these fields:

Field

Value

Calculation Value Definition Name

Bonus Rate Age Group 2 Location Default Rate

Value Definition Group

Bonus

Retrieval Date

Date Earned

8. Select the Default Criteria check box and click OK.

Related Topics

• Overview of Values Defined by Criteria

• Generate HCM Rates

Limit Pension Contributions

This example demonstrates how to create criteria to limit pension contributions based on the employee's job. This table
summarizes the key decisions for this scenario.

Decisions to Consider

In this Example

What jobs and contribution limits should
be used?

•

•

If the employee is an Associate Consultant, limit pension contribution to 5,000

If the employee is a Consultant, limit pension contribution to 10,000

• For all other jobs, limit pension contribution to 17 percent of annual salary

This example:

1. Creates the pension limits criteria definition
2. Creates job criteria
3. Creates the value definition for job 1

301

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

4. Creates the value definition for job 2
5. Creates the value definition for the default criteria definition

Create the Pension Limits Criteria Definition

1. On the Home page, click the Values Defined by Criteria quick action under the My Client Groups tab.
2. Click Create.
3. Complete these fields:

Field

Name

Value

Pension Limits

Effective Start Date

1/1/15

Legislative Data Group

Select your legislative data group.

4. Select the Use existing value definition group radio button.
5. Select Limit Rules in the Value Definition Group field.
6. Select Flat Amount in the Default Calculation Type field.
7. Click OK.

Create Job Criteria

1. Select the row with the Pension Limits criteria definition.
2. Click New.
3. Select Criteria and then click OK.
4. For each criteria definition you create, complete these fields:

Field

Job 1

Calculation Value Definition Name

Job 1

Job 2

Job 2

Value Definition Group

Limit Rules

Limit Rules

Retrieval Date

Date Earned

Date Earned

Sequence

1

2

Database Item Name

PER_ASG_JOB_CODE

PER_ASG_JOB_CODE

Operand

=

=

Literal Value

Associate Consultant

Consultant

302

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Field

Job 1

Job 2

5. Click OK each time you create a criteria definition.
6. To create a default group for the job criteria, repeat steps 1 through 3.
7. Complete these fields:

Field

Value

Calculation Value Definition Name

Other Jobs

Value Definition Group

Limit Rules

Retrieval Date

Date Earned

8. Select the Default Criteria check box and click OK.

Create the Value Definition for Job 1

1. Select the row with the criteria definition as Job 1 = Associate Consultant.
2. Click New.
3. Select Value and click OK.
4. Complete these fields:

Field

Value

Calculation Value Definition Name

Contribution Limits 1

Value Definition Group

Limit Rules

Retrieval Date

Date Earned

Calculation Type

Flat Amount

Periodicity

Annually

Unit of Measure

Money

Currency

LDG Currency

Flat Amount

5,000

303

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Field

Value

5. Click OK .

Create the Value Definition for Job 2

1. Select the row with the criteria definition as Job 2 = Consultant.
2. Click New.
3. Select Value and click OK.
4. Complete these fields:

Field

Value

Calculation Value Definition Name

Contribution Limits 2

Value Definition Group

Limit Rules

Retrieval Date

Date Earned

Calculation Type

Flat Amount

Periodicity

Annually

Unit of Measure

Money

Currency

LDG Currency

Flat Amount

10,000

5. Click OK.

Create the Value Definitions for the Default Criteria Definition

1. Select the row with the Default Criteria definition.
2. Click New.
3. Select Value and click OK.
4. Complete these fields:

Field

Value

Calculation Value Definition Name

Other Jobs

304

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Field

Value

Value Definition Group

Limit Rules

Retrieval Date

Date Earned

Calculation Type

Flat Rate

Rate

.17

5. Click OK.

Related Topics

• Overview of Values Defined by Criteria

• Generate HCM Rates

Calculate Location Allowance Rate

Let's look at an example to calculate a location allowance, based on the hire date and location of an employee.

In this example, an employee who's hired in California or Colorado before 01-JAN-19 is eligible to location allowance
payments calculated at 15% of the salary. An employee hired in these states on or after 01-JAN-19 isn't eligible to receive
the location allowance.

Create the Location Allowance Values by Criteria

1. On the Home page, click the Values Defined by Criteria quick action under the My Client Groups tab.
2. Click Create.
3. Complete these fields:

Field

Name

Value

Location Allowance Rate

Effective Start Date

Enter a valid date

Legislative Data Group

Select your legislative data group

4. Select the Create new value definition group option.
5. Enter Location Allowance in the New Value Definition Group field.
6. Enter Flat Rate in the Default Calculation Type field.
7. Click OK.

305

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Create Criteria for Each Location Eligible for Payment

1. Select the row with the Housing Allowance Rate criteria definition.
2. Click New.
3. Select Criteria and then click OK.
4. For each criteria definition you create, complete these fields:

Field

Value

Calculation Value Definition Name

Location

Value Definition Group

Location Allowance

Retrieval Date

Enter a valid date.

Sequence

Select a sequence.

Database Item Name

Select a database item name.

Operand

=

Literal Value

California

5. Click OK each time you create a criteria definition.
6. To create a default group for each location criteria, repeat steps 1 through 3.
7. Complete these fields:

Field

Value

Calculation Value Definition Name

Location Allowance Default Rate

Value Definition Group

Location Allowance

Retrieval Date

Date Earned

8. Select Default Criteria and then click OK.

Create Hire Date Rule Criteria for Each Location

1. Select the row with the Location = California criteria definition.
2. Click New.
3. Select Criteria and then click OK.

306

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

4. For each criteria definition you create, complete these fields:

Field

Value

Calculation Value Definition Name

Hire Date Rule for California

Value Definition Group

Location Allowance

Retrieval Date

Enter a valid date.

Sequence

Select a sequence.

Database Item Name

Select a database item name.

Operand

<

Literal Value

01-JAN-2019

5. Click OK each time you create a criteria definition.
6. To create a default group for each location criteria, repeat steps 1 through 3.
7. Complete these fields:

Field

Value

Calculation Value Definition Name

Hire Date Rule for California Default Rate

Value Definition Group

Location Allowance

Retrieval Date

Date Earned

8. Select the Default Criteria check box and then click OK.

Create Value Definitions for the Hire Date Rule for Each Location

1. Select the row with the Hire Date Rule for California criteria definition.
2. Click New.
3. Select Value and then click OK.
4. Complete these fields:

Field

Value

Calculation Value Definition Name

Location Allowance for California

307

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Field

Value

Value Definition Group

Location Allowance

Retrieval Date

Date Earned

Calculation Type

Flat Rate

Rate

0.15

5. Click OK.

Create Value Definitions for the Default Criteria Definitions

1. Under the job criteria definition, select the row with the Default Criteria definition.
2. Click New.
3. Select Value and then click OK.
4. Complete these fields:

Field

Value

Calculation Value Definition Name

Housing Allowance Default Rate

Value Definition Group

Housing Allowance

Retrieval Date

Date Earned

Calculation Type

Flat Rate

Rate

0.0

5. Click OK.

Create the Rate Definition for Location Allowance

1. On the Home page, click the Rate Definitions quick action under the My Client Groups tab.
2.

In the Search Results section, click Create.

308

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

3. Complete these fields.

Field

Category

Value

Derived Rate

Chapter 4
Rates and Values by Criteria

Effective Start Date

Select a date that's after the creation date of the objects that you're referencing

Legislative Data Group

Select your legislative data group

4. Click OK.
5.

In the Basic Details section on the Create Rate Definition page, complete these fields:

Field

Name

Value

Enter the name for your rate definition. For example, Rate - Location Allowance.

Short Name

Enter a short name.

6.

In the Returned Rate Details section, complete these fields:

Field

Value

Factor Rule

Value by Criteria

Name

Select the value for the housing allowance that you created using values defined by criteria. For

example, Location Allowance Rate.

Create Rate Contributors

In the Rate Contributors section, click Create.

1.
2. Select Rate Definition as the contributor type and then click OK.
3. On the Create Rate Contributors page, complete these fields:

Field

Add or Subtract

Value

Add

Rate Name

Select your salary rate definition.

309

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

4. Click Save and Continue.
5. Click Submit.

Chapter 4
Rates and Values by Criteria

Calculate Housing Allowance

Let's look at an example to calculate a housing allowance rate that's limited to maximum of 1,000 per year.

In this example, housing allowance is a percentage of the salary. The percentage value is derived based on the job of the
employee.

You can choose to calculate housing allowance rates with a job criteria with a maximum rate limit. Use the Values
Defined by Criteria task to define the conditions and housing allowance values. Use the Rate Definitions task to
associate the values defined by criteria to the housing allowance rate and apply the maximum limit rule.

In this example, you calculate housing allowance payments based on the type of the job. Create values by criteria for
housing allowance, and then define criteria for each type of job.

You can also calculate the housing allowance payments based on a percentage of salary. You can do so by first entering
values for each of the job criteria conditions. For example, if the job 'Help desk Manager' is eligible for 10% of the salary,
enter a rate value of 0.10. Specify the value for the default criteria as 0.00. This ensures that you don't pay the allowance
to employees who don't meet the job criteria.

Create the Housing Allowance Values by Criteria

1. On the Home page, click the Values Defined by Criteria quick action under the My Client Groups tab.
2. Click Create.
3. Complete these fields:

Field

Name

Value

Housing Allowance Rate

Effective Start Date

Enter a valid date

Legislative Data Group

Select your legislative data group

4. Select the Create new value definition group option.
5. Enter Housing Allowance in the New Value Definition Group field.
6. Enter Flat Rate in the Default Calculation Type field.
7. Click OK.

Create Criteria for Each Job Type

1. Select the row with the Housing Allowance Rate criteria definition.
2. Click New.
3. Select Criteria and then click OK.

310

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

4. For each criteria definition you create, complete these fields:

Field

Value

Calculation Value Definition Name

Job

Value Definition Group

Housing Allowance

Retrieval Date

Enter a valid date.

Sequence

Select a sequence.

Database Item Name

Select a database item name.

Operand

=

Literal Value

Help Desk Manager

5. Click OK each time you create a new criteria definition.
6. To create a default group for the job criteria, repeat steps 1 to 3.
7. Complete these fields:

Field

Value

Calculation Value Definition Name

Housing Allowance Default Rate

Value Definition Group

Housing Allowance

Retrieval Date

Date Earned

8. Select the Default Criteria check box and then click OK.

Create Value Definitions for Each Job Type

1. Select the row with the Job = Help Desk Manager criteria definition.
2. Click New.
3. Select Value and then click OK.
4. Complete these fields:

Field

Value

Calculation Value Definition Name

Help Desk Manager Rate

311

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

Field

Value

Value Definition Group

Housing Allowance

Retrieval Date

Date Earned

Calculation Type

Flat Rate

Rate

0.10

5. Click OK.

Create Value Definitions for the Default Criteria Definitions

1. Under the job criteria definition, select the row with the Default Criteria definition.
2. Click New.
3. Select Value and then click OK.
4. Complete these fields:

Field

Value

Calculation Value Definition Name

Housing Allowance Default Rate

Value Definition Group

Housing Allowance

Retrieval Date

Date Earned

Calculation Type

Flat Rate

Rate

0.0

5. Click OK.

Create the Rate Definition for Housing Allowance

1. On the Home page, click the Rate Definitions quick action under the My Client Groups tab.
2.

In the Search Results section, click Create.

312

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

3. Complete these fields.

Field

Category

Value

Derived Rate

Chapter 4
Rates and Values by Criteria

Effective Start Date

Select a date that's after the creation date of the objects that you're referencing

Legislative Data Group

Select your legislative data group

4. Click OK.
5.

In the Basic Details section on the Create Rate Definition page, complete these fields:

Field

Name

Value

Enter the name for your rate definition. For example, Rate - Housing Allowance.

Short Name

Enter a short name.

6.

In the Returned Rate Details section, complete these fields:

Field

Value

Factor Rule

Value by Criteria

Name

Select the value for the housing allowance that you created using values defined by criteria. For

example, Housing Allowance Rate.

Maximum Rate Rule

Maximum Value

Value

1,000

Create Rate Contributors

In the Rate Contributors section, click Create.

1.
2. Select Rate Definition as the Contributor Type and then click OK.

313

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 4
Rates and Values by Criteria

3. On the Create Rate Contributors page, complete these fields:

Field

Add or Subtract

Value

Add

Rate Name

Select your salary rate definition.

4. Click Save and Continue.
5. Click Submit.

FAQs for Values Defined by Criteria

Does the order in which I add criteria definitions matter?
Yes, each criteria definition that you add is defined as a separate level and placed in priority order. The order produces a
tree structure, which affects processing and the value that's returned.

You can change the sequence of the criteria definitions at any time to suit your business needs and fix processing
problems.

How do I define minimum or maximum rules for a values by criteria rate?
Create a value by criteria definition. Create a rate definition that has a category of Value by Criteria and associate the
rate definition to the value by criteria definition.

Create a rate definition that has a category of Derived Rate. Create a rate contributor with a contributor type of Rate
Definition, and then select the values by criteria rate definition. You can now define return rate rules for your derived
rate, such as a minimum or maximum values. These return rate rules will be applied to the values by criteria rate.

When do I define a default criteria for values defined by criteria?
You must always create a default criteria definition. The application uses this default criteria if the employee's record
misses the conditions that you have set.

Why hasn't a rate been calculated based on the values specified on the values defined
by criteria?
Ensure that a value identifier is entered only for those values defined by criteria that have multiple value records for a
criterion.

314

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

5  Payroll Processing Rules

Payroll Process Configuration Groups

Overview of Payroll Process Configuration Groups

Payroll process configuration groups provide sets of processing parameters, primarily related to logging and
performance.

Select a process configuration group when you run a process, such as a new-hire flow or termination flow, or an extract
process or report.

If you don't select a process configuration group, the application uses the parameters in the default group. You must
specify the default group in the Process Configuration Group ACTION_PARAMETER_GROUPS profile option.

Here's the list of tasks you can use to set up profile options and default process configuration groups.

Action

Task and Page

Edit predefined process configuration
groups

Default Group tab of the Payroll Process Configuration page.

Create additional process configuration
groups

Group Overrides tab on the Process Configuration Group page.

Select a process configuration group as
the default at the site or user level

Manage Administrator Profile Values task in the Setup and Maintenance area.

To open the Payroll Process Configuration page, use the Payroll Process Configuration task under Show More >
Payroll in My Client Groups on the Home page.

Create a group with the logging parameters turned on to troubleshoot processes. You can also specify different
performance parameter values, such as chunk size and buffer size, for running different processes.

Payroll Process Configuration Parameters

Payroll processing parameters are system-level parameters that control aspects of payroll-related processes, such as
flows and reports.

Values for each parameter are predefined with the application, but you can override these values as part of your initial
implementation and for performance tuning. Use the Payroll Process Configuration task under Show More > Payroll in
My Client Groups on the Home page.

315

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Processing Parameters
The effects of setting values for specific parameters may be system-wide. When you submit a process that uses flows,
such as a batch upload, new hire, or report process, the process reads values from the PAY_ACTION_PARAMETERS
table.

Note:  You should understand the concept of array processing and how this affects performance before setting some
parameters.

The application doesn’t allow a blank value for any parameter. Unless the parameter is required, you must delete the
parameter row.

This table describes processing parameters and lists values and predefined default values. These parameters apply to
HR applications including payroll and payroll interface.

Parameter

Description

Values

Assignment ID to End Logging

Assignment ID upon which logging ends.

Default: All assignments

Assignment ID to Start Logging

Assignment ID upon which logging starts.

Default: All assignments

Balance Buffer Size

Buffer size for array inserts and updates of
latest balances, based on one row per balance.

Maximum: 1000

Tip:
If your trace files show differences between
execute and retrieve timings, look at the
buffer sizes you're using. Try setting each of
these to 100.

Minimum: 1

Default: 500

Batch Error Mode

Determines error notifications for the HCM data
loads.

ALL = all rows

Chunk Size

Number of payroll relationship actions
that process together. See also the Parallel
Processing Parameters topic.

ANY = any rows

NONE = no errors

Default: ANY

Maximum: 16000

Minimum: 1

Default: 20

Disable Locking Code in Check Process Post-
Populate Method

Disables the locking code added to the post-
populate method to improve check process
performance.

Yes, No

Default: No

This parameter isn't available by default. To add
the parameter, search for the lookup type PAY_
ACTION_PARAMETER_TYPE on the Common

Only change this value if advised by Oracle
Support.

316

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Parameter

Description

Values

Element Entry Buffer Size

Lookups page and add the lookup code ORA_
DISABLE_POST_POP_FIX.

Buffer size that payroll runs use in the initial
array selects of element entries, element entry
values, run results, and run result values per
assignment.

Maximum: 1000

Minimum: 1

Default: 500

Formula Execution Logging

Sets the logging level to investigate formula
code problems. See also the Logging
Processing Parameters topic.

Unless the parameter is required, delete the
parameter row.

Historic Payment

Removes the validation to look for banks
active as of the process date. This validation is
enforced by the payments process.

Yes, No

Default: No

Logging Area

Logging Category

This parameter isn't available by default. You
can add it in test environments only. To add
the parameter, search for the lookup type
PAY_ACTION_PARAMETER_TYPE on the
Common Lookups page and add the lookup
code HISTORIC_PAYMENT.

Area to log code. See also the Logging
Processing Parameters topic.

The values correspond to C-code entries in the
form PY_ENTRY, that includes the functional
area that has logging enabled.

Helps investigate problems with large volumes
of detailed data. See also the Logging
Processing Parameters topic.

You can set any number of categories by
specifying multiple values. For example, enter
GMPE, for general logging information, routing
information, performance information, and
element entry information.

Refer to the Logging Processing Parameters
topic in the Related Links section for applicable
values.

Unless the parameter is required, delete the
parameter row.

Manual Task Processing

Determines processing of manual tasks when
SOA server is unavailable.

Y, N

Default: Y

Maximum Errors Allowed

Number of payroll relationship actions that you
can roll back, when rolling back a process.

Minimum: 0

Maximum File Size for View Report Output

Maximum size in bytes of the report file to
show in the output window.

This parameter isn't available by default. To add
the parameter, search for the lookup type PAY_
ACTION_PARAMETER_TYPE on the Common

Default: CHUNK_SIZE or 20

Must be a positive number.

Default: 10000000

317

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Parameter

Description

Values

Lookups page and add the lookup code BI_
OUTPUT_SIZE.

Maximum Iterations Allowed per Run Action

Maximum number of iterations allowed per run
action within net-to-gross calculations within
the payroll run.

Minimum: 0

Default: 15

Maximum Number of Payroll Relationship
Actions to Roll Back

Number of payroll relationship actions that you
can roll back, when rolling back a process.

Multithreaded XML Generation for Extracts

Generates XML for extracts using multiple
threads.

Minimum: 1

Default: 50

Y, N

Default: N

New Hire Flow Pattern

Name of the customer-defined flow that’s
triggered as part of the new hire process.

Unless the parameter is required, delete the
parameter row.

Notifications Expiration Offset

Number of days before a payroll flow
notification is automatically deleted.

Minimum: 5

Default: 5

Payroll Batch Loader Encryption Type

The type of encryption applied to source files
loaded using the HCM data loader.

PGPSIGNED, PGPUNSIGNED,
 PGPX509SIGNED, PGPX509UNSIGNED

Unless the parameter is required, delete the
parameter row.

Payroll Criteria for Element Eligibility

Enables eligibility by payroll for assignment-
level elements.

Yes, No

Default: No

Process Timeout

Number of minutes before the Run Balance
Generation process times out.

Minimum: 0

Default: No timeouts limit enforced.

Unless the parameter is specified, delete the
parameter row.

Remove Report Assignment Actions

Removes report processing actions after
generating reports.

Yes, No

Default: Yes

Run Result Buffer Size

Buffer size for array inserts and updates, based
on 1 row for each payroll run result.

Maximum: 1000

Shuffle Chunk Processing

Random processing of order chunks for
assignment actions.

Minimum: 1

Default: 500

Yes, No

Default: No

318

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Parameter

Description

Values

Suppress Empty XML Tags in Extract Reports

Reduces the size of extract output for reports
by excluding tags with blank values in XML
output files.

Y, N

Default: Y

Termination Flow Pattern

Name of the customer-defined flow that’s
triggered as part of the termination process.

Unless the parameter is required, delete the
parameter row.

(No predefined Termination flow pattern).

Threads

Trace

Trace Level

User Messaging

XML_DATA_SOURCE

Total number of subprocesses that you can run
from the Oracle Enterprise Scheduler Service.
See also the Parallel Processing Parameters
topic.

Minimum: 1

Default: 1

Enables the database trace facility for
application processes written in C only.

Yes, No

Default: No

Sets the trace level of the trace event. To
generate the finest level of detail, enter the
highest value.

1, 4, 8, 12

Default: None

Enables detailed logging of user-readable
information to the PAY_MESSAGE_LINES table.

Yes, No

Default: No

For document records delivery options
performance purposes, determines if XML is
derived from the database.

Y, N

Default: Y

Payroll-Specific Processing Parameters
This table lists the processing parameters that are applicable only for Oracle Global Payroll.

Parameter

Description

Values

Accounting Date for Transfer to General Ledger

The date to transfer and post journal entries for
costing results to Oracle Fusion General Ledger.

E = Date Earned

P = Process Date

DP = Date Paid from payroll time periods for
calculate payroll and QuickPay only.

EVE = For the Partial Period Accrual Reversal
process, date earned is used. However, if the
date earned isn't defined for the time periods
on the Payroll Definition page, the payroll
period end date is used.

319

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Parameter

Description

Values

For the payroll run that includes the actual
costs, the process date of the payroll run is
used.

Default: P

Maximum: 1000

Minimum: 1

Default: 500

E = Date earned

P = Date paid

Default: P

Date value in YYYY/MM/DD format

Cost Buffer Size

Buffer size for array insert and select
statements when calculating the costing of the
payroll run results.

Date to Retrieve Assignment Status

Date earned or date paid, used to determine the
effective date for checking assignment status in
payroll calculations.

Earliest Retroactive Processing Date

Sets earliest date that retroactive processes
are calculated. Updates made before this date
aren’t recalculated.

Note:  If you define a static retroactive start
date and a rolling retroactive start date, the
retropay process uses the latest of the two
dates. For example, if the static retroactive
start date is 01-JAN-2020 and the rolling
retroactive start date is 15-MAR-2019, the
retropay process uses a start date of 01-
JAN-2020.

Controls the start date of the retroactive period
for the Calculate Payroll for Retroactive
Changes flow (retropay) as well as for an
individual employee

Extract Data Group for Payroll Register

Limits the records to include in the output file
based on the specified data group name.

Default: No data group

Limit Payroll Register Output by Data Group

Enables processing a subset of records to
include in the output file when an extract data
group parameter value is also specified.

Y, N

Default: N

Number of months in rolling period for
retroactive changes

Sets the number of months in the retroactive
pay rolling period.

Default: 12

If you don't want to limit the duration of the
retroactive pay period, change the default of 12
month rolling period to 999 months.

320

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Parameter

Description

Values

Note:  You can limit the number of payroll
periods included in the retroactive pay
process by setting the earliest start date for
the process for the process for all retroactive
notifications using both the Earliest
Retroactive Processing Date parameter
and this parameter. For example, you may
want to set a static start date based on your
payroll go-live date and use a rolling period
to ensure retroactive pay doesn't calculate
for more than a 24 month period. Retroactive
pay uses the latest of the two dates when
both parameters are set.
If you don't want to limit the duration of the
retroactive pay period, change the default 12
month rolling period to 999 months.

Reversal and Balance Adjustment Accounting
Date

Accounting date based on one of these dates:

• The process date of reversal or balance

adjustment

• The process end date of the Transfer to
Subledger Accounting task. You can use
this task to transfer journal entries for
costing results to Oracle Fusion General
Ledger.

T = Transfer using end date of the Transfer to
Subledger Accounting task as the accounting
date

P = Use process date of the reversal or balance
adjustment as the accounting date

Default: P

Wage Basis Rules Buffer Size

Used in array selects from the PAY_
 TAXABILITY_RULES table within the Payroll
Calculation process.

Minimum: 100

Default: 500

Related Topics

• Payroll Process Configuration Groups

• Logging Processing Parameters

• Parallel Processing Parameters

Logging Processing Parameters

Use logging parameters to investigate problems that aren't easily identified in other ways. In a normal operation, disable
logging because it can impact the performance of the process you're logging.

Note:  Prepare log files before contacting Oracle Support for assistance. Define the logging area, category, and range
of assignments before resubmitting the problem.

321

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Logging Parameters
Typically, you use this feature during your initial implementation and testing before you go live. In a normal
operation you should disable detailed logging.

The three processing parameters for logging are:

• Logging Area

• Logging Category

• Formula Execution Logging

Logging Area

The Logging Area parameter works with the Logging Category parameter to limit the code area for logging. Even if you
set the logging category, you must also set the logging area if you want to limit logging to a particular code area.

The values correspond to C-code entries in the form PY_ENTRY, which includes the functional area that will have
logging enabled.

Logging Category

Logging categories define the type of information included in the log. You can set any number of categories by
specifying multiple values to focus on specific areas that you think may be causing a problem. The application doesn’t
allow a blank value and you must delete the parameter row if logging isn’t required.

This table explains each logging category. It provides the log output information to investigate the problems
encountered.

Parameter Value

Logging Category

Description

B

C

E

F

G

Balance Information

C cache structures information

Element entry information

Formula information

General logging information

Provides output information that shows the
creation and maintenance of balances used
during payroll processing.

Provides output information that shows details
of the payroll cache structures and changes to
the entries within the structure. While working
on a service request, Oracle may ask you to use
this parameter to gather additional information.

Provides output information that shows the
state of the element entries in the process
memory after retrieving entries from the
database. The information is provided
whenever data for an entry is changed during
processing.

Provides output information that shows
details of formula execution, including formula
contexts, inputs, and outputs.

Provides general information, rather than
a specific information type. This parameter
doesn't provide sorted output. In general, it's

322

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Parameter Value

Logging Category

Description

I

L

M

P

Q

R

S

Balance output information

Balance fetching information

Entry or exit routing information

Performance information

C cache query information

Run results information

C cache ending status information

T and Z

PL/SQL detail and PL/SQL output

recommended that you choose parameters that
provide specific types of information.

Provides output information that shows details
of values written to the database from the
balance buffers.

Provides output information that shows the
balances retrieved from the database and
whether or not the process will use those
balances. (If balances such as Year To Date
totals have expired because the year has
changed, the process resets them and uses the
new balance.)

Provides output information to show when any
function is entered and exited.

This information is indented to show the
call level, and can be used to trace the path
taken through the code at the function call
level. Often, this information is useful when
attempting to track down a problem such as a
core dump.

Provides output information to show the
number of times certain operations take place
at the assignment and run levels and why the
operation took place. This parameter is often
used to balance the buffer array write operation.

Provides output information that shows the
queries being performed on the payroll cache
structures. While working on a service request,
 Oracle may ask you to use this parameter to
gather additional information.

Provides output details of run results and run
result values from the Run Results buffer or
the Values buffer before writing them to the
database. This enables verification that the
buffer contents were correct.

Provides output information that shows the
state of the payroll cache before the process
exits, whether that process ends with success
or an error. While working on a service request,
 Oracle may ask you to use this parameter to
gather additional information.

To obtain detailed information about the PL/
SQL calls made by the Payroll application, use
the combination of the T parameter and the Z
parameter.

323

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Parameter Value

Logging Category

Description

This combination is typically useful for
obtaining information about payroll processes
that use a large amount of PL/SQL code, such
as prepayments and archive.

Using this parameter, the process buffers
output while it's running and places it the end
of the log file after processing is complete.
Each payroll process instance has its own log
file, located under the log subdirectory for the
particular process ID.

Formula Execution Logging

Formula execution logging is the code area where logging is performed. This processing parameter mechanism is only
available for formula logging in the payroll run. Specify parameter values as a character or combination of characters
to determine the area for logging. For example, the string di (the combination of d and i) corresponds to the logging of
database item cache access and formula input and output values. The default value is no logging.

CAUTION:  Use the dump logging options in rare circumstances only. The T trace option, which generates very large
amounts of data, would significantly slow down processing.

The following table lists formula execution logging parameter values and its details.

Parameter Value

Meaning

c

d

D

f

F

I

m

n

s

T

Change contexts

Database item cache access

Database item cache dump

Formula cache access

Formula cache dump

Formula input/output values

Miscellaneous

Nested calls

SQL execution (database item and PL/SQL formula function calls)

Trace (very large level that provides the inputs and outputs of every call made when executing a
formula)

324

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Parameter Value

Meaning

w

W

1

2

3

4

5

Working storage area access

Working storage area dump

Level 1 (combination of c. f, i, and m)

Level 2 (combination of 1, c, d, n, and w)

Level 3 (combination of 2, D, s, and W)

Level 4 (combination of 3 and F)

Level 5 (combination of 4 and T)

Related Topics

• Payroll Process Configuration Groups

• Payroll Process Configuration Parameters

• Parallel Processing Parameters

Parallel Processing Parameters

Payroll processes are designed to take advantage of multiprocessor computers. You can improve performance of your
batch processes, such as Calculate Payroll or Calculate Gross Earnings, by splitting the processing into a number of
threads, or subprocesses, which run in parallel.

To improve performance you can also set the number of payroll relationship actions that process together and the size
of each commit unit for the batch process.

Here’s a list of parameters that you can use for parallel processing.

Parallel Processing Parameters
Threads

When you submit a batch process, the Threads parameter determines the total number of subprocesses that run
concurrently. The number of subprocesses equals the Threads value minus 1.

Set this parameter to the value that provides optimal performance on your computer:

• The default value of 1 is set for a single-processor computer.

325

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

• Benchmark tests on multiprocessor computers show that the optimal value is approximately 2 processes per

processor.

For example, if the server has six processors, set the initial value to 12 and test the impact on performance of
variations on this value.

Chunk Size

The Chunk Size parameter:

•

Indicates the size of each commit unit for the batch process.

• Determines the number of assignment actions that are inserted during the initial phase of processing.

• Sets the number of assignment actions that are processed at one time during the main processing phase.

This parameter doesn't apply to all processes, such as Generate Check Payments and Retroactive Pay.

To set the value of the Chunk Size parameter, consider the following points:

• Parameter values range from 1 to 16,000.

• The default value is 20, which was set as a result of benchmark tests.

• Each thread processes one chunk at a time.

• Large chunk size values aren't desirable.

Related Topics

• Payroll Process Configuration Groups

• Payroll Process Configuration Parameters

• Logging Processing Parameters

FAQs for Payroll Process Configuration

How can I improve performance and troubleshoot flows?
Add parameters to a payroll process configuration group to optimize performance and troubleshoot your payroll
processes. To process large volumes of records, use the Threads and Chunk Size parameters.

To troubleshoot processes, add the Logging Category or Formula Execution Logging parameters to a configuration
group and rerun the process using that configuration group. Using these parameters enables you to investigate formula
code problems.

Restrict Payroll Processing

Select rules to control which payroll relationships and which elements to process in a payroll run.

For example, a skip rule or frequency rule. Specify flow parameters when you submit the calculation process to restrict
the payroll relationships and further restrict the elements that the run processes. For example, Calculate Payroll or
Calculate Gross

326

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Earnings.

Chapter 5
Payroll Processing Rules

Restrict the Elements Processing Based on Rules
You can create skip and frequency rules that control when the payroll run processes the recurring element.

Rules

Skip

Frequency

Use To

Examples

Include or exclude the element entry for the
person using rules in a formula

A once-each-period rule stops recurring
element entries from processing more than
once in a payroll period.

Specify which payroll periods to process the
entries

Changed to: A frequency rule might specify that
the payroll run processes an element only on
the first and third weeks of a month.

Restrict the Records to Process Based on Flow Parameters
As this table shows, specify flow submission parameters to restrict the number of records for the calculation process.

Parameter

Use To

Payroll Relationship Group

Restrict processing to the payroll relationships within the group, which you can define using static or
dynamic rules, based on payroll relationship or assignment information.

Element Group

Run Types

Restrict processing to the elements in the group, which you can define by selecting element
classifications and including or excluding specific elements.

Determine which payroll calculations to perform and how to pay the results. The application processes
an element in all the run types, unless you set up the element in these ways:

• To process separately

• As a trigger for a run type, in which case it's automatically excluded from the other run types

This table shows the flow submission parameters for the calculation process including dates that control which records
to process:

Date

Process Date

Payroll Period

Date Earned

Required?

Comments

No

Yes

Yes

This is typically the payroll run date of your
payroll definition.

Used to derive other dates for processing.

Identifies these element entries

• To include in the payroll run

327

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Date

Required?

Comments

• That belong to a proration group and

ended within the payroll period

Related Topics

• Overview of Object Groups

Optimize Performance of Multi-Thread Processes

The automatic multi-thread feature optimizes the performance of multi-thread processes, such as the Calculate Payroll
process, by automatically identifying and assigning the correct number of threads and chunk size to the process.

The automatic multi-thread feature supports all multi-thread payroll processes such as Calculate Payroll and Make
EFT Payments. It also supports predefined HCM Extracts such as the Gross-to-Net report and user-defined extracts
including copied extracts.

Maximum Number of Threads
By default a payroll process executes in single-threaded mode. Use the Maximum Number of Threads action
parameter to enable the automatic multi-threading and chunk size feature. This parameter indicates the maximum,
total number of sub-processes dynamically created for a process.

The application automatically assigns the optimum number of threads and generates multiple secondary sub-processes
that are executed in parallel to optimize performance.

Here’s a list of features supported by the automatic, multi-threading parameter:

• The number of threads is automatically determined based on the Maximum Number of Threads parameter
plus the complexity of the process. For example, the Calculate Payroll process is a very complex process and
hence the number of employees that can be calculated in each chunk should be lower than less complex
calculations such as retry or prepayments. As a result, the number of threads automatically assigned to the
Calculate Payroll process is higher than the number of threads used when retrying a process.

• The number of threads used doesn’t exceed the maximum number defined on the Threads action parameter.

Complex processes such as the Calculate Payroll process may use the maximum number of threads you define.

• The maximum thread setting applies to all your payrolls such as weekly and semimonthly. The total number of
employees processed in each payroll can vary. The automatic multi-thread solution dynamically reduces the
number of threads used for smaller payroll to ensure more resources are available for any other processes that
can be run in parallel.

• Check the log file to view the number of threads used by the process. Enable logging to view the log file for the

process.

Enable the Automatic, Multi-Thread Process
Use the Payroll Process Configuration task and edit the default process configuration group for the process:

• Remove the Threads action parameter. This determines the total number of sub-processes that run under the

concurrent manager.

328

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

• Remove the Chunk Size action parameter. This is the number of relationship actions that should process

together in chunks during the main processing phase.

• Add the Maximum Number of Threads action parameter. This parameter indicates the maximum, total

number of sub-processes dynamically created for a process. The default value is '20' and you must specify
the maximum number of threads. This action parameter enables the automatic multi-thread and chunk size
feature.

Note:  The value you enter in the new Maximum Number of Threads field must be the same as that given
in the Threads field. For example, if ‘25’ was defined in the Threads field, you should enter ‘25’ in the new
Maximum Number of Threads field.

• The Threads field determines the total number of sub-processes that run under the concurrent manager, and
the new Maximum Number of Threads parameter indicates the maximum, total number of sub-processes
dynamically created for the process action parameter.

Optimize Performance of the Payroll Background
Process

The payroll background process is a daemon process that runs continuously to handle periodic requests for processing.
It’s used to submit processes such as the QuickPay for Anytime Pay process and Event Action Notifications.

Enable automatic multithreading for the payroll background process to enhance performance of the submitted payroll
processes and run multiple processes concurrently.

Use the Payroll Process Configuration task under Payroll to search for the delivered Pay Daemon Group process
configuration group. Edit and enable the Pay Daemon Group configuration group to optimize the performance of the
payroll background process by automatically identifying and assigning the correct number of threads to the process.
The payroll background process can then execute large number of processing requests and handle multiple processes
concurrently. For example, multiple runs of QuickPay for Anytime Pay can be processed concurrently.

Use the Maximum Number of Threads action parameter to enable automatic multithreading for the payroll
background process. This parameter indicates the maximum, total number of subprocesses dynamically created for a
process. Perform these steps to enable the Pay Daemon Group.

1. On the Payroll Process Configuration page search for the default group and under Parameter Name search for

the Maximum Number of Threads parameter and note the value.

2. Search for the delivered Pay Daemon Group and click Add under Parameter Name. Search for the Maximum

Number of Threads parameter and enter an Override Value.

Set this parameter to about 10% of the Maximum Number of Threads on your default group for the process.

For example, if the Maximum Number of Threads action parameter is set to 30 on the default group, set it to 3
on the Pay Daemon Group process configuration group.

When you don't enter a value for the Maximum Number of Threads action parameter, the payroll background process
runs using a single thread process.

329

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

The process sets the threads depending on the number of processing requests or pay daemon actions in the queue at
a given time. A new thread is submitted for each 5,000 processes in the queue for the payroll background process until
the Maximum Number of Threads is reached.

Enable Logging
Use the Pay Daemon Group process configuration group to control other parameters for the payroll background
process, such as logging. If you want the processes running on the daemon to generate a log output, enable logging in
the Pay Daemon Group.

Note:  It’s recommended that you enable logging on the Pay Daemon Group process configuration group and not on
the default group for the process.

Dynamic Parameters
The flow parameters for the Payroll Background Logging and Monitoring flow are enabled as dynamic parameters.
When you select the value for one parameter on the redesigned Redwood flow submission page, depending on the
input value, the values for the other parameters on the page are automatically enabled or disabled.

The required or optional parameters for the flow are grouped together in a single section on the flow submission page,
irrespective of whether they are required or optional. Depending on the value you select or enter for a parameter on the
flow submission page, the other parameters on the page can change as either required or optional.

Logging and Monitoring the Payroll Background Process

Use the Payroll Background Logging and Monitoring flow to identify and resolve payroll queries for features that use
the payroll background process.

This flow is useful for those who manage customer environments, test payroll processes, and troubleshoot issues with
payroll processes. For example, your system administer can use this flow to generate log files for features that uses the
payroll background flow such as Anytime Pay.

Note:  Payroll features that use the payroll background flow include Anytime Pay and Event Notification Processing
that has rate events enabled. The payroll background process is an ESS process that runs continuously in the
background to improve the performance of payroll features. Since it runs continuously, it’s not required for the ESS
server to start or stop whenever you submit a process such as the submission of the QuickPay process for Anytime
Pay. Leave the Legislative Data Group field blank when you submit the Payroll Background Logging and Monitoring
flow.

330

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Considerations for Using the Payroll Background Logging and Monitoring
flow
Consider these points when you use the Payroll Background Logging and Monitoring flow.

• Leave the Legislative Data Group field blank when you submit the Payroll Background Logging and Monitoring

flow.

• Use the Actions field to perform any of the actions given in this table on the payroll background ESS process.

Action

Description

Start Process

When called by a feature, the payroll background ESS process starts automatically and will

continue to run. You can use this option to override this default behavior and manually start the

process.

Stop Process

Use this option to stop the background payroll ESS process. Any process that's already running

using the payroll background process will complete, but the next process in queue will not start.

Report

Use this option to report on the status of the background payroll ESS process.

Resubmit Process

Use this option to resubmit a process submitted using the payroll background ESS process and

is in error.

• Use the Job Identifier field to identify the process submitted using the payroll background process. Each

background process has a job ID number, similar to an ESS job number.

• Use the Report Type field to select the type of report you want to generate using this flow. These reports are
intended for users who are trying to identify the root cause of an issue. This table lists the type of reports you
can generate.

Type of Report

Description

Processing Report

This report displays all processes that are currently running or are in the payroll background

queue for today. For example, a QuickPay has been submitted for Anytime Pay but no results

are generated for the employee. Use this report to check if the QuickPay is stuck in a queue of

processes waiting to be completed by the payroll background process.

Scheduled Report

This report identifies all pending processes in the payroll background queue for the specified

date range.

Error Report

This report identifies all error messages for the payroll background process. For example, a

QuickPay has been submitted for Anytime Pay but no results are generated for the employee.

Use this report to check if the payroll background process has hit an error that stopped the

submission.

Log File

Use this option to enable detailed logging information for a process submitted using the payroll

background process.

331

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Note:  Use the predefined PAY DAEMON GROUP payroll process configuration group for processes submitted using
the payroll background process.

Expedited Processing

Overview of Expedited Processing

Streamline the payroll processing of time card employees through expedited payroll runs. You can make immediate
payments for absences, late time cards, or time card errors that an employee submits late on a time card.

You can process expedited runs only for absence and time entries that are retroactively modified on a time card and
marked for expedited processing. Time card of employees that aren't marked for expedited processing are paid in the
next scheduled regular payroll cycle.

When you define time and absence category elements, the application creates these value definitions for expedited
processing.

• Expedite: Determines if this time card or absence entry corresponding to prior pay period adjustment needs to

be included for expedited processing.

• Override Payment Method: Overrides the payment method on the Prepayments and QuickPay Prepayments
process to Check. You can select this value only for time cards that you have marked for expedited processing.

• Override Check Printer: Tracks the check printer for the expedited time cards that are paid through check. The

application ignores the Override Check Printer value if the employee isn't paid by check.

Related Topics

• How Expedited Processing Works

• Expedited Payroll Flow

Expedited Processing Rules

Expedited processing includes prior period adjustments to time, absence, and mandatory elements like taxes and
percentage-based deductions. By default, the expedited run includes all the element entries for those employees who
have an expedited time card.

Use Expedited Processing Rules option to exclude certain elements such as salary or flat amount based deductions
from expedited payroll run. To review and create new payroll elements, use the Elements task in My Client Groups.

Expedited Processing Rule Option

Use To

Based on the element entry value

Initiate expedited processing depending on other parameters on the time card. This option applies
only to time card and absence elements having the three input values and value definitions for
expedited processing and is set automatically during element creation. The application processes
elements with this rule based on the element entry value for 'Expedite'.

332

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Expedited Processing Rule Option

Use To

Do not include in expedited payroll runs

Exclude elements like salary and flat amount-based deductions that are processed only once per pay
period from expedited payroll runs. Set this option to include these elements only in the nonexpedited
payroll run.

Include in both expedited and
nonexpedited payroll runs

Include elements like taxes and percentage-based deductions in the expedited payroll runs. If you
leave the Expedite Processing Rule blank, this option acts as the default behavior.

Related Topics

• How Expedited Processing Works

• Expedited Payroll Flow

Add Override Check Printer in XML File

Use the Override Check Printer attribute to track the check/cheque printer for the expedited time cards that are paid
through check/cheque. The application ignores the Override Check Printer value if the employee isn't paid by check/
cheque.

You can add the Override Check Printer in the XML file that the Generate Check Payments process generates.The
bursting file references this Override Check Printer setting for printing the checks/cheques.

Before You Begin
Configure the list of printers in the HCM Common Lookup ORA_EXPEDITE_CHECK_PRINTER to find the list of values for
Override Check Printer.

Add Override Check Printer
Perform these steps to add the override check printer attribute in the XML file.

In the Setup and Maintenance work area, go to the Extensible Flexfields for Payroll task.

1.
2. On the Extensible Flexfields for Payroll page, click Deploy Flexfield.
3.
4. Click Done.
5.

In the Confirmation dialog box, click OK.

In the Setup and Maintenance work area, go to the Manage Enterprise HCM Information task in the
Workforce Structures functional area.

6. On the Enterprise page, click Edit and select Correct.
7.
8. For each element entered on the time card, enter these values and click Submit.

In the Global Payroll Element Information to Archive section, click Add.

Field

Value

Legislative Data Group

Appropriate LDG

Element

Any retro result element

333

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 5
Payroll Processing Rules

Field

Value

Input Value 1

Override Check Printer

Related Topics

• How Expedited Processing Works

• Expedited Payroll Flow

334

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

6  Payroll Definition Details

Payroll Definitions

Overview of Payroll Definitions

When you create or modify payroll definitions, the application generates a calendar of payroll periods based on your
selections. The choices you make for these values determine the resulting schedule of payroll periods:

Effective Start Date
The effective start date is the first date that the payroll definition is available for employee data. The start date must
be on or before the earliest date of any historical data that you want to load. For example, for a payroll starting on 01-
JAN-2013 with five years of historical payroll data to load, you set the start date of the payroll definition to 01-JAN-2008.

The effective start date doesn't affect the generated calendar of payroll periods. The start date for the first payroll
period is based on the first period end date.

First Period End Date
The first period end date is the end date of the first payroll period that the application generates for a payroll definition.
The first period end date is typically based on the date of implementation, tax year, benefits enrollments, or a particular
payment cycle. For example, if your weekly payroll work week is Saturday through Friday, and your first payment date is
on 06-JAN-2012, you could use 30-DEC-2011 as your first period end date.

Ledger
You can select a primary ledger that will be used for payroll costing. The ledger determines the accounting information,
such as, the chart of accounts and the accounting calendar.

Suspense and Default Accounts
You can associate accounts to the payroll definition that will be used by the payroll costing process for suspense and
default accounting purposes.

Number of Years
The number of years you enter represents how many years of time periods to generate starting from the beginning of
the first payroll period, which is determined by the first period end date. This table shows an example for a semimonthly
payroll definition.

Effective Start Date

First Period End Date

Number of Years

Generated Time Periods

01-JAN-2014

15-JUN-2014

5

01-JUN-2014 to 31-MAY-2018

335

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

Once you save a payroll definition, you can later only increase but not reduce its number of years because a calendar of
time periods for the payroll was already generated.

Note:   The application generates the calendar of payroll periods in increments of ten or fewer years. For example,
if you want a 12-year calendar of payroll periods, you first enter 10 years and submit your changes. Then you set the
payroll definition number of years to 12.

Offsets
Depending on the payroll period type, you can elect for your payroll cycle events to occur on specific dates, or to have
the application calculate dates based on offsets from period start or end dates.

This table describes the predefined payroll cycle events that you can offset.

Date

Cutoff Date

Meaning

Final date that payroll information is entered for the payroll period.

This date is for information purposes only. Your departments, such as HR, may need this payroll
deadline to submit information that affects the payroll run

Payslip Availability Date

Date on which payees can view payslips.

Payroll Run Date

Date used by payroll calculation processes to retrieve effective values such as employee details. The
process date, if provided when submitting a payroll process, overrides this value.

This date is predefined for your country or territory and is typically based on either date earned or date
paid that payroll calculation uses as the process date.

Date Earned

Date on which the application processes element entries for the payroll run.

The date earned must be within the effective dates of the payroll period.

Date Paid

Date the employee is marked as paid. For check/cheque payments, this is the date that the check/
cheque is valid for cash or deposit. For electronic funds transfer (EFT) payments, it's the transfer date.

Planned Submission Date

Date to inform the payroll administrator or payroll manager on the planned date to submit the payroll
run for each payroll period.

Dynamic Offsets
When you create a payroll definition, you can use dynamic offsets for payroll cycle events. All of the predefined payroll
time periods you can use support dynamically generated dates for offsets. Use dynamic offsets to offset each payroll
cycle event by a specified number of days before or after the start or end date.

Fixed-Date Offsets
The predefined Monthly (Calendar) payroll time period supports both dynamic offsets and fixed-date offsets. Use fixed
date to adjust the exact date of each of the payroll cycle events for the first payroll period. Any adjustments that you

336

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

make are reflected in the payroll calendar for subsequent payroll time periods. For example, if you set the cutoff date as
the 25th of the month, then all payroll periods in the calendar will have those offsets.

Specific Date Adjustments
Once you generate the payroll time periods, you can further adjust any specific calendar dates, as needed. For example,
if you know of a particular bank holiday that falls on a payment date, you might want to adjust the dates manually on
the payroll calendar's time period. Make these adjustments when you create a payroll definition or any time after then,
as long as the time period is in the future. Adjust the dates of an existing time definition on the Time Periods tab on the
Manage Payroll Definitions page.

Related Topics

• Periodicity Conversion

• Statutory and Earning Periods

• Create Payroll Definitions

Payroll Definitions

Payroll definitions contain calendar and offset information used to determine when you calculate and cost payments.
Payroll period types, such as weekly or monthly, determine the interval at which you pay employees.

Use the Payroll Definitions task to specify payment frequency, processing schedule, and other parameters for a
particular payroll.

Create at least one payroll definition for each payroll period type you use to pay employees. For example, to pay
employees semimonthly, create a payroll definition using the semimonthly payroll period type, ensuring that tax
calculations and other calculations produce correct results for those employees.

Create Payroll Definitions
When you create a payroll definition, the application generates the complete payroll schedule based on the payroll
period type, the offsets or calendar adjustments, and the number of years that you specify. Each payroll in the schedule
is assigned a unique name. Assign employees to payroll definition on the Manage Payroll Relationships page. You can
configure the payroll calendar by increments of ten or fewer years. Create a payroll definition to replace one that expired
or end-dated.

Each payroll must belong to a consolidation group, which the application requires for processing purposes and a
legislative data group so make sure these exist before creating your payroll definition.

Modify Payroll Definitions
When you modify a payroll definition, the application adjusts the payroll schedule based on the values you have
modified. Modify an existing payroll definition to increase the number of years and generate more payroll time periods
that configure the payroll calendar.

Note:  Payroll names in the payroll schedule are unique. You can edit the generated payroll names, but you must
ensure they're unique within the payroll definition.

337

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

Related Topics

• Overview of Payroll Definitions

• Create Payroll Definitions

Create Payroll Definitions

This shows you how to create two payroll definitions for different payment frequencies that are associated with one
consolidation group and one legislative data group.

Watch video

The InFusion Company requires payroll definitions for two sets of employees. A set of permanent salaried employees
paid on a semimonthly basis and a set of temporary employees paid on a monthly basis using time card data. Costing is
managed monthly and uses results from all payroll runs by using the consolidation group name as an input parameter
in the costing run. You can see in this example how to create two payroll definitions with different payment periods
with the same consolidation group. Both definitions are effective starting on 1/1/11 and generate payroll time periods
covering five years.

Prerequisites

1. Ensure that the legislative data group for your payrolls exists, such as InFusion LDG.
2. Ensure that organization payment methods exist for your payrolls, such as InFusion Employee Check/cheque

and InFusion Employee EFT.

3. Create a consolidation group named InFusion Employee Group assigned to the InFusion LDG.

Create Payroll Definitions
Create two payroll definitions:

• One to pay permanent employees on a semimonthly basis. This payroll definition includes dynamically

generated offset dates.

• One to pay temporary employees using time card data on a monthly calendar basis.

Perform the following steps twice, first using the semimonthly values and then using the monthly values.

In the Search Results section of the Payroll Definitions page, click the Create icon.

1. Payroll Definitions task.
2.
3. Select the InFusion LDG legislative data group from the list.
4. Enter 1/1/11 as the effective start date you want the payroll to be available for use, and then click Continue.
In this example, the company hires all employees after the effective start date of this payroll definition, so
there's no issue with loading historical employee data.
In the Basic Details section, complete the fields as shown in this table, and then click Next.

5.

Field

Name

Semimonthly Value

Monthly Value

InFusion Employee Semimonthly

InFusion Employee Monthly

338

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

Field

Semimonthly Value

Monthly Value

Reporting Name

InFusion Semimonthly

InFusion Monthly

Consolidation Group

InFusion Employee Group

InFusion Employee Group

Period Type

Semimonthly

Monthly (Calendar)

First Period End Date

6/15/12

6/30/12

Default Payment Method

InFusion Employee Check/cheque

InFusion Employee Check/cheque

Valid Payment Method

InFusion Employee EFT

InFusion Employee EFT

6. On the Payroll Offsets page, in the Number of Years field, enter 5.

Note:   The application generates the calendar of payroll periods in increments of 10 or fewer years. For
example, if you want a 12-year calendar of payroll periods, you first enter 10 years and submit your changes.
Then you edit the payroll definition, setting the number of years to 12.

7. For the semimonthly payroll, use dynamic variables to define offsets as shown in this table, and then click Next.

Field

Falls Value

Day Type Value

Base Date Value

Cutoff Date

Planned Submission Date

Payroll Run Date

Payslip Availability Date

Date Earned

Date Paid

5

4

0

0

0

0

Before

Before

Before

Before

Before

Before

Period End Date

Period End Date

Period End Date

Period End Date

Period End Date

Period End Date

339

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

8. For the monthly payroll, use fixed dates to define offsets as shown in this table, and then click Next.

Field

Fixed Date

Cutoff Date

Date Earned

Value

Yes

6/25/12

6/28/12

Payroll Run Date

6/28/12

Date Paid

6/28/12

Payslip Availability Date

6/28/12

Planned Submission Date

6/26/12

9. On the Payroll Calendar page, adjust payroll days to account for a bank holiday, as shown in this table.

Column

Semimonthly Value

Monthly Value

Payroll Run Date

Old Value: 11/28/13

Old Value: 5/27/13

New Value: 11/27/13

New Value: 5/28/13

10. Click Next.
11. Review the details of the payroll definition, and then click Submit.

Related Topics

• Payroll Definitions

• Overview of Payroll Definitions

• How Payment Methods and Payroll Definitions Work Together

• Payroll Setup for Costing Accounts

• Overview of Ledger and Subledgers

340

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

Time Card Required Option

If a worker's pay calculations depend on the worker submitting time cards, you must indicate that a time card is required
at the appropriate employment level. Select the Time Card Required checkbox for each assignment level that the
requirement applies.

For example, don't select the Time Card Required checkbox for these scenarios:

• A salaried employee completes project time cards for billing purposes, but isn't paid based upon those time

entries.

• An hourly employee is normally paid based on a predefined work schedule and only submits a time card for

overtime or when absent.

Select the Time Card Required Option
Your role determines where typically you select the Time Card Required checkbox:

• HR specialists can select the checkbox on the Employment Information page of the new hire flow.

• Payroll Managers and Payroll Administrators can select the Payroll Relationship quick action in the My Client
Groups tab. The Payment Details section of the Person Details page includes the Time Card Required checkbox
on the Assignment sections.

This table shows which hours the payroll process uses for elements with a calculation rule of hours multiplied by rate.

Time Card Required

Hours Used in Calculations

Yes

No

Time card entries

Work schedule, unless you enter hours as element entries

Related Topics

• Payroll Elements for Time Card Attributes

• Create Time Card Elements for Time Entries

FAQs for Payroll Definition

Why doesn't my payroll definition appear in search results?
Because you don't have sufficient security access to the payroll definition. Either the payroll security profile associated
with your duty role privileges doesn't include the appropriate payroll definition, or you don't have the View All security
profile.

You must have a privilege that enables you to manage payroll definition data, and your security profile must include the
payroll you want to query. Contact your help desk for assistance.

341

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

Pay Frequency

How Pay Frequency Components Work Together

Pay frequency components provide the flexibility to implement complex time-related objects used in payroll definitions,
payroll processes, and payroll tasks that use start and end dates.

Pay frequency components work together to provide payroll functionality for your organization. Each component
requires its own setup and implementation.

Consolidation Groups
Consolidation groups are used process the results from more than one payroll run in a single action or process the
results for one payroll in separate actions. With consolidation groups, produce one set of results per payment method
for several payrolls, one set of reports, and one set of costing results. For example, you may submit a regular payroll run
and a supplementary payroll run for the same payroll period. If the regular run and supplementary run both belong to
the same consolidation group, use a single consolidation group to process all the results for the post-run processing.
Optionally, you can enter a different consolidation group for the supplementary payroll run and use it to process the
post-run results for the supplementary payroll separately from the regular payroll.

Payroll Definitions
Payroll definitions are essential to your payroll implementation because they indicate the payment frequency and
processing schedule. Payroll definitions associate employees with the payroll run through payroll relationships.

Time Definitions
Time definitions can be static periods of unusual length based on a given static date, or they can create dates based on
dynamic variables. Specify dynamic variables for a time span, a retrieval date, or a more complex definition type for you
to use with a user-defined date. The application uses time definitions in many areas, including payroll periods, payroll
employment management, balance dimensions, retroactive and proration events, element start and end dates, and
overtime periods.

Run Types
Run types control the elements and payment types you process in a payroll run. Two predefined run types, Regular
and Supplemental, group the other run types and determine their processing sequence. The predefined Regular and
Supplemental run types include the two component run types described in this table.

Run Type Component

Description

Process Separately

Generates a separate payroll calculation for each element entry marked to process separately.

After processing separate processes:

•

Includes element run results with normal payroll run results in a single payment.

• Excludes element run results in regular tax calculation on the normal run, for example, to use

supplemental tax rates.

342

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

Run Type Component

Description

Separate Payment

Creates a separate payment for each element entry marked to pay separately.

For each of the component run types, you can specify payment methods that override the default payment methods for
the payroll definition. You can also select the element classifications processed by runs of this type, and exclude specific
elements from these classifications.

Related Topics

• Payroll Definitions

• Examples of Using Consolidation Groups

Statutory and Earning Periods

When you create a payroll definition, a payroll earnings calendar is generated based on the first period end date.

The calendar assigns each payroll period a period name that includes the period number. In some countries, the
statutory tax year doesn't coincide with the dates generated for the earnings calendar. These countries also use a
statutory calendar with statutory period numbers. The statutory calendar ensures that the payroll run uses the correct
period for taxation purposes.

Statutory frequencies are defined in months and weeks, and map to the payroll definition frequencies. For example, a
biweekly calendar is based on a weekly statutory calendar. A quarterly payroll calendar is based on a monthly statutory
calendar. Typically, countries that support semimonthly payroll periods don't use statutory periods.

When you submit a payroll calculation, such as a QuickPay process, you select a payroll period. The calculation uses the
process date for the selected payroll period to identify the statutory period. The process date is the payroll run date on
the payroll definition.

If your country uses a statutory calendar, you can view period numbers, start, and end dates on the Person Process
Results page and statement of earnings.

Related Topics

• How Pay Frequency Components Work Together

• Payroll Definitions

FAQs for Pay Frequency

When would I close a payroll period?
Closing a payroll period can prevent changes to recurring entries. Payroll periods aren't like General Ledger periods.
Closing payroll periods isn't necessary.

343

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

Why can't I find my organization payment method when creating other payroll
objects?
When you update an object's organization payment method, you must make the effective start date of the organization
payment method on or before the effective date of the change.

For example, to create a payroll definition effective on 4/1/2012 with a default organization payment method, the
organization payment method must have an effective start date on or before 4/1/2012. You can only select an
organization payment method that has an effective start date on or before the date you're creating or updating the
object.

Periodicity

Periodicity Conversion

Rate conversion formulas convert amounts to different periodicities for payroll calculations. The following calculations
use rate conversion formulas:

• Proration

• Hours multiplied by rates calculation of an element run result

• Rates based on rate definitions

Predefined Periods
This table lists the predefined periods that you can use to set periodicity.

If these values don't meet your requirements, you can copy a predefined rate conversion formula and edit its periodicity
values.

Periodicity

Annually

Bimonthly

Biweekly

Calendar Monthly

Daily

Hourly

Lunar Month

Valid for Payroll Periods

Number of Periods per Year

Yes

Yes

Yes

Yes

No

No

Yes

1

6

26

12

365

2920 (365 days multiplied by 8 hours)

13

344

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

Valid for Payroll Periods

Number of Periods per Year

Periodicity

Periodically

Quarterly

Semiannually

Semimonthly

Workday

Weekly

Work Hour

No

Yes

Yes

Yes

No

Yes

No

Defining Periodicity
This table lists the different ways in which you can define periodicity:

Object

Elements

Task

Elements

Payrolls

Payroll Definitions

Rates

Rate Definitions

Rate Conversion Formulas
Rate conversion formulas change the periodicity of an amount.

Payroll frequency determines the number of
periods to use in the rate conversion.

4

2

24

260

52

2080 (260 days multiplied by 8 hours)

Description

The Periodicity input value specifies the
frequency of the element value.

For example, salary element entries that hold
annual salary values have an annual periodicity.

Period Type specifies the number of payroll
periods.

For example, the Monthly Lunar period type
includes 13 payroll periods.

Rate definition can specify the following
periodicities:

• Return periodicity of the rate

• Periodicity of each rate contributor

• Periodicity of the calculated sum of the

rate contributors

345

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

For example, the Standard Rate Annualized conversion formula can convert an annual salary amount to a weekly
amount.

This table lists the predefined rate conversion formulas to change the periodicity of an amount.

Rate Conversion Rule

Description

Example

Standard Rate Annualized

Standard Rate Daily

Calculates the annual rate using the input
periodicity and converts the amount to an
output periodicity and rate.

This rule uses default values, such as 2080
hours or 260 working days, to calculate the
annual rate. You select the day or hourly basis
during element definition.

To convert a weekly amount to a semimonthly
periodicity, the formula:

1. Multiplies the weekly amount by 52.

2. Divides the result by 24.

Calculates the daily rate using the input
periodicity and converts the amount to an
output periodicity and rate.

This rule uses a default value, such as 260
working days a year, to calculate the daily rate.

To convert an annual amount to daily
periodicity, the formula:

1. Divides the annual amount by 365.

2. Multiplies the result by the number of days in
the payroll period.

Standard Working Hours Rate Annualized

Uses the employee's standard working hours to
convert the monetary value and working hours
to an annual value before calculating the rate.

The employee works 40 hours a week with a
monthly salary of 1000:

((1000*12)/(40.00*52) = 5.77 an hour

Assignment Working Hours Rate Annualized

Uses the employee's working hours to convert
the monetary value and working hours to an
annual value before calculating the rate.

The employee works 40 hours a week, with 37.5
standard working hours a week, and a monthly
salary of 1000:

((1000*12)/(37.50*52) = 6.15 an hour

Periodic Work Schedule Rate Annualized

Uses the employee's work schedule for the
payroll period for daily and hourly conversions.

For an employee:

• With a monthly salary of 1000

• Assigned a monthly payroll

The formula checks the work schedule details
for the month.

For a daily conversion:

1000 a month/20 days in the month = 50

Note:
For compensation calculations where the
employee isn't assigned a payroll, the rate is
calculated using the weekly rate calculation.
The amount is converted to an annual figure
and divided by the number of days or hours
in that week based on the work schedule.

346

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

The impact of rate conversion rule is summarized here.:

Periodicity: The conversion rule for periodicity applies to Flat Amount, Hours * Rate, and Days * Rate calculation rules.
You can override the periodicity used as the default for the element definition at the element entry level.

Work Units: The Work Units conversion rule applies only to flat amount calculation rules for standard and supplemental
earnings elements. The selection of which work units to use in reports and payslips determines the conversion
calculation. The application creates the element input values using the default values of the rate conversion formulas.

For example, this table illustrates how the payroll process determines the standard work units for any given pay period:

Work Units Selected

Example

Hours

Days

None

2080/24 = 86.67

260/24 = 10.83

No input values are created

Proration: The element template includes a new question for proration units. Proration rate conversion rules replace
the previous proration methods in the element template. You have greater flexibility, for example, to base proration on
calendar days when using work units for conversion.

Note:  If the conversion rules don't meet your requirements, you can copy and edit the rules using the Fast Formulas
task under My Clients Group on your Home page.

Related Topics

• Options to Configure Rate Definitions

• Configure Periodicity Conversion Rules

• Overview of Using Formulas

• Create Conversion Formulas for Proration

Consolidation Groups

Overview of Consolidation Groups

Use consolidation groups to segregate or combine the results of multiple payroll runs for further downstream
processing. You can process the results of more than one payroll run in a single action, or you can process the results of
one payroll in separate actions.

For example, suppose you submit a regular payroll run and a supplementary payroll run for the same payroll period. If
you use the same consolidation group for the regular run and the supplementary run, you can use the combined results
of the regular and supplementary runs for post-run processing. Optionally, you can enter a different consolidation

347

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

group for the supplementary payroll run and use it to process the post-run results for the supplementary payroll
separately from the regular payroll.

Use consolidation groups to segregate and produce one set of results per payment method for several payrolls, one set
of reports, and one set of costing groups. These are runs you make in addition to your regular payroll runs.

A consolidation group is used as an input parameter for a payroll run. There are no predefined consolidation groups.
Before you can use a consolidation group in a payroll run, you must create the consolidation group and assign it to a
payroll definition.

To create a consolidation group:

1. Select the Consolidation Groups quick action under Payroll in My Client Groups on your Home page.
2. On the Consolidation Groups page, click Add Row.
3. Enter a Name for the consolidation group. The application assigns the same value for the consolidation group

Code.

4. Select a Legislative Data Group. Adding the Description is optional, but it's useful to provide
5. Click Save.

Use this consolidation set code to identify the consolidation group used for a payroll run or when you load the
consolidation group using services or the HCM Data Loader.

Once created, you can't change the consolidation set code. However, the consolidation group name is editable. Any
changes made to the consolidation group name, doesn't have any impact on the payroll process, because the process is
stamped with the consolidation set code, and hence can be identified by the code for future references.

Related Topics

• Examples of Using Consolidation Groups

• Overview of Combining Payroll Flows

Examples of Using Consolidation Groups

Here are some examples of how you can use consolidation groups.

Post-Run Processing
Consolidation groups facilitate separating or segregating payroll run results for supplemental processing. For most
payroll post-run processing, you can use the consolidation group as an input parameter. You may want the results
of a supplemental payroll run to be kept separate from those of an already submitted regular payroll run. To use a
consolidation group to keep supplemental run results separate from the regular payroll runs:

1. Create a consolidation group to process the supplemental payroll run.
2.

Initiate the supplemental payroll run, specifying the new consolidation group as an input parameter.

Separate Costing and Payment
You can use multiple consolidation groups to control processing. For example, you want to process and pay a particular
set of employees separately within a single payroll to keep separate records of payment and costing.

348

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

To process employees separately:

Chapter 6
Payroll Definition Details

1. Create payroll relationship groups that restrict the employees.

You can use rules to identify them dynamically or you can specify the employees by their payroll relationship
numbers.

2. Create a consolidation group for each payroll relationship group you have created in the previous step.
3. Run the Calculate Payroll process for each payroll relationship group separately. Specify the new consolidation

group for each run separately.

4. Use the original consolidation group to run the Calculate Payroll process in one single action and return a

consolidated run result for all the employees.

Purposes of Reporting
You can use consolidation groups for reporting purposes. For example, you may want to run the Periodic Payroll Activity
Report for a subset of payrolls.

To process the report for a subset of payrolls:

1. Create a consolidation group to specify the payrolls for which you want to run the report.
2. Run the Periodic Payroll Activity Report, specifying the new consolidation group.

Related Topics

• Consolidation Groups for the US

Time Definitions

Overview of Time Definitions

A time definition is either a date or a span of time. Time definitions can be static periods of unusual length based on a
given static date, or they can generate dates based on dynamic variables.

You can define static definitions using multiple periods, additional adjustments, or both.

This image shows the different types of time definitions and how and where you can use them.

349

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

You can use time definitions in many areas, including payroll periods, payroll employment management, balances,
retroactive and proration events, earnings start date, and overtime periods.

These sections describe the type of time definitions you can create.

Static Time Definition
Static time definitions create recurring patterns of dates, such as overtime periods. For example, a company's overtime
period is a standard five day work week. You can create a static time definition with a weekly frequency that generates
time periods for 3 years. Formulas can use these date patterns to allocate earnings within a payroll period.

User-Defined Date Time Definition
Use user-defined date time definitions to define the last standard process and final close dates of the element entries
for an employee. The last standard process date is the last date on which the element is considered for normal
processing in the payroll run. The final close date is the date from which the element is no longer considered for
processing and thus is no longer date-effective.

For example, Vision Corp provides housing allowance to its employees and wants the allowance to end 30 days after the
employee is terminated. You define a user-defined date time definition based on the last standard earnings date, which
is the termination date plus 30 days.

Time Span Time Definitions
Use time span time definitions to create segments of time that define intervals for scheduled operations, such as payroll
frequency. You can use these time definitions within other time definitions.

A company wants to make employee payments on the last day of the month and third-party payments five days later.
The company creates a time definition of type time span and uses it when defining the payment method for the payee.

Retrieval Date Time Definitions
Retrieval date time definitions are based on balance fetch operations. Anything that exists in the database of Date
format and owned by the payroll application can be used as a trigger.

350

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

Let's assume that the rate contributor for the severance rate definition uses a balance as of termination date. You can
define a retrieval date time definition based on a database item that retrieves the termination date. You can then use
this time definition as the reference date for the balance value in the rate contributor.

Related Topics

• Use Time Definitions for Severance Pay

• How Pay Frequency Components Work Together

• Rate Contributors for Derived Rates

• Example of Loading Time Definitions

Use Time Definitions for Severance Pay

This example illustrates how you can set up a user-defined time definition and as a payroll administrator, how you can
associate it with elements so that you can extend the latest entry date for severance payments to employees.

Scenario
The InFusion Corporation makes severance payments, including regular salary, and car allowance. For most terminated
employees, these payments should end on the termination date. However, you must be able to make payments for
employees who receive severance pay.

Element Duration Dates
When you create an element, you select the latest entry date. The options are predefined time definitions: last standard
earnings date, last standard process date, or final close date. Typically, standard earnings elements use the last standard
earnings date. However, this option doesn't support severance payments because you can't have a last standard
earnings date that's beyond the termination date.

To support severance payments, create a user-defined time definition based on last standard earnings date and select it
as the latest entry date for payments after termination. On the payroll relationship record of terminated employees, the
value of the user-defined time definition is the termination date by default, but payroll administrators can edit it to make
payments for certain employees.

Resulting Setup
To implement a user-defined time definition for this scenario, your implementor must complete the following setup
during implementation:

1. Use the Time Definitions task under Payroll in My Client Groups  on your Home page, to create a time

definition.

This table lists field names and their respective values for creating a user-defined time definition.

Field

Type

Value

User-defined date

351

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

Field

Name

Value

Last Earnings or Severance Date

Short Name

LastEarnSevDate

User-Defined Date

Last Standard Earnings Date

User-Defined Date Usages

Assigned payroll end date

Element entry end date

Payroll assignment end date

Payroll relationship end date

Payroll term end date

This creates a time definition based on the last standard earnings date.

2. Use the Elements task to create the Regular Salary, Car Allowance, and Alimony elements.
3.

In the Durations area, select Last Earnings or Severance Date as the latest entry date for the element.

To extend the payment date for a terminated employee, complete these steps.

1. Use the Payroll Relationships task, and search and select the terminated employee.
2.
3.

In the Payroll Details area, select the assignment.
In the Element Duration Dates area, in the row for the Last Earnings or Severance Date time definition, change
the End Date value to the desired final entry date for payments.

For example, add 6 months of severance pay for an employee who was terminated effective 20 November 2012.
Change the End Date value of the Last Earnings or Severance Date time definition to 21 May 2013.

The employee's element entries for the Regular Salary, Car Allowance, and Alimony elements end on this date.

Related Topics

Run Types

Overview of Run Types

Run types control elements and payment types you process in a payroll run. You may specify default payment methods
to override the default payment methods on the payroll definition.

352

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

Two predefined run types, Regular and Supplemental, group the other run types and determine their processing
sequence.

• The Regular run type includes these run types:

◦ Regular Normal
◦ Process Separately
◦ Separate Payment

• The supplemental run type includes:
◦ Supplemental Normal
◦ Process Separately
◦ Separate Payment

A Separate Payment run type creates a separate payment for each element entry marked to pay separately.

A Process Separately run type generates a separate payroll calculation for each element entry marked to process
separately.

When the separate processes are completed, the element run results are included with the normal payroll run results
in a single payment. You use a separate process to exclude element run results in regular tax calculation on the normal
run, for example, to use supplemental tax rates. It therefore results in a lower rate for the normal run as well as for the
supplemental earnings.

The run types are predefined and you will rarely create additional run types.

Related Topics

• How Pay Frequency Components Work Together

Object Groups

Overview of Object Groups

Object groups are sets of elements or persons. Use object groups to define subsets of objects for processing or
reporting.

Use the Object Group task to define these object group types.

• Element

• Payroll Relationship

• Work Relationship

• Process Information Group

Note:  If you're loading an object group with a large number of inclusions or exclusions, you're recommended to use
the individual Object Group Amend file to achieve that. This supports the data to be multithreaded and minimizes the
processing time.

353

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

Element Groups
Use Element groups to limit the elements processed for payroll, reporting, cost distribution, and for global transfer
purposes.

This table explains the usages for an element group.

Element Group

What It Does

Run group

Specifies the elements to be processed in a payroll run.

Distribution group

Defines the elements on which the cost results are distributed

Configuration group

Restricts the elements that can be updated on the Element Entries page.

All element groups are static. You can select element classification to include in or exclude from the group. You can also
select specific elements to include in or exclude from the group.

Payroll Relationship Groups
Use Payroll relationship groups to limit the persons processed for payroll, data entry, and reporting.

Defining a payroll relationship group is a two-step process.

1. Specify a payroll definition. Every group is limited to the payroll relationships assigned to a single payroll that

you select.

2. Optionally, define the group to be either static or dynamic.

a. To define a static group, select the payroll relationships and assignments to include in or exclude from

the group.

b. To define a dynamic group, use a fast formula of type Payroll Relationship Group. The formula contains
the criteria to establish the payroll relationships and assignments included in the group. Then, you can
individually select additional payroll relationships and assignments to include in or exclude from the
group.

Work Relationship Groups
You can use Work relationship groups to limit the persons processed for Human resources and reporting. For example,
you can use work relationship groups in your user-defined extracts. You can define the group to be either static or
dynamic.

•

•

In a static group, select the work relationships and assignments to include in or exclude from the group.

In a dynamic group,

◦ Use a fast formula of type Work Relationship Group. This formula contains the criteria to establish the

work relationships and assignments included in the group.

◦ Individually select additional work relationships and assignments to include in or exclude from the group.

354

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

Process Information Groups
You use a bank reprocessing group to load the bank corrections file returned by your bank. Each payroll period, you
transfer payroll payments directly into the bank accounts designated by the employee. If any of the bank account
records are invalid, your bank returns a file containing these details.

For example, an employee can have an incorrect account number which results in the payment being rejected by the
bank. Alternatively, the payment could have been transferred to an invalid branch number due to the closure of a bank
or merger of a bank branch with another.

Related Topics

• Overview of Loading Object Groups

• Example of Loading Object Groups

• Set Up Distributed Costing for an Element

Process Information Group Security

Use the View Process Information Group Quick Action to create a bank correction group. You use a bank correction
group to load the bank corrections file returned by your bank.

You can use either of these navigation paths to access the View Process Information Groups Quick Action from your
Home page and create a Bank Correction group:

• My Client Groups > Show More > View Process Information Groups under Payroll

• My Client Groups > Payroll > View Process Information Groups

The View Process Information Groups Quick Action task provides access only to the Bank Correction groups. When you
use this task to create a Bank Correction group, you first search for a person and then create the group in the context of
the assignment of the person.

Note:  You must use the PAY_RESPONSIVE_PERSON_SEARCH_CLASSIC_ENABLED profile option to enable
Responsive Person Search on this Quick Action.

Before you use this Quick Action task, secure the View Process Information Groups Quick Action task and the
predefined roles that inherit it, using the following aggregate role privileges:

• Aggregate Role: Manage Process Information Group

(ORA_PAY_MANAGE_PROCESS_INFORMATION_GROUP)

• Function Privilege: Manage Process Information Group

PAY_MANAGE_PROCESS_INFORMATION_GROUP

• Data Privilege: Manage Process Information Group Data

PAY_MANAGE_PROCESS_INFORMATION_GROUP_DATA

Update the function and data security to use this aggregate privilege. The aggregate privilege provides restriction for
users to access person data based on their data security profiles.

355

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 6
Payroll Definition Details

If you're using the predefined roles of Payroll Manager and Payroll Administrator, no action is necessary. However,
if you're using a user-defined version of these roles, you must ensure that the defined job roles have this aggregate
privilege:

• Manage Process Information Group

(ORA_PAY_MANAGE_PROCESS_INFORMATION_GROUP)

Note:  You can also use the Object Groups task to create a Process Information Group object group. However you
don't need this aggregate role privileges to use this task because you create the object group for an LDG and not in
the context of a person.

Related Topics

• Overview of Object Groups

Create an Element Object Group

In this example, you create an element object group.

Watch video

In the Create Object Groups dialog box, Name field, enter Element Group.
In the Legislative Data Group field, select US Legislative Data Group.
In the Type field, select Element Group.

1. On the Object Groups page in the Search Results section, click Create.
2.
3.
4.
5. Click Continue.
6. On the Create Object Group page, in the Basic Data section for the Start Date field, enter 1/1/2016.
7. For the End Date field, enter 12/31/2018.
8. Select the object group parameter.

◦ In the Object Group Parameters section, in the Value column, click Search.
◦ In the Object Group Parameters  field, enter %.
◦ Click Search.

Note:  For element groups, the usage type can be a run group, distribution group, or configuration
group. This element group will be used to specify the elements to be entered in batch loader.

◦ Click Distribution Group.

Note:  This element group will include all elements in the Standard Earnings classification, with the
exception of Shift. Also, you must add federal taxes to be included.

9. Click Next.

356

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

7  Payroll Balances

Balance Definitions

Overview of Payroll Balance Definitions

A balance is a positive or negative accumulation of payroll results for an element or group of elements, over a specified
period of time.

The balance can be monetary values, time element, such as hours or days worked, or any other numeric value. Every
time you run a payroll process, such as, Calculate Payroll or Calculate Gross Earnings, the application updates these
values.

Each defined balance holds a value for an individual at one of the two levels of the employment model.

• Payroll relationship

• Assignment

Most of the balances you require are predefined. Depending on your country extension, additional balances are
automatically created when you create elements. You can edit the definition of these generated balances, or create
additional balances.

For example, the Employer Contributions amount on the Statement of Earnings is fed by elements with a classification
of Employer Taxes or Employer Liabilities. Similarly, an employee's Taxable Benefits is fed by elements with a
classification of Taxable Benefits.

Balance Name
It's the actual name of the balance, such as, Regular Earnings. You can't have the same name for more than one balance.
However, more than one balance can have the same reporting name.

A reporting name is the balance name that reports and payslips display. When multiple balances are created due to
differences in setup but need to be reported the same way, you can assign the same reporting name for all of the
balances.

Balance Categories
Each balance definition has a predefined balance category for quicker processing. Balance categories are a way of
grouping balances so that you can set group attributes. Balance categories are predefined, and you can't create your
own balance categories or modify the balance categories. When you create a balance during the implementation phase,
associate it to one of the predefined categories.

You can however, create your own localized version of the balance categories you want to use. In the Setup and
Maintenance area, use the Configure Payroll Legislations task to view the predefined balance categories. Edit the
balance category name to include a display name appropriate for your legislation.

357

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

Units of Measure
When you create a balance, the predefined units of measure available for selection are Day, Hour (with different
combinations of minutes and seconds), Integer, Money, and Number. Match the unit of measure of the balance with the
unit of measure of the element input values that feed it.

Balance Contexts
Contexts restrict the run results included in a balance value. Context values are specified as part of the balance
dimensions. For example, the REGULAR_ASG_TU_YTD balance is a Regular Earnings balance type with these context
values associated in the balance dimension:

• Assignment

• Tax Reporting Unit

All contexts are predefined.

Generated Balances and Database Items
The country extension you select on the Features by Country or Territory page, determines what payroll-related
components the element template generates when you create an element. The element template also creates a
database item for each balance dimension. You can use the database items in your formulas or HCM extracts to use the
value of a balance.

This table explains the components the element template creates, based on your selection of the country extension.

Country Extension

Components Generated by the Element Template

Payroll

Payroll Interface

When you create an element, the element template creates the element and associated objects, such
as input values, formulas, and balances.

When you create regular and supplemental earnings elements, the element template creates the
element and associated objects, such as input values, formulas, and balances. For all other elements,
 the template generates no other associated objects.

Human Resources or None

The element template doesn't generate associated objects like formulas, or balances.

Base Balances
You can specify a base balance when there is a dependent relationship between balances for processing and reporting.
For example, Taxable Wages could be the base balance for Tax Withheld.

Remuneration
Only one balance in each legislation is predefined as the remuneration balance. This balance generates payments
for employees and is predefined for the legislation. For example, a legislation might use Net Pay as the remuneration
balance. This calculated balance is the sum of standard earnings and supplemental earnings minus all the deductions
calculated for the run.

358

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Related Topics

• Balance Dimensions

Balance Dimensions

Chapter 7
Payroll Balances

Balance dimensions identify the specific value of a balance at a particular point in time. Balance dimensions are
predefined and typically combine these components:

• Time span, such as run, period-to-date, or fiscal year-to-date

• Employment relationship level, either assignment or payroll relationship

• Context, required for some balances only, such as tax reporting unit, state, or payroll

For example, if you select the Core Assignment Tax Unit Year-to-Date dimension for the Gross Earnings balance, you
create the defined balance GROSS_EARNINGS_ASG_TU_YTD. This defined balance accumulates gross earnings for an
assignment in a specific tax reporting unit from the beginning of the calendar year-to-date.

Optionally, they can also include other context values such as tax reporting unit, tax jurisdiction, and deduction
reference number.

Each payroll balance can have multiple dimensions.

Balance Feeds

The value assigned to a balance during processing is determined by the feeds defined for the balance. You can feed
payroll balances by any of these options.

Balance Feeds by Element
Balance feeds by element indicates the following:

• When you create an element, the element template creates this balance and feed automatically.

• One or more element input values add to or subtract from a balance.

• For each balance, all the input values must have the same unit of measure.

•

If a balance is fed by only one element, it's called a primary balance.

Balance Feeds by Classification
Balance feeds by classification indicates the following:

• The primary output value of every element belonging to a specific classification contributes to the balance

value.

• The balance feeds can be from the primary element classifications, secondary element classifications, or the

subclassifications.

•

If you add a primary classification as a balance feed, you can't add its children from the secondary classification
or subclassifications.

359

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

For example, if you use the Supplemental Earnings primary classification as a balance feed, you can't use both
the secondary classifications and subclassifications of Supplemental Earnings as feeds to the same balance.

• The unit of measure of this input value must match the unit of measure of the balance.

Balance Feeds for Initial Balance Loading
You can select elements in the Balance Initialization classification to feed a balance for initialization purposes only.
Select one element for each level of the employment hierarchy associated with a dimension that you want to initialize.

The feeds can add to (+) or subtract from (-) a balance. The sign of a feed is independent of the sign of the result that
feeds the balance. For example, deductions feed Net Pay with a negative feed. However, if an excess deduction of $100
is returned, the deduction result itself is -$100 and will effectively increase Net Pay by $100.

Related Topics

Primary Balances

When you create an element, the element template creates a balance with a primary feed from the element to
accumulate its run results. This is the primary balance for that element.

There are rules that govern primary balances and the input values that feed the balances.

For example, let's assume that Vision Corp has the following defined elements and balances that these elements feed
into:

• A Bonus element that generates the Earnings Calculated input value for the Bonus balance. The primary feed

for this balance is the Bonus element.

• A Festival Bonus element that's the primary feed for the Festival Bonus balance.

• Both the Bonus element and the Festival Bonus element also feed the Discretionary Earnings balance. These

are non-primary feeds.

Normally, a primary balance is only fed by a single input value as it's exclusive to an element. But there are exceptions to
this rule. In the above example, let's say a few years later, Vision Corp has a revised compensation policy and defines the
additional Bonus_v2 element to include additional input values for sales incentives. The Bonus_v2 element should feed
into the same Bonus balance.

The Bonus balance has these two feeds now:

• From the Bonus element, which is the primary feed.

• From the Bonus_v2 element to take care of sales incentives. This is a non-primary feed.

This table explains the rules for the primary balances and the input values that feed the generated balances, for this
example.

Rule

In this example

A primary balance can have only one
primary balance feed.

The primary balance Bonus can only have a primary feed from the Bonus element, and therefore can't
have a primary feed from the Bonus_v2 element.

360

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

Rule

In this example

A primary balance can have a non-primary
feed from a different input value, as long
as that input value doesn't feed any other
primary balance.

Since Bonus_v2 element is assigned as a non-primary feed to primary balance Bonus, it can't have its
own primary balance.

An input value can feed only one primary
balance.

Since Bonus and Bonus_v2 elements feed a primary balance, example Bonus balance, it can't feed
any other primary balance, say Festival Bonus. However, they can feed a non-primary balance like
Discretionary Earnings.

Balances in Net-to-Gross Calculations

When you create an earnings element, you can indicate that it pays a person a guaranteed take-home net pay per
payroll period, or a bonus of a specified net amount.

Use either or both of these options to control balance feeds.

Enable Inclusion in Net-to-Gross Calculations
Use the Balance Definitions task to view the dimensions that are enabled for inclusion in net-to-gross calculations. You
can also view which of the enabled dimensions are included by default for each new net-to-gross earnings element.

To enable a dimension, or enable and include a dimension within a balance definition for net-to-gross processing, select
the Enable or Include check boxes, as required, under the Gross-Up Calculation column in the Balance Dimensions
section of the Balance Definition page.

Exclude Balances from a Specific Net-to-Gross Earnings Element
If a balance is enabled but not included, you can still use it in the processing of a specific net-to-gross earnings element.
Use Balance Feeds on the Elements Overview page while creating the Gross-to-Net Earnings element and review
the balances to which the net pay amount or bonus contributes. Use the Gross Balance Exclusions option to add the
balance. You can also use this task to exclude balances that are included by default.

Related Topics

• How Net-to-Gross Earnings are Calculated

• Create a Net-to-Gross Earnings Element

Generate Run Balances

The payroll calculation process generates run results and values for all balances. Creating or updating balance
definitions and balance feeds can impact balance calculations and also the stored balance values for run balance
dimensions.

When stored balance values are no longer accurate, the Run Balance Status column on the Balance Definitions task
displays the status of the balance dimensions as invalid. Reports and processes continue to obtain accurate values from
the summed run results, but summing run results can slow performance.

361

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

To improve performance and accuracy, recalculate the invalid balance values for saved run balance dimensions by
submitting the Generate Run Balances process.

This topic covers:

• Submit the Generate Run Balances process

• Use Generating Run Balances Examples

Submit the Generate Run Balances Process
Submit the Generate Run Balances process before you submit the payroll run or after you create or update these tasks:

• Balance definition using the Balance Definitions task, for example to add balance feeds or new balance

dimensions

• Balance feeds to an element using the Elements task

When you submit the process, you specify parameters that control which balances to generate as shown in the following
table.

Flow Submission Parameters

Purpose

Balances to Include

Identifies the set of balances to include when submitting the process:

• All balances

• All invalid balances

• Single balance

Note:
If you select a single balance, you must specify both a balance and a dimension name.

Balance Name

Lists balance names marked as run balances when a single balance is selected.

Dimension Name

Lists run dimensions when a single balance is selected. The list is filtered again when the balance name
is selected.

Use Generating Run Balances Examples
Here are two different ways you can use generate run balances to improve performance and accuracy in your payroll
application.

• Updating a balance feed effective date

Your enterprise stops the transportation allowance element as of January 1. This ends the balance feeds
between the element input value and the related balances, such as gross-to-net. It also sets the status of
the balance values for completed payroll runs to invalid. You submit the Generate Run Balance process to
recalculate the balance values and set the status to valid.

362

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

• Adding a new balance feed

Chapter 7
Payroll Balances

You receive a notification on January 31 that a non-taxable earning became taxable as of January 1. You add
a balance feed to the earnings element so that the input value feeds a taxable pay balance. You submit the
Generate Run Balances process and recalculate the balance values for the taxable pay balance.

Related Topics

• Payroll Balance Definitions

Automate Generate Run Balances

Enable automatic generation of run balances so that when you make changes to a balance feed it automatically initiates
the Generate Run Balances flow.

As a result, the payroll run results and payroll reports will always display the correct and updated run balance values.

You can now automatically recalculate any run balance dimension values. Creating or updating balance definitions and
balance feeds can impact balance calculations and stored balance values for run balance dimensions. The Generate
Run Balances process recalculates any invalid balance values for saved run balance dimensions thereby improving the
performance and accuracy of payroll calculations.

The Generate Run Balances flow generates run balances for the Balance Type ID of the balance for which you have
made changes.

Note:  Generation of run balances will be submitted for the same legislative data group for which the balance feed
changes belong to. Create an event group and associate it to an event action that automatically runs the Generate Run
Balances flow when you make changes to a balance feed.

1.

2.

3.

4.

5.

Create an event action using HCM Data Loader.

Create an event group to identify the type of changes to be monitored. You recalculate stored run balance
values for a single balance type, all balances, or all invalid balances.

Associate the event group to an event action that automatically runs the Generate Run Balances flow when
you make changes to a balance feed.

Use HCM Data Loader to load an event action. Load the Event Action.dat file and the Event.Group.dat files.

Once you load the files successfully, you can view the created Event Action and Event Group from the Event
Action Groups page. Now when the Balance Feed change happens, based on the Loader setup, the Generate
Run Balances flow is automatically submitted.

Event Group and Event Action for Recalculation of Run Balances

This topic shows how you can create an event group and associate it to an event action to recalculate run balances.

When you create or update a balance definition or feed, you must consider if the change impacts future payroll
calculations and reports only, or if there's a requirement to recalculate the balances retrospectively.

363

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

If you need to recalculate the balance amounts, such as the retropay calculations, you've the option to run the Generate
Run Balances process. The Generate Run Balances process ensures that the retrospective balance change doesn't cause
performance issues.

Use event groups to identify the type of changes that require the Generate Run Balances process to be submitted
automatically.

Let’s consider an example where you want to track balance definitions and balance feed changes impact balance
calculations and stored balance values for run balance dimensions.

When an event in your group is triggered, a balance change event notification is triggered so that the Generate Run
Balances process is automatically submitted.

This example EventGroup.dat file creates a single Event Group component and associates it to the Event Action. For the
Generate Run Balances calculations, the EventGroupType attribute value must be A.

Create Event Action Group

METADATA|EventAction|FLEX:PAY_EVENT_ACTIONS_DDF|BaseFlowName(PAY_EVENT_ACTIONS_DDF=ORA_PAY_SUBMIT_FLOW_ACTION)|

FlowInstanceName(PAY_EVENT_ACTIONS_DDF=ORA_PAY_SUBMIT_FLOW_ACTION)|

FlowParameterNameOne(PAY_EVENT_ACTIONS_DDF=ORA_PAY_SUBMIT_FLOW_ACTION)|

FlowParameterValueOne(PAY_EVENT_ACTIONS_DDF=ORA_PAY_SUBMIT_FLOW_ACTION)|

FlowParameterNameTwo(PAY_EVENT_ACTIONS_DDF=ORA_PAY_SUBMIT_FLOW_ACTION)|

FlowParameterValueTwo(PAY_EVENT_ACTIONS_DDF=ORA_PAY_SUBMIT_FLOW_ACTION)|

FlowParameterNameThree(PAY_EVENT_ACTIONS_DDF=ORA_PAY_SUBMIT_FLOW_ACTION)|

FlowParameterValueThree(PAY_EVENT_ACTIONS_DDF=ORA_PAY_SUBMIT_FLOW_ACTION)|

ScheduleSkip(PAY_EVENT_ACTIONS_DDF=ORA_PAY_SUBMIT_FLOW_ACTION)|

ScheduleInterval(PAY_EVENT_ACTIONS_DDF=ORA_PAY_SUBMIT_FLOW_ACTION)|EventActionName|EventActionCode|

EffectiveStartDate|EffectiveEndDate|EventActionTypeCode|ActionSubmission|LegislativeDataGroupName

MERGEIEventAction|ORA_PAY_SUBMIT_FLOW_ACTION|Generate Run Balances|NK THREAD_{FLOW_NAME}|Legislative Data Group

Identifier|{LEGISLATIVEDATAGROUP_ID}|Process End Date|{SYSTEM_DATE}|Balances To Include|ORA_PAY_ALL_INVALID_BAL|

N||NK_EA_CRFL_3|1950/01/4712/12/31|ORA_PAY_SUBMIT_FLOW_ACTION|SYNC|CRFL RRF LDG US1

Create Event Group

METADATA|EventGroup|EventGroupCode|EventGroupName|EventGroupType|LegislativeDataGroupId|LegislativeDataGroupName

MERGE|EventGroup|NK_EG_CRFL_3|NK_EG_CRFL_3|A||CRFL RRF LDG US1

Indicate the type of events within the Event Group

METADATA|DateTrackedEvent|ColumnName|UpdateType|LegislativeDataGroupId|EventGroupCode|DatedObjectName|

LegislativeDataGroupName

MERGE|DateTrackedEvent||DT_INSERT||NK_EG_CRFL_3|

oracle.apps.hcm.payrolls.balances.setup.protectedModel.entity.BalanceFeedDEO|CRFL RRF LDG US1

MERGE|DateTrackedEvent||DT_ZAP||NK_EG_CRFL_3|

oracle.apps.hcm.payrolls.balances.setup.protectedModel.entity.BalanceFeedDEO|CRFL RRF LDG US1

MERGE|DateTrackedEvent|SCALE|DT_CORRECTION||NK_EG_CRFL_3|

oracle.apps.hcm.payrolls.balances.setup.protectedModel.entity.BalanceFeedDEO|
CRFL RRF LDG US1s MERGE|DateTrackedEvent|SCALE|DT_UPDATE_COLUMN||NK_EG_CRFL_3|
oracle.apps.hcm.payrolls.balances.setup.protectedModel.entity.BalanceFeedDEO|CRFL RRF LDG US1

Associate your Event Action to the Event Group

364

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

METADATA|EventGroupAction|EventActionCode|EffectiveStartDate|EffectiveEndDate|EventGroupCode|

LegislativeDataGroupName

MERGE|EventGroupAction|NK_EA_CRFL_3|1950/01/01|4712/12/31|NK_EG_CRFL_3|CRFL RRF LDG US1

Balance Groups and Usages

Balance Groups

Balance groups represent a collection of balance definitions, including their dimensions that you can use to retrieve
balance values for reports, archives, and balance views. Balance group usages determine which reports, pages, and
processes use the group to display or process balance information.

Use the Balance Groups task to manage your balance groups.

Balance Group Level
You can define a balance group at the employee or organization level. The balance group level determines the group
level at which you can include the balance dimensions.

Employee level applies to balances at a payroll relationship level or lower. Organization level or Group level applies to
any dimensions higher than the payroll relationship level, including Group Person dimensions.

Balance Definitions
On the Balance Definitions page of a balance group, you can see the balances associated with the balance group. The
information includes the balance name, balance dimension, balance category, unit of measurement, and legislative
data group. A balance category groups together similar balances. It is similar to the element classifications, for each
element classification there is a corresponding balance category. You can also use this page to search for and add
balance definitions to your own balance groups and to certain predefined balance groups.

Use Select and Add to add multiple balance definitions at a time.

Tip:  You can select multiple balance definitions in the Select and Add window. Hold down the Shift key to select a
group of consecutive balance definitions. To select individual balance definitions hold down the Control key and select
the balance definitions that you want to add to the balance group. Click Apply and keep the dialog window open to
add the query to search the selected balance definitions . Click OK to add the selected balance definitions and close
the dialog window.

Restrictions
Restrictions limit the balances that you can add to the balance group. You can add a list of balance categories, a list of
balance dimensions, or a combination of balance categories and dimensions.

The Included Balances Restricted by Category and the Included Balances Restricted by Dimension check boxes are
automatically updated on the Balance Group Details page as you add restrictions on the Restrictions page. For example,
the standard earnings category means that the balance group is restricted to all balances based on the standard
earnings category.

365

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

You can also define a balance group without any restrictions.

Note:  In some situations you can update a restriction if it's not used by balance definitions and default inclusions.
The Edit button on the Restriction page is enabled if the selected row can be updated. A balance group may be
defined without restrictions.

Default Inclusions
Default inclusions are combinations of balance categories and dimensions that are automatically added to the balance
group. This means that any balance definition you define (manually or through the element template), or existing
already for the specified category and attached to the specified dimension, is included in the balance group by default.
However, if you need to include any other balance definition outside of those in the Default Inclusions, you must
manually add the defined balance to the balance group.

Balance Group Usages

Balance group usages represent an instance of how a particular balance group is used.

A balance group must have at least one usage. The usage can be a report, process, or page that uses the balance values
from the group. The group can also many balance group usages.

Balance group usages store detailed info about how the balance data is formatted and sequenced. Payroll reports use
balance groups to determine the balances to include in specific sections of the report.

Use the Balance Group Usages task to manage your balance group usages.

Matrix and Table Formats
A balance group usage can use a matrix or table format to display the balance dimensions. You choose the option when
you create the balance group usage.

For a matrix format, you select balance dimensions as columns in the matrix and decide their position in the matrix
using Position. The first position must be 1, and any additional positions must be sequential. It displays only the balance
dimensions that you select as columns for the matrix. If you don't specify the balance dimensions as matrix items, they
don't display, regardless of what dimensions the defined balances in the balance group contain.

Sorting
Sorting determines the order in which balance types and dimensions display for the balance group usage. If you select
Table, it returns all balances in the balance group one line at a time in the table format. If you select Matrix, you can add
balance dimensions and decide their positions in the matrix.

This table shows the options you can use to define your sorting order.

Field

Values

Sort Method

Select one of these options:

• Name, to sort by balance name.

• Value, to sort by balance value.

366

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Field

Values

Chapter 7
Payroll Balances

• Static Order, to sort by the sequence you specify in the Sort Items table.

You can also create a static order by selecting the balance name and sequence in Sort Items. For example, you can sort
the summary balances for the gross-to-net report type in the processing order rather than the alphabetic order. Here's
an example of a static order of the Gross to Net summary balances for the Statement of Earnings. The balances shown
here are sorted in the order of Gross to Net Calculation.

• Gross Pay

• Pretax Deductions

• Employee Tax Deductions

•

Involuntary Deductions

• Voluntary Deductions

• Nonpayroll Payments

• Net Payment

Examples

Report type

What balance dimensions they use

Global Archive

Archive of current and year-to-date tax code balances for areas 1, 2, and 3

Global Balance Views

Earnings default balances for the Balance Views page

Global Deduction

Balances for involuntary, pre-statutory, social insurance, and tax deductions

Global Element Results

Nonpayroll payment tax balances at the assignment and relationship levels

Global End-of-Year Archive

Payroll Relationship level balances

Global Payroll Activity Report

Earnings balances at the payroll relationship level for the current payroll period and year-to-date

Global Payroll Run Result Report

Balances for all earnings at the assignment and relationship levels

Global Statutory Deductions Report

All city, county, state, and school tax deduction balances for the current period and year-to-date

Global Gross-to-Net

Direct payment balances for a group tax unit for the current period and year-to-date

Statement of Earnings

City, county, and state pretax deductions for the current payroll period and year-to-date

367

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

Related Topics

• Balance Groups

• Payroll Balance Definitions

• Create Balance Groups and Usages

Create Balance Groups and Usages

This example demonstrates how to create a balance group and balance group usage for a user-defined report of
voluntary deductions.

Before You Begin
If you're creating a user-defined report, create a lookup code for the report in the PAY_BALANCE_REPORT_TYPE
lookup.

In the Setup and Maintenance work area, go to the Manage Common Lookups task.

1.
2. Search for and select the PAY_BALANCE_REPORT_TYPE lookup type.
3. Add the lookup code, meaning, and description for the user-defined report in the Lookup Codes section.

How to Create a Balance Group
To create a balance group:

1. On the Home page, click the Balance Groups quick action under the My Client Groups tab.
2. Click Create to open the Create Balance Group dialog box.
3. Select a legislative data group and enter a name for the balance group.
4. Click Continue.

The Balance Group Details page displays.
5. Select Employee as the balance group level.
6. Click Save.
7. Select the Balance Definitions folder under the Balance Group Overview list.
8. Click Select and Add.
9.

In the Select and Add: Balance Definitions dialog box, enter these values.

Field

Value

Dimension Name

Relationship Run

Category

Voluntary Deductions

10. Click Search.

368

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

11.

In the Results section, select the balance definitions that you want to add and then click OK.

Tip:  You can select multiple balance definitions in the Select and Add window. Hold down the Shift key to
select a group of consecutive balance definitions. To select individual balance definitions hold down the
Control key and select the balance definitions that you want to add to the balance group. Click Apply and
keep the dialog window open to add the query to search the selected balance definitions . Click OK to add the
selected balance definitions and close the dialog window.

12. Click Submit.
13. Click Done.

How to Create a Balance Group Usage
To create a balance group usage:

1. On the Home page, click the Balance Groups quick action under the My Client Groups tab.
2. Click Create .
3.

In the Create Balance Group Usage dialog box, complete the fields as shown in this table.

Field

Value

Legislative data group

Enter the same LDG as the balance group for which you're creating the usage.

Name

Employee voluntary deduction run balances

Balance Group

The group you created in the previous task

Format Type

Table

4. Click Continue.

You're returned to the Balance Group Usage Details page.

5. Select the report type (this was the report type that you added as a lookup code to the

PAY_BALANCE_REPORT_TYPE lookup).

6. Click Save.
7. Select the Sorting folder under Balance Group Usage Overview list.
8. From the Actions drop down list on the right, select Create.
9. Enter these details.

Field

Name

Sort Method

Value

Any

Name

Sort By

Balance Type

369

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

Field

Order

10. Click Save.
11. Click Done.

Value

Ascending

Examples of Balance Group Usages

Add matrix items to predefined balance group usages and associate them with existing balance groups for use in
reports, archives, and views. While you can't modify existing usages that are predefined, you can modify matrix items
that are user-defined.

You can include balance dimensions for multiple time periods in your balance group usage, such as the current payroll
run, month-to-date, or year-to-date.

Balance group usages are used to display balance values. You select the usage associated with the balance group.
Additionally, you can sequence balances using balance group usages to display in a certain sequence, which may not
necessarily be a standard sort sequence.

Here is a list of the predefined report types and the different kinds of balance dimensions they use.

Note:  The report type is the owner of the balance group usage. A usage can have only one report type

Report Type

Global Archive

Global Balance Views

Used in Which Reports

Balances Included

Payroll Register Report, Payslip, Payslip
Reprinting Report, Payroll Register for the
Latest Process

Archive of current and year-to-date balances

Earnings default balances for the Balance
Results page

Balances for involuntary, prestatutory, social
insurance, and tax deductions

Global Deduction

Deduction Report

Global End of Year Archive

Archive End-of-Year Payroll Results

Payroll Relationship level balances required for
End-of-Year Statutory reporting

Global Payroll Activity Report

Payroll Activity Report, Employee Active Payroll
Balance Report, Payroll Activity Report for the
Latest Process

Balances at the payroll relationship level for the
current payroll period and year-to-date

Global Payroll Run Result Report

Payroll Balance Report

Current balances at the assignment and
relationship levels

370

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

Report Type

Used in Which Reports

Balances Included

All city, county, state, federal, and school tax
deduction balances for both the employee and
employer in the current period and year-to-date

Summary balances for a group tax unit for the
current period and year-to-date in the order of
gross-to-net calculation.

Summary and detailed balances for a specific
employee and payroll run.

Global Statutory Deductions Report

Statutory Deductions Register

Global Gross-to-Net

Gross-to-Net Report

Statement of Earnings

Statement of Earnings

Scenario

Related Topics

• Rules for Editing Balance Groups and Their Usages

• Balance Groups

• Balance Group Usages

• Create Balance Groups and Usages

Rules for Editing Balance Groups and Their Usages

The limitations on the changes you can make to balance groups and usages are different for predefined and user-
defined groups.

Balance Group Rules
These are the actions you can take for both predefined and user-defined balance groups.

Action

Predefined Balance Group

User-Defined Balance Group

Create balance group

Edit balance group

Delete balance group

Add balance definitions

No

No

No

No, unless the Add button in the table menu is
enabled

Yes

Yes

Yes

Yes

Remove balance definitions

No, unless the balance definitions are added by
the user.

Yes

371

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

Action

Add restrictions

Edit restrictions

Delete restrictions

Edit the balance group level

Predefined Balance Group

User-Defined Balance Group

No

No

No

No

Yes

No

Yes

Yes, if the group contains no balance
definitions, default inclusions or dimension
restrictions.

Add default inclusions

No, unless the Add button in the table menu is
enabled

Yes

Edit default inclusions

Delete default inclusions

No

No

Yes

Yes

Balance Groups Usage Rules
The only change you can make to a predefined balance group usage is to add matrix items.

For a user-defined usage, you can:

• Edit or delete the usage

• Edit the usage details

• Add or delete matrix items

• Create, edit, or delete sorting definitions

CAUTION:  You can't change the format type of a usage after you save it. Additionally, you can't change the sort
method unless you delete the existing sort items.

Balance Exceptions

Overview of Balance Exceptions

Balance exceptions define the criteria you use to identify overpayments, underpayments, and trends. The variance may
also be a result of incorrect setup or adjustment.

Create a balance exception and the Balance Exception Report, and then run the Balance Exception Report. Run the
report to generate a report output that displays payroll balance results as per the defined exception criteria. This
information helps you detect the balance adjustments needed to correct payments or correct the balance setup.

372

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

Use the Balance Exceptions task to create a balance exception and consider these components when you create a
balance exception.

Comparison Types
When you're creating balance exceptions, select a comparison type. Comparison types define the period that you use to
determine whether an exception has occurred. For example, select Average in months as the comparison type and enter
3 in the Comparison Value field. In this scenario, the current month value is compared to the average of the previous
three months.

Some comparison values are preset and you can't change them:

• Current month, Current period, Current quarter, and Current year always have a comparison value of 0.

• Previous period and Previous month have a comparison value of 1.

This table lists each comparison type that you can select and explains how it operates as a basis of comparison.

Comparison Type

How it Operates as a Basis of Comparison

Average in months

Compares the current month to date balance with the average of previous months to date. Only
available if you have a Month to Date balance dimension for assignment or payroll relationship.

Current month

Current period

Current quarter

Current year

Previous month

Previous period

Compares values to the total for the current month to date balance. Doesn't use any previous month as
a basis for comparison. Only available if you have a Month to Date balance dimension for assignment
or payroll relationship.

Compares values to the total for the current period to date. Doesn't use any previous period as a basis
for comparison. Only available if you have a Period to Date balance dimension for assignment or
payroll relationship.

Compares values to the total for the current quarter to date. Doesn't use any previous period as a basis
for comparison. Only available if you have a Quarter to Date balance dimension for assignment or
payroll relationship.

Compares values to the total for the current year to date. Doesn't use any previous period as a basis
for comparison. Only available if you have a Year to Date balance dimension for assignment or payroll
relationship.

Uses the previous month as a basis of comparison. Only available if you have a Month to Date balance
dimension for assignment or payroll relationship.

Uses the previous period as a basis of comparison. Only available if you have a Period to Date balance
dimension for assignment or payroll relationship.

Note:   Comparison Value  field is shown for Average in Months. It is hidden for other comparison types.

If you select a Comparison Type of Average in months, you must enter a Comparison Value to determine the number of
months that are averaged for the comparison.

373

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

Variance Operators
Variance operators enable you to specify the precise range of variance that you want to report on.

For example, you want to determine the monthly car allowance paid to employees in excess of 600 more than the
previous month for the same payroll relationship. You can setup a balance exception for this example using these
values:

• Comparison type is previous month

• Balance name is monthly car allowance

• Dimension name is relationship month to date

• Previous month amount is 500

• Variance value is 100

This table describes the effect of using each of the variance operators for balance exception reporting. The Results
column indicates the effect of selecting each variance operator.

Variance Operator

Balance Exception Report Output

Results (based on sample data)

Variance, plus or minus

Note:
This operator applies only for comparison
types of 'Previous', like Previous Months
or Previous Period, as well as 'Average in
Months'.

All relationships whose balance value either
exceeds or are less than the previous month
amount by the amount or percentage stated in
the variance value.

Returns all relationships with a value less than
or equal to 400 and greater than or equal to
600.

Less than

Less than or equal

Equal

Greater than

Greater than or equal

All relationships that are less than the previous
month amount by the amount or percentage
stated in the variance value.

Returns all relationships with a value of less
than 400.

All relationships with a current value either
equal to or less than the previous month
amount by the amount or percentage stated in
the variance value.

Returns all relationships with a value of 400 or
less.

All values that are exactly equal to the higher
limit or the lower limit of the variance value.

Returns all relationships with a current value
equal to 400 or 600.

All relationships that are greater than the
previous month amount by the amount or
percentage stated in the variance value.

Returns all relationships with a value of more
than 600.

All relationships with a current value either
equal to or greater than the previous month
amount by the amount or percentage stated in
the variance value.

Returns all relationships with a value of 600 or
more.

Does not equal

All relationships with a current value not equal
to the previous month amount.

Returns all relationships with a value other than
500.

374

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

Variance Operator

Balance Exception Report Output

Results (based on sample data)

Select a Balance Type and Balance Dimension that specifies the balance value that's evaluated for the exception. You
can only select balance dimensions that are compatible with the Comparison Type you specified. For example, if the
Comparison Type is Current Period, you can only select balance dimensions of type 'Period to Date'.

Severity Level
Severity Level controls the order in which the exceptions are displayed in the balance exception report. Balance
exceptions with the higher severity are displayed first (1 being the highest).

Using Formula Variance Type
You can write a fast formula using the Balance Exception formula type to return a variance value that you can use
for identifying exceptions for a balance. To use this feature, select the Formula variance type on the Create Balance
Exception page and then select the formula that you created from the Formula Name field.

Using Balance Variance Type
To reference two balances in the balance exception equation, select the Balance variance type on the Create Balance
Exception page and then select the Target Balance Name and Target Dimension Name. This is applicable only when
the Comparison Type is of type Current Month, Period, Quarter, or Year. The context values for Target Dimension
Name are inherited from the Dimension Name you select on the left-hand side of the Create Balance Exception page
as the first dimension. No additional contexts are set for Target Dimension Name.

Run Dimension Support
Define balance exceptions based on a balance value for a payroll run. For example, use these values to define an
exception to track employees with salary greater than $2,000 in the current run.

• Comparison Type: Current Run

• Dimension: Relationship Tax Unit Run

Define the following to support this exception rule:

• Balance Name: e.g. Salary

• Variance Type: Amount

• Variance Operator: Greater Than

• Variance Value: 2,000

• Severity: 1

When you run the Balance Exception Report, the generated report shows employees having salaries greater than $2000
for the current run only.

Flow Connector Rule Support
The Balance Exception Report supports flow connector rules to view the consolidated run balances for connected flows.
For example, during a payroll period, you run several off-cycle QuickPay runs to accommodate ad hoc late payments or
bonus payments to your employees or payment settlements for terminated employees. You also run the usual on-cycle
payroll runs for the same payroll period.

375

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

Use flow connectors to consolidate the flows. When you run the enhanced Balance Exception Report, the generated
report honors the defined flow connector rules and displays run balances for all the connected flows.

Examples of Balance Exceptions

Here are two examples to illustrate two different types of balance exceptions that you may want to include in your
balance exception report.

Track Increases in Commissions
Your company plans to train incoming sales staff on productivity techniques. To identify exceptional sales staff in the
organization, you can run a report that lists workers whose commissions increased by 25 percent compared to their
averages for the previous 3 months. You can set up a balance exception using the values in this table.

Field

Values

Balance Exception Name

Commission Increases Over 25 Percent

Comparison Type

Average in Months

Comparison Value

3

Balance Name

Commissions

Dimension Name

Relationship Month to Date

Variance Type

Percent

Variance Operator

Greater than

Variance Value

Severity Level

25

3

Note:
Enter a lower value for a high priority exception.

Track Gross Earnings
Before you certify the current payroll run, as a payroll manager, you may want to know if the current gross payments are
in line with the previous payroll run. The previous run verified the established levels of earnings that the company wants
to maintain for the remainder of the quarter. This table provides an example of the values you enter to set up a balance

376

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

exception to find out if the current gross earnings exceeds the gross earnings of the previous period by more than 10
percent:

Field

Values

Balance Exception Name

Gross Earnings

Comparison Type

Previous period

Comparison Value

1

Balance Name

Gross Earnings

Dimension Name

Relationship Period to Date

Variance Type

Percent

Variance Operator

Greater than

Variance Value

Severity Level

10

1

Note:
Enter a lower value for a high priority exception.

Balance Exception Report

Overview of the Balance Exception Report

Use the Balance Exception Report to identify potentially incorrect payments or amounts withheld. The report identifies
values that vary for the same balance dimension. This variance could indicate overpayments or underpayments.

Use the Submit a Payroll Flow  quick action under the My Client Groups tab to run this report.

Before you run this report:

• Use the Balance Exceptions task to create a balance exception.

• Use the Balance Exceptions and Reports task to create a balance exception report that groups together one or

more balance exceptions.

377

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

• Create an Exception Report Name that you can use to run the Balance Exception Report. For instance, you
can create an Exception Report Name of Monthly Car Allowances Paid in Excess of the Previous Month, to
determine the monthly car allowance paid to employees in excess of 600 more than the previous month.

Report Parameters

The parameter values determine which records to include in the report. For example, you can run this report for a
specific consolidation group or payroll relationship group. Predefine these groups before you can use them. Most
parameters are self-explanatory, while the following have special meaning in the context of this report.

Payroll Flow

The name of the payroll flow you use to run this report. The selected flow uniquely identifies a specific instance of the
report execution.

Process Start Date

Use this field to specify the first effective date of the payroll process to include in the report. All processes with an
effective date same or greater than the Process Start Date are reported.

Process End Date

Use this field to specify the last effective date of the payroll process to include in the report. For Payroll Runs this is the
'Payroll Run Date'. All processes with an effective date equal to or prior to the Process End Date are reported.

Note:  For offset payrolls, the effective date of the payroll or QuickPay run could be after the end date of the payroll
period. In such cases, ensure that your Process End Date must be on or after the effective date of the process you
want to include in the report.

Balance Exception Report

The name of the Balance Exception Report you use to run this report.

Payroll

Select the required payroll name.

Process Configuration Group

Use this field to run the report for a specific process configuration group, instead of the default one. A process
configuration group is used to set rules for payroll processes, such as enabling logging or setting the number of threads.
You can select a value only if you have a predefined process configuration group.

Note:  Use the Payroll Process Configuration  task to define a Process Configuration Group, before you can use it
here.

Consolidation Group

Use this field to run the report against a consolidation group. For example, you can use this field to run this report for
a subset of payrolls. You can select a value only if you have a predefined consolidation group. If you specified a value
when defining the exception report, select the same value or leave it blank.

The value chosen while submission takes precedence over the one used while defining the report. If you leave the field
blank, the report runs for all consolidation groups.

378

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Payroll Statutory Unit

Chapter 7
Payroll Balances

Select a value to report on the balances of employees in a specific PSU. If you leave the field blank, the report runs for all
PSUs.

Tax Reporting Unit

Select a value to report on the balances of employees in a specific TRU. If you leave the field blank, the report runs for all
the TRUs.

Location

Use this field to view the balance results for employees who have at least one assignment for the selected location. The
balance values may not necessarily correspond to the location parameter only. It is also dependent on the dimensions
and the other associated contexts.

Payroll Relationship Group

Use this field to run the report for persons belonging to a specific payroll relationship group. You can specify a value
only if you have a predefined payroll relationship group.

Note:  Use the Object Groups task to define a process configuration group, a consolidation group, or a payroll
relationship group, before you can use it here.

After you have entered the above details, in the Linked Flows section, select the payroll flow as the Current Flow and the
Run Balance Exception Report as the task. This ensures that the report uses the payroll balances for the current payroll
flow.

Report Results
The report provides details of payroll balance results for matching persons, filtered by the defined exception criteria,
specified time frame and the selected parameters. The output report includes:

• Payroll Statutory Unit

• Tax Reporting Unit

• Person Number

• Person Name

• Payroll Relationship Number

• Employment Level

• Current Balance

• Variance Value

The report output additionally displays the Previous Balance, Difference, and Difference % columns when the
Comparison Type is Previous Period or Previous Month.

How to Create a Balance Exception Report

In this example, you create a balance exception and run the Balance Exception Report to compare the total payments
made to your employees for the current payroll period with the payments you made in the previous payroll period.

379

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

Before you create and run the Balance Exception Report, you must create a balance exception for this example.

Create a Balance Exception
Let's look at the steps to create a balance exception to compare the net pay amounts for the current and the previous
period.

1. On the Home page, click the Balance Exceptions quick action under the My Client Groups tab.
2. Click Create.
3. Select a legislative data group and click OK.
4. Complete the fields as shown in this table:

Field

Value

Balance Exception Name

Compare Net Payment Amounts to the Previous Period

Comparison Type

Previous period

Comparison Value

1

For comparison types that begin with Previous, the application enters 1 as the default value and

makes it read only.

Balance Name

Net Payment

Dimension Name

Relationship Period to Date

Variance Type

Percent

Variance Operator

Greater than

Variance Value

Severity Level

10

1

Note:

Enter a lower value for a high priority exception.

5. Click Submit.

Create a Balance Exception Report

1. On the Home page, click the Balance Exceptions and Reports quick action under the My Client Groups tab.

380

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

2. Click Create.
3. Select the same legislative data group you selected in the previous task and click OK.
4. Complete the fields as shown in this table:

Field

Value

Exception Report Name

Compare Net Payment Amounts to the Previous Period

Consolidation Group

Select a value to restrict this exception report to a specific consolidation group. Leave blank to

not restrict the output or to decide at the time of report submission.

Payroll

Select a value to restrict this exception report to a specific payroll. Leave blank to decide at the

time of report submission, where payroll is a required parameter.

5. Click Add.
6. Select the Compare Net Payment Amounts to the Previous Period  balance exception name and then click

OK.

7. Click Submit.

Run the Balance Exception Report

1. On the Home page, click the Submit a Flow quick action under the My Client Groups tab.
2. Select the same legislative data group as in the previous tasks.
3. Select the Run Balance Exception Report flow pattern and then click Next.
4. Complete the fields as shown in this table:

Field

Value

Payroll Flow

Enter an appropriate name for this instance of the report.

Process End Date

Enter a value.

Balance Exception Report

Compare Net Payment Amounts to the Previous Period

Payroll

Select a value to restrict this exception report to a specific payroll. Enter the same name as in

the previous task, if one was specified.

5. Click Next.

When you enter information on the Linked Flow section of the Submit a Flow page, select Current Flow as the
payroll flow and Run Balance Exception Report as the task to ensure the report uses the payroll balances results
for the current payroll flow.

6. Click Next.
7. Click Submit.When you submit a flow, it creates an instance of the flow, the application generates a checklist by

default.

381

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

In the task list click the Run Balance Exception Report. View and monitor the status of the flow on this page.

8. Click OK and View Checklist.
9.
10. Click on the on the task to go to the Process Results Details page.
11. You can view the output from the Output and Log files section.

Related Topics

• Examples of Balance Exceptions

• Balance Exceptions

• Balance Exception Report for the US

• Balance Exception Formula Type

Severity Level for Balance Exceptions

Severity Level controls the order in which the exceptions are displayed in the balance exception report.

While defining a balance exception, enter a severity level to specify the priority of the exception. An exception with a
lower severity level has a higher priority than one with a higher severity level value.

When you run the Balance Exception Report, you can act on the exception based on its severity level. Let's say, you have
these two exceptions:

• Net Pay less than 100

• The difference in Base Salary from previous period to current period is 1000

Ideally, you should enter a lower value for the first exception, so that when you run the Balance Exception Report, the
payroll user can first look into reconciling the lower Net Pay exception.

Note:  The value you enter has no impact on the balance exception calculation.

Related Topics

• Examples of Balance Exceptions

• Severity Level for Balance Exceptions

• How to Create a Balance Exception Report

• Balance Exception Formula Type

• Balance Exceptions for the US

Copy Balances During Global Transfer

Overview of Copying Balances

Carry forward assignment and relationship level balances using balance adjustments from the source to the target legal
employer during the global transfer of employees.

382

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

Several payroll calculations would require the knowledge of prior calculations in other payroll relationships. It's
necessary for the balances to be brought forward to the new payroll relationship so that calculations within the new
payroll relationship are made aware of all prior results within the appropriate time frame of that balance. The overall
balance that's copied includes,

• The balances calculated within the payroll relationship

• The balances copied to the source payroll relationship for prior global transfers

Any further payroll deduction calculations on the target employment record must consider the calculations in the prior
employment records for the same person. The payroll run can't access balances across payroll relationships. So you
must copy the final balance from the source before the first payroll run on the target employment record.

Although you're using balance adjustments for the balances copy process, the application automatically generates
the adjustment element, similar to the balance initialization process. The application creates a balance feed from the
initialization element for both the target and source balance. You'd require this balance feed to read what's copied to the
target using the source balance in the next copy process. For example, you want to copy the Car Loan Accrued balance
to the target relationship. This copy process uses a REL_ITD dimension and the application copies it into a separate
balance called Prior Accrued. The source balance should include the balance calculated within the source relationship,
and the balances received from any previous global transfers.

You can copy balances to the target record through these methods:

• Select the Copy balances to the new employment record checkbox to start the copy of balances

automatically after the global transfer is complete. You can find this checkbox in the Payroll Details section
of Local and Global Transfer and Mass Legal Employer Change flow. Once the copy process is complete,
you can view the status message on the Change Legal Employer Dashboard. You can preconfigure the list
of balances by an object group; called Process Information Group. You can use the delivered Default Global
Transfer Group or define an object group according to your requirements.

• Submit the Transfer Balances flow if you think that the balances aren't ready on the source at the time of

global transfer and you want to start the copy later. You can identify the readiness of the balance by these two
conditions,

◦ Any further payroll activity on the source
◦ Time left for the first payroll activity on the target

The Transfer Balances process copies balances through a balance adjustment batch with adjustments for each balance
listed in the specified object group. The application records these adjustments using an application-generated element
with the Balance Initialization classification. If the source defined balance has one or more balance contexts, the process
creates separate adjustments for each context value.

The Transfer Balances flow consists of two tasks:

• Create Global Transfer Adjustment Batch: Creates the balance adjustment batch for copying balances

between employment records.

• Adjust Multiple Balances: Processes the adjustment batch and also supports rollback and retry operations.

You can run the Transfer Balance process again if more payroll runs take place on the source employment record. This
process assumes that the source balance value is the source of truth and adjusts for differences in balance values
between the source and target employment records, even negative ones. So the best idea is to leave the Exclude Target
Assignment with Payroll Results parameter in the Transfer Balances flow at its default value. This approach would
prevent accidentally reversing the results of calculations on the target employment record that aren't part of the source
balance value.

383

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

Before You Set Up the Object Group

There are several factors you must consider when configuring the application to copy balances between employment
records.

Source and Target Balances
The source balance is the balance used to read values on the source assignment or payroll relationship. You must
choose the source balance based on which calculation results should be visible to the target payroll calculation. For
example, when continuing a Total Owed deduction on the target assignment or payroll relationship. You must also copy
the Accrued balance, as that's what the payroll calculation checks to determine the remaining amount to deduct.

The target balance is the balance adjusted on the target assignment or payroll relationship. The most common choice
for target balance is the same as source balance. However, this choice may not meet every requirement, especially if
you need to separate the Previous Balance from the balance calculated within the current legal employer for reporting
purposes. To meet these requirements you will require additional manual configuration, such as new balances, and
should be done only when necessary.

Source Balance Dimension
To read the balance value on the source employment record you will require a defined balance, which is a combination
of the balance and the associated balance dimension. The balance dimension is determined by three factors based on
how the copied balance is used on the target employment record.

1. Employment Level: Assignment or Payroll Relationship
2. Time Span: The period over which the balance value must be fetched and copied. For example, an Arrears or
Accrued balance for a deduction would require Inception to Date (lifetime) values. On the other hand, annual
statutory limits on a pre-tax deduction would require Year to Date values.

3. Context or References: If you want to copy the values separately based on logical partitions such as Tax

Reporting Unit, Deduction Reference, State/Province, then select the dimension that contains the necessary
contexts. Calculation Breakdown is an implicit context and you can exclude this using a No Calculation
Breakdown dimension. For example, if a state imposes an annual statutory limit on employee earnings, which
is exempt from state income tax. In this case, you would want to copy the exempt earnings from the source
legal employer for the year to date separately for each state. You can do this by using a State Year to Date
dimension. The application reads and adjusts the balances for every value of the context, where the balance
values differ between the source and target employment records.

Element Entry as a Prerequisite for Copying Balances
The most common use case for copying balances is to bring visibility of calculation results to the payroll calculation
on the target payroll relationship. You can use the calculation formula associated with the element entry that uses the
balance value to determine the final calculated result. You can choose to copy the balance always or only if such an
element entry exists.

Although, copying balances only if an element entry exists might seem like the most efficient method by avoiding
copying balance values that may never be used on the target employment record, you must consider the possibility of
the following scenario:

• The application assigns an element entry after the copy process. For example, a pre-tax deduction that's

subject to an annual statutory limit.

384

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

Related Topics

• Overview of Copying Balances

• Example to Carry Forward Total Owed Deductions

• Global Transfer Overview

Example to Set Up Voluntary Deduction Balance to Object Group

This example describes how to configure the list of source and target voluntary deduction balances by Process
Information Group. You can add balances to the delivered Default Global Transfer Group or define an object group
according to your requirements.

Here's how you can add the Car Loan Repayment balance to the object group:

1. On the Home page, click the Object Groups quick action under the My Client Groups tab.
2. Select a Legislative Data Group.
3. Search for and select the Default Global Transfer Group as the object group name.
4. Click Edit on the Object Groups page, and click Next.
5.

In the Object Group Store section, select Global Transfer Balance Adjustment in the Context Segment field.
Click Search.

6. To add a new entry, click the Create button.
7. Select the Source Defined Balance as Car Loan Repayment Accrued Relationship No Calculation

Breakdown Inception to Date to read the value on the source employment record.

8. Select the Target Balance as Car Loan Repayment Accrued that's adjusted on the target employment record.
9. Optionally, select the Prerequisite Target Element as Car Loan Repayment if you want to copy the balance

only when the employee has a prerequisite element entry.

FAQs for Balances

Can I calculate balances that go back 12 months?

Yes. You can use certain balance dimensions to calculate balances based on a 12-month period rolling back from the
effective date. The 12-month rolling balance provides a sum total for the balance dimension that you select.

If the balance dimension is used in a payroll run or report, however, it calculates a balance based on the 12-month period
prior to the effective date of the run.

For example, let's say you wanted to retrieve balances for an employee for 12 months. If the effective date is 31-
AUG-2015, you can then use a balance dimension to summarize all run results for the period from 01-SEP-2014 to 31-
AUG-2015.

385

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 7
Payroll Balances

What balance dimensions can I use to calculate balances for a 12-
month roll back period?

You can use these balance dimensions to calculate balances for a 12-month roll back period:

This table lists the available balance dimension types and balance dimensions.

Balance Dimension Type

Balance Dimension

Rolling 12 Month Balance Dimensions

• Relationship Tax Unit Rolling 12 Month

• Assignment Tax Unit Rolling 12 Month

Resident City Balance Dimensions

• Term Tax Unit Resident City Month-to-Date

Statutory Report Code Balance
Dimensions

• Term Tax Unit Resident City Quarter-to-Date

• Term Tax Unit Resident City Year-to-Date

• Assignment Tax Unit Resident City Month-to-Date

• Assignment Tax Unit Resident City Quarter-to-Date

• Assignment Tax Unit Resident City Year-to-Date

• Relationship Tax Unit Statutory Report Code Run

• Relationship Tax Unit Statutory Report Code Month-to-Date

• Relationship Tax Unit Statutory Report Code Quarter-to-Date

• Relationship Tax Unit Statutory Report Code Year-to-Date

• Relationship Tax Unit Statutory Report Code Period-to-Date

• Term Tax Unit Statutory Report Code Run

• Term Tax Unit Statutory Report Code Month-to-Date

• Term Tax Unit Statutory Report Code Quarter-to-Date

• Term Tax Unit Statutory Report Code Year-to-Date

• Term Tax Unit Statutory Report Code Period-to-Date

• Assignment Tax Unit Statutory Report Code Run

• Assignment Tax Unit Statutory Report Code Month- to-Date

• Assignment Tax Unit Statutory Report Code Quarter-to-Date

• Assignment Tax Unit Statutory Report Code Year-to-Date

• Assignment Tax Unit Statutory Report Code Period-to-Date

386

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

8  Payments

Bank Accounts

Chapter 8
Payments

Considerations When You Create Accounts

Banks, branches and accounts fit together on the premise of the Bank Account model. The Bank Account model enables
you to define and track all bank accounts in one place.

The Bank Account Model can explicitly grant account access to multiple business units, functions, and users. Consider
the following when you set up bank accounts:

• Assign a unique general ledger cash account to each account, and use it to record all cash transactions for the

account. This facilitates book to bank reconciliation.

• Grant bank account security. Bank account security consists of bank account use security, bank account access

security, and user and role security.

Legal Entity-Based Data Access for Bank Account Setup
By default, users with the necessary function security privileges have access to create and manage all internal bank
accounts.

Optionally, restrict access to bank account information based on the user's legal entity data access. This allows cash
managers to add, review, or modify only the bank accounts associated with the legal entities that the user has access
to. For example, only users who have been assigned the Manage Bank Account (CE_MANAGE_BANK_ACCOUNT_PRIV)
privilege for Vision Operations legal entity, can create, review, or modify internal bank accounts associated with this
legal entity.

Decentralized organizations will benefit with improved security by ensuring that users only manage the bank account
setup for the organizations they're authorized for.
Business benefits include:

•

Improve security and increase control of bank account setup by limiting user access to bank account
information.

• Helps decentralized organizations that require users only to manage the bank account information for the

organizations they're authorized for.

To enable the feature Legal Entity-Based Data Access for Bank Account Setup, you must:

1. Use the Opt in UI to enable the feature.
2. Assign users to the appropriate legal entity security context:

a.

In the Setup and Maintenance work area, Select the Offering as Financials, Functional Area as Users and
Security, and Task as Manage Data Access for Users.

b. On the Manage Data Access for Users page, create data access for users by entering the user name, Cash
Manager as role, legal entity as security context, and legal entity name as security context value, to create
the data access for the user.

c. Save the changes.

387

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Once the feature is enabled, legal entity-based data access security is applied when an internal bank account is created
or managed using either the UI or REST API.

Account Use
Account Use refers to accounts created for:

• Oracle Fusion Payables

• Oracle Fusion Receivables

• Oracle Fusion Payroll

Select the appropriate use or uses when creating an account in one or more of these applications.

Account Access
Payables and Receivables account access is secured by business unit. Before the bank account is ready for use by
Payables or Receivables, you must:

1. Select the appropriate use for the application.
2. Grant access to one or more business units.

Note:  You can only assign access to the business units that use the same ledger as the bank accounts owning the
legal entity,

User and Role Security
You can further secure the bank account so that it can only be used by certain users and roles. The default value for
secure bank account by users and roles is No. For Payables and Receivables, you must have the proper business unit
assigned to access a bank account even if the secure bank account by users and roles is No. If the secure bank account
by users and roles is set to Yes, you must be named or carry a role assigned to the bank account to use it.

• To set up banks, branches, and accounts, your custom role must have the security duty role Cash

Management Administration. You must have the assigned the Manage Bank Account Security privilege
(CE_MANAGE_BANK_ACCOUNT_SECURITY_PRIV) to modify the User and Role Security.

• To restrict the access to the Security tab, you must create a custom role and remove the Manage Bank Account

Security (CE_MANAGE_BANK_ACCOUNT_SECURITY_PRIV) privilege. For example, you'd copy the Cash
Management Administration duty role, rename it, and remove the privilege.

GL Cash Account Segments
Consider selecting the option to enable multiple cash account combinations for reconciliation to reconcile journal lines
of multiple cash account combinations matching the same natural account and other specified segment values.

For example, if you set up 01-000-1110-0000-000 as your cash account, and select Account and Subaccount as GL
Cash Account Segments, you can manually or automatically reconcile journal lines entered on different account code
combinations matching the same natural account '1110' and subaccount '0000'.

Related Topics

• Assign Data Access to Users

388

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

How Bank, Branch, and Account Components Work Together

Banks, branches, and accounts fit together on the premise of the Bank Account model.

The model enables you to define and keep track of all bank accounts in one place and explicitly grant account access to:

• multiple business units

•

functions

• users

This eliminates the redundant duplicate bank account setup in different business units when these business units share
the same bank account.

Banks
Creating a bank is the first step in the bank account creation. You can:

• Search for existing banks to view and update

• Create a new bank from an existing party

Consider the following:

• The option to create from an existing party is implicitly implemented by the matching option.

• The option is available only after the existing party has been found with the same bank.

•

If you select the matching option, the page repopulates the information from the matched party.

Branches
Once you have created your bank, the next step is creating a branch or branches associated to the bank. The matching
option is also available when creating branches. To create a new branch without using the matching option, manually
enter the required information. You can also define other branch- related attributes in the same page.

If you don't use the matching option when an existing party is found, a branch with the same party name is created.

Accounts
The four areas associated with defining an account are:

• General information

• Control of the account

• Security and access to the account

• Business unit assignment

Once the bank and branch are created, proceed to the bank account setup by doing the following:

• Select the bank branch you want to associate to your bank account.

389

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

• Assign the owner of the bank account.

Chapter 8
Payments

Note:  To create a bank account for Payables or Receivables, add the Business Unit Access first for the
business units to use the bank account.

Consider the following:

• The Oracle Fusion Account Payables or Receivables accounts are identified by the business unit.

• The Oracle Fusion Payroll accounts are identified by the legal entity.

• The program, Inactivates Banks and Bank Branches enables you to inactivate all banks and bank branches that

have no active internal and external bank accounts.

• Optionally, secure the access to bank account information based on the user's legal entity data access, by

enabling the opt-in Legal Entity-Based Data Access for Bank Account Setup.

• Legal entity-based data access for bank account setup:

◦ Improves security and increases control of bank account setup by limiting user access to bank account

information.

◦ Helps decentralized organizations that require users only to manage the bank account information for

the organizations they are authorized for.

Related Topics

• Considerations When You Create Accounts

• Reconciliation Matching Rules

• Assign Data Access to Users

Bank Account Number Masking in Payroll Reports

To prevent display of sensitive bank account information, you can use the option of masking or encrypting bank
account information in these reports:

• Payslips

• Payment Register

• Third-Party Payment Register

Masking involves displaying only a few specific characters of the account number or IBAN number, usually characters
at the start or end of the number. The remaining characters are obfuscated and you can't see them on the reports. For
example, a customer may want to display only the last 4 characters of the account number. In such cases, an account
number ABC123456 displays as XXXXX3456 in reports and UIs that support masked account numbers.

Encryption requires a secure key for decoding the encrypted account number and IBAN number through an API. The
application displays the truncated account or IBAN number when the encryption is turned on and the full, clear number
when the encryption is turned off.

390

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Settings that Affect Account Number Masking
The application stores the bank account number and IBAN number information in these columns of the database
tables:

• Original column that stores the visible unmasked portion of the numbers.

• Masked column that stores the masked numbers. When masking isn't enabled, these columns store the full

numbers.

• Secured column that stores the encrypted numbers and requires a secure key to retrieve the data.

This table shows how the bank account numbers are stored in the tables depending on how you configure masking and
encryption.

Actual Account
Number

Configuration -
Masking

Configuration -
Encryption

Original Column

Masked Column

Secured Column

ABC123456

ABC123456

ABC123456

No

Yes

Yes

No

No

Yes

ABC123456

ABC123456

ABC123456

ABC123456

XXXXX3456

ABC123456

3456

XXXXX3456

ABC123456

Note:  The above table assumes that the masking setup displays only the last four characters of the bank account
number.

• The first row in the table shows the default settings where both masking and encryption is turned off. The

original full number is stored in all the three columns.

• The second row in the table depicts a scenario where masking is turned on but encryption is turned off. In this

case the masked column displays only the last four characters of the account number.

• The third row depicts a scenario where both masking and encryption is turned on. In this case the original

column contains the truncated four-digit account number. You need the secure key to retrieve the full account
number from the secured column.

When you turn on encryption, the unsecured account number and IBAN columns only shows the visible characters
as defined by masking. This means that to turn on encryption, you must turn on masking. However, you can turn on
masking without turning on encryption.

How Account Number Masking Works
Use the new Extract Unmasked Bank Information (ORA_PAY_UNMASKED_ACCOUNT_INFO) process configuration
parameter to display either the masked or full numbers in the reports. This new parameter ensures:

• Consistency across the three reports

• Control how you display the numbers on the reports

391

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

The following figure shows how account number masking happens for the three reports.

The figure shows the following:

• The first stream layer shows the table columns that store the account number information.

• The second stream layer shows the XML tags and process configuration groups.

• The third stream layer shows the RTF fields shown on the report template.

As explained in the previous section, the application stores the account number information in three separate columns.

The new ORA_PAY_UNMASKED_ACCOUNT_INFO process configuration parameter controls the MASKED_ACCOUNT_NUM tag to display:

• The masked account number when the process configuration parameter is by default or set to No, or

• The clear or full account number when the process configuration parameter is set to Yes.

For example, if you mail a copy of the Third-Party Payment Register to the payee, you may want to mask the sensitive
bank account information. If the same report is shared securely within the Payroll Department to verify the bank
account details, you may run the report with the process configuration parameter set to Yes.

All the three reports use the MASKED_ACCOUNT_NUM XML field to display the Account Number.

You can use the BANK_ACCOUNT_NUM field if you use an older copy of the three reports. If you do so and you have
turned on encryption, you can use the ORA_PAY_DECRYPTED_ACCOUNT_INFO parameter to switch between a clear and
truncated number.

Related Topics

• Options for System Security

• Enable Encryption of Sensitive Payment Information

392

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

How Do I Extract Unmasked Bank Account Details In User-Defined
Reports?

To extract and display unmasked bank account numbers in user-defined reports, use these data base items (DBIs):

• Clear Bank Account Number

• Clear Bank Account IBAN

Use these DBIs from one of these user entities:

• PERSONAL_PAYMENTS

• PERSONAL_PAYMENTS_RANGE

• ORG_PAYMENTS_RANGE

By default, the Make EFT Payments and Generate Check Payments process writes unmasked bank
account numbers. For any other report that uses the payment XML to write bank account details, set the
ORA_PAY_DECRYPTED_ACCOUNT_INFO payroll action parameter to Y, to extract the decrypted bank account and
IBAN in the payment XML.

Similarly, use the ORA_PAY_UNMASKED_ACCOUNT_INFO process configuration parameter and set it to Y so that the
MASKED_ACCOUNT_NUM tag displays the unmasked, full bank account number in the reports.

Bank Account User Rules by Country

Country-specific user interface rules have been predefined for employee bank accounts in the simplified bank account
page.

The fields displayed on the user interface are governed by the rules defined in the table CE_CTRY_SPECIFIC_UI_RULES.
The tables on the UI Rules list the predefined country-specific user interface rules for employee bank accounts in the
simplified bank account page.

Related Topics

• Employee Bank Account Rules by Country: Argentina to Guernsey

• Employee Bank Account Rules by Country: Hong Kong to Norway

• Employee Bank Account Rules by Country: Oman to Vietnam

393

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Payment Methods

How Payment Methods and Payroll Definitions Work Together

When you create objects, such as payroll definitions, third-party payment methods, and personal payment methods,
you select a payment method to associate with the object. Understanding the functional relationship between the
payment methods and the objects that use them is important.

Functional Relationships
This table helps you understand the functional relationship of payment methods with other objects.

Object

Function

Personal Payment Method

Associates a person to a payment method, currency, and payment source for payroll payments.

Third-Party Payment Method

Associates third parties, who aren't on the payroll, to payment information, such as currency and
bank. Payments to third parties might be garnishments to control how you pay or other involuntary
deductions and are typically processed separately from the payroll.

Payroll Definition

Associates a default payment method for payments to employees when a personal payment method
isn't defined.

Note:
You can't set EFT payment methods as default payment methods because each payee must have a
personal payment method with bank account information to know where to deposit the money.

Run-Type Payment Method

Associates a default payment method for a run type for payments to employees with no personal
payment method defined. This overrides the payroll default payment method.

For example, your regular payroll is by EFT but you issue check/cheque bonuses once a year. Using
the Separate Payment run type, the payment method overwrites the default payment method of the
payroll.

Related Topics

• Organization Payment Methods Overview

• Payroll Definitions

• Third-Party Payment Methods

394

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Organization Payment Methods

Overview of Organization Payment Methods

Organization payment methods (OPM) control how you pay payroll payments to your employees and third parties.
OPMs interact with payroll definitions, payment sources, payment rules, prenotifications, and link the personal payment
methods (PPMs) with your organization payment sources.

After setting up the banks, bank branches, and bank accounts that you use, you can define payment methods for your
organization. OPMs include key information, such as payment type, currency, and company bank information.

You must create one organization payment method for each combination of legislative data group, payment type,
and currency that you use to disburse wages and other compensation. You can also create rules to determine the
distribution of payments from a specific bank account for a specific group of payees. Use the Organization Payment
Methods page to view, create and edit.

Note:  Create one organization payment method per payment type and currency, such as a direct deposit being paid
in USD. Define payment sources and payment method rules to determine which payment source will pay which group
of payees. If you decide to create more than one OPM per payment type and currency, you must configure payment
method preferences to define OPMs available for employees to use.

Payment Types
When you create an organization payment method, select a payment type.

These are the most common payment types and the name of the corresponding payment processes:

Payment Types

Payment Process

Direct Deposit

Make EFT Payment

Check/cheque

Choose one of these 2 check/cheque payment processes:

• Use the Generate Check Payments process to run the check process for your employees and third

parties in one process.

• Use the Generate Check Payments for Employees and Third Parties process to run the check

process for your employees and third parties in separate processes.

International Transfer

Make EFT Payments

Cash

There's not a cash payment process. You can make cash payments outside of the application and
record as an external payment.

395

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Note:  The exact list of payment types and their names can vary by country. Your enterprise may support a different
range of types that are appropriate for your localization. For example, in the US, the payment type for EFT is Direct
Deposit; in the UK it's BACS, and in Australia it's BECS.

Currency
Currency is typically defined as the same currency as your company's source bank account. Define currency in the OPM
for payment transfers, such as EFT files.

The prepayment process supports currency conversions but it's important to make sure your localization and bank
support multi-currency payments, to include the format of the payment file that supports international payments. For
example, your output currency for your elements is defined as USD. All payroll calculations use your element currency,
to include net payment amounts. When you define an international transfer OPM with GBP currency and associate it to
an employee's personal payment method, the prepayments process converts the payment amount from USD to GBP for
the employee. And, the payment process payment file contains the converted amounts in GBP to send the payment in
the employee's currency.

Payment Information
Use the payment information region to capture details for your payments. For example, you can specify a maximum
limit for each payment made using the organization payment method. You also have an option to define a maximum
limit for the total payment transaction.

The exact content of this region can vary based on the selected payment type and your localization.

Note:  You can enter payment information at the organization payment method level, the payment source level,
or both. Entries at the payment source level take priority over entries at the organization payment method level. If
you define details at the payment source level, to use those details when you process payments, you must enter the
payment source when you submit the payment process.

Prenotifications
Prenotifications or prenotes are typically 0 amount electronic entries you send to a bank to verify the routing number
and account number of the receiving bank. Use the Organization Payment Methods task, to configure following
prenotification rules for direct deposit payment types.

Field Name

What it does

Prenotification Required

Designates the prenotification is required for employees.

Prenotification Amount

Designates the prenotification transaction amount. is required for employees. Default value is 0 USD.

Days

Number of days required for a prenotification wait period. Until the waiting period is complete, the
employee is paid by check. For example, if you set the prenote wait period to 10 days, depending on
the timing for weekly payroll runs, the employee may receive 2 checks before the direct deposit begins.

If you prenote bank accounts in your legacy system, you may choose to skip the prenote process when you implement
payroll. To do this use the Payroll Bank Account Prenote Status Update data loader.

396

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Payment Sources
Payment sources identify your company bank accounts debited for payroll payments. You must associate at least one
payment source to an organization payment method.

This validation occurs to ensure the bank account on the payment source are available for payroll payments:

• Must be associated to a Payroll Statutory Unit (PSU). You must either assign a PSU legal entity to the bank

account or assign a legal employer with a parent PSU to the bank account.

• Must be enabled for payroll payments. You must select Payroll in the Account Use option for the bank account.

• Must have active bank account. You must assign a bank account that's active at the time of the payroll

payment.

This diagram highlights the bank account set-up required for Cloud Payroll. Use the payroll
extension option on the Features by Country or Territory page to register Cloud Payroll.

Note:  In order for a bank account to appear in the payment source page it must be associated to a Payroll Statutory
Unit (PSU), enabled for payroll payments and active.

Note:  If you use a third-party payroll product, you can create an organization payment method without a payment
source record.

Note:  If you cost your payments, enter cost account information on the Costing of Payment Sources page.

You can use the same bank account in different payment sources in more than one organization payment method, as in
this example.

Organization Payment Method

Payment Source

Bank Account

Check/cheque

Bank of America Account A

Bank A - Account 7890045

EFT

Bank of America Account B

Bank A - Account 7890045

Payment Method Rules
Payment method rules define the appropriate payment source to be used for payment to a specific group of payees. If
you define multiple payment sources for an organization payment method, you must set up payment method rules.

397

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

You can define standard payment method rules based on the tax reporting unit (TRU) of an employee. You can also use
the payment criteria feature to set up payment method rules to derive payment sources within a single TRU, such as
rules based on department, job or location.

This example shows payment method rules based on the TRU of the payee. The organization payment method has
three different payment sources.

Payment Source

Tax Reporting Unit

Default Payment Source

Payroll EFT Source A

Bank A - Account 7890045

Payroll EFT Source B

Bank B - Account 1238900

Payroll EFT Source C

Bank C - Account 8765999

None

TRU1

TRU2

Yes

No

No

The first payment source that you add is the default payment source, but you can select another payment source as the
default, or not have a default payment source.

To understand the effect of a default payment source, consider these examples that describe what happens when a TRU
changes, and causes an invalid payment rule.

Approach

Example

With a default payment source, the
payment process pays employees with the
default payment source.

Without a default payment source,
 the payments process issues error
notifications to ensure that you use the
appropriate payment source to fund the
payment.

This approach might suit a company with multiple independent franchises, each with its own TRU. If a
franchise holder sells the franchise, payments don't fail.

This approach might suit a company with strict policies about payment rule compliance.

International Transfer Payment
The international transfer payment type supports payment methods for electronic funds transfer (EFT) payments to a
country different from the originating payment source.

In order for you to use this functionality, you must be able to support payments to international bank accounts. For
example, the US supports a file format called IAT NACHA, which supports making payments from the US to bank
accounts which reside outside of the US. Attach the file format to the 'International EFT' report category.

398

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Related Topics

• Configure Payment Method Preferences

• Payment Method Rules Setup Examples

• Payment Sources in Organization Payment Methods Setup Examples

• How do I import organization data?

• Example of Skipping Prenotes

Payment Sources in Organization Payment Methods Setup
Examples

You set up payment sources when you create organization payment methods (OPM) for payroll processing. Use the
Organization Payment Methods task.

Derive Payment Source Based on TRU
You pay your workers by electronic funds transfer (EFT) payments. To comply with tax reporting unit (TRU) regulations
for out-of-TRU payments, payment rules are created based on TRU to pay from two different banks. This table helps
you understand your key decisions for this scenario:

Decisions to Consider

In This Example

How many OPMs do you need?

One.

How many payment sources do you need?

Three.

One default payment source for the TRU1, one source for payments in TRU2, and one source for
payments in TRU3.

How many bank accounts do you need?

Three.

One for each payment source.

What payment method rules do you need?

Rules for bank accounts used as payment sources based on each TRU.

Prerequisites
Verify you have completed these before you continue:

1. Primary ledger is set up in Oracle Cloud General Ledger.
2. Banks, branches, and account info to use as the payment sources are set up in Oracle Cloud Cash Management.
3. Legal entity associated with the legislative data group is assigned to a general ledger.
4. TRUs are set up.

399

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Create the OPM with Basic Details
Add new OPM in the Organization Payment Methods page with this info:

1. Click the Organization Payment Methods task.
In the Search Results section, click Create.
2.
3. Select your legislative data group. This example is InFusion LDG.
4. Select the date this payment method is to be available for use.

Tip:  Select a date that's on or before the effective date this payment method will be used by the payroll
definition or other objects.

5. Click Continue.
6.

In the Basic Details section, complete the fields with this info:

Field

Name

Value

Payroll Direct Deposit

Payment Type

Direct Deposit

Note:

The available payment types for OPMs can vary by legislation.

Currency

Payment currency

7. Click Save.

Add EFT File Info
When you select the EFT payment type, you have the option enter EFT info at these levels:

Note:  EFT file info entered at the payment source level takes priority over info entered at the organization payment
method level.

1. Payment source level
2. Organization payment method level
3. Both levels

Create Payment Sources
Perform these steps three times to create each payment source.

1.

In the Payment Sources section under Payment Source Information, click Create.

400

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

2. On the Create Payment Source page, complete the fields in order, as shown in this table:

Field

Name

Source 1

Source 2

Source 3

Payroll EFT Source 1

Payroll EFT Source 2

Payroll EFT Source 3

Bank Account Name

Bank A

Bank B

Bank C

Bank Reference

123456789

234567890

345678901

Company Reference

456789012

567890123

678901234

Tip:  Keep your payment source names unique and specific as possible for each scenario. This naming
convention helps you manage complicated combinations of OPMs and payment rules.

3. Click Continue.

Create Payment Rules
Perform these steps three times to create each payment source.

1.
2.

In the Payment Method Rules section, for Payroll EFT Source US, ensure that the default setting is Yes.
In the same section, click Create and select the values shown in this table to create two payment rules that map
a payment source to a TRU.

Field

Default

Tax Reporting Unit

Source 2

Source 3

No

TRU2

No

TRU3

Payment Source

Payroll EFT Source 2

Payroll EFT Source 3

3. Click Submit.

Create Same Payment Source for Pay Workers and Third Parties
Your organization pays all workers and third-party payees from the same source bank account. In this scenario, no
special payment method rules are required. Perform these steps for this scenario:

1. Ensure the payment source is set as the default.
2. Leave the Third-Party Payment, Tax Reporting Unit, and Payment Criteria fields blank.
3. Click Continue.

401

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Create Separate Payment Source for Pay Workers and Third Parties in a Specified TRU
Your enterprise is based in one tax reporting unit (TRU1), but you have some workers in another tax reporting unit
(TRU2). To comply with TRU1 regulations for out-of-TRU payments, you specify a payment source for the TRU2. In this
scenario, your payment source for TRU1 is already set as the default payment source, so no change is needed for TRU1.
Perform these steps for the TRU2 employees:

1. Add a payment method rule.
2. Select the TRU2.
3. Select the TRU2 payment source.
4. Click Continue.

Create Separate Payment Sources for Pay Workers and Third Parties in the Same TRU
You currently pay everyone in your TRU using Payment Source A. Your company recently employed a private consultant,
Jon Moore, from a third-party auditing company. A new company requirement states that payments must come from a
new payment source, Payment Source B. For this scenario:

1. Create John as a third-party person payee.
2. Leave the Third-Party Payment, Tax Reporting Unit, and Payment Criteria fields blank.
3. Click Continue.

Create Separate Payment Source for Pay Workers in a Specified Department

Note:  This scenario has these prerequisites:

• An information element exists named Default Payer with an input value named Payment Criteria.

• A formula exists that retrieves department names and the assignment IDs of the employees associated with

them.

• The processing rules in the Default Payer element refer to the formula. The result rules target field is set to

Payment Criteria. The returned field is set to the value specified in the formula.

You use different payment sources to pay employees in the Sales and Development departments. Perform these steps
for this scenario:

1. Create a payment method rule for each department.
2. Enter the department name in the Payment Criteria field.
3. Select the TRU and payment source.
4. Click Continue.

Related Topics

• How Bank, Branch, and Account Components Work Together

• Organization Payment Methods Overview

• Payment Method Rules Setup Examples

• Derive Payment Sources Example

402

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Payment Method Rules Setup Examples

These examples show you can use payment method rules to handle payments to different parties and from different
payment sources. Set payment method rules on the Organization Payment Methods page.

Create the Same Payment Source for Pay Workers and Third Parties
Your organization pays all workers and third-party payees from the same source bank account. In this scenario, no
special payment method rules are required. Add a payment rule in the Payment Method Rules section as stated in these
steps:

1. Ensure that the payment source is set as the default.
2. Leave the Third-Party Payment, Tax Reporting Unit, and Payment Criteria fields blank.

Create Separate Payment Sources for Pay Workers and Third Parties in a Specified
TRU
Your organization is based in one tax reporting unit (TRU1), but you have some workers in another tax reporting unit
(TRU2). To comply with TRU1 regulations for out-of-TRU payments, you specify a payment source for the TRU2. In this
example, your payment source for TRU1 is already set as the default payment source, so no change is needed for TRU1.
For the TRU2 employees. Add a payment rule in the Payment Method Rules section as stated in these steps:

1. Select the TRU2.
2. Select the TRU2 payment source.

Create Separate Payment Sources for Pay Workers and Third Parties in the Same TRU
You currently pay everyone in your TRU using Payment Source A. Your company recently employed a private consultant,
Jon Moore, from a third-party auditing company. In this example, you have a new company requirement that states
payments must come from a new payment source, Payment Source B. Add a payment rule stated in these steps:

1. Create John as a third-party person payee.
2. Add the Payment Source B payment source and a new payment method rule in your organization payment

method.

3. Select the Third-Party Payment check/cheque box, Jon's name as the third-party person to pay, and Payment

Source B in the payment method rule.

Create a Separate Payment Source for Pay Workers in a Specified Department
You use different payment sources to pay employees in the Sales and Development departments. Add a payment rule in
the Payment Method Rules section as stated in these steps:

1. Create a payment method rule for each department.
2. Enter the department name in the Payment Criteria field.
3. Select the TRU and payment source.

403

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Note:  This scenario has these prerequisites:

Chapter 8
Payments

• An information element exists named Default Payer with an input value named Payment Criteria.

• A formula exists that retrieves department names and the assignment IDs of the employees associated with

them.

• The processing rules in the Default Payer element refer to the formula. The result rules target field is set to

Payment Criteria. The returned field is set to the value specified in the formula.

Related Topics

• Derive Payment Sources Example

• Payment Sources in Organization Payment Methods Setup Examples

Derive Payment Sources Example

Use payment criteria to set up your rules to derive payment sources within a single tax reporting unit (TRU). The
prepayments process uses the rules to identify the source bank information from the employee's TRU and any
additional payment criteria you define.

This example uses department, but you can use other criteria, such as business unit.

Steps to Derive Payment Sources by Department
You want to pay employees in the Sales and Development departments from separate payment sources. You define
the payment rules in organization payment method, create fast formulas get department names from HR and call the
employees department names by Assignment ID, and create an element with the default payer information. The default
payer element passes the department name as a run result value.

1. Define the payment rules .in the Organization Payment Method page.

◦ Add one payment rule for each department in the Payment Method Rules section, as shown in this table:

Field

Development Department

Sales Department

Tax Reporting Unit

TRU 1

Payment Criteria

Development

TRU 1

Sales

Payment Source

Payment Source A

Payment Source B

Note:  In the Payment Sources section, create the payment sources to use in the payment rules, if they
don't already exist.

2. Create the formula to get department names from HR.

404

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

◦ Enter information on the Fast Formulas page, as shown in this table:

Field

Value

On the Fast Formulas page, create

XX_Employee_Department

the formula with values as shown in

this table:

Formula Type

Payroll Access to HR

Description

Formula to return the department of an employee.

Effective Date

01/01/1951

Note:

Enter the same date used to create elements during implementation.

◦ In the Formula Text section, enter this content:

Default for PER_ASG_ORG_DEPARTMENT_NAME is ' '
l_dept_output = PER_ASG_ORG_DEPARTMENT_NAME
Return l_dept_output

◦ Click Submit.
◦ Click Complete.

3. Create the formula to get the departments for employees to use as payment criteria value.

Note:  This formula calls the department names formula to get employee department by Assignment ID,
which are used to find employees values.

◦ Enter information on the Fast Formulas page, as shown in this table:

Field

Value

On the Fast Formulas page, create

XX_Default_Payer_Payment_Criteria

the formula with values as shown in

this table:

Formula Type

Payroll

Description

Formula to use the returned Department database item as Payment Criteria input for

Default Payer element.

405

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Field

Value

Effective Date

01/01/1951

Note:

Enter the same date used to create elements during implementation.

◦ In the Formula Text section, enter this content:

Default for ASG_HR_ASG_ID is 0
SET_INPUT('HR_ASSIGNMENT_ID', ASG_HR_ASG_ID)
EXECUTE('XX_Employee_Department') /* Formula to retrieve the
Employee Department. */
Emp_Dept = GET_OUTPUT('l_dept_output','Null')
Return Emp_Dept

◦ Click Submit.
◦ Click Complete.

Create the Element to Derive Payment Source by Department
Create the Default Payer element with the Payment Criteria input value, and automatic element eligibility.

1. Create an element on the Elements page using the Information primary classification and the values shown in

this table:

Field

Name

Value

Default Payer

Note:

This name must match exactly. This name is how the application identifies any existing

payment criteria.

Reporting Name

Default Payer

Effective Date

01/01/1951

Note:

Enter the same date used to create elements during implementation.

What is the earliest entry date for this

First Standard Earnings Date

element?

406

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Field

Value

What is the latest entry date for this

Last Standard Process Date

element?

2. Edit the new element to create an input value named Payment Criteria:

◦ Click Input Values in the Element Overview section.
◦ Select Create Input Values from the Actions menu.
◦ Enter values as shown in this table:

Field

Name

Value

Payment Criteria

Display Sequence

10

Unit of Measure

Character

◦ Click Save.

3. Edit the new element to create element eligibility that is set to automatic entry:

◦ Click Element Eligibility in the Element Overview section.
◦ Select Create Element Eligibility from the Actions menu.
◦ Enter Payment Criteria Element Eligibility in the Element Eligibility Name field.
◦ Select Automatic entry.
◦ Click Save.

4. Edit the new element to create processing rules:

◦ Click Status Processing Rules in the Element Overview section.
◦ Select Create Status Processing Rules from the Actions menu.
◦ Select XX_Default_Payer_Payment_Criteria in the Formula Name field.
◦ Add a row in the Result Rules section using the values in this table.

Field

Value

Result Returned

EMP_DEPT

Result Rule

Direct Result

Target Input Value

Payment Criteria

407

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Field

Value

◦ Click Submit.

Related Topics

• Payment Sources in Organization Payment Methods Setup Examples

Personal Payment Methods

Overview of Personal Payment Methods

Personal payment methods (PPM) determine how you pay payroll payments to your employees. PPMs includes key
information, such as bank information for direct deposits, payment type and payment amount.

If personal payments aren't created for an employee, payments are made using the default organization payment
method for the employee's assigned payroll.

Related Topics

• Configure Payment Method Preferences

• How Payment Methods and Payroll Definitions Work Together

• Personal Payment Method Alerts Template

Bank Info for Personal Payment Methods

You can create bank, branch, and bank account info as part of implementation, or you can let employees add their own
bank info. Once created, you can use bank accounts in other Oracle applications, such as Cloud expenses.

Enter Bank Info for PPMs
This table summarizes approaches to create bank info for employees.

Approach

Purpose

Manage Banks and Manage Bank
Branches pages

Create, edit, and view your bank account information.

Note:
In order to manage banks and branches, you must have the Manage Bank and Manage Bank Branch
privileges.

408

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Approach

Purpose

Chapter 8
Payments

Payment Methods page

Create, edit and view employee bank account details to receive payroll payments.

HCM Data Loader

Use an integrated Excel workbook to load personal payment methods and employee bank account
details.

You can use CE_USE_EXISTING_BANK_BRANCH profile option to control to whether or not your employee can create
their own bank and branch data. On the Manage Cash Management Profile Options page, set the Use Existing Banks
and Branches profile option to either Yes or No.

•

•

If you set the option to Yes, you need to load bank and branch data. Administrators and employees select bank
and branch details from a list of values in the bank region on the Payment Method page.

If you set the option to No (default setting), you don't need to load any bank details. Administrators and
employees enter their bank and branch details as free text.

Access to PPMs and Bank Info
The table shows the privileges you need to access PPMs and bank info:

User

Privileges

Access Description

Employee Self-service

Manage Personal Payment Method

Employee Self-service

View Personal Payment Method

Allows users to manage their own personal
payment methods

Allows users to view their own personal
payment methods

Employee Self-service, Implementors,
Administrators, or Managers

Payee Bank Account Management Duty

Allows users to create bank accounts

Implementors, Administrators, or Managers

Manage Worker Personal Payment Method

Implementors, Administrators, or Managers

View Worker Personal Payment Method

Allows access to manage employee personal
payment methods

Allows access to view employee personal
payment methods.

Related Topics

• How Bank, Branch, and Account Components Work Together

• Configure Payment Method Preferences

• Examples of Loading Banks

• Examples of Loading Bank Branches

• Example of Loading Personal Payment Methods

409

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Configure Payment Method Preferences

Configure preferences related to payment methods within a legislative data group (LDG) using Payment Method
Preferences. Preferences are applied when your self-service employees enter payment methods for payroll payments.

Note:   If you support multiple organization payment methods of the same payment type, you MUST indicate which of
these should be available to your self-service users, using the Payment Method Preferences page.

Note:   If you intend to support multiple organization payment methods of the same payment type, then the
Organization Payment Method field will appear on the Payment Methods page.

Preference Rule

Action

Example

Legislative Data Group

Choose from the list of existing LDGs for the
Payment Method Preference.

Payment Method Preferences are applied to
LDGs. In all cases, choose your LDG for the
preference.

What organization payment methods should be
available for employees to select?

Choose from the list of existing OPMs for the
LDG you want available to your employees on
the Payment Method page.

Note: When you choose multiple OPMs for the
same payment type, employees will select from
an OPM list instead of a payment type list to set
up their personal payment methods.

You support check/cheque and EFT payment
methods but you only want checks/cheques to
be issued under certain circumstances. In this
case, choose your EFT OPM and don't choose
your check/cheque OPM from the list.

What is the maximum number of payment
methods an employee should be allowed to
create?

Enter the maximum number of payment
methods you want an employee to create.

You want to restrict the number of personal
payment methods employees can create to 1. In
this case, enter 1 into the field.

Note: This number means an employee can
create as many payment methods as they want
equal to or less than this number.

What payment amount types should be
available for employees to select?

Choose from the list of payment amount types
you want available to your employees on the
Personal Payments page.

You want employees to only create payment
methods with percentages. In this case, choose
Percentage from the list.

Note: The system default is Both.

What payment methods should employees not
be allowed to edit?

Choose from the list of existing OPMs for the
LDG you want to restrict your employees from
editing on the Payment Method page.

You support paying employees by Pay Card,
 however, you want the personal payment
method details to only be entered by
professional users. In this case, choose your pay
card OPM from the list for your employees to
view this information but not make any edits.

Should the above selected payment methods
be excluded from the 100% validation logic?

Choose Yes or No from the list to include the
available payment methods that aren't allowed

You support Pay Card, however, you want to
exclude this from the 100% validation rule
so that your employees' salary can't be split

410

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Preference Rule

Action

Example

to be edited but are included in the 100%
validation rule.

between Pay Card and another payment
method. In this case, choose Yes from the list.

Related Topics

• Bank Info for Personal Payment Methods

• Organization Payment Methods Overview

• Payment Method Rules Setup Examples

Prenotifications

The purpose of prenotifications is to validate routing numbers and account numbers of the receiving banks. Once you
have set up prenotifications for your organization payment method, the prenotification status is on in the professional
payment method page.

Depending on the prenote status, you may edit the prenotification status field to update the prenote status.

This table describes the prenote status and actions that you can take:

Prenote Status

Not Submitted

Submitted

Complete

Rejected

Marked as Complete

Description

Statuses available?

This status will show when the bank account is
first created and added to a payment method.

Marked as complete

This status will show when the payment
method is processed prepayments, for the
number of prenote days as defined in the
Organization Payment Method page.

Marked as complete

Rejected

This status will show when the prenote period
has completed.

N/A

This status can be set by the professional user if
the bank rejects the bank account information.

N/A

This status can be set by the professional user
if they want to bypass the prenote process for a
specific employee.

N/A

For example, your prenote process requires a 5 day wait period. You have a new hire, on a monthly payroll, with the first
period end date being the 30th Jan. They enter their bank account details on 15th Jan. When the payroll department
runs the prepayment process with an effective date of 30th Jan, the prenote statuses will appear as follows:

411

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Not Submitted

Submitted

15th Jan -29th Jan

30th Jan - 3rd Feb

Complete

4th Feb -

The employee will receive a check payment for the first payroll period and the bank account will be used for payment
effective 4th Feb and after.

Note:  A professional user can also update the prenote date field, when the status is submitted, if for example, they
need longer to verify the account.

Important prenotification banner messages show at the top of the page to let you know that the bank account isn't
currently used for payment because it's still in Submitted status or is in Rejected status. This table explains these banner
messages:

Prenotification Banner Message

Banner Shows on Page

This bank account will be used once the
prenote process is complete.

During Submitted status, from the time the bank is first entered and attached to a payment method
until the prenote process is complete.

This bank account was rejected during the
prenote process and will not be used.

During Rejected status, This will be shown when the bank has been marked as rejected.

Skip Prenotification

There are situations where you may choose to skip the prenote process, such as if you recently migrated data into HCM
Cloud and the bank prenote was completed in your legacy system. The prenote process automatically triggers when
new bank accounts are loaded. Because prepayments process pays the employees by check until prenote process is
complete, you must skip the prenote process to avoid this. Manually skip the prenote process or use HCM Data Loader.

Related Topics

• Organization Payment Methods Overview

• Example of Skipping Prenotes

• Payment Sources in Organization Payment Methods Setup Examples

Personal Payment Method Alerts Template

Personal payment method (PPM) alert template automatically sends personalized email notifications to employees.
Based on logic, the email notification includes details about the PPM type created, updated or deleted.

You can use the PPM_ALERT alert templates as delivered or deactivate the delivered template and create new to change
logic for notification generation, email content, font size, font style, graphics and links, to meet your communication
style.

412

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Use the Alerts Composer tool to enable and configure your email notifications. The templates are in Groovy
programming language and contain tokens. Tokens are placeholders where information specific to the alert is filled in
and included in the email notification.

These are the tokens supported by the personal payment method template:

Token

Definition

SessionUserName

User Name of the person performing the Operation self-service user or Administrative User.

UserName

ssoUser

PPMName

PersonId

User Name of the employee associated with the PPM.

Identifies when the action is performed by self-service user.

Name of the personal payment method.

Person Id of the employee associated with the PPM.

EffectiveStartDate

Effective Start date of the PPM.

EffectiveEndDate

Effective End date of the PPM.

Operation

Action performed on PPM, such as create, update, or delete.

CREATE_EFT

Identifies when the action creates an EFT source type of PPM. If PPM is created with an EFT source
Type, bank, branch, account number and masked account number are associated.

BankName

Name of bank associated with the PPM of EFT source type.

BankBranchName

Name of bank branch associated with the PPM of EFT source type.

MaskedAccountNum

Masked account number associated with the PPM of EFT source type.

CREATE_NON_EFT

Identifies when the PPM is created with a non-EFT source Type, like check.

UPDATE

Identifies when the PPM is updated.

CORRECTION

Identifies when the PPM is corrected.

END_DATED

Identifies when the PPM is end-dated.

ZAPPED

Identifies when the PPM is permanently deleted.

413

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Both the subject and body of the delivered template contain the same logic to determine when to send an email
notification, to whom, and what to include for each notification. However, the logic in the alert subject sends the content
for the subject, the logic in the alert body sends content for the body, and they're sent in one single email notification.
There are 6 Groovy expressions in each that cover the following 11 scenarios to send ppm alerts to the employee. With
the exception of the deletion of a personal payment method, each expression handles 2 scenarios using the common IF,
THEN, ELSE logic.

Scenario

Alert Logic

Email Notification

An EFT PPM (direct deposit) is created

Subject:

Hello <%if(UserName

and

it's created by the employee self-service user

<% if(Operation.equals('CREATE_EFT'))
{ %> <%if(ssoUser){%>Your PPM with bank
information was created<%}else{%>Your PPM
with bank information was created for you <
%}%> <%} %>

Your Personal Payment Method
(${PPMName}) with bank account ending with
${MaskedAccountNum} has been created
successfully.

Body:

Contact your Payroll Specialist with any
questions.

Hello <%if(UserName !=null){%>${UserName}<
%}%>z<BR>

Thank you

<% if(Operation.equals('CREATE_EFT')){ %>
<%if(ssoUser){%>Your Personal Payment
Method (${PPMName}) with bank account
ending with ${MaskedAccountNum} has
been created successfully. Contact your
Payroll Specialist with any questions.<
%}else{%> Your Personal Payment Method
(${PPMName}) with bank account ending with
${MaskedAccountNum} has been created for
you. Contact your Payroll Specialist with any
questions.<%}%> <%} %>

<BR>Thank you

An EFT PPM (direct deposit) is created

Same logic as above for the ELSE expression.

Subject:

and

it's NOT created by the employee self-service
user

A non-EFT PPM (check) is created

Subject:

and

it's created by the employee self-service user

Hello <%if(UserName !=null){%>${UserName}<
%}%>z<BR>

Hello <%if(UserName

Your PPM with bank information was created
for you

Body:

Your Personal Payment Method
(${PPMName}) with bank account ending with
${MaskedAccountNum} has been created for
you.

Contact your Payroll Specialist with any
questions.

Thank you

Your Personal Payment Method (${PPMName})
has been created successfully.

Contact your Payroll Specialist with any
questions.

414

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Scenario

Alert Logic

Email Notification

<% if(Operation.equals('CREATE_NON_EFT'))
{ %> <%if(ssoUser){%>Your PPM was created<
%}else{%> Your PPM was created for you <
%}%> <%} %>

Thank you

Body:

Hello <%if(UserName !=null){%>${UserName}<
%}%>z<BR>

<% if(Operation.equals('CREATE_NON_EFT'))
{ %> <%if(ssoUser){%>Your Personal Payment
Method (${PPMName}) has been created
successfully. Contact your Payroll Specialist
with any questions. <%}else{%>Your Personal
Payment Method (${PPMName}) has been
created successfully for you. Contact your
Payroll Specialist with any questions.<%}%> <
%} %>

<BR>Thank you

A non-EFT PPM (check) is created

Same logic as above for the ELSE expression.

Subject:

and

it's NOT created by the employee self-service
user

Your PPM was created for you

Body:

Hello <%if(UserName

Your Personal Payment Method (${PPMName})
has been created successfully for you.

Contact your Payroll Specialist with any
questions.

Thank you

A PPM is corrected

Subject:

Subject: Your PPM information was updated

and

it's corrected by the employee self-service user

<% if(Operation.equals('CORRECTION')){ %>
<%if(ssoUser){%>Your PPM information was
updated<%}else{%> Your PPM information was
updated for you<%}%><%} %>

Body:

Hello <%if(UserName

Body:

Your Personal Payment Method (${PPMName})
has been updated successfully.

Hello <%if(UserName !=null){%>${UserName}<
%}%>z<BR>

Contact your Payroll Specialist with any
questions.

Thank you

<% if(Operation.equals('CORRECTION')){ %>
<%if(ssoUser){%> Your Personal Payment
Method (${PPMName}) has been updated
successfully. Contact your Payroll Specialist
with any questions.<%}else{%>Your Personal
Payment Method (${PPMName}) has been
updated successfully for you. Contact your
Payroll Specialist with any questions. <%}%> <
%} %>

<BR>Thank you

415

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Scenario

Alert Logic

Email Notification

A PPM is corrected

Same logic as above for the ELSE expression.

Subject:

and

Your PPM information was updated for you

it's NOT corrected by the employee self-service
user

A PPM is updated

and

Subject: <% if(Operation.equals('UPDATE')){%>
<%if(ssoUser){%>Your PPM information was
updated<%}else{%> Your PPM information was
updated for you<%}%><%} %>

it's updated by the employee self-service user

Body:

Hello <%if(UserName !=null){%>${UserName}<
%}%>z<BR>

<% if(Operation.equals('UPDATE')){%> <
%if(ssoUser){%>Your Personal Payment
Method (${PPMName}) has been updated
successfully. Contact your Payroll Specialist
with any questions.<%}else{%>Your Personal
Payment Method (${PPMName}) has been
updated successfully for you. Contact your
Payroll Specialist with any questions. <%}%><
%} %>

<BR>Thank you

Body:

Hello <%if(UserName

Your Personal Payment Method (${PPMName})
has been updated successfully for you.

Contact your Payroll Specialist with any
questions.

Thank you

Subject:

Your PPM information was updated

Body:

Hello <%if(UserName

Your Personal Payment Method (${PPMName})
has been updated successfully. Contact your
Payroll Specialist with any questions.

Thank you

A PPM is updated

Same logic as above for the ELSE expression.

Subject:

and

Your PPM information was updated for you

it's NOT updated by the employee self-service
user

A PPM is end-dated

Subject:

Body:

Hello <%if(UserName

Your Personal Payment Method (${PPMName})
has been updated successfully for you.

Contact your Payroll Specialist with any
questions.

Thank you

Subject:

and

<% if(Operation.equals('END_DATED')){%> <
%if(ssoUser){%>Your PPM information was

Your PPM information was end-dated

416

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Scenario

Alert Logic

Email Notification

it's end-dated by the employee self-service user

end-dated<%}else{%> Your PPM information
was end-dated for you<%}%><%} %>

Body:

Hello <%if(UserName

Your Personal Payment Method (${PPMName})
has been end-dated as of ${EffectiveEndDate}.
Contact your Payroll Specialist with any
questions.

Thank you

Body:

Hello <%if(UserName !=null){%>${UserName}<
%}%>z<BR>

<% if(Operation.equals('END_DATED')){%>
<%if(ssoUser){%>Your Personal Payment
Method (${PPMName}) has been end-dated as
of ${EffectiveEndDate}. Contact your Payroll
Specialist with any questions. <%}else{%>Your
Personal Payment Method (${PPMName}) has
been end-dated as of ${EffectiveEndDate} for
you. Contact your Payroll Specialist with any
questions. <%}%><%} %>

<BR>Thank you

A PPM is end-dated

Same logic as above for the ELSE expression.

Subject:

and

it's NOT end-dated by the employee self-
service user

A PPM is deleted

Subject:

Hello <%if(UserName

Your PPM information was end-dated for you

Body:

Your Personal Payment Method (${PPMName})
has been end-dated as of ${EffectiveEndDate}
for you. Contact your Payroll Specialist with any
questions.

Thank you

Subject:

and

<% if(Operation.equals('ZAPPED')){%> Your
PPM information was deleted for you<%}%>

Hello <%if(UserName

there is no condition for type of user

Your PPM information was deleted for you

Body:

Hello <%if(UserName !=null){%>${UserName}<
%}%>z<BR>

<% if(Operation.equals('ZAPPED')){%> Your
Personal Payment Method (${PPMName}) has
been permanently deleted for you. Contact your
Payroll Specialist with any questions.<%} %>

<BR>Thank you

Body:

Your Personal Payment Method (${PPMName})
has been permanently deleted for you. Contact
your Payroll Specialist with any questions

Thank you

Related Topics

• Personal Payment Methods

• Functions and Groovy Expressions

417

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

FAQs for Personal Payment Methods

Why does an inactive bank account still shows as active?
Your bank account is active until the end of the day you marked it inactive. An end date is saved as of the date you mark
your bank account inactive and remains active until midnight of its inactive date.

For example, if today is the 25th of January and you mark your bank account as inactive, it's active until midnight.
Tomorrow, 26th of January, when you view your bank account in the payment method page, your bank account shows
an inactive status with the end date.

Note:  If your inactive bank account is linked to a payment method, you see a reminder banner on the payment
method page to associate an active bank account with your payment method.

Related Topics

• Bank Info for Personal Payment Methods

• Considerations When You Create Accounts

Why can't I select a bank account in the payment source page?
In order for a bank account to appear in the payment source page it must be associated to a Payroll Statutory Unit (PSU),
enabled for payroll payments and active.

Check these items for compliance:

• Assign a PSU legal entity to the bank account or a legal employer with a parent PSU to the bank account.

• Select Payroll in the bank account Account Use option.

• Effective dates of payment source must be within effective dates of the bank account.

Related Topics

• Payment Sources in Organization Payment Methods Setup Examples

Third-Party Payment Methods

Third-Party Payment Methods Overview

A third party is any person or entity outside of your organization and a third-party payment method (TPPM) determines
how you pay them. TPPMs includes key information, such as bank information for direct deposits, and payment type.

418

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Related Topics

• Third-Party Payment Methods

• Employee and Third-Party Check Payments Overview

• Employee and Third-Party Check Payments Process

• Examples of Third-Party Payments

• Third Parties Overview

Third Parties Overview

You create third parties to process payments to external organizations and to people who aren't on the payroll. Use the
Third Parties task to create third-party persons or organizations, such as pension providers, professional bodies, or
disability organizations.

Note:  When you create third-party persons and organizations, they're also defined as trading community members
in the Trading Community Architecture (TCA), to allow use in other products.

This shows you the decision steps to create third parties.

Party Usage Codes
For third-party persons, the application automatically assigns a party usage code of External Payee. For third-party
organizations, you assign a party usage code.

This table describes the party usage codes for third-party organizations.

419

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Party Usage Code

Use For

Examples

External Payee

Organizations when the others party usage
codes don't apply.

State Disbursement Unit for child support
payments

Payment Issuing Authority

Pension Provider

Professional Body

Bargaining Association

Organizations responsible for issuing
instructions for involuntary deductions, such
as a tax levy or bankruptcy payment order.
Payment issuing authorities don't receive
payments.

Court, agency, or government official

Organizations that provide pension
administration for employee pension
deductions.

Stock broker, investment company, benefit
administrator, labor union

Organizations entrusted with maintaining
oversight of the legitimate practice of a
professional occupation.

The American Society for Mechanical Engineers
in the US

Organizations that represent employees
in negotiations. Bargaining associations
associated with trade unions may receive
payments for union fees deducted from an
employee's pay.

The Air Line Pilots Association International
(ALPA) in Canada and the US

Disability Organization

Organizations that are authorized to make
disability assessments. Disability organizations
don't receive payments.

The Royal National Institute of Blind People in
the UK

Related Topics

• Third-Party Payment Methods

• How Payment Methods and Payroll Definitions Work Together

• Example of Loading Organization Payment Methods

• Example of Loading Third-Party Personal Payment Method

• How do I import organization data?

Third-Party Payment Methods

Create third-party payment methods for third-party persons or external organizations. Use either the Third-Party
Personal Payment Methods task or the Third-Party Organization Payment Methods task to create.

Typical payments to third parties include:

•

Involuntary deductions, such as court-ordered garnishment.

• Voluntary deductions, such as pension plan or union membership payments.

420

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Note:  You must use the Third Parties task to create the third party and ensure the organization payment method for
the payment source exists before you create a third-party payment method.

As you create your third-party organization payment methods, you will notice additional fields that can be captured,
such as whether or not to exclude the third party from the Run Third-Party Payment Rollup process or to separate
worker payments by reference. These identifiers will determine how these payees are paid and reported at the time of
payment.

• Use the Exclude from Third-Party Rollup Process checkbox, if you run the Run Third-Party Payment Rollup
but have to pay certain third parties that require an individual check per employee payment. For example,
the UK requires deduction from earnings orders, such as child maintenance payments, to be sent as separate
transactions. By checking this box, payments to this third party, won't be rolled up into a single payment.

Note:  When checking this box, the Separate Worker Payments by Reference box is automatically checked
because it's typical for an employee making multiple payments to this third party that each payment is to be
reported by reference separately. However, you may deselect, if this is your requirement.

• Use the Separate Worker Payments by Reference checkbox to generate employee payments to a given third
party, based on reference. For example, if an employee is making multiple payments to a given third party,
these can be generated separately, each with the corresponding reference.

Note:  The calculation card's calculation component has a reference field to uniquely identify the deduction,
such as a court order number, case number, or other identifier provided by the issuing authority. The
prepayment process breaks down the employee payments by this reference number captured against the
employee deduction, which is mandatory for all countries.

You can still select the Separate Worker Payments by Reference checkbox even if you don't select the Exclude from
Third-Party Payment Rollup Process checkbox to roll up the third-party payment and separate employee payments
based on reference. These choices allow you to roll up the third-party payments during the Run Third-Party Payment
Rollup process and separated out by on reference during the prepayments process the employee payments to that
third party. You can then retrieve the information if you need to extract the details in the payment file, or reports. For
example, you need to send a single consolidated payment to a loan company but you also need the employee payments
paid to multiple loans at the same loan company separated out.

• Use the Time Definition list of values to pay a third-party on a date that's different from the employee payment
date. For example, you want to make employee payroll payments on the last day of the month and make third-
party payments 5 days later.

To create a third-party organization payment method, follow these steps:

1. Select the Third-Party Organization Payment Methods task.
2. Click the Create icon.
3. Select a Legislative Data Group.
4. Select the Third-Party Name from the list.
5. Select the Organization Payment Method from the list.

Note:  Payment Type and Currency populate based on chosen Organization Payment Method.

6. Select Effective Start Date.
7. Select Exclude from Third-Party Payment Rollup Process, if the third party isn't part of the Run Third-Party

Payment Rollup.

8. Select Separate Worker Payments by Reference if separate payments are generated for employee payments to a

given third party, based on reference.

421

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

9. Select the Time Definitions from the list, if you have defined a time definition to pay the third party on a

10.

different date than the rest of your third-party payments.
If you're creating a direct deposit to a third party, perform these additional steps in the Bank Account region to
create the associated bank account.

◦ Click the Create icon.
◦ At a minimum, fill in the required fields identified by an asterisk.

- *Account Number
- *Account Type
- Check Digit
- Account Holder
- Secondary Account Reference
- *Bank
- *Bank Branch
- *Routing Number
◦ Click the Save and Done button.

11. Click Save.
12. Click Done.

To create a third-party personal payment method, follow these steps:

1. Select the Third-Party Person Payment Methods task.
2. Search and select an employee.
3. Click the Create icon.
4. Select a Legislative Data Group.
5. Select the Third-Party Name from the list.
6. Select the Organization Payment Method from the list.

Note:  Payment Type and Currency are based on chosen Organization Payment Method.

7. Select Effective Start Date.
8.

If you're creating a direct deposit to a third party, perform these additional steps in the Bank Account region to
create the associated bank account.

◦ Click the Create icon.
◦ At a minimum, fill in the required fields identified by an asterisk.

- *Account Number
- *Account Type
- Check Digit
- Account Holder
- Secondary Account Reference
- *Bank
- *Bank Branch
- *Routing Number
◦ Click the Save and Done button.

Note:  Depending on your localization, these may differ.

9. Click Save.

422

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

10. Click Done.

Chapter 8
Payments

Note:  The payroll relationship is defaulted for the employee making the payment to the third party. However, if
you create a third-party personal payment method, as part of creating your third party, you must select the payroll
relationship(s) of the person making payment to the third party.

Related Topics

• Organization Payment Methods Overview

• Third-Party Payment Date Options

Third-Party Payment Date Options

Use time definitions when a third-party payee wants payment on a date that's different from the employee payment
date.

Note:  The time definition setup applies only to check/cheque payment types.

A time definition is either a date or a span of time. For example, employee payroll payments are on the last day of the
month, whereas third-party payments are five days later. Create a time definition to define the time span and select this
definition while defining the payment method for this payee.

Use the Time Definitions task to create your time definition for a time span of 5 days with values in this table.

Field

Name

Value

Specify a name: Third Party 5 Days

Short Name

Specify a short name: TP5Days

Type

Period Type

Period Unit

Specify a type: Time Span

Specify a period type: Daily

Specify the unit: 5

Adjustment Type

Specify type of adjustment: Days

Time Span Usages

Specify a usage for the time span: Third-Party Payments

Use the Time Definition field on the Third-Party Payment Methods page to assign this time definition.

Run the Generate Payments for Employees and Third Parties process twice, one for the employees and one for the
third-party payees. Select the relevant process end date and enter an overriding payment date.

423

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Related Topics

• Third-Party Payment Rollup

• Employee and Third-Party Check Payments Overview

• Third-Party Payment Methods

• Third-Party Payment Methods Overview

• Time Definitions

Chapter 8
Payments

Examples of Third-Party Payments

These scenarios show you how to pay third-party payees. Third-party payees can be an individual person or an
organization.

Child Support to a Former Spouse
While this example illustrates payment directly to a third-party person, most child support payments are payable to a
third-party organization such as a State Disbursement Unit.

John Smith is an employee at your organization. Mary Smith receives a child-support payment each payroll period
that's deducted from John's salary. To set up payments for Mary:

1. Create Mary as a third-party person.
2. Create Mary's third-party payment method and select the payroll relationship for John.
3. Add the child support order to John's involuntary deduction calculation card and select Mary's name in the

Order Amount Payee field.

Organization Processing Fee to a County Sheriff's Office
The County Sheriff's office receives an organization fee on garnishment payments. When you create the third-party
organization, designate it as an external payee before you create its third-party payment method. When you add
the garnishment order to the employee's involuntary deduction calculation card, select the County Sheriff in the
Organization Fee Payee field.

Related Topics

• Third-Party Payment Methods Overview

• Third Parties Overview

• Third-Party Payment Methods

• How do I generate payments to third-party payees?

424

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Third-Party Payments

Third-Party Payment Rollup

A third-party payment is a payment you make to an external organization or to a person that isn't on the payroll.

The Run Third-Party Payment Rollup is an optional process to consolidate payments to a third-party payee into one
payment, rather than make multiple individual payments to the same third-party payee. For example, you may have
multiple employees that are members of the same union and you'd like to pay the union with one payment. Or, you
may have an employee with multiple deductions payable to the same third-party payee, such as multiple child support
orders to the children's parent. Use the Submit a Flow task to run the Run Third-Party Payment Rollup.

Third-Party Payment Register Details
You can Run Third-Party Payments Register Report to provide payment details to the third-party payee, to include the
breakout of rollup payments. Use the Submit a Flow task to run the Run Third-Party Payment Register Report.

Here are the details in the output of the Run Third-Party Payments Register Report:

•

Individual third-party payments with the corresponding employee deduction information

• Rollup payments and deduction information of employees who share the same rollup payments

• Consolidated total of each rollup payment

• Payments made to each individual payee

• Consolidated total of multiple deduction payments of each employee

• Component name and component reference of involuntary deductions stored on the calculation cards

• Element name of voluntary deductions

Perform these tasks, in order, to roll up the third-party payments and generate the report details:

1. Calculate and verify prepayments.
2. Run the third-party payment rollup process.
3. Generate the payments.
4. Generate the third-party payment register.

Related Topics

• Employee and Third-Party Check Payments Process

• Third-Party Payment Methods Overview

• Third-Party Payment Date Options

• Calculate Payroll Payment Distribution

425

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Generate Employee and Third-Party Check Payments

Once you have calculated payroll, you're ready to pay your employees and third parties. Use the Generate Payments for
Employees and Third Parties flow to generate check/cheque payments.

This process selects employees and third parties processed in the prepayments process within the payroll run and have
a payment method of check/cheque.

Before you generate the check/cheque payments, consider these scenarios:

• You may have multiple employee deductions made to the same third-party payee, such as multiple child

support orders. Rather than make individual payments for each individual employee deduction, use the Run
Third-Party Payment Rollup process to combine individual employee deductions and make a single payment to
the payee.

• You may have both employees and third parties to pay. Use the Run Generate Payments for Employees and

Third Parties to generate your checks/cheques for employees and then again to generate checks/cheques for
your third parties. Use the Payee Type field to designate which will be included in the process.

• You may have specific third parties to exclude from the Run Third-Party Payment Rollup process to produce an
individual check/cheque per payment. Select the Exclude from Third-Party Payment Rollup Process checkbox
on the Third-Party Organization Payment Methods page to exclude a third-party payee from the Run Third-
Party Payment Rollup process.

• You may have a third-party payee that requires payments on a date that's different from the employee payment
date. For example, your employee payroll payments are on the last day of the month but you may want to make
third-party payments 5 days later. Use the Time Definitions task to create a time definition defining a time span
of 5 days. Select this new time definition in the Time Definition field on the Third-Party Person or Organization
Payment Methods UI. Enter the relevant process dates and run the prepayments process, for example, with a
process date of 30, June. This stamps the effective employee payments date as 30-June and the third-party
payments date as 05-July. The Generate Payments for Employees and Third Parties process is run twice:

◦ Once for the employees with a last day of the month process end date, such as 30-June
◦ Once for the third parties with a process end date of plus 5, such as 05-July, and an overriding payment

date of 05-July

• You may have different banks with different check/cheque templates. To accommodate, you must create a

report category for each separate bank and check/cheque template and then attach it to the payment source:

◦ Define report categories for each unique bank and check/cheque template combination to create a
report category for each separate bank and check/cheque template. Use the Organization Payment
Methods page to associate the report category for third-party payee and report category for worker to
the payment source.

◦ Select the new report category for the requisite bank's payment source so that the process uses the
correct check/cheque template when generating its check/cheque payments. Use the Organization
Payment Methods task to define the payment source for third-party payments. Attach the correct report
category for that payment source. Use the Report Category for Third-Party Payee or Report Category for
Worker field in the Payee Information section of the Create Payment Source page.

• Define report categories for each unique bank and check/cheque template combination if you want to create a
report category for each separate bank and check/cheque template. The report category for third-party payee
and report category for worker are associated to the payment source in the Organization Payment Methods
page.

426

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Related Topics

• Third-Party Payment Rollup

• Third Parties Overview

• Third-Party Payment Methods

• Employee and Third-Party Check Payments Process

Chapter 8
Payments

Employee and Third-Party Check Payments Process

The Generate Payments for Employees and Third Parties flow selects employees and third parties that:

• Are processed in the prepayments process for a given payroll.

• Have a payment method of check/cheque.

Submit the Generate Payments for Employees and Third Parties flow from the Submit a Flow page.

Prerequisites
The prerequisite tasks for the Generate Payments for Employees and Third Parties task include:

• Create the third party, create the third-party payment method, and associate an employee deduction to pay the

third party.

• Add an organization payment method (OPM), to include a payment source.

Note:  The bank details should already be set up.

• Add a payroll definition, to include a default payment method of check/cheque, and all valid payment methods.

• Attach a payroll to the employee.

• Attach element entries to the employee.

• Calculate payroll.

• Run the Calculate Prepayments process to calculate the distribution of net pay.

• Run the Archive Periodic Payroll Results process to archive the earnings, deductions, tax calculation details,

accruals, payment methods, and so on.

Generate Employee and Third-Party Payments
Run this process to generate checks/cheques for your employees and then run the process again to generate checks/
cheques for your third parties.

Follow these steps to run the Generate Payments for Employees and Third Parties flow from the Submit a Flow page:

1. Click Submit a Flow.
2. Select the required legislative data group.
3. Select the Generate Payments for Employees and Third Parties and click Next.
4. Enter a unique payroll flow name.

Note:  Name the flow with a name to easily identify the process later. You need to be able to determine what
you have already run and you may need to locate it to roll back the process.

427

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

5. Specify the required payroll name.
6. Select the payee type for which the check/cheque payment process is run. The available options are Employee

or Third Party. You can generate the check payments for either employees or third parties.

7. Enter a Process Start Date to define the date range of this process.
8. Enter a Process End Date to define the date range of this process.
9. Select the required consolidation group to view the payments for all payrolls that are included in this

consolidation group.

Note:  A consolidation group defines a grouping of different payrolls for reporting purposes. This isn't a
mandatory field. If you don't select a value, the process uses the default consolidation group assigned to the
payroll.

10. Select the OPM you want to use for this process.

Note:  The value you select determines the payment source to make the payments. There could be multiple
payment sources in the OPM.

11. Select the payment source to process for the above payment method. This parameter is optional. If you have

defined attributes, such as a payment file limit or report category, at the payment source level, you should enter
the payment source. When you enter the payment source, the defined attributes are applied.

Note:  You can have different payment sources (bank accounts), with different banks, which have different
check/cheque templates. You must then run the check/cheque process for each payment source and each
set of payees. Select the correct payment source so that the correct stationary is used for the payments.

Tip:  To accommodate this requirement, you must first create a report category for each separate bank and
check/cheque template. Attach the created report category to the appropriate bank's payment source so that
the correct check/cheque template is used to generate the check/cheque payments.

12. Optionally, specify an Overriding Payment Date on which a payment is due to be made to the payee.
13. Specify the Start Check/cheque Number in the sequence of checks/cheques used for payroll processing.
14. Specify the End Check/cheque Number in the sequence of checks/cheque used for payroll processing.
15. Select a Process Configuration Group if available. Use a process configuration group to set rules for payroll
processes, such as passwords or number of threads. If you don't select a process configuration group, the
process uses the parameters in the default group.

16. Click Next.
17. Click Submit.

Related Topics

• Third-Party Payment Rollup

• Employee and Third-Party Check Payments Overview

• Examples of Using Consolidation Groups

• Payroll Process Configuration Groups

428

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Reprocess Rejected EFT Payments

Overview of Reprocessing Rejected EFT Payments

A bank can reject an Electronic Funds Transfer (EFT) payment because of:

•

Incorrect bank account details

• Employee has closed their bank account without notifying the employer

Here's what you can do to reissue a check:

• End date the employee's personal payment method

•

Inactivate the employee's bank account. You must inactivate the invalid bank account so that it's not used for
future payments.

• Void the payment and make an external payment against the rejected EFT payment.

Use the Process Bank Corrections File flow pattern from the Payroll Checklist work area to reissue check payments
against rejected EFT payments.

Before you run the flow, complete these tasks.

1. Transform the information returned by the bank into the requisite Object Group HCM Data Loader file format.
2. Provide a unique name in the Object Group Name field each time you create an HCM Data Loader file.
3. Load the Object Group HCM Data Loader file into the Oracle Web Center Content server.

Here's the list of payroll tasks the Process Bank Corrections File flow pattern includes:

Task Name

Description

1. Upload Bank Corrections File

Stores the information entered in the Object Group HCM Data Loader file into the object group table.
The bank information is stored in the object group table, under the 'Process Information Group' object
group type in the payroll application.

2. Update Personal Payment Methods

Determines through this built-in logic whether the personal payment method needs end dating or
updating. The logic is as follows:

•

•

If there is a value in the Replacement Bank Number, the Replacement Account Number, or the
Replacement Account Type field, then the process updates the Personal Payment Method.

If any of the above mentioned fields are blank, then the process end dates the Personal Payment
Method.

This task uses the Payment Reference number to identify the Personal Payment Method linked to the
bank account identified as incorrect. It also inactivates the incorrect bank details to stop them being
used in future payments.

Note:
The flow task doesn't create a new Personal Payment Method. You must create one manually.

3. Void Payments

Marks the original payments as void.

429

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Task Name

Description

Chapter 8
Payments

4. Make External Payments

Runs the external payment process to ensure that the payments voided in the previous task are paid
externally.

5. Generate Check Payments

Runs the HCM Extract Report to retrieve the check number and other information from the external
payment record to produce the report output. The delivered HCM Extract Report has a built-in logic to
generate the check number, if not available.

Steps 3-5 run only if you have to reissue an external check for a rejected EFT payment.

Note:  You can use the delivered default check template or configure the template to include additional attributes
such as a company logo.

Since a payslip is already issued, this flow doesn't generate the payslip.

Related Topics

• Object Group HCM Data Loader Files for Bank Reprocessing

Object Group HCM Data Loader Files for Bank Reprocessing

Before you run the Process Bank Corrections File flow, use the HCM Data Loader to load the information returned by the
bank.

The bank returns a file containing details of the payments that are rejected. Before you load the information, transform
this information returned by the bank into the HCM Data Loader .dat file formats required by the Object Group HCM
Data Loader.

Provide a unique name in the Object Group Name field each time you create an HCM Data Loader .dat file. You must
then load the Object Group HCM Data Loader file into the Oracle Web Center Content server.

The bank information is stored in the Object Group table, under the Process Information Group Object Group Type. Use
the Object Group UI and the name given in the Object Group HCM Data Loader file to view the information loaded by
the ObjectGroup.dat and ObjectGroupStore.dat files, as part of the Process Bank Corrections Flow.

When you load the ObjectGroupStore.dat file into the Oracle Web Center Content server, a UCM ID is generated. The
Process Bank Corrections File flow uses the UCM ID to retrieve and use the bank information necessary for the flow.

Load Process Information Group Object Group
Create and use the following HCM Data Loader .dat files to process the bank information by the HCM Data Loader.

• ObjectGroup.dat file to create the object group

• ObjectGroupStore.dat file to load the bank information returned by the bank

ObjectGroup.dat File Format
This table lists the attributes for loading the ObjectGroup.dat file.

430

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

HCM Data Loader Attribute

Required

User Interface Prompt

Description

ObjectGroupName

ObjectGroupCode

LegislativeDataGroup

ObjectGroupTypeCode

StartDate

EndDate

Yes

Yes

Yes

Yes

Yes

Yes

Name

The name of the object.

Doesn't appear on the UI.

The code of the object group.

Legislative Data Group

THE NAME OF THE LEGISLATIVE
DATA GROUP.

The meaning of the code is
displayed in the Type field.

The code of the object group
type. The supported value for the
process information group type is
PROCINFO.

Start Date

The start date of the object group.

End Date

The end date of the object group.

ObjectGroupStore.dat File Format
This table lists the attributes for loading the ObjectGroupStore.dat file.

HCM Data Loader Attribute

Required

User Interface Prompt

Description

ObjectGroupCode

Doesn't appear on the UI.

The code of the object group.

LegislativeDataGroup

Legislative Data Group

SequenceNumber

Yes

Sequence

assignmentNumber

Assignment Number

paymentDate

processDate

Payment Date

Process Date

THE NAME OF THE LEGISLATIVE
DATA GROUP.

A unique identifier for a row of data
in the object group store file.

The assignment number of
the employee whose payment
is rejected, or whose bank
information needs updating.

The original payment date of the
rejected payment.

This date overrides the process
date entered in the flow. The date
entered here, is stamped against
each process in the flow. It's the
date the personal payment method
is end dated and the payment is
voided. Enter a value if you want
one particular payment to have a
different payment date to that of

431

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

HCM Data Loader Attribute

Required

User Interface Prompt

Description

paymentReference

Yes

Payment Reference

Amount

checkNumber

Amount

Check Number

replacementBranchNumber

Replacement Branch Number

replacementAccountType

Replacement Account Type

replacementAccountNumber

Replacement Account Number

makeExternalPayment

Make External Payment

Returnreasoncode

Return Reason Code

Employeename

Employee Name

the payment date entered in the
flow.

A unique identifier for a specific
payment line, such as the payment
in the original NACHA file that was
sent to the bank.

The original amount of the rejected
payment.

The check number used in the
External manual payment task and
printed on the manual external
payment check template.

Enter a value if the branch number
(routing transit number) needs
updating. If a value is entered in
this column, it tells the process that
the bank account associated to the
personal payment method (PPM)
used for payment needs updating.

Enter a value if the employee's
account type needs updating. If
a value is entered in this column,
 it tells the process that the bank
account associated to the PPM
used for payment needs updating.

Enter a value if the employee's
account number needs updating.
If data is entered in this column,
 it tells the process that the bank
account associated to the PPM
used for payment needs updating.

Enter 'Yes' if you want to void
the original payment and make a
manual external check payment.
Valid values for this attribute are
'Yes' or 'No'.

The reason for rejecting an EFT
payment. The entered value is
stamped on the external manual
pay record.

Name of the employee whose
payment is rejected, or whose bank
information needs updating.

432

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

The Update Personal Payment Methods task within the flow determines, through built in logic, whether the personal
payment method needs end dating or updating. The logic is as follows:

•

•

If there's a value in the 'Replacement Branch Number' field, the 'Replacement Account Number' field or the
'Replacement Account Type' field, then the process updates the Personal Payment Method.

If any of the above mentioned fields are null then the process end dates the Personal Payment Method.

You can delete information loaded to the process information group object group type using the HCM Data Loader. You
must take care when deleting the records, because you can't recover the deleted records.

For more information on creating the HCM Data Loader .dat files and using the HCM Data Loader to upload data, refer
to the HCM Data Loader User's Guide on My Oracle Support.

Related Topics

• Reprocessing Rejected EFT Payments

Configure Payslips and Checks

Overview of Online Payslip

A payslip is a printable record of a payment made to an employee during a payroll pay period or as a bonus or
commission payment.

It includes details of the payment, such as employee and employer information, pay period, earnings, deductions and
accruals, and net pay distribution details.

Use these two predefined templates to configure the payslip template to include your specific statutory requirements:

• Payslip Main Template

• Payslip Sub Template

For more information, refer to 'Configure the Payslip Report Template' topic in the Help Center.

After you configure the payslip template, and before you generate the payslips, consider the following.

Task

Where to find more information

Generate the worker's payslips in a
language of their choice depending on
what's set as the workers correspondence
language.

Refer to these topics in the Help Center:

• Multilanguage Support for Payslips

• Generate Payslips in the Worker's Correspondence Language

• Add Bursting to Print Delivery Option

Mask or encrypt bank account information
to prevent display of sensitive information.

Refer to 'How Account Number Masking in Payroll Reports Work' in the Help Center.

Set the precision value for the number of
decimal places for the rates displayed on
the payslip.

Refer to 'Rate Precision in Payslips' in the Help Center.

433

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Task

Where to find more information

Add text and input values to payslips.

Refer to 'How to Add Text to Payslips and Checks' and 'Examples of Input Values for Payslip and Check
Text' in the Help Center.

The Generate Payslips process is run once each payroll period and it generates the payslip XMLs based on the payroll
archive and prepayments data. The payslip PDFs are created and stored in the Document of Records for future
reference and retrieval.

During the payslip process, payslip template files get downloaded, including files for multiple installed languages. You
can quickly retrieve payslip templates that support large templates or multiple templates for different languages.

You can preview payslips PDF documents directly from the Payslip page without having to download. Use options
in payslip preview window to zoom, scroll, print, download, or save payslip document. Use back arrow to exit payslip
preview window and return to payslip list.

Multicurrency Support for Payslips Page

Configure the payslip page to support multicurrency payments.

A typical international organization, such as a United Nations organization, has employees working in many different
countries. These employees often receive salary payments in a currency other than their base currency, such as
the currency of their work location or the currency of their home country. The base currency is the currency of the
legislative data group (LDG) you belong to.

In some instances, the employee chooses to receive salary payments split between multiple currencies. For example,
John opts to receive 50% of his salary in GBP and remaining pay in the bank account of his home .

John has a calculated net pay of 1000 USD of which 50% converts to 375 GBP and the remaining 50% is 500 USD. The
payslip page displays a net pay value in the base currency.

To configure the payslip page for multicurrency payments, perform the following:

• Create an organization payment method with payment type of international transfer.

• Configure personal payment methods with an international transfer payment type and associate to the

international bank accounts.

For our example:

a. Define two bank accounts and two personal payment methods for John, one for the US and one for the

UK.

b. When you create the personal payment method for the UK bank account, select international transfer as

the payment type and associate the UK bank account.

c. Enable the ORA_PAY_PAYSLIP_DISPLAY_NET_PAY_BALANCE_CURRENCY for the payslip page to reflect

correct net pay amount, in the base currency of the LDG.

Related Topics

• Overview of Online Payslip

434

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

How to Configure the Payslip Report Template

Use the predefined payslip template and edit it to include legislative requirements as mandated by your country or
territory. For example, you may want to add your company logo or add additional fields to the template.

Configuring the delivered payslip template includes these tasks:

1. Create a copy of the delivered payslip report
2. Edit a copy of the payslip sub template to include additional components as per your requirements
3. Add the changed template to the report
4. Set the priority of the payslip report as Critical
5. Test the configured payslip report in BI Publisher

Create a Copy of the Delivered Payslip Report
You can use the Customize function (if available) to create an editable copy of the delivered report in the Custom folder.

• The copied report has the same privileges as original report.

• Creates the necessary folder structure and keeps the same name as the original Payslip report.

• Ensures that the copied report is placed in the same folder structure under the 'Custom' folder and the BI
Publisher automatically chooses to use this modified report and you don't have to add the delivery option
changes.

•

If you choose to copy the template, you must manually add the delivery options.

Note:  You must have BI Publisher Developer or BI Publisher Administrator role to create or edit reports from the BI
Publisher.

If the Customize option isn’t available, manually copy the report or template into the Custom folder.

Complete these steps to copy the delivered report template.

1. Sign in to the Oracle BI Publisher using an environment link or URL that ends with ‘xmlpserver’.
2. Click Catalog to open BI analytics.
3. Navigate to /Shared Folders/Human Capital Management/Payroll/Regulatory and Tax Reporting/

Country Name folder to open the delivered Payslip for a country.

For example, for Canada, you can find the Canada Payslip Report at /Shared Folders/Human Capital
Management/Payroll/Regulatory and Tax Reporting/Canada folder.

4. Select More > Customize for the payslip report.
5. Navigate to /Shared Folders/Custom/Human Capital Management/Payroll/ Regulatory and Tax

Reporting/Country Name folder and check if you can see the customized report in the folder.

It is recommended that you save all user-defined or configured reports in the Custom catalog folder under
Shared Folders. Any reports created outside of the Custom folder will not be migrated and will be lost during
patching or upgrade.

435

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Edit Copy of the Payslip Sub Template
A BI report can have multiple layouts. Find the template or layout you’re trying to change. For example, edit the
delivered Payslip Sub Template and include the legislative and statutory changes you want to incorporate.

1. Navigate to /Shared Folders/Human Capital Management/Payroll/Payment Distribution/Payslip Sub

Templates.

2. Click Edit. Select the layout you want to edit, Payslip Sub Template.
3. Click Property.
4. Download the layout template (RTF), make required changes, and upload the revised template into the Custom

folder.

For more information on how you can edit RTF report template, refer to these topics on the Oracle Help Center.

• Create and Edit RTF Report Layout Templates

• How can I change the logo in the layout template?

Add the Revised Template to the Copied Report
Use these steps to add the revised template to the report you created in the first task.

1. Navigate to /Shared Folders/Custom/Human Capital Management/Payroll/Payment Distribution/

Payslip Sub Templates.

2. Click Edit.
3. Click Add New Layout.
4. Select Upload and enter these details in the Upload Template File page.

Field

Value

Layout Name

Name of the report you created in the first task.

Template Name

Select the template you just modified in the second task.

Type

Locale

RTF

English

5. Click OK to upload and overwrite the current template.
6. Click Return to review all the layouts. Use the Save icon to save all the changes.

The Priority of payslip report on the BI server is by default set as Normal and hence is processed on first in,
first out basis. To avoid interruptions, set the priority of the payslip report as Critical, so that it is executed on
priority.

a. Navigate to the copied report in the /Shared Folders/Custom/Human Capital Management/Payroll/

Regulatory and Tax Reporting folder.

Note:  You should make any revisions only to the copied version of the report.

b. Click Edit and then click Properties.
c. On the Report Properties window, under the General tab, select Critical in the Job Priority field.

436

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

d. Click OK.

Chapter 8
Payments

Note:  Setting the report as critical reduces chances of failure when there is an issue with the BI server
or a performance issue with a previous report job in the process.

Test the Configured Payslip Template in BI Publisher
To test the configured template, you must first run the delivered template and generate the payslip.

1. Navigate to /Shared Folders/Human Capital Management/Payroll/ Regulatory and Tax Reporting/

Country Name folder to open the delivered Online Payslip for the country.

2. Select Job History for the delivered report.
3. Clear the value of the fields Start Processing and Owner.
4. Click Search and choose first row with success status.
5. Click Report Job Name link.
6. Record the value of these fields: Archive Action Identifier, Delivery Option Identifier, and Payroll Action

Identifier.

7. Follow these steps to test your configured report template in the custom folder.

a. Navigate to /Shared Folders/Custom/Human Capital Management/Payroll/ Regulatory and Tax

Reporting/Country Name folder and open the report you created.

b. Enter values for Archive Action Identifier, Delivery Option Identifier, and Payroll Action Identifier fields

you noted.
c. Click Apply.
a. Verify that the payslip is generated successfully.

Note:  If the payslip didn't generate successfully, check your configured report and template for errors.

Enable the Redwood Payslip Report Template in your Custom
Folder

When you enable the Redwood Payslip template profile option, the payslip process uses the Redwood Payslip template.

If an existing customization exists, the BI Publisher resolves templates from the Custom folder.

If the Redwood Payslip Template isn’t available in the Custom folder of the BI Publisher and the profile option is enabled
(and an existing customization exists), the Payslip process fails.

The Redwood Payslip is generated using BI Publisher and is independent of the ORA_HCM_VBCS_PWA_ENABLED
profile option.

After you have enabled the redesigned Redwood Payslip template, complete these two steps:

1. Ensure Redwood Payslip Template exists in your Custom folder.
2. Create the custom Redwood payslip.

Ensure Redwood Payslip Template Exists in your Custom Folder
If you enable the Redwood Payslip profile option, ensure that the Redwood Payslip Template exists in the Custom folder.

437

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Here’s how to navigate to the custom folder for a country:

1. Sign in to the Oracle BI Publisher using an environment link or URL that ends with ‘xmlpserver’.
2. Click Catalog to open BI analytics.
3. Navigate to the custom folder for a country: /Shared Folders/Custom/Human Capital Management/

Payroll/ Regulatory and Tax Reporting / Country Name folder.

For example, for Canada, you can find the custom Canada Payslip Report at: /Shared Folders/Custom/Human Capital
Management/Payroll/Regulatory and Tax Reporting/Canada folder.

The Custom folder can contain multiple layouts. Ensure the correct Redwood template exists when the Redwood profile
option is enabled.

Create the Custom Redwood Payslip
If the correct Redwood template isn't available in the custom folder, follow these steps to create the customized
Redwood payslip template.

1. Navigate to the seeded folder for a country: /Shared Folders/Human Capital Management/Payroll/

Regulatory and Tax Reporting / Country Name folder.

2. Find the Payslip report and select More > Customize for the payslip report.
3. Navigate to /Shared Folders/Custom/Human Capital Management/Payroll/ Regulatory and Tax

Reporting/Country Name folder and check if you can see the report in the folder.

It is recommended that you save all user-defined or configured reports in the Custom catalog folder under Shared
Folders. Any reports created outside of the Custom folder will not be migrated and will be lost during patching or
upgrade.

If the Redwood Payslip profile option is disabled, the Payslip process uses the old payslip behavior, even if a Redwood
template exists in the Custom folder.

When you customize a delivered payslip report, including the Redwood Payslip Template, the BI Publisher creates a
copy of the report in a Customfolder. After customization, the report always runs from the Custom folder and doesn’t
automatically receive updates made to the delivered report.

Expand Payslip Name to Include Date and Amount Details

Add information into the payslip title to uniquely identify each document.

This topic applies to the global payslip template.

The payslip document name on the Payslip page includes payment date and net pay in the title and link. With each
payslip link uniquely named, it easier to identify and choose the correct payslip to view, print or download.

If you are using a seeded localization payslip templates or your own payslip templates, the name format may differ. For
example, if you are using a your own payslip template, you must store the intended payment date and payment date in
the respective property fields, Information Date 2 and Issue Date, in your delivery option for the file name. This data is
then reflect the payslip title.

You can remove the date and net pay from the document title by setting the Include date and net pay in payslip name
(ORA_PAYSLIP_NAME_DETAIL) action parameter to N.

Note:  The payslip document name is generated during the process. Therefore, the date shown in the payslip
attachment name link won't adhere to the user's date preference set for the UI view.

438

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Change Date Format
In the document name field on your delivery option, enter the date format you want to appear in the document name,
such as <MM/DD/YYYY>. If you want to keep the string, such a Payslip, append the date format after the string.

Remove the Existing Document Name
If you have a string, such as Payslip, in the document name field but want to remove it and just display the document
name as date and net pay, you can remove the string. However, you must enter the date format that you want to display,
such as <MM/DD/YYYY> so that the application knows to remove the delivery option output name as part of the
attachment name.

If you decide later to change the action parameter to N because there is no longer a string in the document name field,
the attachment name is then the delivery option output name. Re-enter a string in the document name field if you don't
want it to be the delivery option output name.

Related Topics

• Overview of Online Payslip

• How to Configure the Payslip Report Template

Add Text to Payslips and Checks

Configure your checks/cheques and payslips to display additional text. Depending on your implementation, in addition
to these steps, you may also need a new formula.

Setup steps:

1. Create the information element, its element eligibility, and the input values you want displayed.
2.

If you need a formula to calculate the run results, perform the following steps:

a. On the Manage Fast Formulas page, create a formula of type Payroll to return the values that you want to

add.

b. On the Manage Elements page, edit the information element to:

- Create a status processing rule associated with your new formula.
- Add formula result rules to return formula results to the element's input values.
3. On the Manage Enterprise HCM Information page, in the Organization Information EFF section, add the

information element and input values.

Note:  The Organization Information EFF configuration is at the enterprise level. For each LDG you want to
archive payroll information, you must add a separate row for the information element.

4. Create employee element entries, unless you selected the Automatic Entry option for the element.
5. After calculating the payroll and prepayments, run the Archive Periodic Payroll Results process.
6. Modify the check/cheque template or payslip template, as appropriate. Refer to the Report Designer's Guide for

Business Intelligence Publisher for more information.

Related Topics

• Examples of Input Values for Payslip and Check Text

439

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

Examples of Input Values for Payslip and Check Text

Create element input values to store your information, such as congratulatory messages and detailed earnings
information, that you want displayed on checks/cheques or payslips. These scenarios show you how to archive payroll
information for this purpose.

Display Earnings by Earned Weekly Period
You want to display earnings details on payslips, such as overtime pay per week within a semimonthly pay period. In this
example, before modifying your payslip template, you create an element using the Information element classification.
You create these input values in your element and add them to the payroll information to archive:

• Description

• Start Date

• End Date

• Hours

• Rate

• Multiple

• Amount

Display a Message on a Check/Cheque
You want to display a message on a check/cheque, such as a birthday or a congratulations message. In this example,
before modifying your check/cheque template, you could create an element using the Information element
classification with the following input values:

• Message Title

• Message Description

Related Topics

• Add Text to Payslips and Checks

Multilanguage Support for Payslips

The Generate Payslips process is run once each payroll period and it generates the payslip XMLs based on the payroll
archive and prepayments data. The application creates the payslip PDFs and stores them in the Document of Records
for future reference and retrieval.

Print Payslip PDFs
Some workers may opt for a printed payslip and you must provide individual PDF payslips to them.

440

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

The application supports producing all printed payslips in a single file for ease of printing. However, for the payslip
labels to be translated, each payslip must have its own individual PDF output file. To enable single PDFs, add the
Bursting configuration onto the Print Delivery option within the Payslip extract definition.

For more details on how to add the Bursting option, refer to Adding Bursting to Print Delivery Option: Procedure on the
Help Center.

Translate the Payslip
You can now generate individual payslips in the worker's correspondence language of choice. Run the Generate Payslips
process just once and generate the payslips for the various workers in a language of their choice depending on what's
set as the worker's correspondence language.

The process translates:

• The metadata, the layout labels, and the static text on the payslip template.

• The underlying data that comes from the transactional and setup tables, and the data that the Payroll Archive

process archives for the payslip.

Set the process configuration parameter, Enable Payslip Translation, to Y, before running the Payroll Archive process.
You must set this only once. If you have run the Payroll Archive before setting this parameter, you must roll back the
process, set the Enable Payslip Translation parameter to Y, and rerun the Payroll Archive process.

Install the Correspondence Language
Although the worker's correspondence language may be set to one of several languages, only those languages that are
installed are supported for translation. To determine the number of languages you must install, consider how diverse
the worker population is in terms of their preferred correspondence language.

If the correspondence language isn't one of the installed languages, the Payslip is produced in the base language.

To enable translation of the payslip labels, set the Locale property of both Document of Records and Print Delivery
options within the Payslip Extract Definition to Correspondence Language. If you don't want the payslip labels to be
translated, leave the Locale property blank or set it to the base language, for example, en-us, for US English.

For the payslip data that's not delivered by Oracle, the translated values of the data must be available in the application.
Enter translated values for the base language and each of the installed languages that needs payslip translation
support. For example, if you have created additional element names and its associated balances, you must also enter
their translated values in the application. Otherwise, the translated values aren't reflected in the payslip PDFs.

Related Topics

• Overview of Translating Modified Text

Add Bursting to Print Delivery Option

When you enable payslip translation, both the transactional data and the labels on the payslip are translated.

As only one language can be applied to all the labels on a payslip, payslips for different languages must be in their own
PDF. Add the Bursting configuration on the Print Delivery option within the Payslip Extract Definition so that payslips for
different languages are in their own PDF.

441

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

How to Add the Bursting Configuration
Complete the following steps to add Bursting to the Print Delivery option for the payslip:

1. Select the Extract Definitions task from My Client Groups > Show More > Data Exchange on your Home

page.
In the Search window, enter Payslip in the Name field.

2.
3. Select Archive Retrieval in the Type field.
4. Select a legislative data group and click Search.
5. Click Payslip in the Search Results region.
6. Click the Deliver tab in the HCM Extract Definitions: Payslip page.
7. Select the Printed Payslip Delivery Option Name row in the Extract Delivery Options section.
8. Complete the following in the Additional Details section.

a. Select Default in the Value column of Bursting.
b. Remove content in the Value column of Locale.
c. Select Search in the Attribute column of Locale.
d.

In the Search and Select: Attribute window, enter these details.

Field

Value

Parent Data Group

Global Archive Payroll Calculation Breakdown

Attribute

Correspondence Language

Record

Global Calculation Breakdown ID Information

9. Click Search, and then OK.
10. Click Save and then Submit.

Related Topics

• Overview of Translating Modified Text

Rate Precision in Payslips

Use the Payslip Rate Precision process configuration parameter to set a fixed, positive integer value as the precision
value for rates displayed on the payslip. The default value is two decimal places. Set this parameter before you run the
Periodic Payroll Archive process.

A fixed rate precision value ensures ease of implementation, user control, and consistency across different rates and
element entries. Setting the rate precision value doesn't impact the calculation of payroll or the accuracy or precision of
payments. You are only defining the number of decimal places for the rates shown on the payslip.

442

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

The precision value you set for the number of decimal places for the rates displayed on the payslip, is dependent on
these two factors:

• Currency: Some currencies require a rate precision value higher than the default value of two.

• Multiplying factor for the rate: The precision value you set for the element rates displayed on the payslip is

dependent on how high you expect the quantity to be. For example, if you expect the quantity, say hours to be
high, set a precision value higher than the default value of two.

Here are some factors you must consider while setting the precision value.

• The precision value you set on the Archive process applies for the calculation results and appears by default on
all reports that use the archived data. However, you can configure your report template to display a value that's
lower than the value on the Archive process.

• Any precision value you set on the report template overrides the value you set on the Archive process. For rates
needing a lower precision value, you must define it in the report template. You can't set a value that's higher
than that on the Archive process.

For example, suppose you want your hourly employees to see four decimal places for rates and the salaried employees
to see only two decimal places on their payslips. Set the Payslip Rate Precision process configuration parameter to
four decimal places. Then, modify the report template to display the rates with two decimal places only for salaried
employees.

Related Topics

• Overview of Online Payslip

• How Do I Set the Payslip Rate Precision Value

• Report Days and Units in Payroll Reports

• How to Configure the Payslip Report Template

How Do I Set the Payslip Rate Precision Value

The precision value defines how many decimal points the payslip uses when showing rate amounts. While the default
is two decimal places, you can change it. Changing the precision value doesn't change the accuracy of the payroll
calculations.

To change the default payslip rate precision value, you must change how the rates are captured in the periodic payroll
archive.

1. Start the Payroll Process Configuration task from My Client Groups > Show More > Payroll.
2. Create a configuration group, and give it a meaningful name.
3. Select the Details tab, add a row, and select Payslip Rate Precision.
4. Set the number of decimal places in the Override Value field.
5. Click Save.

When you run the Archive Periodic Payroll Results process, use the Process Configuration Group parameter to select
this configuration group.

You can modify the precision value set on the report template itself, and this value will override the value you set on
the archive process. For example, suppose you want your hourly employees to see four decimal places for rates on
their payslips and the salaried employees to see only two decimal places. In this case, follow these steps to make the
changes.

1. Set the Payslip Rate Precision process configuration parameter to four decimal places.

443

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

2. Modify the payslip report template to display the rates with two decimal places only for salaried employees.

To modify the payslip report template, refer to 'How to Configure the Payslip Report Template' in the Help Center.

Related Topics

• Rate Precision in Payslips

• Overview of Online Payslip

• How to Configure the Payslip Report Template

Add a New Balance Dimension to an Existing Balance in the
Payslip XML

This topic explains how you can add a new balance dimension to an existing balance, if the balance isn't displayed on
the payslip.

After you add the balance dimension, you can display the balance dimension on the payslip XML.

For example, add the Inception to Date balance dimension to the Absence Accruals balance and display the Assignment
Inception to Date Absence Plan balance in the Payslip XML.

You can add balance dimensions to other balance group records in the Archiver. Add dimensions that have the same
level as the records in the balance group. For example, to add a relationship-level balance dimension, find balance
group records in the Archiver that correspond to payroll or assignment relationships and add dimensions starting with
'Relationship'.

Here's the list of tasks you must complete:

1. Associate the balance dimension to the balance group.
2. Generate Payments (Generate Check Payment and Make EFT Payment, if applicable)
3. Archive Periodic Payroll Results

Note:  Complete these tasks in the order as listed above.

Complete these tasks only if you want to regenerate the payslips to include the newly added balance dimension.

Associate the Balance Dimension to the Balance Group
Associate the Inception to Date dimension to the Absence Accruals balance group so that the values for the absence
accrual balances are retrieved for the inception to date period. Use either of these options to add the balance
dimension.

• Manually add a specific dimension to the group. Use this option if you want to add a specific dimension and not

all the dimensions under a category to the balance group. Follow steps 4 and 5, given here.

• Use Default Inclusions, as given in steps 6 and 7, to add all existing dimensions within a category and any new

dimensions that you include to a category.

Complete these steps to add a balance dimension to a balance group.

1. Navigate to Balance Groups under Payroll in My Client Groups on the Home page.

444

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

2. Enter these details and click Search for the requisite balance group.

Field

Value

Balance Group Usage

Global Absence Accruals for Global Archive

Legislative Data Group

Select a Legislative Data Group.

3. Click Global Absence Accruals Balance Group in the Search results section, to open the balance group page.
4. Click Balance Definitions in the left pane. Check if the Balance Name and Dimension Name appears in the list.
5.

If not, use the Select and Add option under Actions and add the Assignment Inception to Date Balance
Dimension. Click Save.

Note:  Alternately, if you want to view all of the balance dimensions within the category, you can use the
Default Inclusions, and perform steps 6 and 7.

6. Select the correct Balance Category and Balance Dimension row and click Default Inclusions in the left pane.
7. Click Add and enter these details to create an Inclusion item.

Field

Value

Balance Category

Absence Accruals

Balance Dimension

Assignment Inception to Date

Legislative Data Group

Select a Legislative Data Group

8. Click Save and then Submit.

Add the Balance Dimension to the Balance Group Usage
Complete these steps to add the Assignment Inception to Date balance dimension to the Global Report Archive Balance
Group Usages.

1. Navigate to Balance Group Usages under Payroll in My Client Groups on the Home page.
2. Enter these details and click Search for the requisite balance group.

Field

Value

Balance Group Usage

Global Absence Accruals for Global Archive

Legislative Data Group

Select a Legislative Data Group.

3. Click Global Absence Accruals Balance Group in the Search results section, to open the balance group page.
4. Click Matrix Items in the left pane. Check if the Dimension Name appears in the list.

445

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

5.

If not, use the Select and Add option under Actions and add these details to create the Matrix Item. .

Field

Value

Matrix Item Type

Balance Dimension

Name

Position

Assignment Inception to Date

Enter the next numeric Position

Legislative Data Group

Select a Legislative Data Group.

Note:  You can select any Assignment level balance for the Inception to Date dimension, for example,
Assignment Inception to Date or Assignment Tax Unit Inception to Date balance.

6. Click Save and then Submit.

Run the Archive and Payments Process

1. Run the Archive Periodic Payroll Results and Payment processes, so that you include the newly added balance
dimension in the archive and payments run. The payslip displays the newly added balance dimension only if
you include it in the archive and payments processes

Generate the Payments and Payslips

1. Run the following processes:

◦ Generate Check Payments or Make EFT Payments
◦ Generate Payslips

2. After you run the Payslip, download the Payslip XML from Reports and Analytics > Report Job History. Confirm
that the Balance values at ASG ITD dimension is showing in the Payslip XML in tag < LIFETIME> under the
<GLB_PAY_ARCH_PAY_ASG_ABSENCE_ACCRUALS> node.
In the Payslip XML, the <LIFETIME> tag contains values of the Inception-to-Date dimension. The <YEAR> tag
contains values of the Year-to-Date dimension, and you must add the YTD balance dimension if you need YTD
values on the Payslip XML.
These are the XML tags or short codes you can use for the balance dimensions:

◦ PERIOD
◦ MONTH
◦ QUARTER
◦ YEAR
◦ TMONTH
◦ TQUARTER
◦ THYEAR

446

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

◦ TYEAR
◦ FMONTH
◦ FQUARTER
◦ FHYEAR
◦ FYEAR
◦ HYEAR
◦ MONTHS
◦ LIFETIME
◦ R1MTH
◦ R3MTH
◦ R6MTH
◦ R12MTH

3. Configure the Payslip RTF template if you want to add the newly added Balance dimension to the Payslip PDF.

Related Topics

• Examples of Input Values for Payslip and Check Text

• How to Configure the Payslip Report Template

Disable or Override the Printed Delivery Option for the Payslip

A delivery option defines where and how the report output is delivered, including the output file format, choice of
template, and optionally a destination such as an FTP server.

A report category is a set of delivery options grouped together so that you can generate the report in more than one
output format with a single submission of the report.

You can define your own delivery option and include it in a report category, or you can also disable the delivery option
for the report.

Use the Payslip Reprinting Report if the count of employees getting the printed payslips is very less compared to the
overall employee population. This helps in optimizing the processing time to generate the printed payslips. Disable the
Printed Payslip delivery option if you don't plan to use it.

Complete these tasks to disable the predefined Printed Payslip delivery option for the payslip.

1. Create a delivery option and set the start date and end date of the payslip to very early dates, for example from

01/01/1951 to 31/01/1951.

2. Override the existing printed delivery option using this newly created delivery option.

Here are the steps required to disable the Printed Payslip delivery option for the Payslip.

In the Search window, enter Payslip in the Name field.

1. Select the Extract Definitions task in the Data Exchange work area on the Home page.
2. Click Show Filters.
3.
4. Select Archive Retrieval in the Type field.
5. Select a legislative data group (LDG) and click Search.
6. Click the pencil icon to edit the Payslip in the Search Results region.

447

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

7. Select the Extract Delivery Options tab under the Hierarchy panel on the left, and complete these steps.

a. Add Overriding Delivery Mode column to the Extract Delivery Options table if it isn't already present.
b. Click Add to add a row for the delivery option you're about to create.
c. Enter these details.

Field

Start Date

Value

01/01/1951

End Date

31/01/1951

Delivery Option Name

Printed Payslip

Output Type

Select a value, for example, PDF.

Report

Enter the same location as in the Printed Delivery option.

Template Name

Enter the same name as in the Printed Delivery option.

Output Name

Enter Name of the report output, for example, Printed Payslip.

Delivery Type

Select None.

Required

Select this checkbox if this delivery option is a required option.

Overriding Delivery Mode

Select an existing printed delivery option you want to override, example, US Printed

Payslip.

When you run the payslip, because the dates defined for the delivery option doesn't match with the actual print
dates, the printed payslips aren't generated.

8. Click Save and Close.

Override the Printed Delivery Option for the Payslip
Follow these steps to override an existing delivery option, example, the US Printed Payslip, and create and use a new
delivery option.

Override the printed payslip with a new delivery option using a custom data model only if the Payslip Reprinting Report
doesn't filter the employees as required. You need to identify and filter employees who have opted for a printed payslip.

1. Create a delivery option as given in the previous section.
2. Set the Start Date and End Date of the new delivery option to the actual print dates.

448

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

3. Create a custom data model and report template. For more information on how to create the custom data

model and report template, see the Define the BI Publisher template in HCM Extracts topic on the Oracle Help
Center.

For printing the payslip for a group of employees who have opted for the printed payslip, use the data set
logic from the original payslip data model. Select the Payslip XML for the selected employees by filtering on
source_type='PRA' from the pay_file_details table. For example, the SQL in the custom data model is as given
here:

select file_fragment

from pay_file_details

where source_type='PRA'

and source_id = '<Get the employee_payslip_rel_action_id>'

As an example, see the SQL in Payslip Bursting Data Model here, /Shared Folders/Human Capital
Management/Payroll/Payment Distribution/Data Models/Payslip Bursting Data Model.
4. Select the Required checkbox to use the new delivery option instead of the one you're overriding.
5. Use the Overriding Delivery Mode field to select the delivery option you want to override.

Related Topics

• Add Bursting to Print Delivery Option

• Delivery Options for Extract-Based Payroll Reports

• Define the BI Publisher Template in HCM Extracts

449

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 8
Payments

450

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 9
Events, Retroactive Pay and Proration

9  Events, Retroactive Pay and Proration

Payroll Event Groups

Overview of Payroll Event Groups

A payroll event group defines the types of data changes monitored for features such as the retroactive recalculation of
payroll, the retroactive recalculation of time cards, and the retropay for late hires.

There are three types of payroll event groups:

• Proration

• Retroactive

• Event Action

Proration
Using proration, you can calculate proportionate earnings and deduction amounts whenever payroll-relevant data
changes during a payroll period.

For example, you can calculate proportionate earnings and deduction amounts if:

• A person joins or leaves an organization in the middle of a payroll period

• A person's pay rate changes during a payroll period

If you want to prorate an element, such as basic salary, assign a proration event group to the element with proration
points that affect a person's salary. You can use the predefined event group, or create a new one. When you create an
event group, you select the events that activate proration calculation, such as changes to:

• Hourly or annual pay rates

• Working hours

• Allowances or deductions

• Assignment changes, such as grade or position

Tip:  You can only select events that represent changes to element entries, calculation cards, calculation value
definitions and assignments.

Retroactive
Retroactive processing ensures that your payroll run for the current period reflects any backdated payments and
deductions from previous payroll periods. A retroactive event group defines the types of changes that trigger a
retroactive event notification. These types of changes are Entry Changes for Retro and trigger notifications when
changes are made in a prior payroll period. You can make additional events trigger the recalculation process by editing
the group or creating a new event group for the element. All events trigger in real time.

451

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 9
Events, Retroactive Pay and Proration

Within a retroactive event group, select the events that produce notifications if a backdated change occurs. Specify the
entity, update type, and attribute, as shown in the examples provided in the following table.

To disable notifications for an element, within the Manage Element UI, query the 'base' element that you no longer want
to be processed by retropay and remove the specified 'Retroactive Event Group'. This prevents new events from being
triggered.

Entity

Update Type

Attribute

Element Entry Value

Correction

SCREEN_ENTRY_VALUE

Element Entry

Element Entry

Update

Update

EFFECTIVE_START_DATE

EFFECTIVE_END_DATE

Element Entry

Logical Date Change

Element Entry

Insert

Element Entry

Delete Changes

Event Actions
An event action links a process to the events within an event group. When an event occurs, the process is triggered
based on a set of conditions defined on the event action. You can use event actions to control the submission of
features, which use event groups of type action such as generate HCM Rates and time card reprocessing. Event actions
control the aspects of submission such as, if the process is automatically submitted when an event occurs or when
submitted through a payroll flow.

There are two event action submission types:

• Manual: The application processes the event action notifications using the ‘Process Event Action’ flow.

Schedule this process to run on a regular basis to ensure your information is kept up to date such as your
stored rate values. Also, add this task to your payroll cycle flow so it is submitted before you calculate payroll.

• Automatic: The application automatically submits processes such as retropay late hires, each time an event

action notification is generated.

There are different types of event actions, each with its own set of submission control rules such as:

• Resubmission of time cards

• Retropay for late new hires

• Absence resubmission

• HCM Rates Recalculation

• Mexico SDI calculations

Use HCM Data Loader to create an event action.

452

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 9
Events, Retroactive Pay and Proration

Related Topics

• How Retroactive Pay Is Calculated

• Set Up Element Proration

• Overview of Loading Event Actions and Event Action Groups

Event Action Notifications

When an event is triggered, the application filters the applicable event groups which include that event, and generates
event notifications for each event action included in those event groups.

Let's consider an example where the application triggers an event for a worker due to a change in their job. This event is
included in an Event Action Group associated with the HCM Rates Recalculation event action. As a result, the application
creates an event action notification for the worker, for HCM Rates Recalculation in the Awaiting Processing status.

When the rates process is run, the application determines all workers with an event action notification of HCM Rates
Recalculation in the awaiting processing status and recalculates rates for these employees. Once this process is
completed successfully, the notification status is updated to Completed.

You can view and manage event notifications in two ways:

• For event notifications related to retroactive payroll and proration, use the Event Notifications page. You can

configure the events that trigger these notifications using the Event Groups  page.

• For all other event notifications associated with event actions such as time card resubmission, retroactive
payroll for late hires and generate HCM rates, use the Event Action Notifications page. The event action
groups configure these event actions and loads them through HCM Data Loader.

In order to visualize the impact of an event and the underlying cause for an event notification, you can navigate
between event notifications and events. You can view event action notifications and drill down to view the events
associated with that event notification to detect the type of change, when the change occurred, and who made the
change. You can use the Event Notifications button on the Event Action Notifications page to navigate to the Event
Notifications page for the selected person. This lets you view retropay notifications for the selected person. The back
arrow on the Event Notifications page returns you to Event Action Notifications page.

Alternatively, you can also view the events raised for a person on the Events page, including those events that didn't
raise any event notification. You can then drill down to view the event notifications associated with an event.

The Event Action Groups page consists of the event group setup. Here you can view all the event action groups loaded
through HCM Data Loader and see if any are set up to watch the type of event you're interested in.

Event Notification Status
When an event is triggered, the payroll application generates event notifications for features such as the retroactive
recalculation of payroll and retropay for late hires. The Notification Status attribute supports these values for an event:

• Not Started: Notification processing hasn't yet started.

• Complete: Notification processing is complete.

• Error: Notification processing has failed.

• Event Canceled: The event has been canceled.

Use the event notification status to review and take an appropriate action on an event.

453

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 9
Events, Retroactive Pay and Proration

Calculate Rates Based on Events

You can calculate rates based on events triggered for the employee.

Use HDL Data Loader to perform the following set-up steps:

1. Create an event action for generate HCM rates. The event action defines the set of conditions for the rates

event process. For example, indicate if the rates processes should be automatically submitted when an event is
raised or if the recalculation should be initiated manually using the ‘Process Event Action’ flow.
2. Create an event group to identify the type of changes to be monitored for rate recalculations such as

assignment updates.

3. Associate the HCM Rates event action to your HCM Rates event group.

Some points to consider when implementing rates based on events:

•

If you are monitoring element entry changes in your rates event action group, you must enable event
processing using the background flow. Set the action parameter ‘Process Payroll Events on Background Payroll
Flow’ to ‘Y’.

Note:  This setting will move all payroll event processing to a payroll process which continuously runs in the
background. The evaluation and generation of all payroll event notifications and actions will no longer be
performed as part of the main transactions such as a new hire.

• You can set the submission type of the rates event action to ‘Manual’ which indicates the rates will be

recalculated when the user submits the ‘Process Event Action’ flow. This flow will generate reports to validate
the results of the rates process:

◦ Person Process Status Report: This report lists all the employees included in the process, the status of

their rate calculation, and any warning or error messages.

◦ Rates Report: This report indicates rate values calculated for each employee included in the process, the

effective start date of the rate and details of when the rate was last recalculated.

• You also have the option to automatically submit the rates process each time an event notification is raised for

an employee, but no reports are generated for this type of action submission.

• When you implement rates, you should first run the Generate HCM Rates process to calculate and capture

rate values for all employees. Going forward, use the event feature to recalculate rates for any employee who
has an event such as a salary update. If you are using the Process Event Action flow to recalculate rates, it is
recommended you run the process on a daily basis.

•

If you calculate rates based on payroll balances, you may still need to run the Generate HCM Rates process
because changes to this type of rate are not event based.

Related Topics

• Overview of Loading Event Actions and Event Action Groups

• Example of Loading Event Actions for HCM Rates Recalculation

• Example of Loading Event Group and Associating to an Event Action for HCM Rates Recalculation

454

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 9
Events, Retroactive Pay and Proration

Submit the Process Event Actions Manual Process Flow

Use the Process Event Actions flow to submit all unprocessed event action notifications with a manual submission
type. For example, use the flow to calculate rates for all employees with an unprocessed rate event action notification.

Here’s how you submit the flow:

1. Navigate to My Client Groups > Show More > Payroll > Submit a Flow.
2. On the Flow Submission page, leave the Legislative Data Group field blank.
3.

In the Select a Flow section, search for the Process Event Actions flow pattern.

The Submit a Payroll Flow - Process Event Actions page is displayed.
In the Payroll Flow field, enter the name for the instance of the process event actions flow.

4.
5. From the Event Action Type drop-down list, select the type of event action.

For example, select the HCM Rates Recalculation event action to calculate rates for all employees with an
unprocessed event action notification.

Note:  You create the event action groups using HCM Data Loader. For more information, see Overview of
Loading Event Actions and Event Action Groups.

6. From the Event Action drop-down list, select a user-defined event action to be included in the process event

actions flow.

The displayed options are filtered based on the selected event action type such as HCM Rates Recalculation.
This list displays all event actions for the specified event action type, which are set to Manually Later.
(Optional) From the Process Configuration Group drop-down list, select a group. If you don’t select any group,
by default, the process configuration group created for the selected event action, is used.

7.

8. Specify the schedule and (optional) linked flows.
9. Click Submit.

When you submit this process for HCM Rates Recalculation, it generates a report with the rate values calculated for
each employee included in the process. You can validate the results of the processes submitted by the Process Event
Actions flow using the generated report. This lists all the employees included in the process, the status of the process,
and any warnings or error messages. The Process Event Actions Manual flow pattern will be displayed on the View
Flows, Checklist, and Process Results Summary pages.

Related Topics

• Overview of Loading Event Actions and Event Action Groups

Retroactive Pay

How Retroactive Pay Is Calculated

Retroactive pay is the recalculation of prior payroll results because of changes that occurred after the original payroll
calculation run.

455

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 9
Events, Retroactive Pay and Proration

For example, an employee receives a backdated salary award or a performance bonus.

You run the Recalculate Payroll for Retroactive Changes process to calculate retroactive pay. This process creates
retroactive element entries based on retroactive events.

Note:  Only the elements that have retroactive pay enabled will have retroactive results calculated.

Set up Elements for Retroactive Pay
To enable retroactive processing of an element:

1. On the Event Groups page, review the types of changes that automatically trigger a retroactive notification for
the predefined event group, called Entry Changes for Retro. It is recommended you use this group or you can
create a new event group for the element, if required.

2. On the Element Additional Details page, select Yes for these questions:

◦ Is this element subject to proration?
◦ Is this element subject to retroactive changes?

3. On the Element page, select the predefined event group or a new group that you have created.

Note:  This step is only if you want to attach your new group to an existing element. If your group exists
and you are using the template to create the element, you do not need to navigate to the element page.
You can attach the group from the template.This step is only if you want to have a different element pay the
retroactive adjustment.

4. On the Retroactive Components page, create a full retroactive calculation with a reprocess type of 'Reprocess'

5.

and choose 'Yes' for the default component.
In the Retroactive Pay Elements section of the Retroactive Components page, create an entry with effective
dates, adjustment type of 'Standard' and choose the target element of the results element that you want the
retroactive pay process to use when creating a retroactive entry.

Note:  This step is only if you want to have a different element pay the retroactive adjustment.

Process Retroactive Pay
Whether creating a flow pattern for retroactive tasks, incorporating tasks into a Payroll Cycle flow pattern, or running
individual processes, it is advised to run them in the following order:

1. Submit the Retroactive Notifications Report.

Note:  You can also Review or create retroactive events on the Event Notifications page and download results
to Excel to view retroactive events in a report format.

2. Submit the Recalculate Payroll for Retroactive Changes process with the Submit a Flow task or the process may

run automatically as part of your payroll flow.

Note:  This process creates one or more retroactive entries to receive the process results and never
overwrites historical payroll data.

3. Submit the Retroactive Entries Report.
4. Review the Retroactive Entries Report.
5. Submit the Calculate Payroll process.

456

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 9
Events, Retroactive Pay and Proration

Note:  Always run the Recalculate Payroll for Retroactive Changes process immediately before you run a payroll.
Otherwise, if you run it after the Calculate Payroll process, retroactive adjustments are held over until the next payroll
period.

If you don't get the expected retroactive notification, here are some suggestions to review:

• The transaction that caused the event

• Element setup

• Element eligibility for the person

• The retroactive event group entities and attributes that are set up to trigger retroactive events

• The proration event group entities and attributes setup that triggers proration

Exclude Retroactive Element from the Retroactive Pay Process
If you enabled the element for retroactive pay but now you don't want it included in the process, follow these steps to
prevent it from being considered in the process comparison:

1. On the Element Additional Details page, Remove the two retroactive components rows.
2. On the Event Groups page, remove the event group.

Note:  To process an element in a retroactive payroll run, the element must have retroactive components that define
the processing rules. These steps remove these defined processing rules and disable event notifications.

Related Topics

• Overview of Payroll Event Groups

• Create Conversion Formulas for Proration

Add a Retroactive Event Notification Manually

Retroactive Events are typically created automatically when you create retroactive adjustments, such as backdated
salary changes.

You can enter the retroactive event manually to generate the correct payslip, such as if payroll hasn't made the pay rate
change effective last pay period for an employee being terminated effective immediately.

Create a Payroll Relationship Event

1. Select the Event Notifications task.
2. Click Create.
3. Use the information in this table enter information into the Create Payroll Relationship Event window.

Field

Value

Approval Status

Awaiting Processing

Payroll Relationship

The person to process

457

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 9
Events, Retroactive Pay and Proration

Field

Value

Process Date

Date when the retroactive change process is run.

Note:

This date indicates when the element change was triggered.

4. Click Save and Close.

Create a Retroactive Event

1. On the Event Notifications page, click the name of the person associated with the payroll relationship event you

created.

2. On the Retroactive Events page, click Create in the Entry Details section.
3. Select the element you want to reprocess, the date the recalculate payroll runs, and a retroactive component.

The element from which the change will be paid to the person is the retroactive component.
4. Repeat the previous step if you want to recalculate multiple elements for this payroll relationship.
5. Click Submit.

Retroactive Pay for Late Hires

Use retropay for late hires to identify employees entered in the application after the regular payroll has been processed.
The application detects and processes late hires when regular payroll result exists for a date later than the employee's
hire date.

For example, Jane was hired on 22-Mar-2022, but the HR team entered her details late into the application. Jane wasn't
included in the payroll run that was processed and paid on 26-Mar-2022.

The application will create a payroll action for Jane for the 26-Mar-2022 payroll period. Also, the application displays
the payroll action on the process results page with action status 'Retroactively Added'. This action enables retropay to
calculate her missing earnings for the 26-March payroll period.

You can also use retropay for late hires to support changes in the hire date. For example, David Ellis was entered in the
application with a hire date of 01-Nov, but they actually commenced employment on 01-Oct-2022. Retropay for late
hires enables retropay to calculate David' earnings for the October payroll periods.

Set Up Retropay For Late Hires
To enable retropay for late hires, create a new Event Group and Event Action for their legislative data group.

The event group identifies the late hire. The event action creates a payroll action for the late hire. Also, the employee
appears in the process results for that payroll with the action status as Retroactively Added.

This lets late hires to be processed within the Recalculate Payroll for Retroactive Changes process. This flow pattern
contains two tasks:

• Calculate Payroll for Late Hire

458

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

• Late Hire Retropay Notification

Chapter 9
Events, Retroactive Pay and Proration

These tasks replace the need to manually enter an element entry against the late hire, as the Late Hire Retropay
Notification task automatically creates the notification. You can view the late hire details for an employee using the
Person Results and Payroll Checklist pages.

Use the sample HCM Data Loader (.DAT file) to enable all or some of the following events:

• Create Flow: If set to Y, generates the Evaluate Late Hire flow pattern with its Calculate Payroll for Late Hire and

Late Hire Retropay Notification tasks.

• Hire Date Later: If set to Y, the retroactive net pay result is generated when an employee's hire date is later than

the payroll process date.

• Run Payroll Relationship Group: If set to Y, the retroactive net pay result is generated even when the original

payroll was run with a payroll relationship group.

• Additional Assignments: If set to Y, the retroactive net pay result is generated when a late assignment is added

to a payroll relationship.

You can view the flow results in the View Flows, Process Results, and Person Results pages.

• Use the View Flows page to drill down to the Evaluate Late Hires details.

• Use the Person Results page to drill down to the Calculate Payroll for Late Hires details.

For more information on the sample .DAT files for these event groups and event actions, see “Example of Loading
Retropay for Late Hires Event Action” in the HCM Data Loading Business Objects guide.

As this illustration shows, you follow a three step process to set up retropay for late hires.

Configure Employee Details
After you have enabled the feature, and you late hire the employee on 01-Mar-2022, complete these payroll steps to
recalculate payroll for the retroactive changes.

(Optional) Assign Element Entries and Calculation Cards
(Optional) Review the Hire Date Flow to ensure both tasks are complete
(Optional) Review the employee’s Process Results to see the retroactively added Calculate Payroll process
(Optional) Review Event Notification

1. Assign Payroll
2.
3.
4.
5.
6. Run Retro Payroll Process
7. Run Regular Payroll

As shown in this illustration, add a payroll to the employee to control how and when the employee is paid and verify
the process results. Assign element entries and calculation cards. Then, run the retropay process, which picks up the
retro notification and processes the late hire. Validate the process results. Finally, run the process for regular payroll and
validate the process results.

459

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 9
Events, Retroactive Pay and Proration

If the original payroll run used a relationship group, restricting who was processed, this new late hire feature ignores
that run. This is only applicable if you haven’t enabled allowing payrolls with payroll relationship groups to be enabled
in the Event Action HDL. The late hire only adds late hires to payroll calculations that weren't restricted by a relationship
group.

Related Topics

• Example of How to Transfer Payrolls

• Guidelines for Loading Time and Labor Event Groups

460

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 10
Auditing and Data Validation

10  Auditing and Data Validation

Audit Payroll Business Objects

Set up auditing policies to maintain a history of changes to your important data: what changed, who changed it, and
when.

The audit tracks changes to attributes of payroll business objects made using the application pages, web services, or
payroll processes, which use Oracle Enterprise Scheduler.

You can view the audit history to determine how a business object obtained its current value and to compare old
and new values. To view the history or to create an audit report from the Audit History work area, you require
appropriate duty roles and privileges. Enterprises typically assign the following two audit duty roles to the application
implementation consultant and master data management application roles:

• Audit trail management, which determines the objects audited

• Audit trail report viewing to view the audit history

Payroll Business Objects
When you set up auditing for payroll, you configure Oracle Fusion Applications business objects on the Manage Audit
Policies page in the Setup and Maintenance area:

1. Select the HCM Payroll application on the Configure Business Object Attributes page.
2. Specify the attributes to audit for the objects.

For example, you might audit the start and end date attributes for the calculation card component details.

This table lists the payroll business objects you can set up for auditing payroll. You track changes to attributes specified
for these objects.

Payroll Business Object

Description

Assigned Payroll

Holds date-effective attributes about payrolls assigned to a worker.

Assigned Payroll More Details

Holds details that aren't date-effective about the payroll assigned to a worker.

Calculation Card

Holds values required for calculating payroll components.

Calculation Card Component

Holds the definition of a component that represents one or more logically related payroll components.

Calculation Card Component Detail

Holds the input values of a person's calculation card.

Calculation Reporting Card

Defines the tax reporting units that report the calculation.

461

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 10
Auditing and Data Validation

Payroll Business Object

Description

Calculation Reporting Card Usage

Attaches a reporting card to a person record.

Element Entry

Holds earning and deductions details for a person.

Element Entry Value

Holds the values of the compensation and benefits granted to a person.

Payroll Calculation Range Value

Defines the values or sets of values used in the calculation of a value definition.

Payroll Calculation Value Definition

Defines how a value is calculated in payroll processing.

Personal Payment Method

Holds the payment method details for a person.

Related Topics

• Audit Policies

• Audit Configuration for Business Object Attributes

• Audit Reports

Audit Element Security Profiles

Complete these tasks to enable audit of the element security profiles business object and its child objects and track and
view changes to element security profiles.

1. Enable auditing of the Element Security Profile and its attributes
2. Run the Audit Report

Enable Audit of the Element Security Profile
Follow these steps to enable auditing of the Element Security Profile and its attributes.

1. Search for and use the Manage Audit Policies task from Setup and Maintenance.
2. On the Manage Audit Policies page, select Auditing as the Audit Level for Oracle Fusion Applications. This

setting turns on the auditing functionality.
3. Click Configure Business Object Attributes.
4. On the Configure Business Object Attributes page, select Global Payroll as the Product. The business objects

associated with that product appear in the Objects section.

5. Select the check boxes for the Element Security Profile and its attributes Legislative Data Group, Element,

and Element Classification.

6. Click Save and Close.

Run the Audit Report
After you have enabled auditing, use the Audit Reports quick action to view the change history of the Element Security
Profile and its attributes Legislative Data Group, Element, and Element Classification.

462

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 10
Auditing and Data Validation

Note:  To view the change history of a business object or to create a report, you must have a role with the View Audit
History (FND_VIEW_AUDIT_HISTORY_PRIV) privilege assigned to it.

1. Navigate to Tools > Audit Reports from the Home page.
2. On the Audit Reports page, select the values as shown in this table.

Field Name

Value

Date

Select Equals and use the date picker to set a date as on which you want to track the change

history of the Element Security Profile and its attributes.

Product

Event Type

Business Object Type

Global Payroll

Select Equals and the All check box.

Select one of these:
◦ Element Security Profile
◦ Element Security Profile - Legislative Data Group
◦ Element Security Profile - Element
◦ Element Security Profile - Element Classification

3. To audit security profiles and all their objects, select Element Security Profile, and select the check box

Include child objects. To audit a specific object within the security profiles, select that object from the list.

4. Click Search.

Transactional events in the application trigger the audit process based on the create, update, and delete operations
on the enabled business object and its attributes or child objects. The report output displays the event type, business
object type and attribute name, and the old and new values.

When an element is removed from the Element Security Profile, it is tracked in the Audit Report. However, when an
element that is included in a security profile is deleted from the Manage Element page, it is automatically removed from
the security profile. This deletion isn't shown in the Audit Report.

Payroll Validations for Absence and Time Entries

You can upload and manage time and absence entries to the Oracle Payroll application from any of these source
applications:

• Oracle Time and Labor or Oracle Absence Management application

• Any third-party absence or time collection application

When you are using a third-party absence or time collection application, use HCM Data Loader (HDL) to load this
information to the Oracle Payroll: application:

• Load absence information using the AbsenceEntry.dat file.

• Load time information using the PayrollTimeCard.dat file.

463

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 10
Auditing and Data Validation

Ensure you're using the correct business objects to load this information onto the Oracle Payroll application using the
HDL. This helps you reconcile all absence and time entries processed by Oracle Payroll with the information held in the
source application.

If you’re using Oracle Absence Management, the absence details are automatically transferred to payroll when an
absence is approved. If you’re using Oracle Time and Labor, you can transfer time entries to payroll using the Load Time
Card Batches process.

Note:  If you’re using the generic calculation card CalculationCard.dat file. to load absence or time into payroll, you
must change your integration to use the absence and time files. Using these files helps reduce the errors you face
using the generic calculation card business object to load this type of information. A warning message displays when
you load absence and time information using the generic calculation card file. A warning message is also displayed
if you enter or update absence and time information on the classic calculation card page because this information
should be managed in the source application to enable you to reconcile absence and time entries.

Note:  You are not impacted by this change if you import absence and time from a third-party system using standard
element entries.

Audit Policies

Auditing is used to monitor user activity and all configuration, security, and data changes that have been made to an
application. Auditing involves recording and retrieving information pertaining to the creation, modification, and removal
of business objects.

All actions performed on the business objects and the modified values are also recorded. The audit information is
stored without any intervention of the user or any explicit user action.

Use audit policies to select specific business objects and attributes to be audited. The decision to create policies usually
depends on the type of information to be audited and to the level of detail required for reporting.

Enabling Audit Functionality
For Oracle Applications Cloud, you must configure the business objects and select the attributes before enabling audit.
If you enable audit without configuring the business objects, auditing remains inactive. By default, auditing is disabled
for all applications. To enable and manage audit, ensure that you have a role with the assigned privilege Manage Audit
Policies (FND_MANAGE_AUDIT_POLICIES_PRIV). For appropriate assignment of roles and privileges, check with your
security administrator.

To enable auditing for Oracle Fusion Middleware products, select one of the levels at which auditing is required for that
product. The audit levels are predefined and contain the metadata and events to be audited. For more information, see
Audit Events for Oracle Applications Cloud Middleware (Doc ID 2114143.1) on My Oracle Support.

If you don't want an application to be audited, you can stop the audit process by setting the Audit Level option to None.
Also, note that there's no specified retention period for the audited data or the logs. Follow your company policy for
retaining or removing such data.

464

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 10
Auditing and Data Validation

Note:  You won't be able to enable audit if you're working in a sandbox. If you try to set up audit while you're in
a sandbox, you will see the message "Audit setup is disabled in a sandbox". You'll also notice that the buttons
associated with the audit functionality are disabled.

Related Topics

• Audit Configuration for Business Object Attributes

• Overview of Audit Configuration

Audit Configuration for Business Object Attributes

Audit enables tracking the change history of particular attributes of a business object. However, those objects and their
attributes must be selected for audit and auditing must be enabled for that application.

The configuration settings determine which attributes to audit for a given object, and when the audit starts and ends.
Auditing takes into account all the operations performed on an object and its attributes, such as create, update, and
delete. To configure audit business object attributes, use the Manage Audit Policies task in the Setup and Maintenance
work area.

Selecting an Application
To set up auditing, you must select a web application that contains the required business objects that can be audited.
From the list of business objects, select those business objects that you want to audit. Selecting a business object also
displays its attributes that are enabled for auditing.

Selecting Attributes
For each selected business object to be audited, select the corresponding attributes to include in the audit. All attributes
that belong to that object are by default selected for audit and appear on the user interface. However, you can add or
remove attributes from the list. When you remove an attribute from the list, you stop auditing it even when the parent
object is selected for audit. So, if you want an attribute to be audited, you must add it to the list. If the object selected in
an audit hierarchy is also a part of several other audit hierarchies, the attribute configuration for that object is applicable
to all the hierarchies in that application.

For business objects based on flexfields, select the Flexfields (Additional Attributes) check box to view, add, or remove
flexfield attributes. The selected objects are audited.

Note:  You can't audit LOB (BLOB, CLOB, and NCLOB), rich text, and long text attributes.

Starting and Stopping Audit
The business object is ready for audit after you select its attributes and save the configuration changes. However, to
start auditing, the audit level for Oracle Applications Cloud must be set to Auditing on the Manage Audit Policies page.

To stop auditing an object, you can deselect the entire object and save the configuration. As a result, all its selected
attributes are automatically deselected and aren't audited. To continue to audit the business object with select
attributes, deselect those attributes that aren't to be audited. When users view the audit history for an application, they

465

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 10
Auditing and Data Validation

can specify the period for which they want the results. Therefore, make a note of when you start and stop auditing an
application.

For example, users intend to view the audit history of an object for the previous week, but auditing for that object was
stopped last month. They wouldn't get any audit results for that week, because during the entire month that object
wasn't audited. Even if you enable audit for that object today, users can't get the wanted results because audit data until
today isn't available.

Note:  When users export the report summary to a Microsoft Excel file, there's a limit on the number of rows that are
displayed in the file.

•

•

For Oracle Fusion Middleware products, the maximum limit is 25000. By default, the limit is set as 10000. You
can change this limit using the FND_AUDIT_FMW_EVENT_LIMIT profile option.

For Oracle Fusion Application Business Objects, the maximum limit is 10000 per table. This is
set as the default value. Sometimes, the actual rows returned might be more than the limit set,
because a single transaction can update multiple tables. To decrease this limit, you can create the
FND_AUDIT_EXPORT_ENTITY_LIMIT profile option and set a lesser value for it.

See Why is it taking so long to get search results when exporting audit summary of Fusion Application
Business Objects?

Audit Reports

You can use the Audit Reports work area to view changes to the application data, such as the business objects that were
created, updated, and deleted.

To view the history or to create a report, you must have a role with the View Audit History
(FND_VIEW_AUDIT_HISTORY_PRIV) privilege assigned to it. For appropriate assignment of roles and privileges, check
with your security administrator.

Audit Events
Transactional events in the application trigger the audit process based on the create, update, and delete operations. For
events to trigger the audit process for the business objects, you must first enable the objects for auditing.

These are the events that trigger the audit process.

Transactional Event

When the Audit Activity is Triggered

Audit Report Content

Create

Update

Whenever business object data is created and

• Name of the created object

stored in the database

• Name of the user who created the object

• Time of creation

Whenever the existing business object data is

• Both old and updated values of the object

updated

• Name of the user who updated the object

• Time of updating

466

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 10
Auditing and Data Validation

Transactional Event

When the Audit Activity is Triggered

Audit Report Content

Delete

Whenever the existing business object data is

• The last value that the object attributes

removed from the database

contained

• Name of the user who deleted the object

The event details are stored in the audit table. The attributes of the audited object data can be used in lookups
and foreign keys to display values in the audit history. The application supports displaying the audited information
according to the language settings configured.

For Oracle Fusion Middleware products, events such as failed sign-in attempts are used as triggers. In absence of an
audit table, the information is stored in the sandbox and presented only in English.

Note:  This topic focuses on the create, update, and delete event types available in Fusion Applications. For details on
events used in the Oracle Fusion Middleware products, refer to the Oracle Fusion Middleware documentation. See:
Introduction to Oracle Fusion Middleware Audit Framework

Related Topics

• View Audit Reports

Data Security in Payroll Data Validation Reports

Configure the Data Validation Report to run based on the profile of the user who submits the report.

For example, if a user has access to employees only within a specific payroll or department, you can configure the report
to only report data for those employees. The access the user has is defined by the data security profile attached to the
user's role.

Here are the tasks required to configure and run the report based on the profile of the user submitting the report:

1. Sign in as IT Security Manager and define HCM data roles and setup data security. Assign the data roles to the

application user as per the requirement of your enterprise.

2. Sign in as Payroll Manager and secure the 'Payroll Data Validation Report' at the Legislative Data Group level.
3. Sign in as application user to whom the privileges are assigned and run the report.

Define Data Roles and Assign Data Roles to the Application User
No predefined HCM data roles exist. While creating an HCM data role, include a job role. The secured HCM object types
that the job role accesses are identified automatically, and sections for the appropriate security profiles appear. Select or
create security profiles for those object types in the HCM data role.

For each object type, you can include only one security profile in an HCM data role, which is known as Security Profile.
Consider the following to complete the setup.

• You must have the IT Security Manager Job role to perform this task.

• To create an HCM data role, use the Assign Security Profiles to Role task in the Setup and Maintenance work

area.

467

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 10
Auditing and Data Validation

• For more information on setting up the data security as per the requirement of the enterprise, see Oracle

Human Capital Management Cloud Securing HCM.

Here are the steps required to configure the report based on the profile of the user submitting the report.

1. Search and select the Payroll Flow Patterns task from Payroll  in My Client Groups on your Home page.
2. Search for the Run Payroll Data Validation Report flow pattern.
3. Select the required Legislative Data Group.
4. Click Edit.
5. Click Go to Task and click Edit.
6. Select the row and click the Edit on the tool bar for the row.
7. Select the Secure Process or Report check box and click Save.
8. Alternately, you can click on Remove all Updates.

Repeat these steps for each Legislative Data Group, where the setting must apply. This configuration, although done on
the delivered flow pattern, is preserved during patching and upgrades.

Submit Report
When you submit the report, consider the following:

• Select the Payroll Statutory Unit (PSU) from a secured list of values. If the user's data security is restricted by

the PSU, then the user can only run the report for that PSU they have access to, even if the report is run as the
elevated user by default.

•

If the user's data access is restricted based on other attributes like department or payroll, configure the report
based on the user profile. This is only if you must restrict the report to the profile of the user submitting the
report and only data for the department or payroll is reported.

468

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 11
Implementing Payroll Costing

11  Implementing Payroll Costing

Overview of Payroll Costing

Payroll costing tracks all your costs incurred to compensate your employees and distribute those costs to General
Ledger. For example, salary, bonuses, paid leave, employer-paid portion of all payroll taxes are tracked and disbursed as
expenses to your work structure.

• The Payroll Cost Allocation key flexfield is the basis for the accounting entries to be created and reported to
track your labor costs. Consider all aspects and impact of this flexfield and its uses during your planning.

• Calculate Payroll flow calculates payroll, produces run results and costs them to your work structure and

costing hierarchy:

◦ Cross-Validation Rules validate payroll cost account combinations during the costing process and prevent

invalid combinations entries sent to general ledger.

◦ Payroll costing derives a cost account number for each payroll run result. Typically each segment of the

cost account number represents the general ledger accounting structure; however this may not always be
the case.

◦ Payroll costing values are mapped to various segments of the customer's general ledger accounting

structure.

• Calculate Costing of Payments flow creates costing results based on the prepayment results. And, when

applicable, after the cash management reconciliation it allocates costs for payment results, to include voided,
cleared and external payments.

• Calculate Retroactive Costing flow recalculates costs for retroactive changes to costing.

• Cost Adjustments are corrective actions applied to the payroll run costing result and, based on the payroll run,

to reports and calculations.

• Calculate Partial Period Accruals flow calculates costs for a pay period that overlaps two accounting periods to

create accrual entries for partial pay.

• Transfer to Subledger Accounting flow transfers payroll costs to subledger accounting (SLA) for review, reports

and posts to the General Ledger.

• Reverse Transfer to Subledger Accounting flow reverses the payroll subledger accounting entries that were

posted in final mode using the Create Accounting process.

Setup Tasks and Considerations
Set up enterprise structures, legal entities, and organizations to create and maintain information related to people,
employment, and work structures. The setup also includes tasks to define payroll business objects required for
processing and costing payroll, processing payments, and generating statutory reports.

Use this table of setup tasks to plan your implementation of payroll and payroll costing for your business requirements.

Payroll

Description

Cost Accounting

Legal entities, legal reporting units, tax reporting units, payroll statutory units, legal authorities, legal
registrations and jurisdictions, and legal authorities.

469

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 11
Implementing Payroll Costing

Payroll

Description

Cost and Profit Planning

Organization structures, business units, and organization models that best suit your business process.

Landed Cost Management

Configure elements and formulas to record earnings and deductions for processing payroll and
reporting.

Project Costing Base

Define payroll objects and payment methods required for payroll calculations and reporting, and
processing and making payments.

Payroll Costing Setup
Use Payroll Costing and Cost Allocation setup tasks to configure key flexfields, value sets, descriptive flexfields,
messages and other costing structures.

Start your implementation of Global Human Resources Cloud Payroll Costing as a user with the Application
Implementation Consultant role (ORA_PAY_APPLICATION_IMPLEMENTATION_CONSULTANT_JOB). Refer to the
Functional Setup Manager guide to manage the opt-in and setup of your offerings.

You typically set up costing during your initial payroll implementation. As new objects, such as payrolls, departments
and jobs are added, you may have additional configuration but only at the costing level.

• Costing setup may use person-specific data, such as a department or a legislative area like state, county or city,

referred to as contexts.

• Unique costing for a person or an element entry may be entered on an as needed basis during regular payroll

processing.

Refer to the Administering Global Payroll Costing guide in the Oracle Help Center for details about implementing and
administering payroll costing.

Related Topics

• Overview of Payroll Flows

• About This Administering Global Payroll Costing Guide

• How Payroll Costing Components Integrate with Other Applications

• How Distributed Costing Is Calculated

• Payroll Costing Report

470

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 12
Implementing Payroll Core

12  Implementing Payroll Core

Overview of Payroll Core

Implement Payroll Core for countries that Oracle doesn't have a localized version of the payroll application.

The Payroll Core application is a flexible payroll solution for companies that manage different pay structures for
employees working around the world. These employees are often not subject to local pay rules like taxes, overtime, or
minimum wage but they must adhere to unique international pay practices.

Oracle provides localized versions of the global payroll product to meet country-specific statutory and legislative
requirements for several countries across the globe: United States, Canada, Mexico, United Kingdom, China, Kuwait,
Saudi Arabia, United Arab Emirates, Qatar, and Bahrain at present time.

With Payroll Core, Oracle allows you to set up payroll requirements for countries Oracle doesn’t support. Payroll Core
typically includes the following:

• A generic set of features for you to run the basic payroll processes.

• A set of payroll objects that you must configure for the specific country. For example, you must define the

country and set the default currency of the country that you are processing payroll and paying your employees.

• The application doesn’t have any predefined objects like jurisdictions, elements, balances, payment types, and

so on. You must define these objects as required.

• Taxation isn’t delivered, but it can be configured with Elements and Fast Formulas.

Setup Tasks for Implementing Payroll Core

To implement the Payroll Core application, sign-in as a user with Application Implementation Consultant or Payroll
Implementor role and opt into the offerings applicable to your business requirements.

Refer to the Functional Setup Manager guide to manage the opt-in and setup of your offerings.

Before you begin implementing Payroll Core, you must complete:

•

•

Initial application setup.

Implementation of Global Human Resources and HR setup tasks for implementing and processing payroll. For
more information, refer to the Implementing Global Human Resources.

The Payroll Core application is best suited for countries that do not have complex local taxes and social insurance
calculations and hence has no requirement for setting up calculation components and calculation cards. The application
uses elements and formulas to calculate employee wages and compensation and aggregate balance accruals.

Before you begin, refer to the ‘Setup Tasks for Implementing Global Payroll’ topic in the Implementing Global Payroll
guide. The following sections explain the points that you must consider and are specific to the Payroll Core application.

To implement Payroll Core you will need to perform most of these tasks from the Setup and Maintenance work area.
Use My Enterprise on the Home page to navigate to Setup and Maintenance.

471

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 12
Implementing Payroll Core

Prerequisite Tasks for Payroll Core Setup
Before you set up the payroll components ensure that you have completed these tasks.

1. Create an Implementation Project

Setup tasks for organization structures are defined in an implementation project. Create an implementation
project and select the Workforce Deployment offering to generate the setup tasks required to set up the Payroll
Core application.

2. Create Country

Use the Manage Territories task and search for your territory on the Manage Territories page. If you find your
territory, you can edit the description to match your requirements. Don't edit territory names or codes. Use the
territory code and name to verify geographies, create legal addresses, and select the country extension.
If you are unable to find your country in the predefined territories list in the application, create the country.

3. Select Default Currency

On the Manage Territories page, select the default currency for the country. This is the currency in which
balances are accumulated for this legislation.

4. Verify Geographies

Use the territory code to verify predefined geographies and load any additionally required local geographies.

5. Define Enterprise Structures for HCM

The Enterprise classification represents the top most structure in the organization. A person exists within the
context of an enterprise. An enterprise doesn’t adhere to any legislation. Country specific attributes are stored
at the level of a Legal Entity.

a. Define a legislative data groups (LDGs) for your country and associate it with one or more payroll

statutory units (PSUs). Each PSU can belong to only one LDG. An LDG is used to partition your payroll
and related data. Payroll-related info, such as elements, is organized by LDG.

b. Create legal addresses for all organizational units of the enterprise before you create legal entities. A legal

address is the address of record for an entity.

c. Define a legal entity that is both a legal employer and a PSU. Define Legal Entity HCM information as

required.

Payroll Setup Tasks

1. Select Country Extensions and Address Validation Rules

Since you are processing payroll and paying your employees, select Payroll as your country extension. Select
the address style and address validation for your country. The address style you select determines which
address attributes are available and maintained in the application. The combination of address style and
address validation determines the level of validation.

2. Define Payroll Legislations

a. Use the Configure Legislations for Human Resources task to define legislative rules. Legislative rules

govern default values and determine how you manage employee records in your organization. Base your
selections for the following attributes on the statutory requirements of your country.

- Payroll relationship rule for your country determines how employment records are created when

employees are hired or rehired.

- If you plan to capture information for payroll payment purposes, map a person type to a payroll

relationship type. Select appropriate values for your country.

472

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 12
Implementing Payroll Core

b. Use the Configure Payroll Legislations task to define payroll-related data, such as legislative rules,
element classifications, payment types, component groups, balance dimensions, and other related
objects.

3. Define Elements

Elements are the building blocks of payroll and benefits. You can define elements using the element template.
Define elements to calculate specific earnings, deductions, and other payroll data for reporting, compensation,
absences, and benefits calculations.

4. Define Balances

Payroll balances show the accumulation of values over a period of time. The values can be currency, hours,
or any other numeric value. Balances are created automatically when creating elements. You can edit the
definition of these generated balances, or create additional balances for calculations or reporting.

The value assigned to a balance during processing is determined by balance feeds defined for the balance.
Balance feeds can be by element input values or by balance classification run results. When you create a new
balance, it must be associated with a category and categories cannot be added or modified.

5. Define Formulas

The Elements task generates standard element skip and calculation formulas. Use the Fast Formulas task to
modify the formulas to suit your requirements. Refer to ‘Overview of Using Fast Formulas’ for more information
on formula types and how you can use them to control processing and validate element entry values.

6. Define Payroll Definitions

When you create a payroll definition, the application generates the complete payroll schedule based on the
payroll period type, the offsets or calendar adjustments, and the number of years that you specify. Each payroll
in the schedule is assigned a unique name. Assign employees to a payroll definition on the Payroll Relationships
page.

7. Define Payment Methods and Payment Types

Create at least one Organization Payment Method (OPM) for each combination of LDG, payment type, and
currency that you use to disburse wages and other compensation. When you create an OPM, select a payment
type and define at least one payment source for each OPM.

Other Document References
For more detailed information about the setup tasks and other related applications and tasks, refer to these guides at
docs.oracle.com/cloud/latest/globalcs_gs/docs.htm.

•

Implementing Global Payroll

• Administering Global Payroll

• Administering Global Payroll Flows

• Administering Fast Formula

• Administrating Payroll Costing

•

•

•

•

Implementing Absence Management

Implementing Benefits

Implementing Time and Labor

Implementing Workforce Compensation

473

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 12
Implementing Payroll Core

TRU Defaulting Rules for Payroll Core

For an international payroll legislation such as United Nations, you can automatically assign a Tax Reporting Unit (TRU)
to a newly hired employee.

The TRU triggers the creation of a deduction card for the employee and the necessary TRU and assignment
associations. This information ensures that an international employee is successfully processed in the Calculate Payroll
process.

Use the Configure Legislations for Human Resources task and select any of the TRU defaulting rule options in the
Deduction Card – Tax Reporting Unit Association section on the Legislative Rules page. The option you select controls
how deduction cards and associations are created for a newly hired employee. The three TRU defaulting rule options are
explained here.

Assign Employee Details Using Main TRU
Select this option if you have these requirements:

• You don't have a need to calculate employee taxes.

• You are paying all your employees within a legislative data group in the same currency.

• You don’t have to capture tax reporting information at employee level for tax calculation purposes.

The payroll run assigns the main TRU for the organization to the newly hired employee and automatically creates the
deduction card and association at the assignment level.

Assign Employee Details Using TRU Currency
Select this option if you have these requirements:

• Your organization has employees who are in multiple countries and are paid in different currencies within a

single legislative data group.

• You don’t have a requirement to calculate employee taxes.

For each currency that you pay your employees, define a TRU within a payroll statutory unit.

The payroll run uses the salary basis currency of the employee to assign a TRU with the corresponding currency to the
newly hired employee. For example, when an employee is assigned to a salary basis with a currency of USD, they are
assigned to the TRU that also has a USD currency.

The run automatically creates the deduction card and association at assignment level.

Enter Employee Details
Select this option if you have a need to capture tax reporting information at employee level for tax calculation purposes.

During new hire manually assign a TRU, deduction card, and assignment association to an employee.

474

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 12
Implementing Payroll Core

Considerations to Assign Employee Details Using TRU
Currency

While configuring an international payroll legislation, select the Assign employee details using TRU currency option if
you have the following requirements:

• You have an organization that has employees in multiple countries and you pay the employees in multiple

currencies.

• You don’t have a requirement to calculate employee taxes.

• You need to generate separate payroll reports for each currency.

Here are some aspects you must consider while configuring the legislation.

Create TRU
For each currency that you pay your employees, define a tax reporting unit (TRU) within a payroll statutory unit (PSU)
and capture the currency of the TRU. For example, create a TRU for Afghan Afghani currency and a separate TRU for
Euros. All employees located in countries which use the euro currency, such as those based in France or Slovenia, are
allocated to the same TRU. Define both the TRUs within a single PSU.

Note:  You must only create a single TRU for each currency.

Use the TRU to group employees, within a Legislative Data Group (LDG), based on their salary currency.

This approach facilitates the following:

• You can calculate payroll balances for each different currency and TRU.

• You can generate separate payroll reports for each currency. TRU is a supported context for balances used in

payroll reports such as the payslip.

Salary Basis Currency of Employee
The payroll run uses the salary basis currency of the employee to identify a TRU and associate it to the employee. The
salary basis currency of an employee is derived from the input currency of the element associated to the salary basis.

For example, when an employee is assigned to a salary basis with a currency of Euro, the payroll run assigns the
employee to the TRU that also has a Euro currency.

Note:  Define the elements at the assignment level.

What Happens when you Process Payroll?
Subsequently, when you run the payroll, the payroll run initiates and completes the following:

•

Identifies the TRU based on the salary basis currency of the employee and associates the TRU to the employee.

475

Oracle Fusion Cloud Human Resources
Implementing Global Payroll

Chapter 12
Implementing Payroll Core

• Creates the tax card and the assignment association.

• Calculates payroll and completes all other processes. The payroll run uses the TRU context and calculates

balances for each different currency and TRU.

Updates to the Initial Configuration
For any subsequent updates, consider the following:

•

If an employee moves to another country and payment currency, consider the following:

◦ Define a new TRU for the new currency and manually assign the new TRU to the employee.
◦ Create a new assignment and a new tax card for the new assignment. An employee can’t have multiple,
concurrent tax cards. You must end the original tax card and create a new one for the new assignment.

• During a global transfer, consider the following:

◦ For transfers within the same PSU or legal employer, create a new assignment under the same payroll

relationship. TRU and assignment associations are created for the existing deduction card.
◦ For transfers to a different PSU or legal employer, create a new assignment under a new payroll

relationship. A new deduction card, TRU and assignment association are created.

476

