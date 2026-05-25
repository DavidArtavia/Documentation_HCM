Oracle Fusion
Cloud Human
Resources

Implementing Absence
Management

Oracle Fusion Cloud Human Resources
Implementing Absence Management

G34709-01

Copyright © 2011, 2024, Oracle and/or its affiliates.

Author: Shine Mathew

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Contents

Get  Help  ................................................................................................................................    i

1 Absence Management Implementation Overview

1

How You Set Up Absence Management ....................................................................................................................................  1

Setup Tasks for Implementing Absence Management ..........................................................................................................   2

Absence Management Integrations ...........................................................................................................................................   4

How Absence Components Work Together .............................................................................................................................   6

How an Individual's Schedule Is Identified ...............................................................................................................................  9

2 Responsive User Experience Setup

13

Deep  Links  ......................................................................................................................................................................................     13

3 Absence Lookups, Value Sets, and Flexfields

15

Overview of Lookups ...................................................................................................................................................................   15

How Flexfields and Value Sets Work Together ......................................................................................................................   19

Overview of Flexfields .................................................................................................................................................................  20

4 Formula Creation and Error Handling for Absence Management

23

Overview of Using Formulas .....................................................................................................................................................   23

Formulas for Absence Type .......................................................................................................................................................   24

Formulas for Accrual Plans ........................................................................................................................................................   25

Global Absence Elective Disbursement Evaluation Formula ..............................................................................................   27

Formulas for Qualification Plans ...............................................................................................................................................   31

Formulas for Donation Plans .....................................................................................................................................................   31

Example of Writing a Fast Formula Using Formula Text .....................................................................................................  32

Formula Compilation Errors .......................................................................................................................................................  33

Formula Execution Errors ...........................................................................................................................................................  35

FAQs  ................................................................................................................................................................................................     36

5 Eligibility Profiles for Absence Plans

39

How You Configure Eligibility for an Absence Plan ..............................................................................................................  39

Oracle Fusion Cloud Human Resources
Implementing Absence Management

How Eligibility Works With Other Objects ..............................................................................................................................   39

Derived  Factors  .............................................................................................................................................................................     41

Examples of Derived Factors .....................................................................................................................................................  42

Example of Using Range of Scheduled Hours ......................................................................................................................  46

Eligibility Profiles ..........................................................................................................................................................................  47

Examples of Eligibility Profiles ...................................................................................................................................................  51

Single or Multiple Eligibility Profiles ........................................................................................................................................   53

Create a Participant Eligibility Profile ......................................................................................................................................   54

FAQs  ................................................................................................................................................................................................     57

6 Rate Definitions for Absence Payments

59

Rate Definitions for Absence Payments .................................................................................................................................   59

Overview of Rate Definitions ....................................................................................................................................................   60

Options to Configure Rate Definitions ....................................................................................................................................   62

Create Rate Definitions for Leave ............................................................................................................................................   66

7 Elements for Absence Management

69

Define Payroll Elements to Process Absences ......................................................................................................................   69

Define Payroll Elements for an Absence Accrual Plan .........................................................................................................  72

8 Effective Dates in Absence Management

77

Date  Effectivity  ..............................................................................................................................................................................    77

Examples of Correcting Date-Effective Objects ....................................................................................................................  78

Examples of Updating Date-Effective Objects ......................................................................................................................  80

FAQs  .................................................................................................................................................................................................    81

9 Accrual Absence Plans

83

Types of Absence Plans ..............................................................................................................................................................  83

Options to Define Accrual Plans ..............................................................................................................................................   84

Options to Define an Accrual Term .........................................................................................................................................   86

Options to Configure Accrual Enrollment and Termination ...............................................................................................   87

How You Configure Eligibility for Absence Plans .................................................................................................................   88

Carryover Limit Rules ..................................................................................................................................................................  88

Carryover Expiration Rules ........................................................................................................................................................   89

Options to Define Frequency of Accrual Periods .................................................................................................................   89

Plan Limits for Accrual Plans ....................................................................................................................................................   90

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Examples of Accrual Bands .......................................................................................................................................................  90

How You Configure a Plan for Discretionary Cash Disbursement ....................................................................................   93

Options to Enable Absence Accrual Balance Adjustments ................................................................................................   94

Automatic Plan Enrollment and Balance Copy During Local and Global Transfer ........................................................   95

Create a Vacation Accrual Plan .................................................................................................................................................  96

Managing Existing Absence Plans .........................................................................................................................................   102

FAQs  ...............................................................................................................................................................................................    102

10 Qualification Absence Plans

105

Types of Absence Plans ............................................................................................................................................................  105

Options to Define Qualification Plans ...................................................................................................................................   106

Options to Define a Qualification Term ................................................................................................................................   107

Options to Define Overlap Rules for Qualification Plans ..................................................................................................   108

Options to Configure Qualification Enrollment and Termination ......................................................................................  111

How You Configure Eligibility for Absence Plans .................................................................................................................  112

Examples of Qualification Bands .............................................................................................................................................   112

Evaluate Entitlement without Absence Record .....................................................................................................................  115

How Qualification Plan Entitlement Appears .......................................................................................................................   116

Open-ended Absences ...............................................................................................................................................................  117

Create a Maternity Plan .............................................................................................................................................................   118

How You Create a Shared Parental Leave Agreement .......................................................................................................   124

11 Compensatory Time

127

Options to Define Compensatory Plans ................................................................................................................................   127

Expiration Rules for Earned Compensatory Time ...............................................................................................................  128

12 Donation

129

Overview of Donation ................................................................................................................................................................  129

Options to Define Donation Plans ..........................................................................................................................................  129

How You Can Set Up PTO Donations for Your Legislation ...............................................................................................   130

Create a Donation Plan ..............................................................................................................................................................   131

How You Configure Donation Rules on an Accrual Plan for Workers to Donate to Coworkers ...................................  131

Configure Approvals for Donation ..........................................................................................................................................   132

Enroll a Worker in a Donation Plan ........................................................................................................................................   132

13 Absence Types, Reasons, and Categories

135

How Absence Components Work Together ..........................................................................................................................  135

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Absence Display and Processing Rules .................................................................................................................................   137

Absence Approval and Processing Rules ..............................................................................................................................   139

Absence Dates and Duration Rules .......................................................................................................................................   140

Allow Daily Absence Duration Override .................................................................................................................................  141

Options to Configure Display of Supplemental Details ......................................................................................................   141

Examples of Start Date Validation Rule ................................................................................................................................   142

How HCM Assignment Security Works With Absences Impacting Multiple Assignments .........................................   143

How You Configure Absence Types to Prevent Absences From Impacting Multiple Assignments ...........................  145

How You Configure Plans to Offer Concurrent Entitlement .............................................................................................   146

Examples of Prioritizing Absence Plans for an Absence Type .........................................................................................   146

Examples of Configuring a Concurrent Absence Type ......................................................................................................   147

Stop Sending ICS Calendar Invite Files in Absence Notifications ....................................................................................  147

Schedule Hierarchy Start Point Options ...............................................................................................................................   148

Create a Vacation Absence Type ............................................................................................................................................   148

FAQs  ................................................................................................................................................................................................    151

14 Absence Certifications

153

Options for Absence Certification Requirements ................................................................................................................  153

Absence Certification Requirement Types ............................................................................................................................   153

Options to Trigger Certification Requirements ....................................................................................................................  154

Options to Manage Actions For Certification Events .........................................................................................................   155

Create an Absence Certification Requirement .....................................................................................................................  156

15 Absence Processes

159

Overview of Absence Processes .............................................................................................................................................   159

Options for the Evaluate Absences Process ........................................................................................................................   160

Options for the Evaluate Certification Updates Process ....................................................................................................   161

Options for the Update Accrual Plan Enrollments Process ...............................................................................................  162

Options for the Calculate Accruals and Balances Process ................................................................................................   163

Options for the Withdraw Accruals and Balances Process ................................................................................................  165

Generate Daily Breakdown of Absence Details Process ....................................................................................................   166

Create Event Processing Rules to Reprocess Absences ....................................................................................................   168

16 Integrated Workbooks for Loading Absence Data

171

Integrated Workbooks for Absence Management ...............................................................................................................   171

Update Absence Data Using HCM Spreadsheet Data Loader ..........................................................................................   172

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Set Up Desktop Integration for Excel .....................................................................................................................................  172

Guidelines for Using Desktop Integrated Excel Workbooks ..............................................................................................   173

Troubleshoot Desktop Integration for Excel .........................................................................................................................  174

FAQ  .................................................................................................................................................................................................    175

17 HCM Extracts for Absence Data

177

HCM Extracts for Absence Data ..............................................................................................................................................  177

Define Extracts ............................................................................................................................................................................   177

Reconcile Absences and Payroll Info ......................................................................................................................................   181

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Get Help

Get Help

There are a number of ways to learn more about your product and interact with Oracle and other users.

Get Help in the Applications

  to give you access to contextual help. If you don't see any help icons on
Some application pages have help icons
your page, click your user image or name in the global header and select Show Help Icons. If the page has contextual
help, help icons will appear.

Get Support
You can get support at My Oracle Support. For accessible support, visit Oracle Accessibility Learning and Support.

Get Training
Increase your knowledge of Oracle Cloud by taking courses at Oracle University.

Join Our Community
Use Cloud Customer Connect to get information from industry experts at Oracle and in the partner community. You
can join forums to connect with other customers, post questions, suggest ideas for product enhancements, and watch
events.

Learn About Accessibility
For information about Oracle's commitment to accessibility, visit the Oracle Accessibility Program. Videos included in
this guide are provided as a media alternative for text-based topics also available in this guide.

Share Your Feedback
We welcome your feedback about Oracle Applications user assistance. If you need clarification, find an error, or just
want to tell us what you found helpful, we'd like to hear from you.

You can email your feedback to oracle_fusion_applications_help_ww_grp@oracle.com.

Thanks for helping us improve our user assistance!

i

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Get Help

ii

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 1
Absence Management Implementation Overview

1  Absence Management Implementation
Overview

How You Set Up Absence Management

Create absence plans and types to enable people to record their time off. Define authorization rules and set up payment
rules for employees on long term absence, such as maternity and sick leave.

These tasks in the Setup and Maintenance work area are part of the Workforce Deployment offering in the Absence
Management functional area.

Getting Started
Before you begin, review the following documents available in the Absence Management functional area:

• Lists of setup tasks

• Descriptions of the functional areas and features you can select when you configure the offering

• Lists of business objects and enterprise applications associated with the offering

Setup Sequence
The following figure illustrates the sequence for setting up absence management:

1. Add new values to lookups, value sets, and flexfields based on your requirement. Write fast formulas to include
rules in the absence objects in addition to the predefined ones. Create rate definitions to define payment rates
for absence plans.

2. Create absence plans to define rules for time accruals and entitlements. Create certification requests that you
want workers to complete to continue receiving entitlements during absence periods. Create absence reasons
that you want workers to select while recording absences.

3. Create absence types, such as sickness leave or vacation, and associate each type with the relevant plans,

reasons, and certifications.

4. Create absence categories, such as personal leave or medical leave, and associate them with the relevant

absence types for reporting purposes.

1

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 1
Absence Management Implementation Overview

Setup Tasks for Implementing Absence Management

Before you start implementing the Absence Management application, review the following setup tasks.

Task List

Task name

Description

Recommended Help

Define Absences

Absence Certifications

Absence Reasons

Absence Plans

Configure, review, and update
absence certifications, which are
requirements that the worker must
complete to continue receiving
entitlements during an absence
period.

Review, create, and update
absence reasons, which further
describe the nature of the
absence type with which they are
associated.

Review, create, and update
absence plans, which contain
rules to define how absence
entitlements are provided to
employees.

• Options for Absence

Certification Requirements

• Absence Certification
Requirement Types

• Options to Trigger

Certification Requirements

• Options to Manage Actions
For Certification Events

How Absence Components Work
Together

• Types of Absence Plans

• Options to Define Accrual

Plans

2

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 1
Absence Management Implementation Overview

Task List

Task name

Description

Recommended Help

Absence Types

Absence Categories

Leave Agreements

Define Absence Formulas and
Rates

Define Absence Time Periods

Define General Absence

Manage Global Absences Lookups

Manage Global Absences Value
Sets

Manage Global Absences
Descriptive Flexfields

• Options to Define

Qualification Plans

• Options to Define

Compensatory Plans

• Options to Define Donation

Plans

Review, create, and update
absence types, which are used to
record absences. You can configure
rules to determine which fields or
sections a particular worker sees
based on their role. You can also
define the rules of the absence. For
example, you can restrict workers
so that they can record absences
only of a particular duration.

• How Absence Components

Work Together

• Absence Display and
Processing Rules

• Absence Approval and

Processing Rules

• Absence Dates and Duration

Rules

How Absence Components Work
Together

How You Create a Shared Parental
Leave Agreement

Review, create, and update
absence categories, which are used
to group related absence types for
reporting and analysis.

Review, create, and update
shared parental leave agreements
between an employee and partner.
The shared parental leave enables
workers to curtail their maternity or
adoption leave in order to share it
with their partner.

Define formulas and rates for
absence.

Overview of Using Formulas

Define time periods for absence
processing.

Options to Define Frequency of
Accrual Periods

Review and edit predefined lookup
values for global absences, such as
absence categories and reasons,
 and define new values.

Manage value sets to validate the
content of a flexfield segment for
global absences.

Configure validation and
display properties of descriptive
flexfields for global absences.
Use descriptive flexfields to add
attributes to entities.

Overview of Lookups

How Flexfields and Value Sets Work
Together

• Overview of Flexfields

• How Flexfields and Value Sets

Work Together

HCM Availability Types

Review, create, and edit availability
types used to define contracted or
other availability for a worker.

How You Configure and Assign
Work Schedules

3

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 1
Absence Management Implementation Overview

Security Reference
The tasks that people can do and the data that they can see depend on their roles, duties, and privileges. For
information about these factors, see these two guides:

• Securing HCM

• Securing Reference for HCM

Absence Management Integrations

Here's a diagram that shows you which features originating from other products are used in Absence Management. The
diagram also shows which Absence Management features are used elsewhere. Products that require a separate license
are indicated accordingly.

4

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 1
Absence Management Implementation Overview

Here's a table that explains the connections used in the diagram.

5

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 1
Absence Management Implementation Overview

Feature

Description

Integration

License Required

HCM Extracts

Extract past and future absences

Integrates out of Absence

No

and open-ended absences, in

Management

various formats.

HCM Data Loader

Load en masse absence plans,

Integrates into Absence

 absence entries, and balances.

Management

Eligibility profiles

Add eligibility profiles to determine

Integrates into Absence

whether a person qualifies for

Management

enrollment in an absence plan.

No

Yes

Rate definitions

Use a rate definition to determine

Integrates into Absence

Yes

the rate of a single unit of absence

Management

for payment during an absence

period.

Payroll elements

Define elements to calculate and

Integrates both ways

process absence payments.

Calendar

Absence entries display on

Integrates out of Absence

calendar and work schedules.

Management

Time cards

Add absence entries in time cards.

Integrates out of Absence

Management

Fast Formulas

Use formulas to define special

Integrates out of Absence

absence management rules and

Management

calculations.

Yes

Yes

Yes

Yes

How Absence Components Work Together

Configure absence components such as types, categories, patterns, plans, reasons, and certifications to reflect the
absence management policy of your enterprise.

Component

Location in the Absences Work Area

Absence types

Use the Absence Types task to create absence types.

Absence categories

Use the Absence Categories task to create absence categories and associate them with absence types.

Absence patterns

Review these settings on the Display Features tab when you create an absence type.

Absence plans

Use the Absence Plans task to create absence plans.

6

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 1
Absence Management Implementation Overview

Component

Location in the Absences Work Area

Absence reasons

Use the Absence Reasons task to create absence reasons.

Absence certifications

Use the Absence Certifications task to set up a requirement. Then associate the requirement as an
action item with an absence type so that every absence associated with the absence type is subject to
that requirement.

This figure illustrates how the absence management components fit together.

Absence Type
When you create an absence type, such as sick leave, you include rules to determine when users record or manage
an absence of that type. For example, you can restrict workers so that they can record absences only of a particular
duration. An alert appears if the entered duration exceeds the maximum value.

Decide which fields or sections you want to show or hide for specific user roles when they record or approve a specific
absence type.

Absence Category
Create absence categories to group absence types for reporting and analysis. For example, you can create an absence
category called family leave and associate with it absence types, such as maternity, paternity, and child care.

7

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 1
Absence Management Implementation Overview

Absence Pattern
An absence pattern contains a predefined set of rules that you can use as a starting point to create an absence type.
When you create an absence type, you must associate it with any of the following predefined patterns:

•

Illness or injury

• Childbirth or placement

• Generic absence

For example, you can select the Generic absence pattern to create an absence type to schedule vacation time using the
time accrued under a vacation accrual plan.

The pattern that you select determines:

• Whether special fields appear on the absence type pages

• The options available to display and process various aspects of absence recording

For example, the Childbirth or placement pattern displays a field for selecting whether the absence type applies for
childbirth or adoption placement.

Absence Plans
Create absence plans to define rules for accruing leave time and receiving payments during an absence period. You
must associate at least one absence plan with an absence type.

To schedule an absence using an absence plan, the unit of measure defined in the plan must match the unit of measure
defined in the associated absence type. If the unit of measure differs, you can define the conversion formula and attach
it to the absence type. This formula is applicable only if the unit of measure is hours or days for the absence type.

Absence Reasons
Create absence reasons to select from when scheduling an absence. Absence reasons are independent of absence
types. You can use the same reason for multiple absence types. When you create an absence type, you associate the
reasons with the type.

Absence Certifications
Create certification requirements for absences that require documentation to authorize an absence. For example,
in case of an absence due to illness, set up a requirement that workers must submit a doctor's certificate within a
stipulated period of time. This ensures they receive full payment for the absence duration.

Related Topics

• Create a Vacation Absence Type

• Create a Maternity Plan

• Create a Vacation Accrual Plan

• Create an Absence Certification Requirement

8

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 1
Absence Management Implementation Overview

How an Individual's Schedule Is Identified

You can set up an individual's work time in different ways. So, the process that identifies a person's official schedule for
a selected time period uses the individual's current schedule or work hours. It also considers applicable calendar events,
work schedule resource exceptions, and absence entries.

Search Order
The process searches for someone's schedule in this order, before applying the result to the assignment:

1. Published schedule
2. Employment work week
3. Primary work schedule
4. Standard working hours

If the process doesn't find a schedule, it uses the default hours 8:30a to 5:00p.

9

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 1
Absence Management Implementation Overview

Published Schedule (Workforce Management)
The process builds the published schedule using the employment work week, primary work schedule, or standard
working hours for each person. It can also build it using published schedules from other scheduling apps. The published
schedule shows applicable calendar events and absences.

Employment Work Week
The person's employment record can include the setup for their employment work week. Schedules that the process
builds from the work week also show applicable calendar events and absences.

Primary Work Schedule
The primary work schedule links to one of these levels. Schedules that the process builds from the work schedule also
show assigned calendar events and resource exceptions, and applicable absences.

1. Primary assignment of the person
2. Position
3. Job
4. Department
5. Location
6. Legal Employer
7. Enterprise

The process moves through the schedule hierarchy in the specified order and stops as soon as it finds a primary
schedule. This example hierarchy shows primary work schedules associated with three levels.

10

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 1
Absence Management Implementation Overview

Departments 1 and 3 don't have primary schedules, so the primary schedule at the enterprise level applies to everyone,
with one exception. A person in department 3 has a schedule for their primary assignment. That primary assignment
schedule applies instead of the enterprise-level schedule. Department 2 has a primary schedule, and it applies to
everyone in that department.

The calendar events and resource exceptions that exist in the primary work schedule affect everyone's schedules,
regardless of level. Any absences they report during the selected time period also affect the individual's schedule.

Standard Working Hours
The person's primary assignment includes their standard working hours. Schedules built with these hours also show
applicable calendar events and absences.

11

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 1
Absence Management Implementation Overview

12

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 2
Responsive User Experience Setup

2  Responsive User Experience Setup

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

13

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 2
Responsive User Experience Setup

14

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 3
Absence Lookups, Value Sets, and Flexfields

3  Absence Lookups, Value Sets, and Flexfields

Overview of Lookups

Lookups are lists of values in applications. You define a list of values as a lookup type comprising a set of lookup codes,
each code's translated meaning, and optionally a tag.

On the UI, users see the list of translated meanings as the values available for selection. Lookups provide a means of
validation and lists of values where valid values appear on a list with no duplicate values. For example, an application
might store the values Y and N in a column in a table, but when displaying those values in the user interface, Yes or No
(or their translated equivalents) should be available for users to select. For example, the two lookup codes Y and N are
defined in the REQUIRED_INDICATOR lookup type.

Note:  Don't include spaces in lookup codes. Use the underscore character (_) to separate the words if needed. For
example, instead of creating the lookup code as DEV PROGRAM, create it as DEV_PROGRAM.

The following table contains an example of a lookup type for marital status (MAR_STATUS) that has lookup codes for
users to specify married, single, or available legal partnerships.

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

In this case, tags are used for localizing the codes. All legislations list Married and Single. Only the Dutch legislation lists
Registered Partner. And all legislations except France and Australia also list Domestic Partner.

When managing lookups, you need to understand the following.

• Using lookups in applications

• Configuration levels

• Accessing lookups

• Enabling lookups

• The three kinds of lookups: standard, common, and set-enabled

Using Lookups in Applications
Use lookups to provide validation or a list of values for a user input field in a user interface.

15

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 3
Absence Lookups, Value Sets, and Flexfields

An example of a lookup used for validation is a flexfield segment using a table-validated value set with values from a
lookup type. An example of a lookup in a list of values is a profile option's available values from which users select one
to set the profile option. Invoice Approval Status gives the option of including payables invoices of different approval
statuses in a report. The lookup code values include All, so that users can report by all statuses: Approved, Resubmitted
for approval, Pending or rejected, and Rejected.

Configuration Level
The configuration level of a lookup type determines whether the lookups in that lookup type can be edited. This applies
data security to lookups.

Some lookup types are locked so no new codes and other changes can be added during implementation or later, as
needed. Depending on the configuration level of a lookup type, you may be able to change the codes or their meanings.
Some lookups are designated as extensible, so new lookup codes can be created during implementation, but the
predefined lookup codes can't be modified. Some predefined lookup codes can be changed during implementation or
later, as needed.

The configuration levels are user, extensible, and system. The following table shows the lookup management tasks
permitted at each configuration level.

Permitted Task

User

Extensible

System

Deleting a lookup type

Inserting new codes

Updating start date, end date, and
enabling the lookup code

Deleting codes

Updating tags

Updating module

Yes

Yes

Yes

Yes

Yes

Yes

No

Yes

Yes, only if the code isn't
predefined data

Yes, only if the code isn't
predefined data

No

No

No

No

No

No

No

No

Predefined data means LAST_UPDATED_BY = SEED_DATA_FROM_APPLICATION.

If a product depends on a lookup, the configuration level must be system or extensible to prevent deletion.

Once the configuration level is set for a lookup type, it can't be modified. The configuration level for newly created
lookup types is by default set at the User level.

Access to the REST Resources
Users can retrieve information about lookups using the following REST resources:

• standardLookupsLOV

• commonLookupsLOV

16

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 3
Absence Lookups, Value Sets, and Flexfields

• setEnabledLookupsLOV

• genericLookupsLOV

However, you can control whether a lookup is a part of the LOV or not. On the UI, for each lookup you can specify the
REST Access Secured value that in turn determines whether it's included in the response or not. These values are:

• Anonymous: Lookup is available to a user having anonymous role or authenticated role.

• Authenticated: Lookup is available to a user having only the authenticated role.

• Secure: Lookups aren't available to users as part of generic REST Resources (Standard, Common, or Set-

Enabled). To make it available, your security administrator must assign a specific function security policy for
each lookup type to a role and assign that role to the selected users.

Note:  The function security policy is provided only for predefined lookup types.

For all lookups, the default value is set to Secure. So, if you want to make the lookup available to users through any of
those resources, you must change the value to Authenticated or Anonymous, depending on who needs to access that
information.

Standard, Common, and Set-Enabled Lookups
The following table shows the available types of lookups.

Lookup Type

Description

Standard

Lists the available codes and translated meanings.

Set-enabled

Associates a reference data set with the lookup codes.

Common

Legacy lookups or lookups that have attributes.

Standard lookups are the simplest form of lookup types consisting only of codes and their translated meaning. They
differ from common lookups only in being defined in the standard lookup view. Common lookups exist for reasons
of backward compatibility and differ from standard lookups only in being defined in the common lookup view. These
can also be lookups having attribute columns. Set-enabled lookup types store lookup codes that are enabled for
reference data sharing. At runtime, a set-enabled lookup code is visible because the value of the determinant identifies
a reference data set in which the lookup code is present.

Accessing Lookups
Standard, set-enabled, and common lookups are defined in the Standard, Set-enabled, and Common views,
respectively. Applications development might define lookups in an application view to restrict the UI pages where they
might appear.

In lookups management tasks, lookups might be associated with a module in the application taxonomy to provide
criteria for narrowing a search or limiting the number of lookups accessed by a product specific task such as Manage
Purchasing Lookups.

17

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 3
Absence Lookups, Value Sets, and Flexfields

Enabling Lookups
A lookup type is reusable for attributes stored in multiple tables.

Enable lookups based on the following.

• Selecting an Enabled check box

• Specifying an enabled start date, end date, or both

• Specifying a reference data set determinant

If you make changes to a lookup, users must sign out and back in before the changes take effect. When defining a list of
values for display rather than validation, limit the number of enabled lookup codes to a usable length.

To view the predefined lookups and their lookup codes, use the following tasks in the Setup and Maintenance work
area:

• Manage Standard Lookups

• Manage Common Lookups

• Manage Set-Enabled Lookups

Translating Lookups
You can translate the lookups that you defined to the preferred language(s) without changing the language session
of the application. Use the translation option available on the lookup code table. By default, for each lookup, all the
permitted language rows in the translator dialog box appear in the source language (the current session language).
When you edit a particular language entry, you can modify the translated meaning and description to the language in
which you want the lookup to appear. Once the updates are made, the end-users can view the lookup in the translated
text.

Note:  You can add the translation for only as many languages as are permitted by the administrator. The functionality
to limit the number of languages displayed on the dialog box is controlled through the Translation Editor Languages
profile option. It can be set at the SITE or USER level. If nothing is specified, all active languages are displayed.

Deleting Lookup Types and Lookup Codes
You can delete lookup types and lookup codes from the lookups management tasks in the Setup and Maintenance
work area. For example, you can delete lookups that are part of the Purchasing module, from the Manage Purchasing
Lookups task in the Setup and Maintenance work area. Select the required lookup type to see the lookup codes
associated with it. To delete a lookup code, select the required code and click the Delete icon. To delete a lookup type,
similarly, select the required lookup type and click the Delete icon.

You can also use REST resources to delete lookup types and lookup codes.

• For more information about deleting a lookup type using REST resources, see the Delete a standard lookup

section in the  REST API for Common Features in Oracle Fusion Cloud Applications guide.

• For more information about deleting a lookup type, see the Delete a lookup code section in the  REST API for

Common Features in Oracle Fusion Cloud Applications guide.

18

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 3
Absence Lookups, Value Sets, and Flexfields

Here are a few things to know about deleting lookup types and codes:

• Certain lookup types and codes can’t be deleted, for example, predefined lookup types and codes can’t be

deleted.

• You can’t delete lookup codes in bulk. Instead, you can delete an entire lookup type.

Related Topics

• How can I access predefined lookups?

• Example of a Set-Enabled Lookup

• What's the difference between a lookup type and a value set?

• Example of a Standard Lookup

• How can I enter or edit translated text?

• Create Roles in the Security Console

How Flexfields and Value Sets Work Together

Value sets are specific to your enterprise. When gathering information using flexfields, your enterprise's value sets
validate the values that your users enter based on how you defined the value set.

You can assign a value set to any number of flexfield segments in the same or different flexfields. Value set usage
information indicates which flexfields use the value set.

The following aspects are important in understanding how flexfields and value sets work together:

• Defining value sets

• Shared value sets

• Deployment

Defining Value Sets
As a key flexfield guideline, define value sets before configuring the flexfield, because you assign value sets to each
segment as you configure a flexfield. With descriptive and extensible flexfields, you can define value sets when adding
or editing a segment.

Note:  Ensure that changes to a shared value set are compatible with all flexfield segments that use the value set.

Shared Value Sets
When you change a value in a shared value set, the change affects the value set for all flexfields that use that value set.
The advantage of a shared value set is that a single change propagates to all usages. The drawback is that the change
shared across usages may not be appropriate in every case.

Value Set Values
To configure user-defined attributes to be captured on the value set values in the Manage Value Sets task, configure the
Value Set Values descriptive flexfield. The object's code is FND_VS_VALUES_B.This flexfield expects the context code

19

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 3
Absence Lookups, Value Sets, and Flexfields

to correspond to the value set code. For each value set, you can define a context whose code is the value set code, and
whose context-sensitive segments are shown for the values of that value set. By default, the context segment is hidden
since it maps to the value set code and is not expected to be changed.

You can also define global segments that are shown for all value sets. However, this would be quite unusual since it
would mean that you want to capture that attribute for all values for all value sets.

Deployment
When you deploy a flexfield, the value sets assigned to the segments of the flexfield provide users with the valid values
for the attributes represented by the segments.

Related Topics

• Overview of Flexfield Deployment

• How Flexfields Work with Oracle Application Cloud Architecture

• Validation Type Options for Value Sets

Overview of Flexfields

A flexfield is a set of placeholder fields associated with business objects and placed on the application pages to contain
additional data.

You can use flexfields to modify the business objects and meet enterprise data management requirements without
changing the data model or performing any database programming. Using flexfields, you can capture different data on
the same database table and modify the application features. For example, airline manufacturers may require specific
attributes for orders that aren't predefined. Using a flexfield for the order business object, they can create and configure
the required attribute.

When you first define your flexfields, you choose how many segments you want to use and what order you want them
to appear in. You also choose how you want to validate each of your segments. The decisions you make affect how you
define your value sets. When your user enters a value, your value sets validate that value. The value sets can be one of
these types:

• List of valid values that aren't stored in any application table.

• Table-validated value sets that use a predefined list of values stored in an application table.

• Format only value sets that use any value as long as it conforms to your specified formatting rules. For

example, the value must not exceed the maximum length you define for your value set.

You can assign a value set to a flexfield segment to define the valid values in that segment. While defining valid values
in a segment, either reuse an existing value set or define a new value set. You can reuse a value set as often as you want
across multiple flexfields or different segments within the same flexfield.

Flexfield Types
Here are the types of flexfields:

• Descriptive flexfields

• Extensible Flexfields

20

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 3
Absence Lookups, Value Sets, and Flexfields

• Key Flexfields

Both extensible and descriptive flexfields provide an expansion space that you can use to configure additional attributes
without additional programming. Descriptive flexfields are stored in additional columns on the same table as that of the
object, whereas extensible flexfields are stored in a separate extension table.

Key flexfields consist of one or more segments, where each segment can have a meaning. You can use key flexfields
to enter multipart values, such as a part number, a job code, or an account code. Users see the flexfields as fields or
attributes on UI pages. To manage the flexfields, use any of these tasks in the Setup and Maintenance work area:

• Manage Descriptive Flexfields: To configure descriptive flexfield segments if you have enabled descriptive

flexfields on a page.

• Manage Extensible Flexfields: To configure extensible flexfield segments if you have enabled extensible

flexfields on a page.

• Manage Key Flexfields: To configure key flexfields, which is a configurable multipart key.

• Manage Value Sets: To create reusable value sets to validate values in flexfield segments.

Note:  You can manage value sets within the Manage Descriptive Flexfields or Manage Extensible
Flexfields tasks.

Related Topics

• How can I access predefined flexfields?

• Overview of Descriptive Flexfields

• Overview of Extensible Flexfields

• Overview of Key Flexfields

• Overview of Value Sets

21

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 3
Absence Lookups, Value Sets, and Flexfields

22

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 4
Formula Creation and Error Handling for Absence
Management

4  Formula Creation and Error Handling for
Absence Management

Overview of Using Formulas

Oracle Fast Formula is a simple way to write formulas using English words and basic mathematical functions. You can
use information from your database in formulas without learning the database structure or a programming language.

Each formula usage summarized in this topic corresponds to one or more formula types, requiring specific formula
inputs and outputs.

The formulas delivered in Oracle HCM Cloud contain English language names, but you can write formulas in other
languages. You can provide formula names and descriptions in any language. Formula text isn't translated, but can
handle non-English user-defined elements, input values, or balances. For example, if you define an element name in
Chinese, the base element name is stored in Chinese. If you create a formula, it can have variable names or string values
in other languages and character sets like Chinese.

Calculate Payrolls
You can write payroll calculations and skip rules for elements to represent earnings and deductions.

You can do these tasks using fast formulas:

• Control the repetition of a payroll flow.

• Control when elements are processed in a payroll run.

• Define a set of people for payroll processing, data entry, or reporting.

• Validate one or more element entry values. Provide a default value for an element entry value, or calculate entry

values based on the user's entries in other entry values.

• Validate entries in user-defined tables.

• Proration formulas control how payroll runs prorate element entries when they encounter an event such as a

mid-period change in an element entry value.

• Associate more than one payroll formula with each element to perform different processing for employee

assignments with different statuses.

• Transformation formulas convert inbound data into a format that HCM Data Loader understands.

• Configure payment method preferences. For example, you can limit the number and types of payment

methods.

Benefits Administration
You can use formulas to structure your benefit plans. Formulas provide a flexible alternative to the delivered business
rules. Use formulas to configure:

• Date calculations, such as enrollment start and end dates, rate or coverage start and end dates, waiting periods

and enrollment periods, or action item due dates

• Calculations of rate and coverage amount, minimum and maximum, or upper and lower limits

23

Oracle Fusion Cloud Human Resources
Implementing Absence Management

• Certification requirements

• Partial month and proration calculations

• Eligibility and participation evaluation

Chapter 4
Formula Creation and Error Handling for Absence
Management

For example, you can write a formula to calculate benefits eligibility for those cases where the provided eligibility
criterion doesn't accommodate your particular requirements.

Note:  For more information, see Benefits Fast Formula Reference Guide (1456985.1) on My Oracle Support at https://
support.oracle.com.

Define Configuration for Compensation
Here's what you can modify using formulas and add flexibility to existing compensation plan configuration:

• Start and end dates for compensation allocations under individual compensation plans

• Person selection, hierarchy determination, column default values, and currency selection for workforce

compensation plans

• The source of items displayed in total compensation statements

Define Formulas to Create Rule Templates for Time and Labor
Use formulas with time repository rule templates to create rules. The formulas contain delivered combinations of
rule parameters and output results. You can use one formula with multiple rule templates by varying the template
configuration.

When creating a rule template, you select a formula name, and then configure the parameter type and display name of
the parameters and variables. You don't have to redo the entire formula statement to determine what details to change
to achieve a particular outcome.

Here's what you can use formulas to apply in Time and Labor:

• Logic for processing or calculating time

• Parameters that enable rules to pass values to the formula for use in calculations

• Output variables that the formula uses to return calculation results to the rules

For example, the Period Maximum Hours Template uses the WFM_PERIOD_MAXIMUM_TIME_ENTRY_RULE formula to
compare reported time category hours to defined maximum hours.

Formulas for Absence Type

Use the Absence Types pages to define absence type rules. However, if you want to define other special rules to suit
your requirement, you can write your own formulas.

Formulas for Absence Types
The following table lists the aspects of an absence type for which you can write a formula and identifies the formula
type for each.

24

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 4
Formula Creation and Error Handling for Absence
Management

Rule

Conversion

Validation

Description

Formula Type to Use

Method to convert the absence duration to
other units of measure. For example, your
workers' work schedules are in work hours, but
you want to display the duration in work days.

Global Absence Type Duration

You can use the formula to convert absence
duration values that are in work days or work
hours only.

Rules in addition to the ones that you can
define on the Absence Types pages to check
the validity of the absence.

Global Absence Entry Validation

Formulas for Accrual Plans

Use the Absence Plan page to apply delivered accrual plan rules in the plan. However, if you want to define other special
rules to suit your requirement, you can write your own formulas.

Formulas for Accrual Plans
The following table lists the aspects of an accrual plan for which you can write a formula and identifies the formula type
for each.

Rule

Description

Formula Type to Use

Enrollment Start

Enrollment End

Date when eligible workers are enrolled in
the plan. If a worker is already enrolled in an
existing accrual plan, you can't use this formula
to change the enrollment start date.

Global Absence Plan Enrollment Start

Date when workers are disenrolled from the
plan. This formula works only if there is an
eligibility profile associated with the plan.

Global Absence Plan Enrollment End

Conversion Formula

Method to override the default absence plan
entry duration.

Global Absence Plan Duration

Example: You might have a requirement to
consider only whole working days in a vacation
absence to update the accrual balance. In such
cases, you define logic in a formula to convert
the absence duration to a value that excludes
partial days.

Anniversary Event

Method to determine the employment
anniversary date on which you want the accrual
plan to restart.

Global Absence Plan Period Anniversary Event
Date

25

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 4
Formula Creation and Error Handling for Absence
Management

Rule

Accrual Event

Description

Formula Type to Use

Global Absence Accrual Event

Method to capture information about events
during a calendar year that affect the accrual
band of a worker.

Example: An organization has a vacation plan in
which enrolled workers accrue a certain number
of days every year based on their grade. When
the grade of a worker changes in the middle of
the calendar year, the organization might want
to prorate their total accrual balance. You can
configure this proration rule using the global
absence accrual event formula to capture the
dates when such changes occur.

This formula can't be attached to the plan
definition at any point. When you create
this formula, the formula name needs to be
the same as the absence plan name. This
automatically links the formula to the plan.

Accrual Vesting

Accrual Proration

A period during which workers accrue time, but
can't use it.

Global Absence Vesting

Method to calculate the time workers accrue if
they enroll in the middle of an accrual period.

Global Absence Proration

Ceiling

The maximum time that a worker can accrue.

Global Absence Ceiling

Ceiling Proration

Carryover

Carryover Proration

Accrual Definition

Accrual Formula

Method to return a multiplying factor to prorate
the defined ceiling limit.

Global Absence Ceiling Proration

The maximum unused time that a worker can
transfer to the next accrual term.

Global Absence Carryover

Method to return a multiplying factor to prorate
the defined carryover amount.

Global Absence Carryover Proration

Method to determine the paid time, eligible
workers accrue over the course of an accrual
term.

Global Absence Accrual

Range of eligibility criteria that identify how
much paid time eligible workers accrue over the
course of an accrual term. The criteria may be
years of service, grades, hours worked, or some
other factor that you can define.

Global Absence Accrual Matrix

Partial Accrual Period

Method to determine the prorated accrual
amount for workers who enroll or disenroll from
a plan during the plan period.

Global Absence Partial Accrual Period Rate

26

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 4
Formula Creation and Error Handling for Absence
Management

Rule

Description

Formula Type to Use

Absence Payment Rate

Method to calculate payment during absence
period.

Global Absence Plan Use Rate

Discretionary Disbursement Rate

Method to calculate payment when paying out
part of the accrual balance.

Global Absence Plan Use Rate

Disbursement Rule

Method to determine the minimum, maximum,
 and increment amounts that the worker is
eligible for to request a cash disbursement.

Global Absence Discretionary Disbursement
Rule

Final Disbursement Rate

Method to calculate payment of accruals when
plan participation ends.

Global Absence Plan Use Rate

Liability Rate

Method to calculate cost of accrual balance to
determine employer liability.

Global Absence Plan Use Rate

When you schedule an absence for a worker using an accrual plan with formulas defined, the absence doesn't appear in
the Absence Records section of the Manage Absences and Entitlements page. Instead, you can view the absence in the
Plan Participation section. To view the absence:

In the Accrual Plans section, click the accrual plan to open the Accrual Plan Balance dialog box.

1.
2. Enter the Balance Calculation Date to view the details of the absence. The details are displayed in the

Summary and Details tabs.

Global Absence Elective Disbursement Evaluation
Formula

The Global Absence Elective Disbursement Evaluation formula is used to validate elective disbursements in an accrual
plan and set payment percentages for the disbursement. The formula can also be used to override the disbursement
amount elected by the worker.

An organization might have a rule such that if an employee’s accrual balance as of the election date is below a certain
minimum threshold limit, then the disbursement should not be allowed. Whereas, if the balance is between two other
threshold values, then the payment percentage should be 75%. In such cases, you can compose a Global Absence
Elective Disbursement Evaluation formula and attach it to the accrual plan.

Configuration Point in HCM Cloud
If you have created this formula, you can attach this formula to the absence plan definition.

Navigation

1.
In the Absence Administration work area, click Absence Plans to open the Absence Plans page.
2. On the Search Results section toolbar, click Create to open the Create Absence Plan dialog box.

27

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 4
Formula Creation and Error Handling for Absence
Management

In the Plan Type field, select Accrual.

3.
4. Click Continue.
5. On the Edit Absence Plan page Accruals tab Plan Limits section, select a value other than None in the

Carryover Rule field.

6. After defining the carryover rule as desired, select Formula in the Carryover Proration field
7. Select the defined formula from the Carryover Proration Formula field.

Contexts
The following contexts are available in this formula type:

Context Name

Data Type

ABSENCE_ENTRY_ID

ABSENCE_TYPE_ID

ACCRUAL_PLAN_ID

DATE_EARNED

EFFECTIVE_DATE

END_DATE

ENTERPRISE_ID

HR_ASSIGNMENT_ID

HR_RELATIONSHIP_ID

HR_TERM_ID

JOB_ID

LEGAL_EMPLOYER_ID

LEGISLATIVE_DATA_GROUP_ID

ORGANIZATION_ID

PAYROLL_ASSIGNMENT_ID

PAYROLL_ID

PAYROLL_RELATIONSHIP_ID

PAYROLL_TERM_ID

PERSON_ID

START_DATE

Number

Number

Number

Date

Date

Date

Number

Number

Number

Number

Number

Number

Number

Number

Number

Number

Number

Number

Number

Date

28

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Input Values

Chapter 4
Formula Creation and Error Handling for Absence
Management

Variable Name

Data Type

Description

IV_ACCRUAL

IV_CARRYOVER

IV_CEILING

IV_ACCRUALPERIODSTARTDATE

IV_ACCRUALPERIODENDDATE

IV_CALEDARSTARTDATE

IV_CALEDARENDDATE

IV_PLANENROLLMENTSTARTDATE

IV_PLANENROLLMENTENDDATE

IV_BAND_CHG_DT1*

Number

Number

Number

Date

Date

Date

Date

Date

Date

Date

Accrual value received from the accrual matrix

Carryover limit received from accrual matrix

Ceiling limit received from the accrual matrix

Start date of accrual period

End date of accrual period

Start date of accrual calendar year

End date of accrual calendar year

Start date of enrollment

End date of enrollment

If the accrual matrix band definition consists of

grades or derived factors length of service or

age, then this input value fetches the date on

which worker has had a change in any of these

factors within the period.

IV_BAND_CHG_BEFVAL1*

Number

Accrual value as per the matrix before IV_

BAND_CHG_DT1

IV_BAND_CHG_AFTVAL1*

Number

Accrual value as per the matrix after IV_BAND_

CHG_DT1

IV_EVENT_DATES

Date_Number

Array of dates returned by the Accrual Event

IV_ACCRUAL_VALUES

Number_Number

IV_ACCRUAL_CEILING

IV_DISB_TYPE

Number

Text

IV_DISB_VALUE

Number

formula.

Array of accrual values fetched from the accrual

matrix as of the dates contained in the accrual

event dates array.

Annual accrual limit from the accrual matrix

The disbursement type for current record which

is being processed. Possible values: CSH /

ORA_ANC_CSH_YREND / ORA_ANC_ELECT_

DISB

The disbursement value for current record

which is being processed

IV_DISB_ELECTED_AMT

Number

Elected amount for the elective disbursement

29

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 4
Formula Creation and Error Handling for Absence
Management

Variable Name

Data Type

Description

IV_DISB_ELECTION_DATE

IV_DISB_PROCD_DATE

IV_DISB_ELECT_PENDING

Date

Date

Text

Return Variables

Election date for the elective disbursement

Exact processed date for the elective

disbursement

If the elective disbursement is marked as

pending or not. "Y" stands for pending, "N"

stands for not pending.

Variable Name

Data Type

Description

paymentPercentage

overrideValue

Number

Number

Payment percentage for the elective

disbursement value

Override value for elective disbursement

Sample Formula
Requirement: If the current balance of an employee is below 8 hours, then 0 hours are to be disbursed.

Solution: A Global Absence Elective Disbursement Evaluation formula such as the one below can be used.

FORMULA NAME: ANC_ELECTDISBEVAL

FORMULA TYPE: Global Absence Elective Disbursement Evaluation

DESCRIPTION: This formula validates the elective disbursement values for an accrual plan.

DEFAULT FOR IV_DISB_TYPE IS 'XX'
DEFAULT FOR IV_DISB_VALUE IS -1
INPUTS ARE IV_DISB_TYPE, IV_DISB_VALUE, IV_ACCRUAL_CEILING

ln_plan_balance = GET_PLAN_BALANCE(‘Vision Accrual Plan’)

paymentPercentage = 100
overrideValue = IV_DISB_VALUE

IF (IV_DISB_TYPE = 'ORA_ANC_ELECT_DISB') THEN
 (
 IF (ln_plan_balance <5) THEN
 (
 paymentPercentage = 0
 overrideValue = 0
 )
 )
RETURN paymentPercentage,overrideValue

30

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 4
Formula Creation and Error Handling for Absence
Management

Formulas for Qualification Plans

Use the Absence Plan page to incorporate qualification plan rules. However, if you want to define other special rules to
suit your requirement, you can write your own formulas.

Formulas for Qualification Plan Rules
The following table lists the aspects of a qualification plan for which you can write a formula and identifies the formula
type for each.

Rule

Start Rule

Description

Formula Type to Use

When the rolling backward plan term starts. A
rolling backward term is a specific time period
that precedes the absence start date.

Global Absence Plan Roll Backward End

Qualification Date Rule

Date when eligible workers enroll in the plan.

Global Absence Plan Enrollment Start Date

Conversion Formula

Method to calculate the absence duration
differently.

Global Absence Plan Duration

Example: You want to consider only whole
working days in a sickness absence in the
entitlement calculation. In such cases, you
define logic in a formula to convert the absence
duration to a value that excludes partial
working days.

Entitlement Definition Type

Determines payment percentages to apply
during the absence period.

Global Absence Entitlement

Entitlement Formula

(Qualification Details section)

A level that determines the payment that
workers receive for a specific number of days
during a long leave of absence based on their
length of service.

Global Absence Band Entitlement

Absence Payment Rate Rule

Method to calculate payment during absence
period.

Global Absence Plan Use Rate

Formulas for Donation Plans

Use the Absence Plan page to apply delivered donation plan rules in the plan. However, if you want to define other
special rules to suit your requirement, you can write your own formulas.

31

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 4
Formula Creation and Error Handling for Absence
Management

Formulas for Donation Plans
The following table lists the aspects of a donation plan for which you can write a formula and identifies the formula type
for each.

Rule

Description

Formula Type to Use

Disbursement Rule

Donation Rule

Method to determine the minimum and
maximum amount of leave balance that a
worker can request as a cash disbursement
from their donation plan. Also, an increment,
 which limits the disbursement amount to
specific values between the minimum and
maximum amount from a donation plan.

Method to determine the minimum and
maximum amount of leave balance that a
worker can donate from their accrual plan. Also,
an increment, which limits the donation amount
to specific values between the minimum and
maximum amount.

Global Absence Discretionary Disbursement
Rule

Global Absence Discretionary Donation Rule

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

Are there any input value defaults?

No

What are the return values?

MIN_HOURS, MAX_HOURS, FREQUENCY

32

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 4
Formula Creation and Error Handling for Absence
Management

Creating a Fast Formula Using the Text Editor to Determine a Manager's
Scheduled Hours

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

Formula Compilation Errors

Compilation errors are displayed in the Fast Formulas page after you compile the formula. The compiler stops the
compilation process when it encounters an error. Error messages display the line number and the type of error.

Common Compilation Errors
Here's some of the common formula compilation errors.

33

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Formula Compilation Error

Description

Chapter 4
Formula Creation and Error Handling for Absence
Management

Syntax Error

The formula text violates the grammatical rules for the formula language. For example, if you use IF1
instead of IF in an IF statement.

Incorrect Statement Order

ALIAS, DEFAULT, or INPUT statements come after other statements.

Misuse of ASSIGNMENT Statement

Occurs when any of these conditions exist:

• An ASSIGNMENT assigns a value to a database item.
• A context is assigned a value externally to a CHANGE_CONTEXTS statement.
• The formula assigns a value to a non-context variable within a CHANGE_CONTEXTS statement.

You can use CHANGE_CONTEXTS statements in a formula.

Misuse of ALIAS Statement

You can use an ALIAS statement only for a database item.

Missing DEFAULT Statement

A database item that specifies a default value must have a DEFAULT statement.

Misuse of DEFAULT Statement

You specify a DEFAULT statement for a variable other than as an input or a database item.

Uninitialized Variable

The compiler detects that a variable is uninitialized when used. The compiler can't do this in all cases.
This error often occurs when the formula includes a database item that requires contexts that the
formula type doesn't support. The formula treats the database item as a local variable. For example,
balance database items require the PAYROLL_REL_ACTION_ID, PAYROLL_ASSIGNMENT_ID and CALC_
BREAKDOWN_ID contexts. Typically, you use these statements in formulas of type Oracle Payroll.

Missing Function Call

The compiler doesn't recognize a function call. The combination of return type, function name, and
parameter types doesn't match any available function.

Incorrect Operator Usage

An instance of a formula operator use doesn't match the permitted uses of that operator.

For example, the + operator has two permitted uses. The operands are both of data type NUMBER, or
both of data type TEXT.

Inconsistent Data Type Usage

The formula uses a formula variable of more than one data type. Or the formula uses a database item
or context with the wrong data type.

For example, Variable A is assigned a NUMBER value at the start of the formula, but is assigned a TEXT
value later in the formula.

EXIT Statement Not Within WHILE Loop

A condition that eventually becomes false or an EXIT call for exiting the loop doesn't exist.

Misuse of Context

The formula uses a variable as a context, or a context as a variable.

For example, a formula assigns a value to AREA1 as an ordinary variable, but later uses AREA1 as a
context in a GET_CONTEXT call.

34

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 4
Formula Creation and Error Handling for Absence
Management

Formula Execution Errors

Fast formula execution errors occur when a problem arises while a formula is running. Typically, data-related issues
cause these errors either in the formula or in the application database.

Formula Execution Errors
Here's some of the formula execution errors.

Formula Execution Error

Description

Uninitialized Variable

When the formula compiler can't fully determine if a variable or context is initialized, it generates a
code to test if the variable is initialized.

When the formula runs, the code displays an error if the variable or context isn't initialized.

Divide by Zero

Raised when a numeric value is divided by zero.

No Data Found

Raised when a non-array type database item unexpectedly fails to return any data. If the database item
can't return data, then it should provide a default value.

You can specify a default value using a DEFAULT statement. An error in formula function code can also
cause this error message.

Too Many Rows

Raised when a non-array type database item unexpectedly returns more than a single row of data. The
cause is an incorrect assumption made about how the data is being accessed.

An error in the formula function code can also cause this error message.

NULL Data Found

Raised when a database item unexpectedly returns a NULL data value. If the database item can return a
NULL value, then it provides a default value.

Note:
Some database items can't return a NULL value. If the database items can return a NULL value, then
you can provide a default value for that database item.

Value Exceeded Allowable Range

Raised for a number of reasons, such as exceeding the maximum allowable length of a string.

Invalid Number

Raised when a formula attempts to convert a nonnumeric string to a number.

User Defined Function Error

Raised from within a formula function. The error message text is provided as part of the formula error
message.

External Function Call Error

A formula function returns an error, but doesn't provide any additional information to the formula
code. The function may have sent error information to the logging destination for the executing code.

35

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 4
Formula Creation and Error Handling for Absence
Management

Formula Execution Error

Description

Function Returned NULL Value

A formula function returns a NULL value.

Too Many Iterations

A single WHILE loop, or a combination of WHILE loops has exceeded the maximum number of
permitted iterations. This error is raised to terminate loops that can never end, which indicates a
programming error within the formula.

Array Data Value Not Set

The formula tries to access an array index that has no data value. This error occurs in the formula code.

Invalid Type Parameter for WSA_EXISTS

You specify an invalid data type in the WSA_EXISTS call.

Incorrect Data Type For Stored Item

When retrieving an item using WSA_GET, the actual data type doesn't match that of the stored item.
This error occurs within the calling formula.

Called Formula Not Found

The called formula isn't found when attempting to call a formula from a formula. This error may occur
due to an issue in the calling formula, or because of installation issues.

Recursive Formula Call

An attempt was made to call a formula from itself. The call could be made directly or indirectly from
another called formula. Calling a formula in a recursive manner isn't permitted.

Input Data Has Different Types in Called
and Calling Formulas

When calling a formula from a formula, the input data type within the called formula doesn't match the
data type specified in the calling formula.

Output Has Different Types In Called and
Calling Formulas

When calling a formula from a formula, the output data type within the called formula doesn't match
the data type specified in the calling formula.

Too Many Formula Calls

When a formula calls another formula in its text, resulting in a hierarchy. The maximum depth of the
hierarchy is 10.

FAQs

When do I run the Compile Formula process?

When you create or update multiple fast formulas simultaneously, run the Compile Formula process on the Submit a
Process or Report page.

36

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 4
Formula Creation and Error Handling for Absence
Management

What's the difference between a formula compilation error and an
execution error?

Compilation errors occur on the Fast Formulas page when you compile the formula. An error message explains the
nature of the error.

Common compilation errors are syntax errors resulting from typing mistakes. You can view error messages on the
dashboard or go to the messages tab directly after the process is run.

Execution errors occur when a problem arises while a formula is running. Typically, data-related issues either in the
formula or in the application database cause these errors.

37

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 4
Formula Creation and Error Handling for Absence
Management

38

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

5  Eligibility Profiles for Absence Plans

How You Configure Eligibility for an Absence Plan

Use an eligibility profile to determine whether a person qualifies for enrollment in an absence plan.

Eligibility profiles that you associate with absence plans can determine the following:

• Who can enroll in absence plans

• Who can schedule absences

Using Eligibility Profiles with Absence Plans
To associate an eligibility profile with an absence plan:

1. Create the eligibility profile using the Eligibility Profiles task in the Absences work area.
2. Associate the eligibility profile with the absence plan using the Absence Plans task.

Example: To enable only female employees to record maternity leave, create an eligibility profile using the Manage
Eligibility Profiles task. Then, when you create a maternity qualification absence plan, select the eligibility profile you
created from the Eligibility section on the Participation tab.

Related Topics

• Create a Maternity Plan

How Eligibility Works With Other Objects

You add eligibility criteria to an eligibility profile, and then associate the profile with an object that restricts eligibility.

39

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

The following figure shows the relationships between eligibility components.

Eligibility Criteria
You can add different types of eligibility criteria to an eligibility profile. For many common criteria, such as gender or
employment status, you can select from a list of predefined criteria values. However, you must create user-defined
criteria and derived factors before you can add them to an eligibility profile.

Eligibility Profile
When you add an eligibility criterion to a profile, you define how to use it to determine eligibility. For example, when you
add gender as a criterion, you must specify a gender value (male or female) and whether to include or exclude persons
who match that value.

Associating the Profile with Objects
This table describes associating eligibility profiles with different kinds of objects and whether you can attach more than
one profile.

Object that Uses an Eligibility Profile

Purpose

Whether You Can Attach More Than One
Profile?

Variable rate or variable coverage profile

Establish the criteria required to qualify for that
rate or coverage

No

Checklist task

Control whether that task appears in an
allocated checklist

No

40

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

Object that Uses an Eligibility Profile

Purpose

Whether You Can Attach More Than One
Profile?

Total compensation statement

Apply additional eligibility criteria after
statement generation population parameters

Benefits object

Establish the eligibility criteria for specific
programs, plans, and options

Compensation object

Establish the eligibility for specific plans and
options

Performance documents

Establish the eligibility for performance
documents

Check-in templates

Establish the eligibility to use check-in
templates for creating check-in documents

Goal plans or goal mass assignments

Establish eligibility for the goal

Absence plan

Determine the workers who are eligible to
record an absence that belongs to that plan

No

Yes

Yes

Yes

Yes

Yes

Yes

Related Topics

• Derived Factors

• Eligibility Profiles

• User-Defined Criteria

Derived Factors

Derived factors define how to calculate certain eligibility criteria that change over time, such as a person's age or
length of service. You add derived factors to eligibility profiles and then associate the profiles with objects that restrict
eligibility.

Derived Factor Types
Using the Manage Derived Factors task, you can create six different types of derived factors:

• Age

• Length of service

• A combination of age and length of service

• Compensation

41

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

• Hours worked

• Full-time equivalent

Determination Rules and Other Settings
For each factor that you create, you specify one or more rules about how eligibility is determined. The following table
provides example settings for two factors.

Factor

Age derived

Example Settings

Select a determination rule to specify the day on which to evaluate the person's calculated age for
eligibility.

Example: If the determination rule is set to the first of the year, then the person's age as of the first of
the year is used to determine eligibility.

Full-time equivalent

Specify the minimum and maximum full-time equivalent percentage and whether to use the primary
assignment or the sum of all assignments when evaluating eligibility.

Example: If 90 to 100 percent is the percentage range for the sum of all assignments, then a person
who works 50 percent full-time on two different assignments is considered eligible.

For derived factors pertaining to time and monetary amounts, you can also set the following rules:

• Unit of measure

• Rounding rule

• Minimum and maximum time or amount

Related Topics

• Examples of Derived Factors

• Eligibility Profiles

Examples of Derived Factors

The scenarios described here illustrate how to define different types of derived factors.

Age
Benefits administrators frequently use age factors to determine:

• Dependent eligibility

• Life insurance rates

Age factors typically define a range of ages, referred to as age bands, and rules for evaluating the person's age. The
following table illustrates a set of age bands that could be used to determine eligibility for life insurance rates that vary
based on age.

42

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

Derived Factor Name

Greater Than or Equal To Age Value

Less Than Age Value

Age Under 25

Age 25 to 34

Age 35 to 44

Age 45 to 54

Age 55 to 64

Age 64 or Older

1

25

35

45

55

65

25

35

45

55

65

75

The determination rule and other settings for each age band can use the same values, as shown in the following table:

Field

Value

Determination Rule

First of calendar year

Age to Use

Person's

Units

Rounding

Year

None

Length of Service
You use the length of service derived factor to determine eligibility based on an employee's length of service. For
example, you can create a derived factor to determine if an employee has completed 10 years of service. You can specify
the start date of the length of service period using any rule in the Period Start Date Rule list:

• Adjusted service date

• Date of hire

• Original hire date

• Seniority date

If you select Seniority Date, you use the Seniority Date list to select the specific configuration rule, such as the grade
seniority date, to determine the date. If you have other special requirements to calculate the length of service, you can
use a formula. You indicate the end of the length of service period by using a determination rule, such as end of month,
first of month, as of event date, or end of pay period. The following table shows an example of a set of length-of-service
bands.

43

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

A derived factor for length of service defines a range of values and rules for calculating an employee's length of service.
The following table shows an example of a set of length-of-service bands. You can use the length-of-service bands to
determine eligibility for compensation objects such as bonuses or severance pay.

Derived Factor Name

Service Less Than 1

Service 1 to 4

Service 5 to 9

Service 10 to 14

Service 15 to 19

Service 20 to 24

Service 25 to 29

Service 30 Plus

Greater Than or Equal To Length of Service
Value

Less Than Length of Service Value

0

1

5

10

15

20

25

30

1

5

10

15

20

25

30

999

The determination rule and other settings for each length-of-service band are the same:

Field

Value

Period Start Date Rule

Date of hire

This sets the beginning of the period being measured.

Determination Rule

End of year

This sets the end of the period being measured.

Age to Use

Person's

Units

Rounding

Year

None

44

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

Compensation
A derived factor for compensation defines a range of values and rules for calculating an employee's compensation
amount. The following table shows an example of a set of compensation bands. You can use the compensation bands
to determine eligibility for compensation objects such as bonuses or stock options.

Derived Factor Name

Greater Than or Equal To Compensation
Value

Less Than Compensation Value

Less than 20000

Salary 20 to 34000

Salary 35 to 49000

Salary 50 to 75000

Salary 75 to 99000

Salary 100 to 200000

Salary 200000 Plus

0

20,000

35,000

50,000

75,000

100,000

200,000

20,000

35,000

50,000

75,000

100,000

200,000

999,999,999

The determination rule and other settings for each compensation band are the same:

Field

Value

Determination Rule

First of year

Unit of Measure

US Dollar

Source

Rounding

Stated compensation

Rounds to nearest hundred

Related Topics

• Eligibility Profiles

• Derived Factors

45

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

Example of Using Range of Scheduled Hours

This example illustrates how to define eligibility criteria based on the number of hours a worker is scheduled to work
within a specified period.

Weekly and Monthly Ranges
You want to limit eligibility for a benefits offering to workers who were scheduled to work either of the following ranges.
Both ranges are as of the end of the previous quarter:

• Between 30 and 40 hours each week

• Between 130 and 160 hours each month

To do this, add two different ranges on the Range of Scheduled Hours subtab under the Employment tab of the create
or edit eligibility profile pages. Set the values for the weekly range as shown in the following table:

Field

Sequence

Minimum Hours

Maximum Hours

Value

1

30

40

Scheduled Enrollment Periods

Weekly

Determination Rule

End of previous quarter

Set the values for the monthly range as shown in this table:

Field

Sequence

Minimum Hours

Maximum Hours

Value

2

130

160

Scheduled Enrollment Periods

Monthly

Determination Rule

End of previous quarter

46

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

Related Topics

• Eligibility Profiles

• Create a Participant Eligibility Profile

Eligibility Profiles

Create eligibility profiles to define criteria that determine whether a person qualifies for objects that you associate the
profile with. You can associate eligibility profiles with objects in a variety of business processes.

The following are key aspects of working with eligibility profiles:

• Planning and prerequisites

• Specifying the profile type, usage, and assignment usage

• Defining eligibility criteria

• Excluding from eligibility

• Assigning sequence numbers

• Adding multiple criteria

• Viewing the criteria hierarchy

Planning and Prerequisites
Before you create an eligibility profile, consider the following:

•

If an eligibility profile uses any of the following to establish eligibility, you must create them before you create
the eligibility profile:

◦ Derived factors
◦ User-defined formulas
◦ User-defined criteria

• Consider whether to combine criteria into one profile or create separate profiles depending on:

◦ Whether the object for which you're creating eligibility accepts only one eligibility profile or more than

one

◦ Performance considerations

• Use names that identify the criteria being defined rather than the object with which the profile is associated,

because eligibility profiles are reusable.

Example: Use Age20-25+NonSmoker rather than Supplemental Life-Minimum Rate.

Specifying Profile Type, Usage, and Assignment Usage
This table describes the basic profile attributes that you specify when you create an eligibility profile:

47

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

Setting

Profile Type

Usage

Description

Use only dependent profiles for Benefits plans or plan types when determining eligibility of
participants' spouses, family members, or other individuals who qualify as dependents.

All other profiles are participant profiles.

Determines the type of objects the participant profile can be associated with, such as benefits offerings
and rates, compensation plans, checklist tasks, goal plans or mass goal assignments, or performance
documents.

Selecting Global makes the profile available to multiple business process usages.

Assignment to Use

Determines the assignment that the eligibility process evaluates for the person

• Select Specific assignment when the usage is Compensation or Performance.

• Select a value that includes benefit relationship when the usage is Benefits. You select this

value to restrict eligibility evaluation to active assignments that are associated with the benefits
relationship of the person on a given date. If you select other values, then you might need to
include eligibility criteria to exclude inactive assignments.

• Select one of the following values for all other usages, such as total compensation statements:

◦ Any assignment - enterprise
◦ Employee assignment only - enterprise
◦ Primary employee assignment only - enterprise

Defining Eligibility Criteria
Here's the list of eligibility criteria that you can use to configure benefit offerings:

Category

Personal

Description

• Gender

• Person Type

• Disabled

• Uses Tobacco

• Service Areas

• Home Location

• Postal Code Ranges

• Leave of Absence

• Termination Reason

• Qualification

• Competency

• Marital Status

• Religion

48

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

Category

Employment

Description

• Assignment Status

• Hourly or Salaried

• Assignment Category

• Grade

•

Job

• Position

• Payroll

• Salary Basis

• Department

• Legal Entities

• Performance Rating

• Quartile in Range

• Work Location

• Range of Scheduled Hours

• People Manager

•

•

Job Function

Job Family

• Hire Date

• Probation Period

• Business Unit

Derived factors

• Age

• Length of Service

• Compensation

• Hours Worked

• Full-Time Equivalent

• Combined Age and Length of Service

• Benefit Groups

• Health Coverage Selected

• Participation in Another Plan

• Formula

• User-Defined Criteria

Other

• Benefit Groups

• Health Coverage Selected

• Participation in Another Plan

• Formula

• User-Defined Criteria

Related coverage

• Covered by Another Plan

49

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

Category

Description

• Covered by Another Plan in Program

• Covered by Another Plan Type in Program

• Covered by Another Program

• Dependent Eligible for Another Plan Type in Program

• Eligible for Another Plan

• Eligible for Another Plan Type in Program

• Enrolled in Another Option in Plan

• Enrolled in Another Plan

• Enrolled in Another Plan in Program

• Enrolled in Another Plan Type in Program

• Enrolled in Another Program

• Other Coverage

• Bargaining Unit

• Labor Union Member

• Union

• Collective Agreement

Labor Relations

Some criteria, such as gender, provide a fixed set of choices. The choices for other criteria, such as person type, are
based on values defined in tables. You can define multiple criteria for a given criteria type.

Excluding from Eligibility
For each eligibility criterion that you add to a profile, you can indicate whether persons who meet the criterion are
considered eligible or are excluded from eligibility. For example, an age factor can include persons between 20 and 25
years old or exclude persons over 65.

If you:

• Exclude certain age bands, then all age bands not explicitly excluded are automatically included.

•

Include certain age bands, then all age bands not explicitly included are automatically excluded.

Assigning Sequence Numbers
You must assign a sequence number to each criterion. The sequence determines the order in which the criterion is
evaluated relative to other criteria of the same type.

Adding Multiple Criteria

If you define multiple values for the same criteria type, such as two postal code ranges, a person must satisfy at least
one of the criteria to be considered eligible. For example, a person who resides in either postal range is eligible.

If you include multiple criteria of different types, such as gender and age, a person must meet at least one criterion
defined for each criteria type.

50

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

Viewing the Criteria Hierarchy
Select the View Hierarchy tab to see a list of all criteria that you have saved for this profile. The list is arranged by criteria
type.

Related Topics

• Examples of Eligibility Profiles

• Derived Factors

• Single or Multiple Eligibility Profiles

• Create a Participant Eligibility Profile

• User-Defined Criteria

Examples of Eligibility Profiles

The following examples show how to use eligibility profiles to determine which workers are eligible for a plan,
compensation object, and checklist task.

In each case, you:

1. Create the eligibility profile using the Manage Eligibility Profiles task, which is available in several work areas,

including the Setup and Maintenance work area and the Plan Configuration work area.

2. Associate the eligibility profile with the relevant object, such as a benefit plan.

Savings Plan Eligibility
A savings plan, such as a 401k plan, is restricted to full-time employees under 65 years of age. Create an eligibility
profile to associate with your plan.

The following table provides the values for the eligibility profile definition.

Field

Profile Usage

Value

Benefits

Profile Type

Participant

Criteria Type

Name

Values

Select Exclude Check Box

Employment

Assignment Category

Full-Time

Derived Factor

Age

Select an age derived factor for the
age band of 65 and older

No

Yes

51

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

Bonus Eligibility
You offer a bonus to all employees who received the highest possible performance rating in all rating categories. Create
an eligibility profile to associate with your Bonus compensation object.

The following table provides the values for the eligibility profile definition.

Field

Value

Profile Usage

Compensation, or Global

Profile Type

Participant

Assignment to Use

Specific Assignment

The following table provides the values for the eligibility criteria for each rating category.

Criteria Type

Name

Values

Select Exclude Check Box

Employment

Performance Rating

Select the performance template
and rating name, and then select
the highest rating value

No

Checklist Task Eligibility
A new hire checklist contains tasks that don't apply to employees who work in India. Create an eligibility profile to
associate with each checklist task that doesn't apply to workers in India.

The following table provides the values for the eligibility profile definition.

Field

Profile Usage

Value

Checklist

Profile Type

Participant

The following table provides the values for the eligibility criteria.

Criteria Type

Name

Employment

Work Location

Values

India

Select Exclude Check Box

Yes

52

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

Related Topics

• Eligibility Profiles

• Derived Factors

• How can I restrict benefits enrollment opportunities based on provider location?

• How to Configure Grandfathered Benefits

Single or Multiple Eligibility Profiles

You can define multiple criteria in an eligibility profile or create separate profiles for individual criterion.

To determine the best approach, consider the following:

• Does the object for which you are defining eligibility allow multiple eligibility profiles?

• What is the best approach in terms of efficiency and performance?

• Are your criteria both inclusive and exclusive?

Allowable Number of Eligibility Profiles
If an object permits only one eligibility profile, you must include all criteria in a single profile.

The following table shows which objects permit only one profile and which permit more.

Only One Profile

One or More Profiles

• Checklist tasks

• Benefits offerings

• Variable rate profiles

•

Individual and workforce compensation plans

• Variable coverage profiles

• Performance documents

• Total compensation statements

• Check-in templates

• Absence types

• Goal plans or mass goal assignments

• Absence plans

Efficiency and Performance in the Benefits Hierarchy
For optimum performance and efficiency, attach profiles at the highest possible level in the benefits object hierarchy
and avoid duplicating criteria at lower levels. For example, to be eligible for a plan type, a person must satisfy eligibility
profiles defined at the program and plan type in program levels.

The following objects inherit the eligibility criteria associated with the program:

• Plan types in program

• Plans in program

• Plans

• Options in plans that are in programs

53

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

However, it's sometimes more efficient to create more than one profile and attach the profiles at various levels in the
hierarchy. The following table illustrates applying successively restrictive exclusion criteria at different levels in the
hierarchy:

Level

Program

Eligibility Profile Criteria

Exclude employees who do not have an active assignment.

Plan type in program

Exclude employees who do not have a full-time assignment.

Plan

Exclude employees whose primary address is not within a defined service area.

Using Both Inclusive and Exclusive Criteria
Eligibility criteria can be used to include or exclude persons from eligibility. Sequencing of criteria is more complicated
when you mix included and excluded criteria in the same profile. For ease of implementation, keep excluded criteria in a
separate eligibility profile.

Related Topics

• How Eligibility Works With Other Objects

• What happens if I include multiple criteria in an eligibility profile?

• Best Practices for Setting Up Eligibility in a Benefits Hierarchy

Create a Participant Eligibility Profile

This example demonstrates how to create a participant eligibility profile used to determine eligibility for variable life
insurance rates. Use the Plan Configuration work area to complete these tasks.

The following table summarizes key decisions for this scenario.

Decisions to Consider

In this Example

What is the profile type?

Participant

What type of object is associated with this
profile?

Variable rate for benefits offering

What types of eligibility criteria are defined
in this profile?

Age derived factor (must have been previously defined)

Uses Tobacco criteria

Should persons meeting these criteria be
included or excluded from eligibility?

Included

54

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

Decisions to Consider

In this Example

The following figure shows the tasks to complete in this example:

In this example, you create one eligibility profile that defines the requirements for a single variable rate.

• Typically, you create a set of eligibility profiles, one for each variable rate.

• Create a separate profile for each additional rate by repeating the steps in this example, varying the age and

tobacco use criteria.

Prerequisites

1. Create an age derived factor for ages less than 30.

Creating the Eligibility Profile
Use default values for fields unless the steps specify other values.

In the Tasks panel drawer, click Manage Eligibility Profiles to open the Manage Eligibility Profiles page.

1.
2. On the Create menu, select Create Participant Profile.
3.

In the Eligibility Profile Definition section, complete the fields as shown in this table.

Field

Name

Value

Age Under 30+ Non-Smoking

Profile Usage

Benefits

Status

Active

Assignment to Use

Any assignment - benefit relationship

55

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

Adding the Derived Factor for Age
Use default values for fields unless the steps specify other values.

In the Eligibility Criteria section, select the Derived Factors tab.

1.
2. On the Age tab, click Create.
3. Complete the fields as shown in this table.

Field

Sequence

Age

Exclude

Value

1

Select the derived factor that you previously defined for ages under 30

Make sure that it's not selected

Adding the Criteria for Tobacco Use
Use default values for fields unless the steps specify other values.

1. Select the Personal tab.
2. On the Uses Tobacco tab, click Create.
3. Complete the fields as shown in this table.

Field

Sequence

Tobacco Use

Value

1

None

Exclude

Make sure that it's not selected

4. Click Save and Close.

Associating the Eligibility Profile with a Variable Rate Profile
Use default values for fields unless the steps specify other values.

In the Tasks panel drawer, click Manage Benefits Rates to open the Manage Benefits Rates page.

1.
2. Select the Variable Rates tab.
3. Click Create.
4.
5. Complete other fields as appropriate for the rate.
6. Click Save and Close.

In the Eligibility Profile field, select the eligibility profile you just created.

56

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

Related Topics

• Examples of Eligibility Profiles

• Derived Factors

• Create a Benefit Variable Rate

FAQs

What happens if I include multiple criteria in an eligibility profile?

If you define multiple values for the same criteria type, such as two postal code ranges, a person must satisfy at least
one of the criteria to be considered eligible. For example, a person who resides in either postal range is eligible.

If you include multiple criteria of different types, such as gender and age, a person must meet at least one criterion
defined for each criteria type.

57

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 5
Eligibility Profiles for Absence Plans

58

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 6
Rate Definitions for Absence Payments

6  Rate Definitions for Absence Payments

Rate Definitions for Absence Payments

Use a rate definition to determine the rate of a single unit of absence for payment during an absence period. However,
you calculate and resolve the rates only in Oracle Fusion Global Payroll or a third-party payroll application.

This topic covers the following aspects:

• Using rate definitions with absence plans

• Types of absence payments that support rate definitions

Using Rate Definitions with Absence Plans
To associate a rate definition with an absence plan:

1. Create the rate definition using the Manage Rate Definitions task in the Absences work area.
2. Optionally, associate the rate definition with the absence plan on the Entries and Balances tab of the Manage

Absence Plans task.

Example: If you want to calculate payments of each time unit when you disburse an accrual balance, you create a rate
definition using the Manage Rate Definitions task. Then, when you create an absence plan, you select the rate definition
that you created from the Disbursement Rate Rule list on the Entries and Balances tab.

The rate fields are optional in Absences even when you select the Transfer absence payment information for payroll
processing check box. You can define the rates on the payroll side.

Types of Absence Payments that Support Rate Definitions
The following table describes the types of absence payments for which you can associate a rate definition:

Rates

Description

Absence Payment Rate Rule

Calculates payment during an accrual and qualification absence period.

For a qualification absence plan, you can select this rate definition to calculate payment for a
qualification absence period. When you create a qualification plan, remember that you define
qualification bands to specify the percentage of payment during an absence period.

Example: You want to award the worker 75 percent pay up to the first 90 days of the absence. You use
a rate definition to define the calculation method to translate that percentage into an actual payment
value.

Final Balance Payment Rate Rule

Calculates payment of accruals when plan participation ends.

Example: If the worker is terminated or loses eligibility for the absence plan, you might want to use a
rate definition to calculate the final accrual balance. Create a rate definition that considers the worker's
salary details and calculates the payment value for each unit of accrued time.

Partial Disbursement Rate Rule

Calculates payment when paying out part of an accrual balance.

59

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 6
Rate Definitions for Absence Payments

Rates

Description

Example: If the worker is terminated or loses eligibility for the absence plan, you might want to disburse
the remainder of the accrual balance as cash. Create a rate definition that considers the worker's salary
details and calculates the payment value for each unit of accrued time.

Liability Booking Rate Rule

Calculates the cost of a worker's accrual balance to determine employer liability.

Example: If the is terminated or loses eligibility for the absence plan, you might want to determine
employer liability for worker time accruals for the rest of the accrual term.

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

60

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 6
Rate Definitions for Absence Payments

Categories
To create a new rate, select a category from this table.

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

61

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 6
Rate Definitions for Absence Payments

Category

Grade Rate

Formula

What it Does

Retrieves values based on an employee's grade details.

Retrieves values from a rate definition formula. The Generate HCM Rates process supports the
calculation of most formula-based rates. However, rates that include complex payroll formula contexts
or use balances calculated within the payroll run, are calculated by the payroll run.

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

62

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 6
Rate Definitions for Absence Payments

Field

Element Name

Category

Element

Derived Rate

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

Description

For the Element category, the field is enabled
only when you select the storage type.

If you select the Element category to define a
rate, you must select an element name. This is
required if you're configuring a primary rate.
This is a rate that retrieves a value from a single
element, such as salary.

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

63

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 6
Rate Definitions for Absence Payments

Field

Category

Description

Value by Criteria Name

Value by Criteria

Rate definitions with this option selected are
included when the Generate HCM Rates batch
process is run. Use this feature to report on
primary rates and not derived rates. HCM
extracts use this report to send data to third
parties.

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

64

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 6
Rate Definitions for Absence Payments

Factor Rules
You can apply a factor or multiplier to a calculated rate, or to an individual rate contributor. To apply a factor rule, do
these steps.

• Select Value as the factor rule.

•

In the Factor field, enter the number by which you want to multiply the rate.

• Add the contributor.

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

65

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 6
Rate Definitions for Absence Payments

For example, you can use the HCM Rates Default Value formula type to define the number of workdays in a year for your
organization.

workday = 250
periodicity = YEAR
return workday, periodicity, currency

In addition, you can use a value by criteria definition as the default type. Here, the process uses the value for the first
record created and carries that value forward in subsequent records, unless it's manually overridden. The rate engine
reevaluates the rate that the value by criteria method creates for each subsequent record. So, this rate could change. For
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

66

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 6
Rate Definitions for Absence Payments

What You Need To Consider

For This Example

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
3. Enter these values.

In the Search Results section, click Create.

Field

Category

What You Select

Derived Rate

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

1.
2.

In the Rate Contributors section, click Create.
In the Contributor Type field, select Balance and click OK.

67

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 6
Rate Definitions for Absence Payments

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
6.
7. On the Create Rate Contributor page, enter these values.

In the Rate Contributor section, click Create.
In the Contributor Type field, select Balance and click OK.

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

68

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 7
Elements for Absence Management

7  Elements for Absence Management

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

69

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 7
Elements for Absence Management

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

70

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 7
Elements for Absence Management

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

If your enterprise calculates cost distributions, specify costing for all the element eligibility records. For example, for an
accrual element, you do these steps

1. Define element eligibility records for the accrual, accrual results, accrual retroactive, and accrual retroactive

results elements.

2. Specify costing for the accrual results and retroactive results elements.

The costing process costs the change in the liability balance since the last payroll period, debits the expense account
and credits the liability account.

71

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 7
Elements for Absence Management

Related Topics

• Define Elements, Balances, and Formulas

• How Payroll Elements Hold Information for Multiple Features

• Element Costing Options

•

Import Absence Entries to Payroll

• Rates Used to Calculate Absences in Payroll

Define Payroll Elements for an Absence Accrual Plan

This example shows how to define an absence element for a vacation accrual absence plan.

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

72

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 7
Elements for Absence Management

Decisions to Consider

In This Example

Which rate should the final disbursement
payment use?

Final Disbursement Rate

Does your absence plan enable payment
of partial accrual balances?

Yes

Which rate should the partial
disbursement payment use?

Partial Disbursement Rate

Reduce regular earnings by absence payment

How do you want to calculate deductions
for paid absences for employees not
requiring a time card?

• Reduce regular earnings by the

amount of the absence payment
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

fields.

73

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 7
Elements for Absence Management

5.

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

74

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 7
Elements for Absence Management

Field

Value

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

75

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 7
Elements for Absence Management

76

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 8
Effective Dates in Absence Management

8  Effective Dates in Absence Management

Date Effectivity

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

3

2

1

18 January, 2022

C. Woods

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

77

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 8
Effective Dates in Absence Management

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

Date-Enabled Objects
Some objects, such as work relationships, are date-enabled rather than date-effective. They have start and end dates
that define when they're available, but they have no history of changes. New attribute values overwrite existing attribute
values.

Related Topics

• Examples of Updating Date-Effective Objects

• Examples of Correcting Date-Effective Objects

• How You Make Multiple Updates to Date-Effective Objects in One Day

• How You Delete Physical Records from Date-Effective Objects

Examples of Correcting Date-Effective Objects

You can correct most attributes of date-effective objects, regardless of whether they occur in current, past, or future
physical records.

If you correct the effective start date of an object's first physical record, then the revised date must be before the current
effective start date. For the second and subsequent records, the revised date must be between the record's current
effective start and end dates.

78

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 8
Effective Dates in Absence Management

Correcting a Current Error
On 11 December, 2022 you create a location definition but enter the wrong phone. On 21 December, 2022, you search for
the definition and select the Correct action. Before correction, the object history is as shown in this table.

Physical Record

Effective Start Date

Effective End Date

Location Phone

1

11 December, 2022

650.555.0175

After correction, the object history is as shown in this table.

Physical Record

Effective Start Date

Effective End Date

Location Phone

1

11 December, 2022

650.555.0176

Because you corrected the object, no change history exists.

Correcting a Past Error
A worker's assignment history is as shown in this table.

Physical Record

Effective Start Date

Effective End Date

Job

Working at Home

4

3

2

1

20 October, 2022

Line Manager

18 August, 2022

19 October, 2022

Senior Administrator

10 May, 2022

17 August, 2022

Senior Administrator

25 July, 2021

9 May, 2022

Administrator

No

No

Yes

Yes

You learn that the worker's job was actually Project Leader from 10 May to 19 October, 2022. As this period spans
physical records 2 and 3, you must correct both.

To retrieve physical record 2, you set the effective as-of date in the person search to any date between 10 May and 17
August, 2022. You select the assignment from the search results and make the correction.

You then retrieve physical record 3 and make the same correction.

79

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 8
Effective Dates in Absence Management

Examples of Updating Date-Effective Objects

When you update a date-effective object, you insert a physical record in the object's history. Typically, the inserted
record follows the current record and the effective start date is today. However, you can also enter future-dated changes
and update past records.

Entering Future-Dated Changes
The grade EC3 exists from 17 June, 2019. Its ceiling step changes from 1 January, 2023. On 30 November, 2022, you
change the grade's ceiling step and enter an effective start date of 1 January, 2023. This change creates a physical
record in the grade definition, as shown in this table.

Physical Record

Effective Start Date

Effective End Date

Ceiling Step

2

1

1 January, 2023

17 June, 2019

31 December, 2022

4

3

From 1 January, 2023 physical record 2 is in effect. Until then, physical record 1 is in effect.

Applying Historical Updates to Later Records
Jennifer Watts has one assignment, as shown in this table.

Physical Record

Effective Start Date

Effective End Date

Grade

Location

2

1

18 September, 2022

10 April, 2022

17 September, 2022

A1

A1

Area Office

HQ

You promote Jennifer to grade A2 from 1 July, 2022. You update her assignment with an effective start date of 1 July,
2022 and enter grade A2. This update:

•

Inserts a physical record between existing records 1 and 2

• Sets the effective end dates of physical record 1 to 30 June, 2022 and of the inserted record to 17 September,

2022

You also correct existing physical record 2 to change the grade from A1 to A2.

Jennifer's assignment history is now as shown in this table.

80

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 8
Effective Dates in Absence Management

Physical Record

Effective Start Date

Effective End Date

Grade

Location

3

2

1

18 September, 2022

1 July, 2022

17 September, 2022

10 April, 2022

30 June, 2022

A2

A2

A1

Area Office

HQ

HQ

FAQs

What's the effective as-of date?

A date value that filters search results. For any date-effective object that matches the other search criteria, the search
results include the physical record for the specified effective as-of date. The effective as-of date is one of the search
criteria.

What's the difference between updating and correcting a date-
effective object?

When you update an object, you insert a physical record in the object's history. Typically, the inserted record follows the
current physical record, and the effective start date is today's date. However, you can edit the object history or create a
future-dated change by

When you correct a date-effective object, you edit the information in an existing physical record. You don't create a
physical record.

What happens when I end date an object?

The date that you enter becomes the final effective end date for the object. If physical records exist for the object
beyond the effective end date, either they're deleted automatically or you delete them.

The object's history remains available. For example, the object may appear in search results if the search criteria include
an effective as-of date that's within the object's effective dates.

81

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 8
Effective Dates in Absence Management

82

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

9  Accrual Absence Plans

Types of Absence Plans

Create the following types of plans using the Absence Plans task in the Absences work area:

• Accrual

• Qualification

• No Entitlement

• Agreement

• Compensatory

• Donation

Accrual
Use this type to create absence plans that enable workers to accrue time for taking paid leave, such as a vacation plan.
Configure rules that determine various aspects of leave time, such as:

• Length and type of the accrual term in which workers accrue time

• Maximum time that workers can accrue in a term

• Maximum time that workers can carry forward to the next term

Qualification
Use this type to create an absence plan where workers qualify for the plan and receive payments during the absence
period. For example, use qualification plans for defining absence rules related to events, such as long term illness or
maternity. Configure rules to determine the payment percentages that apply for specific periods during the absence, for
specific workers.

No Entitlement
Create absence plans of this type to track unpaid absences without maintaining an accrual balance or providing leave
entitlements, such as periodic accruals. Similar to an accrual plan, you can define the length and type of the plan term
and determine when eligible workers can enroll in the plan. You can also use plans of this type in combination with a
qualification plan. For example, use a no-entitlement plan if a worker isn't eligible for a standard maternity absence
qualification plan.

Agreement
Create absence plans of this type in accordance with statutory rules for use under an agreement. For example, create a
shared parental leave agreement for a worker and qualified parental partner to allocate paid or unpaid time off among
parenting partners.

83

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Compensatory
Create absence plans of this type to track earned compensatory time that can be used for time off. Compensatory time
is offered as compensation for working outside of regular work schedules. Instead of paying overtime, an employer can
create a policy to give paid time off.

Donation
Create absence plans of this type to track donated time that a worker receives. Workers can donate their accrual plan
balance to a coworker who needs additional time off and is eligible to receive the donated time.

Related Topics

• Create a Maternity Plan

• Create a Vacation Accrual Plan

Options to Define Accrual Plans

Configure the following rules when you create an absence accrual plan in accordance with the leave policy of your
enterprise:

• Plan term

• Plan eligibility

• Enrollment and termination

• Transfer and rollover

• Prior balance reinstatement

• Vesting period

• Plan limits

• Balance Updates

• Payments

• Disbursement

• Donation

Plan Term
An accrual term is a period of time during which workers accrue time. You must specify the type of accrual term to use
for the plan. For example, you can define one of these term types:

• An accrual term of one calendar year that restarts on January 1

• An accrual term that starts on the worker's annual hire date and restarts on every anniversary

Plan Eligibility
Associate an eligibility profile with the accrual plan to determine the set of workers who can enroll in that plan.

84

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Enrollment and Termination
Decide when to enroll workers in the accrual plan. Indicate how to handle negative and positive balances where only
plan enrollment ends, or both plan enrollment and employment ends.

Transfer, Rollover, and Carryover
Define the limits for transfer of some or all of the accrual balance to a new plan when the existing plan is terminated
due to loss of eligibility. The Transfer Rules section is enabled only when you select Transfer positive balance in the
Balance Disposition section.

Additionally, for year end processing, you can define:

• Rollover limits so that employees can transfer remaining balance to a new plan. Select Unlimited if you don't

want to define a limit for rollover.

• Carryover limits to determine the maximum unused leave time that employees can take over to the next term

for the same plan.

If the unused absence balance at the end of the term is above the defined rollover and carryover limit, you can choose
to pay out the remaining balance. If you don't select the Disburse remaining balance check box, the unused accrual
balance expires.

Note:  During the year end processing, the application first processes the rollover, and only then processes the
carryover with the leftover balance.

Prior Balance Reinstatement
Configure accrual plans so that when a worker is terminated or loses plan eligibility, the remaining balance can be
optionally held for reinstatement upon rehire or return to plan eligibility.

Absence plan setup options allow you to define the balance amount eligible for reinstatement along with the time frame
for which the withheld balance can be reinstated. You can configure this option in the Re-enrollment Rules section. You
can find this section in the Plan Participation tab when you create or edit an absence plan.

If you select Allow Prior Balance Reinstatement, a new row in accruals called "Plan Balance close transaction" is
created that deducts the remaining balance on the last day of the employee. This is the transaction that will act as a
reference to calculate the reinstated balance if the employee is re-hired within the time frame limit configured in the
plan setup.

However, if you select Allow Prior Balance Reinstatement, and leave the Balance Reinstatement Limit and Time
Frame Limit fields blank, the entire closing balance can be reinstated any time.

Vesting Period
Define if you want newly enrolled workers to accrue time, but not use it until after a specific amount of time.

Plan Limits
Define rules for the maximum leave time that workers can accrue. For incremental plans, Absence Management
applies the limit to each accrual period. When there are accrual transactions such as adjustments, balance transfers,
and disbursements, which impact the ceiling or carryover value, then the periodic accrual balance calculation takes
precedence and readjusts the balance accordingly.

85

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Balance Updates
You can enable the following types of adjustments that HR specialists can make during maintenance of absence records
and entitlements:

• Balance transfer across plans

• Other adjustments

• Elective disbursements

Payments
Decide how you want to calculate payment of accrual balances for the following scenarios:

• When workers must be paid a different rate during the absence period

• When a part of the accrual balance must be disbursed to workers as cash

• When the cost of accrual balance must be calculated to determine employer liability

• When the accrual balance must be paid to workers when their plan participation ends

Disbursement
Determine whether workers are eligible for cash disbursement requests. Decide who can initiate the disbursement.
Additionally, define disbursement rules and the number of hours that can be disbursed.

Donation
Define whether workers are eligible to donate accrual balances to a coworker. Decide who can initiate the donation.
Additionally, define donation rules and the number of hours that can be donated.

Related Topics

• Create a Vacation Accrual Plan

Options to Define an Accrual Term

When you create an accrual plan, you must select one of the following term types to define an accrual term during
which workers accrue leave:

• Calendar year

• Anniversary year

Calendar Year
The accrual term starts on the month, day, and year that you select. The term restarts next year on the same day. For
example, if you select January 1, 2015, the accrual term starts on that day and restarts on January 1, 2016.

86

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Anniversary Year
The accrual term starts on the hire date and restarts on each anniversary. For example, if the enrolled worker's hire date
is May 1, 2015, the accrual term starts on this date and restarts on May 1, 2016.

Entering a continuous service date when enrolling in the accrual plan doesn't affect the start date. The continuous
service date affects the length-of-service calculations while processing a waiting period, vesting period, or plan limits
defined in an accrual band matrix. However, it doesn't affect the accrual term.

Related Topics

• Create a Vacation Accrual Plan

Options to Configure Accrual Enrollment and
Termination

Workers are enrolled into accrual plans as a result of employment and eligibility. They're disenrolled from accrual plans
when they're terminated or their plan eligibility ends.

Define when you want to enroll or disenroll a worker in the Participation tab of the Absence Plan setup page. Configure
the plan to do the following:

• Automatically enroll workers when they're hired or when a transfer event occurs.

• Use a formula if you want to consider other aspects or rules to determine when to enroll workers.

Define a waiting period if you want newly enrolled workers to start accruing time under that plan only after a specific
amount of time elapses after the date of enrollment.

Configure the plan to automatically disenroll workers as a result of employment termination or loss of eligibility to a
plan. On plan termination, define how to:

• Disburse the amount for payment if the worker has a positive absence balance.

• Recover the amount from the last pay if the worker has a negative absence balance.

For example, if a worker is terminated from employment on October 12, 2017, the following updates can occur to reflect
the termination.

•

•

•

If an absence starts on or after October 12, it's withdrawn.

If there is an absence spanning the termination date of October 12, the end date is automatically calculated
as the termination date for the absence. For example, if the worker schedules an absence from October 9 to
October 17, since the termination date is October 12, the end date of the absence is updated as October 12.

If an absence is open-ended, the end date of the absence is October 12 since the termination date is calculated
as the last day of the absence.

• Plan use is recalculated for all updated absences.

• All active accrual enrollments are updated to reflect an end date of October 12.

• Final disbursements are transmitted to payroll, if final disbursement is configured.

87

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

How You Configure Eligibility for Absence Plans

An eligibility profile in Absence Management defines criteria used to determine whether a person qualifies for an
accrual or qualification absence plan. Define eligibility profiles and then associate it with a plan to determine the set of
workers who can enroll in that plan.

1. Create the eligibility profile using the Manage Eligibility Profiles task in the Absences work area.
2. Associate the eligibility profile with the absence plan using the Absence Plans task.

If you want all workers to be eligible for the absence plan, then don't add an eligibility profile. If a plan doesn't have
an eligibility profile associated with it, then it doesn't mean that workers are enrolled automatically into the plan. New
hires may be enrolled automatically, if that's the option set in the plan definition. Existing workers have to be enrolled
manually.

Carryover Limit Rules

You can transfer your unused leave time from one plan term to the next using the carryover limit configuration options
on the absence plan setup page. The carryover options are available in the Year End Processing section of the Accruals
tab.

You can use these options in the Carryover Limit Rule field:

Carryover Option

Description

No Carryover

No Limit

Flat Amount

No balance (positive or negative) is carried over from the end of the previous plan term to the new
term.

All the balance from the end of the previous plan term (positive or negative) is carried over to the next
plan term without any limit.

Configure the carryover limit in the dedicated field under the Carryover Limit Rule field. The balance
amount carried over from the previous plan term to the next one can’t exceed this limit.

Negative balance is carried over even if the limit is 0.

Include in Matrix

Configure the carryover limit in the Accrual Matrix section.

Negative balance is carried over even if the limit is 0.

Formula

The limit is set by the Global Absence Carryover formula selected in the plan setup.

This formula doesn’t return the carryover value. It only determines the upper limit of the balance from
the end of the previous plan term, carried over to the next plan term.

88

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Carryover Expiration Rules

Set carryover balance to expire after a certain period. To do this, enable the Carryovers expire after specific time
check box available in the Accruals tab of the absence plan setup page. After you enable it, the Expiration Period field
will be available to you where you can select the number of days, weeks, months, or years after which the carryover
expires.

Note:  If you select the Flat Amount, Include in Matrix, or Formula option in the Carryover Limit Rule field instead of
No Limit, you can’t set an expiration period longer than 1 year.

If you make any changes to the plan, you need to run the Calculate Accruals and Balances absence process to calculate
the updated carryover. Select the last day of the previous plan term as the effective date. This will recalculate the
balance from the end of the plan term and change the Carryover value from the first day of the next plan term, based on
the plan changes.

Options to Define Frequency of Accrual Periods

Configure accrual periods to award leave time to workers throughout an accrual term in equal installments.

Determine the frequency of accrual periods by selecting one of the following Balance Frequency Source values on the
Accruals tab in the Create Absence Plan page:

• Person primary frequency

• Repeating time period

It there is a change in payroll relationship, the repeating period is automatically updated when running accruals. For
example, when employee payroll changes from weekly to monthly.

Person Primary Frequency
Select Person Primary Frequency to award time at the start of each payroll period. For example, if the worker enrolled
in the plan receives weekly payroll, the leave time accrues once a week.

Repeating Time Periods
The worker accrues time at the start of each instance in a repeating time period. For example, you created a biweekly
repeating period for an annual accrual term. The worker accrues time every two weeks during the term.

You create the repeating time period using the Manage Repeating Time Periods task in the Absences work area. Then,
associate the repeating time period with the accrual absence plan on the Create Absence Plan page.

Note:  When you create a repeating time period, ensure that the period has a duration of at least 7 days. For example,
if you select a period type of Daily and a period length of More than one day, you need to select a value that's
greater than or equal to 7.

89

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Related Topics

• Create a Vacation Accrual Plan

• Repeating Time Periods

Plan Limits for Accrual Plans

You can configure the following plan limits for accrual plans:

Plan Limit

Description

Annual Accrual Limit Rule

Determines the maximum amount of leave time that workers can accrue within a plan year.

Ceiling Rule

Determines the maximum leave time that workers can accrue.

Use an accrual band matrix to build criteria using various factors, such as length of service, to determine workers who
qualify for specific plan limits. Alternatively, you can use a formula to determine each plan limit.

When accruals and balances are calculated, an annual accrual limit is evaluated. If the current period accrual results in
the accrual balance exceeding the limit, the accrual amount for that period is reduced. If a ceiling is also configured, it
can further impact the accrual amount.

Examples of Accrual Bands

Use accrual bands to vary accrual benefits to workers depending on employment criteria, such as length of service,
grade, or other factors.

You can define various types of accrual bands in the Accrual Matrix section on the Absence Plan setup page. The
examples show accrual bands based on the following factors:

• Length of service

• Location and length of service

• Grade

Creating Bands Based on Length of Service
Scenario: You want to create two accrual bands based on worker length of service, as shown in the following table.

Band Sequence

Length of Service

Accrual Rate

Maximum Carryover

Ceiling

1

Less than five years

15

15

45

90

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Band Sequence

Length of Service

Accrual Rate

Maximum Carryover

Ceiling

2

Greater than or equal to
five years

20

15

60

To create the bands:

1. Create the following length of service derived factors using the Manage Derived Factors task in the Absence

Administration work area.

◦ Length of service less than 5 years
◦ Length of service greater than or equal to 5 years

2. Use the expression builder to create bands using the derived factors that you created:

Band Sequence

Expression

1

2

[LengthOfService.LessThan5]

[LengthOfService.GreaterThan5]

Creating Bands Based on Location and Length of Service
Scenario: You want to create accrual bands of varying length of service for workers who belong to specific geographic
locations, as shown in the following table.

Band Sequence

Location

Length of Service

Accrual Rate

Maximum Carryover

Ceiling

1

2

3

4

Paris

Less than five years

15

Greater than or equal
to five years

20

Tokyo

Less than three years

10

Greater than or equal
to three years

15

To create the bands:

15

15

10

15

45

60

30

45

1. Create the following length of service derived factors for the specific geographic locations using the Manage

Derived Factors task in the Absences work area.

◦ Length of service less than 5 years
◦ Length of service greater than or equal to 5 years
◦ Length of service less than 3 years

91

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

◦ Length of service greater than or equal to 3 years

2. Use the expression builder to create bands using the derived factors that you created:

Band Sequence

Expression

1

2

3

4

[Person.Location] = "Paris" AND [LengthOfService.LessThan5]

The person.location attribute is on the Entities tab in the Expression Builder dialog box. The
LengthOfService derived factors are available from the Derived tab.

[Person.Location] = "Paris" AND [LengthOfService.GreaterThan5]

[Person.Location] = "Tokyo" AND [LengthOfService.LessThan3]

[Person.Location] = "Tokyo" AND [LengthOfService.GreaterThan3]

Creating Date-Effective Accrual Bands Based on Grade
Scenario: Your enterprise wants to change its leave policies every year in accordance with government regulations, as
shown in the following table.

Band Sequence

Effective Start Date

Grade Range

Accrual Rate

Maximum Carryover

Ceiling

1

2

3

4

April 1, 2014

A1 - A3

A1 - A6

April 1, 2015

A1 - A3

A1 - A6

15

20

20

25

15

15

20

15

45

60

30

40

Set the session effective date to April 1, 2014 and create band 1 and band 2 using the following expressions:

Band Sequence

Expression

1

2

[Person.Grade] >= "A1" AND [Person.Grade] <= "A3"

The person.grade attribute is on the Entities tab in the Expression Builder dialog box.

[Person.Grade] >= "A4" AND [Person.Grade] <= "A6"

Save your work and set the session effective date to April 1, 2015. Then, create band 3 and band 4 using the same
expressions that you used for band 1 and band 2:

92

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Band Sequence

Expression

1

2

[Person.Grade] >= "A1" AND [Person.Grade] <= "A3"

[Person.Grade] >= "A4" AND [Person.Grade] <= "A6"

Related Topics

• Create a Vacation Accrual Plan

How You Configure a Plan for Discretionary Cash
Disbursement

Workers can initiate a cash disbursement request for their accrual or donation plan balance. Administrators and
managers also have the option to initiate a cash disbursement request on behalf of a worker.

To enable self-service cash disbursement for a worker and manager, complete these steps:

1. On the Absence Plans page for an accrual or donation plan, go to the Entries and Balances tab, Discretionary

Disbursements section.

2. Select Enable for administrator. The Enable for manager and Enable for worker fields are available for you to

select.

3. Configure the disbursement rules and define limits for the number of hours to disburse. For the disbursement

rule, you can select either Formula or Flat Amount. When you select Flat Amount, you may also specify the
following quantities. When you select Formula, you must specify a formula that returns values for these same
quantities:

◦ The minimum number of hours that the worker is eligible to request a cash disbursement
◦ The maximum number of hours that the worker can request, for instances where you want to limit the

amount to a certain number of hours

◦ An increment to prevent workers from entering decimal places, and thus avoid rounding issues later
If you don't specify any minimum, maximum, and increment quantities, the application assumes that there are no
minimum, maximum, and increment outputs.

Initiate Cash Disbursement Request
Here's how workers and managers start a cash disbursement:

1. Click Cash Disbursements in the Time and Absences page. Managers can navigate to this page using the Cash

Disbursements quick action from My Team page.
2. Click Add in the Request Cash Disbursement page.

93

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

3. Select the date and absence plan you want to disburse from. Enter the amount of time you want to disburse.

Note:  Employees with multiple assignments must select the assignment and then the plan from which they
want to donate. Managers and administrators will see one row per assignment when they search for the
employee. Select the assignment from which donation is to be made.

4. Click Submit.

If you're an administrator, here's how you disburse an employee's balance:

1. Click Absence records in the Absences work area under the My Client Groups tab.
2. Search and select the employee to open the Manage Absences and Entitlements page.
3. Select the absence plan and click Disburse Balance on the Enrollments and Adjustments menu. This menu is in

the Plan Participation section.

4. Select the date and enter the amount to be disbursed.
5. Click Submit.

Approve Cash Disbursement Request
Optionally, you can configure approval notifications for the self-service cash disbursement requests. For example,
you want line managers to approve cash disbursement transactions requested by workers. Managers can view these
notifications by clicking the Notifications icon on the Home page or receive these notifications by email and decide
whether to approve or not.

To configure disbursement approval notifications:

1. Go to the BPM Worklist.
2.

In the BPM Worklist, on the Task Configuration tab, select the AbsencePlanBalanceDisbursementApproval
workflow task to configure, and then click the Edit task icon in the Tasks to be configured toolbar.

3. Open the Assignees subtab and modify the approval rule, if required.
4. Click Save.
5. Click the Commit task icon in the Tasks to be configured toolbar when you're ready to deploy your changes.

Options to Enable Absence Accrual Balance Adjustments

Use the Entries and Balances tab on the Absence Plans page to enable the following types of accrual plan adjustments:

• Balance transfer across plans

• Other adjustments

• Elective disbursements

When you enable these adjustments, it then allows HR specialists to make adjustments to plan balances on the Manage
Absence Records and Entitlements page. To make adjustments, HR specialists can select an option on the Enrollments
and Adjustments menu of the Plan Participation section.

Balance Transfer Across Plans
This adjustment option enables HR specialists to select a source plan and specify an amount of time to transfer to a
target plan balance.

94

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Other Adjustments
This adjustment option enables HR specialists to make special adjustments to plan balances, such as award leave
time to a worker for exemplary performance at work. When HR specialists make adjustments on the Manage Absence
Records and Entitlements page, they can select Clerical Error or Compensatory as the adjustment reason.

Elective Disbursements
This adjustment option integrates benefits election with absences so that participants can sell all or part of their
vacation or sick accrual balance. You can create vacation or sick time sell plans in Benefits. During open enrollment or an
annual anniversary, a participant who's eligible for these plans can select the number of units to disburse and the date
the disbursement should be processed by payroll for payment. When participants make their elections to specify how
much time to sell and when, the information is sent to Absence Management for further processing. These elections
reflect in Absence Management when the accrual process is run.

To integrate benefits election with absences:

1. Select Enable benefits integration.
2. Select Mark as pending to indicate whether the disbursement is finalized or not after the accrual process is run

and the information sent to payroll.

3. Select one of the following options for the Election Date Rule:

◦ Current plan year end: The end date for the current plan year is used as the disbursement date.
◦ Determined by election: The end date is elected within Benefits. If you select this option, the elective

amount is disbursed only if the employee has a valid payroll relationship.

Automatic Plan Enrollment and Balance Copy During
Local and Global Transfer

The Local and Global Transfer process automates accrual plan enrollment and copying of plan balances from the old
organization to the new one. When an employee is transferred, all active plans are end-dated in the old organization. If
the employee is eligible for the same plans in the new organization, the application automatically enrolls the employee
to the same plans in the new entity.

Here’s how other attributes of the absence plan are processed during the transfer:

Configurations

What happens during the transfer

Absence plan with carryover enabled

The carryover amount, as well as the carryover expiration details, if applicable, is copied over to

the new plan. The new plan shows an initial balance copied over from the old organization and any

applicable carryover amounts that expire on or after the transfer.

Absence Plan with vesting options enabled The vesting attributes from the old entity are copied to the new entity. For example, an employee has

8 hours of unvested accruals earned on January 1st that are set to vest on April 1st and a local or global

transfer happens on March 15th. The 8 hours of unvested accruals will still vest on April 1st just like it

would’ve in the old entity.

95

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Configurations

What happens during the transfer

Absence Plan with waiting period options

The same enrollment date based on the waiting period defined in the old entity is copied to the new

enabled

entity. For example, if an employee enrolled in a plan with a 90 day waiting period beginning on

January 1st, is transferred on March 15th, the enrollment in the new entity will be on April 1st just like it

would’ve been in the old entity.

Plans with disbursement and/or rollover

The applicable attributes from the old entity are copied to the new entity.

options enabled

You can view information about all the absences plans, future or scheduled absences and future plan transactions in the
Absences section of the HR Local and Global Transfer page. The Absence Plans section shows you details about all the
plans that the employee is currently enrolled in. This includes the plan’s name, enrollment date, disbursement option,
and balance as of the transfer date. During a global transfer, the final balance is calculated one day before the global
transfer date.

The Existing Absences section displays all absences that are currently in progress. It also shows all future and
scheduled absences, scheduled on or after the transfer date. Open-ended absences that don’t end before the transfer
date will be end dated on the day before the transfer date. All future absences scheduled on or after the transfer date
will be withdrawn automatically. The Additional Transactions section shows you all future plan transactions scheduled
on or after the transfer date that will be withdrawn. These transactions include donations, disbursements, transfers,
compensatory time and adjustments.

Create a Vacation Accrual Plan

This example shows how to create an absence accrual plan for vacation leave. The following table summarizes key
decisions for this scenario.

Decisions to Consider

In This Example

Who is eligible for this plan?

All workers

What unit of measure should this plan use
to process absences?

Days

What is the start date and length of the
accrual plan term?

Start on January 1 and restart the same day in the following year.

When can workers start accruing leave
time on the plan?

1 month after hire date

When can workers start using the leave
time that they accrued

2 months after hire date

96

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Decisions to Consider

In This Example

How much leave time can workers accrue
in a term?

Workers who belong to grade A and B accrue at the rate of 15 days each accrual term. They can carry-
over 5 days to the next term.

Workers who are grade C and D accrue at the rate of 12 days each accrual term. They can carry-over 2
days to the next term.

Do you want workers to accrue time
for the whole term at once or accrue in
increments?

Accrue time each pay period.

What is the maximum leave time that
workers can accrue?

40 days

Can workers use more time than their
standard accruals during the plan term?

Yes, up to 5 days

How do you want to calculate cash
disbursals of partial accrual balances at
any time?

50 percent of the salary amount determines the payment for a unit of absence.

How do you want to calculate final balance
payments for a terminated worker?

The salary amount determines the payment of a unit of absence.

Task Summary
To create the absence plan:

1. Create two rate definitions and a payroll element.
2. Create the absence plan.

Prerequisites
Before you create the absence plan, in the Absences work area:

1. Use the Rate Definitions task to create two rate definitions that calculate payment of a unit of absence based on

50 percent and 100 percent of the salary amount.

2. Use the Manage Elements task to create a nonrecurring element. Specify Absences as the primary classification
and Vacation as the secondary classification in the Create Element dialog box, and complete the sections as
shown in this table.

Section

Value

Absence Plan Details

Select Accrual Balances and Absences as the type of absence information to transfer to

payroll.

Accrual Liability and Balance Payments

Select Yes for these questions:

97

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Section

Value

◦ Calculate Absence Liability?
◦ Does this plan enable balance payments when enrollment ends?
◦ Does this plan enable partial payments of absences?
You must specify a rate for the liability calculation, which should be the same rate specified as

the liability booking rate rule in Absence Management.

Absence Payments

Select the Reduce regular earnings by absence payment option for the following question:

◦ How do you want to reduce earnings for employees not requiring a time card?

Creating the Rate Definitions

In the Absences work area Tasks panel tab, click Rate Definitions.

1.
2. Click Create.
3. On the Create Rate Definition page, complete the fields, as shown in this table.

Field

Name

Value

Unit Rate of 50 Percent Salary

Short Name

UR_50_PC_Salary

Legislative Data Group

Select your legislative data group.

Periodicity (Returned Rate Details

Bimonthly

section)

Balance Dimension

Year to Date

Periodicity (Calculation section)

Bimonthly

4. Click Create.
5. On the Create Rate Contributors page, complete the fields, as shown in this table.

Field

Balance Name

Value

FIT Gross

Balance Dimension

Year to Date

98

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Field

Type

Add or Subtract

Factor Rule

Factor Value

Value

Actual

Add

Value

0.50

6. Click Save and Close.
7. Repeat step 2 through step 6 to create another rate definition. Ensure that you provide the following key

information, as shown in this table:

Field

Name

Value

Unit Rate of Salary

Short Name

UR_ Full_Salary

Factor Value

1.00

Creating the Absence Plan

In the Absences work area Tasks panel tab, click Absence Plans.

1.
2. Click Create.
3.

In the Create Absence Plan dialog, complete the fields, as shown in this table.

Field

Value

Legislation

Select your legislation.

Plan Type

Accrual

4. Click Continue.

99

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

5. On the Create Absence Plan page, complete the fields, as shown in this table.

Field

Plan

Value

Vacation

Legislative Data Group

Select your legislative data group.

Status

Plan UOM

Active

Days

Type

Calendar year

Calendar

Select the first day of your plan term year. In this example, select January 1 of the current year.

6. Click Save.
7. Select the Participation tab, and complete the fields, as shown in this table.

Field

Waiting Period UOM

Duration

Value

Months

1

8. Click Save.
9. Select the Accruals tab, and complete the fields, as shown in this table.

Field

Value

Accrual Method

Incremental

Accrual Frequency Source

Person primary frequency

Accrual Vesting Rule

Elapsed period

Duration

UOM

2

Months

100

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Field

Value

Ceiling Rule

Flat amount

Ceiling

40

Carryover Rule

Include in matrix

Negative balance allowed

Select

Negative Balance Limit

5

10.

In the Accrual Matrix section, create accrual bands, as shown in this table.

Sequence

Expression

Accrual Rate

Carryover Limit

1

2

([Person.Grade] = "A") OR

15

([Person.Grade] = "B")

([Person.Grade] = "C") OR

12

([Person.Grade] = "D")

5

2

11. Click Save.
12. Select the Entries and Balances tab, and complete the fields, as shown in this table.

Field

Value

Final Balance Payment Rate Rule

Select the Unit Rate of Salary rate definition that you created.

Disbursement Rate Rule

Select the Unit Rate of 50 Percent Salary rate definition that you created.

Absence Payment Rate Rule

Select the Unit Rate of Salary rate definition that you created.

Liability Booking Rate Rule

Select the Unit Rate of Salary rate definition that you created.

Transfer absence payment

Select

information for payroll processing

101

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

Field

Element

Value

Select the element that you created as part of the prerequisite task.

13. Review the information you entered in all the tabs.
14. Click Save and Close.

Managing Existing Absence Plans

You can update or correct existing absence plans from the Absence Plans page.

Best Practices for Inactivating Absence Plans
You can inactivate absence plans as of a specific date, but you need to ensure that you don't run accruals beyond this
date. If you do, employees can't add or withdraw absences. That's because the application attempts to rerun accruals
and reprocess future absences that lie beyond the inactive date of the plan.

Ensure that you set the plan inactivation date to a date that's after the accrual run date for all employees. Employees
won't be able to perform transactions if the absence plan is inactivated. Decide how you want to deal with the accrued
leave balances of the employees. You should either un-enroll all employees from the plan before you inactivate it or
withdraw accruals to a date prior to the inactivation date using the Withdraw Accruals and Balances process.

Before you make any date effective changes to the plan, try it out on test environment first. See whether the change
produces the results you expect. If it does, implement the change on a production environment.

FAQs

What happens to absences during an employee's termination or
reverse termination?

When an employee is terminated, the absence plan enrollment end date is set to the termination date. The balance
that's accumulated from the enrollment start date to the termination date becomes the new absence balance. All
disbursements and calculation cards after the termination date are removed.

If the employee's termination is reversed, the original absence plan enrollment date is restored. The absence plan
balance reflects the balance from the last balance run date before the employee was terminated. However, the
disbursements and calculation cards that were removed due to termination aren't restored.

102

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

What happens to the absence plans when I create a global
temporary assignment for an employee?

When you create a global temporary assignment for an employee, the application creates new absence plan enrollments
for the new assignment.

The status of the existing assignment for which the global temporary assignment was created is set to the status of
Suspended - Payroll Eligible. The assignment and the absence plan aren't end dated. The absence plan continues to
accrue balance.

103

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 9
Accrual Absence Plans

104

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

10  Qualification Absence Plans

Types of Absence Plans

Create the following types of plans using the Absence Plans task in the Absences work area:

• Accrual

• Qualification

• No Entitlement

• Agreement

• Compensatory

• Donation

Accrual
Use this type to create absence plans that enable workers to accrue time for taking paid leave, such as a vacation plan.
Configure rules that determine various aspects of leave time, such as:

• Length and type of the accrual term in which workers accrue time

• Maximum time that workers can accrue in a term

• Maximum time that workers can carry forward to the next term

Qualification
Use this type to create an absence plan where workers qualify for the plan and receive payments during the absence
period. For example, use qualification plans for defining absence rules related to events, such as long term illness or
maternity. Configure rules to determine the payment percentages that apply for specific periods during the absence, for
specific workers.

No Entitlement
Create absence plans of this type to track unpaid absences without maintaining an accrual balance or providing leave
entitlements, such as periodic accruals. Similar to an accrual plan, you can define the length and type of the plan term
and determine when eligible workers can enroll in the plan. You can also use plans of this type in combination with a
qualification plan. For example, use a no-entitlement plan if a worker isn't eligible for a standard maternity absence
qualification plan.

Agreement
Create absence plans of this type in accordance with statutory rules for use under an agreement. For example, create a
shared parental leave agreement for a worker and qualified parental partner to allocate paid or unpaid time off among
parenting partners.

105

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

Compensatory
Create absence plans of this type to track earned compensatory time that can be used for time off. Compensatory time
is offered as compensation for working outside of regular work schedules. Instead of paying overtime, an employer can
create a policy to give paid time off.

Donation
Create absence plans of this type to track donated time that a worker receives. Workers can donate their accrual plan
balance to a coworker who needs additional time off and is eligible to receive the donated time.

Related Topics

• Create a Maternity Plan

• Create a Vacation Accrual Plan

Options to Define Qualification Plans

Configure the following rules when you create an absence qualification plan in accordance with the leave policy of your
enterprise:

• Plan term

• Plan eligibility

• Enrollment and termination

• Payments

Plan Term
A qualification plan term is an assessment period for which the Evaluate Absence process calculates entitlements for the
total absent time recorded in that period. When you create an absence qualification plan, you must select the type of
plan term. For example, you can limit the duration of the plan term to the duration of the absence.

Plan Eligibility
Associate an eligibility profile with the qualification plan to determine the set of workers who are eligible to record an
absence that belongs to that plan.

Enrollment and Termination
Decide when to enroll workers in the qualification plan. Also, decide whether ongoing payments under this plan must
continue if a worker is terminated or loses eligibility for the plan.

Payments
Use an entitlement band matrix to determine the payment percentages that apply for specific time periods during an
absence. Decide how you want to calculate the payment rate of a single unit of absence. You can use a rate definition to
include the calculation rules, or use a formula. For example, you want workers who have completed a particular tenure
to receive specific percentage of pay for a specific absence period.

106

Oracle Fusion Cloud Human Resources
Implementing Absence Management

The following table shows a sample scenario:

Length of Service

Payment Rule

5 to 10 years

75 percent up to 10 absent days.

10 to 20 years

75 percent up to 20 absent days.

Chapter 10
Qualification Absence Plans

Decide how you want to calculate the payment rate of a single unit of absence. You can use a rate definition to include
the calculation rules, or use a formula.

Related Topics

• Create a Maternity Plan

Options to Define a Qualification Term

A qualification plan term is an assessment period during which absence entitlement for the total absence time recorded
in that period is considered.

While creating a qualification absence plan using the Absence Plans task, you need to select one of the following plan
term types:

• Calendar year

• Rolling backward

• Rolling forward

• Absence duration

Calendar Year
The qualification plan term starts on the month, day, and year that you select. The duration of the term is one year. For
example, if you select January 1, 2015, the qualification term starts on that day and ends on December 31, 2015.

Rolling Backward
A rolling-backward term calculates absence entitlements based on the total duration of absences for a specific time
period that precedes the absence start date. For example, if you specify a one year rolling period, and the worker's
absence start date is January 1, 2015, then the calculation considers absences scheduled from January 2, 2014. You can
also configure rules to determine how to deal with absences that overlap rolling backward terms.

Rolling Forward
A rolling forward term calculates absence entitlements based on the first date a worker's absence begins and calculates
the end date by adding the term duration to the start date. For example, if the term duration is 365 days and the
absence start date is 12 February, then the end date will be 11 February of the following year. The rolling forward option
evaluates absences between this start date and end date to track plan entitlements for that period.

107

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

Absence Duration
The absence duration determines the qualification plan term. For example, if a worker schedules a maternity absence
from January 1, 2015 to April 15, 2015, then that's the duration of the qualification plan term.

Related Topics

• Options to Define Overlap Rules for Qualification Plans

• Create a Maternity Plan

Options to Define Overlap Rules for Qualification Plans

When you define a rolling backward plan term for an absence qualification plan, you must select an overlap rule that
determines how to deal with absences where only a partial period overlaps the current term.

The examples in this topic will help you understand how you can use the following:

•

Include rule to assess absences that overlap current and previous terms

• Exclude rule to ignore the entire absence that overlaps the current and previous terms

• Split rule to assess absences falling within the current term only

The Include Rule
If an absence overlaps the beginning of the rolling period, you consider the entire absence in the current assessment
period.

Scenario: You defined a six-month rolling-backward term in your qualification plan and set up bands that entitle workers
to 20 days absence at full pay and a further 15 days at half pay.

• The assessment period for a worker began on January 1, 2014.

• The worker starts sick leave on July 1, 2014.

Previously, the worker received payment under the same sick leave entitlement plan for 15 working days from December
20, 2013 to January 7, 2014.

Because you configured the plan term to use the Include rule, the previous absence that overlaps the current
assessment period is considered. So for the absence beginning on July 1, 2014, the worker receives full pay for the first 5
(20 - 15) days of the absence and half-pay for the next 15 days.

The following figure shows the usage of the Include rule in this scenario.

108

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

The Exclude Rule
If a worker is absent at the beginning of an assessment period, this rule ignores the entire absence that overlaps the
period. In the example used in the previous scenario, for a rolling backward term that uses the Exclude rule, the worker
receives:

• Full pay for the first 20 days of the absence

• Half pay for the next 15 days

Even though the previous absence overlaps the current assessment period, the worker receives the entitlement band
benefits for the current absence without any deductions.

The following figure shows the usage of the Exclude rule in this scenario.

109

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

The Split Rule
This rule assesses overlapping absences that fall within the current plan term only. In the example used in the previous
scenario, for a qualification plan that uses the Split rule, the worker receives full pay for the first 15 (20 - 5) days of the
absence and half pay for the next 15 days.

The following figure shows the usage of the Split rule in this scenario.

110

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

Related Topics

• Create a Maternity Plan

Options to Configure Qualification Enrollment and
Termination

Workers qualify for qualification plan entitlements as a result of an event, such as childbirth, and these entitlements
stop when they are terminated or their plan eligibility ends.

111

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

Define when you want to enroll or disenroll a worker in the Participation tab of the Absence Plan setup page. Configure
the plan to do the following:

• Enroll workers in the plan when a worker or an administrator schedules an absence using an absence type

associated with a qualification plan.

• Use a formula if you must consider other aspects or rules that determine when to enroll workers in the plan.

Decide whether ongoing payments under this plan must continue if a worker is:

• Terminated

• Not terminated, but loses eligibility for the plan

How You Configure Eligibility for Absence Plans

An eligibility profile in Absence Management defines criteria used to determine whether a person qualifies for an
accrual or qualification absence plan. Define eligibility profiles and then associate it with a plan to determine the set of
workers who can enroll in that plan.

1. Create the eligibility profile using the Manage Eligibility Profiles task in the Absences work area.
2. Associate the eligibility profile with the absence plan using the Absence Plans task.

If you want all workers to be eligible for the absence plan, then don't add an eligibility profile. If a plan doesn't have
an eligibility profile associated with it, then it doesn't mean that workers are enrolled automatically into the plan. New
hires may be enrolled automatically, if that's the option set in the plan definition. Existing workers have to be enrolled
manually.

Examples of Qualification Bands

Use qualification bands to determine the payment percentages that workers receive for specific time periods during a
long leave of absence. Use employment criteria, such as length of service, grades, or other factors to filter workers.

You can define various types of qualification bands in the Qualification Band Matrix section on the Absence Plan setup
page. The examples show qualification bands based on the following factors:

• Length of service

• Grade

• Length of service and grade

Creating a Single Payment Band for Multiple Length of Service Ranges
Scenario: You want to create a single payment band for workers who have completed the following years of service:

• For workers who have completed between 5 and 10 years of service to receive 75 percent of pay for up to 10

days of absence

• For workers who have completed between 11 and 20 years to receive the same pay percentage, but up to 20

days of absence

112

Oracle Fusion Cloud Human Resources
Implementing Absence Management

To create the bands:

Chapter 10
Qualification Absence Plans

1. Create the following length of service derived factors using the Manage Derived Factors task in the Absence

Administration work area.

◦ Length of service greater than or equal to 5 years and less than 10 years
◦ Length of service greater than or equal to 10 years and less than 20 years

2. Use the expression builder in the Qualification Band Matrix section to create bands using the derived factors

that you created:

Band Sequence

Expression

1

2

[LengthOfService.GreaterThan5_LessThan10]

[LengthOfService.GreaterThan10_LessThan20]

For each band that you create in the Qualification Band Matrix section, you must create band details in the Qualification
Details section.

This table shows the band details that you must create for Band 1, which you created for workers who have completed
between 5 and 10 years of service.

Band Sequence

Detail Name

Duration

Payment Percentage

1

75 percent up to 10 days of
absence

10

75

This table shows the band details that you must create for Band 2, which you created for workers who have completed
between 10 and 20 years of service.

Band Sequence

Detail Name

Duration

Payment Percentage

1

75 percent up to 20 days of
absence

20

75

Creating Multiple Payment Bands for a Grade Range
Scenario: You want all workers who belong to grade A1 and above to receive:

•

100 percent of pay for up to 10 days of leave

• 75 percent of pay for up to a further 15 days of leave

This table shows the band information that you create using the expression builder in the Qualification Band Matrix
section.

113

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

Band Sequence

Expression

1

[Person.Grade] >= "A1"

The person.grade attribute is on the Entities tab in the Expression Builder dialog box.

This table shows the band details that you must create for Band 2 in the Qualification Details section

Band Sequence

Detail Name

Duration

Payment Percentage

1

2

100 percent pay up to 10 days of
absence

10

75 percent pay for the next 15 days

15

100

75

Creating Multiple Payment Bands for Multiple Length of Service and Grade
Ranges
Scenario: You want workers who have completed the following years of service:

Length of Service

Payment Percentage

Less than 5 years

To be eligible for:

• 75 percent of pay for up to 10 days of absence

• 50 percent of pay for a further 15 days of absence

Greater than or equal to 5 years and who
belong to the A1 grade

To be eligible for:

• Full pay up to 10 days of absence

• 75 percent of pay for a further 15 days of absence

To create the bands:

1. Create the following length of service derived factors using the Manage Derived Factors task in the Absence

Administration work area.

◦ Length of service less than 5 years
◦ Length of service greater than or equal to 5 years

2. Use the expression builder in the Qualification Band Matrix section to create bands using the derived factors

that you created:

Band Sequence

Expression

1

[LengthOfService.LessThan5]

114

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

Band Sequence

Expression

2

[LengthOfService.GreaterThan5] AND [Person.Grade] = "A1"

This table shows the band details that you must create for Band 1 in the Qualification Details section.

Band Sequence

Detail Name

Duration

Payment Percentage

1

2

75 percent pay up to 10 days of
absence

10

50 percent pay for the next 15 days

15

75

50

This table shows the band details that you must create for Band 2 in the Qualification Details section.

Band Sequence

Detail Name

Duration

Payment Percentage

1

2

100 percent pay up to 10 days of
absence

10

75 percent pay for the next 15 days

15

100

75

Related Topics

• Create a Maternity Plan

Evaluate Entitlement without Absence Record

Use the Evaluate remaining entitlement without absence record check box to determine how the Manage Absences
and Entitlements page displays entitlements. The check box is available on the Participation tab of the Absence Plan
setup page.

The following table outlines the impact of the check box on the display of information in the Manage Absences and
Entitlements page:

Check Box Value

Actions Available for HR Specialist

Selected

Not selected

View complete qualification plan entitlement details defined for the worker, even without an absence
record

View partial plan entitlement details of scheduled absences with different payment percentages. They
can't view the plan period, qualified entitlement, and remaining entitlement.

HR specialists can view partial plan entitlements in the following scenarios:

115

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

Check Box Value

Actions Available for HR Specialist

• Worker applied for only a single absence for the plan

• Worker applied for multiple absences and all of the absences are falling in the same payment

percentage

• Worker applied for multiple absences and all of the absences are falling in different payment

percentages

If the worker hasn't scheduled any absence for the plan, the Qualification Plans section of the Manage
Absences and Entitlements page displays no plan details.

How Qualification Plan Entitlement Appears

For qualification plans, the qualified entitlement details for a worker are displayed in the Qualification Entitlements
section of the Manage Absences and Entitlements page. The payment percentage defined during plan setup
determines the calculation of these qualified entitlements.

Settings That Affect Display Of Qualification Plan Entitlement
To view all qualified entitlement details, you must select the Evaluate remaining entitlement without absence record
check box. This check box is available on the Participation tab of the Absences Plans page. If you don't select the check
box during plan creation, you can view only the payment percentage and used entitlement in the Qualification Plans
section. No data appears for the plan period, qualified entitlement, and remaining entitlement columns.

How Qualification Plan Entitlement Is Calculated
Scenario: You defined a one-year rolling backward term in your qualification plan. You set up bands that entitle workers
to 30 days absence at full pay and an additional 30 days at half pay.

A worker took an absence for 88 days, from June 1, 2015 to September 30, 2015. The Qualification Plans section displays
the following qualified entitlements for an effective date of Sep 30, 2015 (Plan period will be Oct 01, 2014 - Sep 30, 2015):

Plan

Plan Period

Payment Percentage Qualified Entitlement Used

Remaining

Sick Leave

Sick Leave

100

50

30

30

30

30

0

0

The worker schedules another absence using the same plan from September 1, 2016 to September 30, 2016 for 22 days.
Since you defined a one-year rolling backward term, the details considered for the 365 day time period that precedes
the absence start date are:

Decisions to Consider

In This Example

Rolling backward start date

September 2, 2015

116

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

Decisions to Consider

In This Example

Used entitlements during the rolling
backward time period

21 days at 0 percent (September 1, 2015 to September 30, 2015)

Available entitlements

30 working days at 100 percent, and the next 30 working days at 50 percent

For the 22-day absence from September 1 through September 30, 2016, the worker qualifies for full payment. The
Qualification Plans section displays the following qualified entitlement for an effective date of Sep 30, 2016 (Plan period
will be Oct 01, 2015 - Sep 30, 2016):

Plan

Plan Period

Payment Percentage Qualified Entitlement Used

Remaining

Sick Leave

Sick Leave

100

50

30

30

22

0

8

30

If you don't select the Evaluate remaining entitlement without absence record check box during plan creation, the
qualified entitlements appear as shown in the following table:

Plan

Plan Period

Payment Percentage Qualified Entitlement Used

Remaining

Sick Leave

100

22

Open-ended Absences

For qualification plans, you can record an open-ended absence when the employee isn't sure about the end date of the
absence. This open-ended option is applicable for some absences, such as maternity or illness.

When you select the Open-ended check box, the end date is no longer available. You can enter an estimated end date,
but this date is not used in entitlement calculation. Instead, the entitlement is calculated for 365 days. If the absence
requires an extension beyond one year, a Pending Evaluation record is created, which denotes that the absence can be
extended by 90 days when the Evaluate Absences process is run.

When an end date is entered on the absence, the entitlement is recalculated based on the actual end date.

Calculation of Qualified Entitlements for Open-ended Absences
The applicable payment percentage defined during plan setup determines the entitlement calculation for open-ended
absences.

117

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

For example, an employee is eligible for qualified entitlements for 365 days. When the employee schedules an open-
ended absence, the calculation displays as follows in the Entitlements section of the Plan Use tab:

Absence Duration

Qualified Entitlement Display

365 days

Displays the absence in a new row with the activity as Qualified Entitlement.

Exceeds 365 days

Displays the absence in a new row with the activity as Pending evaluation. This denotes that the
absence can be extended by 90 days when the Evaluate Absences process is run.

After the employee enters an end date, a new row is generated with an Entitlement exceeded entry for the unpaid
days.

Create a Maternity Plan

This example shows how to create an absence qualification plan for employees taking maternity leave.

The following table summarizes key decisions for this scenario.

Decisions to Consider

In This Example

Who is eligible for this plan?

Only full time regular employees

What unit of measure should this plan use
to process absences?

Weeks

What is the plan term to assess
entitlements?

6 months, rolling backward from the absence start date

How do you deal with absences that
overlap the plan term?

Use the Include rule to assess the entire absence.

How do you deal with terminated workers
and workers who lose eligibility while
receiving entitlements from the plan?

Continue entitlements if worker is terminated. Stop entitlements if worker loses eligibility.

For how much leave time are workers
entitled to receive payment?

Workers who have completed less than 5 years of service are entitled to 8 weeks payment at 90
percent pay followed by a further 16 weeks at 50 percent pay.

Workers who have completed more than 5 years of service are entitled to receive payment for the first
6 weeks at full pay followed by 12 weeks at 75 percent pay.

How do you want to calculate payments?

The declared salary determines the payment of a unit of absence.

Transfer payments for payroll processing?

Yes

118

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

Decisions to Consider

In This Example

Prerequisites
Before you create the absence plan, in the Absences work area:

1. Use the Manage Eligibility Profiles task to create a participant eligibility profile to restrict eligibility of the

absence plan to full time regular workers. In the Employment tab, Assignment Category subtab, select Full-time
regular from the Full Time or Part Time list.

2. Use the Manage Derived Factors task to create length of service derived factors. Don't create a qualification

absence plan with multiple expression builders where all expression builders are satisfied. If there is a specific
scenario, create multiple plans instead of multiple expression builders.

3. Use the Manage Rate Definitions task to create a rate definition for payment of a unit of absence based on the

declared salary on the absence start date.

4. Use the Manage Elements task to create a nonrecurring element. Use Absences as the primary classification

and Maternity as the secondary classification. In the Absence Plan Details section, select Qualification Absences
as the type of absence information you want transferred to payroll.

Creating the Length of Service Derived Factors

1.
2.
3.

In the Absences work area Tasks panel tab, click Manage Derived Factors.
In the Length of Service tab, click Create.
In the Create Derived Factor Length of Service dialog box, complete the fields, as shown in this table.

Field

Name

Value

LengthOfService_LessThan5

Unit of Measure

Years

Less Than Length of Service

5

Period Start Date Rule

Date of hire

Determination Rule

As of event date

4. Click Save and Create Another.
5. Complete the fields, as shown in this table.

Field

Name

Value

LengthOfService_GreaterThan5

119

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

Field

Unit of Measure

Value

Years

Greater Than or Equal to Length of

5

Service

Period Start Date Rule

Date of hire

Determination Rule

As of event date

6. Click Save and Close.

Creating the Rate Definition

In the Absences work area Tasks panel tab, click Manage Rate Definitions.

1.
2. Click Create.
3. On the Create Rate Definition page, complete the fields, as shown in this table.

Field

Name

Value

Maternity Leave

Short Name

MAT LEAVE

Legislative Data Group

Select your legislative data group.

Periodicity (Returned Rate Details

Bimonthly

section)

Balance Dimension

Year to Date

Periodicity (Calculation section)

Bimonthly

4. Click Create.
5. On the Create Rate Contributors page, complete the fields, as shown in this table.

Field

Balance Name

Value

FIT Gross

120

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

Field

Value

Balance Dimension

Year to Date

Type

Add or Subtract

Factor Rule

Factor Value

Actual

Add

Value

1.00

6. Click Save and Close.

Creating the Absence Plan

1.
2. Click Create.
3.

In the Absences work area Tasks panel tab, click Manage Absence Plans.

In the Create Absence Plan dialog box, complete the fields, as shown in this table.

Field

Value

Legislation

Select your legislation.

Plan Type

Qualification

4. Click Continue.
5. On the Create Absence Plan page, complete the fields, as shown in this table.

Field

Plan

Value

Maternity

Legislative Data Group

Select your legislative data group.

Status

Plan UOM

Active

Weeks

Type

Rolling backward

121

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

Field

Value

Term Duration

6

Term Duration UOM

Months

Start Rule

Absence Start Date

Overlap Rule

Include

6. Click Save.
7. Click the Participation tab, and complete the fields, as shown in this table.

Field

Value

On Loss of Plan Eligibility Only,

Select

 Terminate Entitlement

Eligibility

Select and add the eligibility profile that you created as part of the prerequisite task.

8. Click Save.

Defining an Entitlement Matrix for the Maternity Plan

1. Click the Entitlements tab.
In the Entitlement Attributes section, select Matrix.
2.
In the Qualification Band Matrix section, click Add to add a row.
3.
4.
In the Sequence field, enter 1.
5. Click the Expression Builder icon.
6.
7. Click Insert Into Expression.
8. Click OK.
9.
10. Repeat step 3 through step 9. Ensure that you provide the following key information, as shown in this table:

In the Derived tab, expand Length of Service, and select LengthOfService_LessThan5.

In the Create Absence Plan page, click Save.

Field

Sequence

Value

2

Derived factor to select in the

LengthOfService_GreaterThan5

expression builder

122

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

11.
12.

In the Qualification Band Matrix section, click the LengthOfService_LessThan5 row.
In the Qualification Details section, complete the fields, as shown in this table.

Sequence

Detail Name

Duration

Payment Percentage

1

2

8 weeks at 90 percent pay

16 weeks at 50 percent pay

8

16

90

50

13.
14.

In the Qualification Band Matrix section, click the LengthOfService_GreaterThan5 row.
In the Qualification Details section, complete the fields, as shown in this table.

Sequence

Detail Name

Duration

Payment Percentage

1

2

6 weeks at full pay

12 weeks at 75 percent pay

6

12

100

75

15. Click Save.
16. Click the Entries and Balances tab, and complete the fields as shown in this table.

Field

Value

Absence Payment Rate Rule

Select the Maternity Leave rate definition that you created.

Transfer absence payment

Select

information for payroll processing

Element

Select the element that you created as part of the prerequisite task.

17. Review the information you entered in all the tabs.
18. Click Save and Close.

Related Topics

• Define Payroll Elements to Process Absences

123

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

How You Create a Shared Parental Leave Agreement

In accordance with government-mandated rules of your country, you can configure a shared parental leave agreement.
The shared parental leave enables workers to curtail their maternity or adoption leave in order to share it with their
partner.

The shared parental leave may be paid or unpaid. The amount of leave which can be taken depends on how much leave
the person curtailing the maternity or adoption leave has left.

Here's how you create a shared parental leave agreement for your legislation:

1. Create absence plans for Childbirth and Adoption using the Absence Plans task in the Absences work area.
2. Create absence types for Childbirth and Adoption using the Absence Types task in the Absences work area.
3. Set up an agreement template that specifies the source plan and the target plan using the Leave Agreements

task in the Absences work area.

Creating Absence Plans for Shared Parental Leave
Select the Agreement plan type and create the following absence plans for Shared Parental Leave:

• Childbirth

• Adoption

Add two bands, one paid and the other unpaid in the Entitlements tab.

Creating Absence Types for Shared Parental Leave
Select the Generic absence pattern and create the following absence types for Shared Parental Leave:

• Childbirth

• Adoption

On the Create Absence Types page:

1.
2.

3.

In the Type Attributes tab, select the Agreement Selection field.
In the Plans and Reasons tab, ensure that the status of the selected plan is Active and the priority is set to 1.
Occupational plans can also be added to the same absence type. However, make sure the priority of those
plans is higher than the statutory plan and they're not concurrent. This ensures that the entitlement under the
statutory plan is always calculated, irrespective of whether the workers are eligible for occupational plans or not.
In the Display Features tab, set the Open Ended field to Do not display. This field is in the Dates and Duration
section.

Setting up an Agreement Template
The Shared Parental Leave functionality is governed using two processes which are based on agreement templates. Two
Agreement Templates patterns are available out of the box:

• Childbirth or placement conversion (Giver)

• Childbirth or placement agreement(Receiver)

124

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

You can use them to set up an agreement template using the Leave Agreements task, which specifies:

• The mother or primary adopter's source plan (Giver) where the entitlement is converted to shared entitlements.

• The partner's target plan (Receiver) associated with the Shared Parental Leave agreement that receives the

mother's or primary adopter's entitlements.

Use agreement templates to define eligibility rules and reason codes for denial or withdrawal of agreements. You can
also specify entitlement or eligibility formula, enable partner selection and entitlement allocations, and give the option
to add documentation certifications.

Once you've created both the agreement templates, you can associate them to an absence if the absence type has been
configured for it during absence entry. The absence will consume from the entitlements shared through the agreement.
However, the absence needs to be entered within the agreement period and must not be longer than the duration
allocated on the agreement.

125

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 10
Qualification Absence Plans

126

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 11
Compensatory Time

11  Compensatory Time

Options to Define Compensatory Plans

Configure the following rules when you create a compensatory plan in accordance with the leave policy of your
enterprise:

• Earned time expiration

• Plan eligibility

• Enrollment and termination

• Vesting period

• Plan limits

• Manual Adjustments

Earned Time Expiration
Define whether compensatory time earned is subject to expiration. If yes, define the expiration limit and time frame,
and how you want to process the expired earned time. You can choose whether to expire the full amount or whether
it should be disbursed for payment. The application consumes compensatory time based on the expiration date. This
means that the absence consumes the hours of the compensatory plan that expires first.

Plan Eligibility
Associate an eligibility profile with the compensatory plan to determine the set of workers who can enroll in that plan.

Enrollment and Termination
Decide when to enroll workers in the compensatory plan and choose when to disenroll a terminated worker from the
plan. Administrators and managers can control the date when balances expire based on your configuration. You can
determine who can control these dates in the Expiration Date Updates section of the Entries and Balances tab.

Vesting Period
Define a vesting period for the plan if you want workers to use it after a specific amount of time after plan enrollment.

Plan Limits
Determine the maximum compensatory time that a worker can accumulate into the plan. Additionally, select if a
negative balance is allowed for the plan.

Manual Adjustments
Administrators and managers can manually adjust the compensatory time balance for workers. You can determine who
can make these adjustments in the Manual Adjustments section of the Entries and Balances tab.

127

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 11
Compensatory Time

Expiration Rules for Earned Compensatory Time

When you create a compensatory plan, you need to select an expiration rule to define if the earned compensatory time
is subject to expiration.

There are four expiration rules available for you to choose from:

• Acquisition date

• End of acquisition pay period

• End of acquisition week

• No expiration

Acquisition Date
Compensatory time expires in a defined amount of time from the acquisition date. For example, if the compensatory
time is earned on December 22 and the expiration time frame is defined as six months, the compensatory time expires
on June 22.

End of Acquisition Pay Period
Compensatory time expires in a defined amount of time from the end of the pay period. For example, if the
compensatory time is earned on December 22, the current pay period is December 16 to December 31, and the
expiration time frame is six months, the compensatory time expires on June 30.

End of Acquisition Week
Compensatory time expires in a defined amount of time from the end of the week the compensatory time is earned.
For example, if the compensatory time is earned on December 22, which is the week of December 17 to December 23,
and the expiration time frame is six months, the compensatory time expires on June 23 since the end of the acquisition
week is December 23.

No Expiration
The compensatory time earned is not subject to expiration.

Related Topics

• Options to Define Compensatory Plans

128

Oracle Fusion Cloud Human Resources
Implementing Absence Management

12  Donation

Overview of Donation

Chapter 12
Donation

Workers can donate some or all of their accrual plan balances to others who need it. Administrators and managers can
also do this on behalf of workers.

Here's how workers and managers donate time:

1. Click Donations in the Time and Absences page. Managers can navigate to this page using the Donations quick

action from My Team page.
2. Click Add in the Donations page.
3. Select the date and absence plan you want to donate from. Enter the amount of time you want to donate.

Note:  Employees with multiple assignments must select the assignment and then the plan from which they
want to donate. Managers and administrators will see one row per assignment when they search for the
employee. Select the assignment from which donation is to be made.

4. Select the alias or name of the recipient. If there's no alias, the recipient name appears.
5. Click Submit.

If you're an administrator, here's how you disburse an employee's balance:

1. Click Absence records in the Absences work area under the My Client Groups tab.
2. Search and select the employee to open the Manage Absences and Entitlements page.
3. Select the absence plan and click Initiate Donation on the Enrollments and Adjustments menu. This menu is in

the Plan Participation section.
.Select the date and amount to be donated
.Select the alias or name of the recipient. If the alias isn't defined, the recipient name appears

4.
5.
6. Click Submit.

Options to Define Donation Plans

Create a donation plan for workers who need additional time off over and above their entitlement using the Absence
Plans task in the Absences work area.

Donation Rules
Configure the following rules when you create a donation plan in accordance with the leave policy of your enterprise:

Rule

Description

Unit of measure

Specify the unit of measure for the donation plan. The unit of measure can be only Hours or Days. An
accrual plan shows donors only donation plans with the same unit of measure as their accrual plans.

129

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Rule

Description

Chapter 12
Donation

Enroll workers in only one donation plan of a specific unit of measure so that when a donor initiates a
donation from their accrual plan, the balance transfers to the correct donation plan. For example, if a
donor initiates a donation from a vacation accrual plan measured in days, the donation process looks
for a donation plan measured in days. When it finds the corresponding donation plan, it transfers the
donated time to the worker's donation plan.

If you know that coworkers can donate from multiple plans with different units of measure, then enroll
the worker into two donation plans, one measured in Hours, the other in Days.

Plan limits

Determine the maximum donated time that a worker can accumulate in the plan. Additionally, specify
whether the plan allows a negative balance.

Termination

Specify how to disburse or recover donation plan balances when the worker is terminated.

Balance updates

Specify which types of donation balance adjustments must be available to HR specialists.

Disbursement

Donation type

Specify whether workers are eligible for cash disbursement requests from the donation plan. Decide
who can initiate the disbursement. Additionally, define disbursement rules and the number of hours
that can be disbursed.

Specify whether workers donate to an individual person or to a balance pool. Donations made to the
pool are maintained as monetary fund by the payroll. When employees require additional PTO hours,
 they can request more hours from the donation pool.

Related Topics

• Overview of Donation

How You Can Set Up PTO Donations for Your Legislation

Set up absences so that you can ensure automatic transfer of donated time off between coworkers.

To configure absences for donation, complete these tasks:

1. Create a Donation plan type using the Absence Plans task. Set the unit of measure to Hours or Days. The

unit of measure for the donation and accrual plans must be the same. This ensures that when workers initiate
donations, the accrual plan can identify the correct donation plan.

2. Specify in the Donation Type field whether the donation is to an individual worker or to a pool.
3. Configure donation rules on the corresponding accrual plan to allow workers to donate their accrual balances.
Use the Entries and Balances tab, Donation section to enable the donation feature on an accrual plan. You can
configure donation rules and define the number of hours that a worker can donate to another worker.

4. You can also configure approval notifications for donation requests.
5. Enroll workers needing additional time off in the appropriate donation plan by selecting Add Enrollment on

the Enrollments and Adjustments menu. This menu is on the Manage Absences and Entitlements page, in the
Plan Participation section, Accrual Plans subsection.

130

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 12
Donation

Related Topics

• Overview of Donation

• Options to Define Donation Plans

Create a Donation Plan

Here's how you create a donation plan:

In the Absences work area, on the Tasks panel tab, click Absence Plans.

1.
2. On the Absence Plans page, click Create.
3. On the Create Absence Plan dialog box, in the Plan Type field, select Donation.
4. Click Continue.
5. On the Create Absence Plan page, Plan Attributes tab, enter the name of the plan.
6. Select the legislative data group.
7.
In the Status field, select Active.
8. Specify in the Donation Type field whether the donation is to an individual worker or to a pool. When creating
a donation pool plan, you need to define the eligibility criteria for both the recipients and the donors on the
Participation tab.
In the Plan UOM field, select Hours or Days so that this plan can receive donations from accrual plans with the
same unit of measure. If coworkers can donate time to the worker from multiple plans with different units of
measure, enroll the worker in 2 donation plans, one with Hours and the other with Days.

9.

10. On the Plan Rules tab, optionally specify a ceiling amount. You can select Flat Amount or Formula. The ceiling
amount limits the total donated amount that this plan can receive. You can also specify how to disburse or
recover donation plan balances when the worker is terminated.

11. On the Entries and Balances tab, specify the transactions that this donation plan allows workers to make. For

example, you can allow workers to cash out the donated leave instead of taking an absence.

12. Select Transfer absence payment information for payroll processing and select an absence element to

transfer the donation balance for payroll processing. To integrate the absence plan with Global Payroll, create
elements using the Manage Elements task in the Payroll Calculation work area. Then, associate the element
with the plan on the Create Absence Plan page.

Related Topics

• Overview of Donation

• Options to Define Donation Plans

How You Configure Donation Rules on an Accrual Plan
for Workers to Donate to Coworkers

Enable the donation feature of an accrual plan on the Absence Plans page. Use the Entries and Balances tab, Donation
section. You can also configure donation rules and limit the number of hours that a worker can donate to another
worker.

131

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 12
Donation

For the Donation Rule, you can select either Formula or Flat Amount. When you select Flat Amount, you can also
specify the following quantities. When you select Formula, you must specify a formula that returns values for these
same quantities:

• The minimum number of hours that the worker is eligible to donate

• The maximum number of hours that the worker can donate, for instances where you want to limit the amount

to a certain number of hours

• An increment to prevent workers from entering decimal places, and thus avoid rounding issues later

If you don't specify any minimum, maximum, and increment quantities, the application assumes that there are none.

Related Topics

• Overview of Donation

• Options to Define Donation Plans

Configure Approvals for Donation

You have the option to configure approval notifications for donation requests.

For example, you want line managers to approve donations initiated by workers. To view notifications, managers
can click the Notifications icon on the Home page. They can also opt to receive notifications by email with approval
options.

Here's how you configure donation approval notifications:

1. Go to the BPM Worklist.
2. On the Task Configuration tab, select the AbsencePlanBalanceDonationApproval workflow task to configure,

and then click the Edit task icon in the Tasks to be configured toolbar.

3. Open the Assignees subtab and modify the approval rule, if required.
4. Click Save.
5. Click the Commit task icon in the Tasks to be configured toolbar when you're ready to deploy your changes.

Related Topics

• Overview of Donation

• Options to Define Donation Plans

Enroll a Worker in a Donation Plan

If the worker is eligible to receive a time-off donation from coworkers, here's how you enroll the worker in a donation
plan:

In the Absences work area under the My Client Groups tab, click Absence Records.

1.
2. On the Manage Absences and Entitlements page, in the Plan Participation section, Accrual Plans subsection, on

the Enrollments and Adjustments menu, select Add Enrollment.

3. Select the donation plan.

132

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 12
Donation

4. Enter the date when the worker's plan eligibility starts.
5. Optionally, enter a unique alias to protect the identity of the donation recipient and comply with privacy

requirements of your organization.

6. Optionally, decrease or increase the ceiling amount in the Ceiling Override field if you want to provide a

different limit from the ceiling amount defined during plan setup.

7. Click Submit.

When workers initiate donations from their accrual plans, they see only recipients for donation plans with the same unit
of measure as their accrual plans. Therefore, it's important to enroll workers in donation plans with the correct unit of
measure.

You can make corrections or change the alias by selecting Update Enrollment from the Enrollments and Adjustments
menu of the Manage Absences and Entitlements page. You can even update the ceiling amount to a value lower than
the current balance. However, this means that no more donations are accepted for this plan because the balance is
higher than the ceiling.

Administrators can also manually enroll a worker into a donation pool plan and add donations. Here's how it's done:

1. Click My Client Group > Absences > Absence Records.
2. Search and select the worker who needs to be enrolled into the pool plan.
3.
4. Select the date and the amount to be donated.
5. Click Submit

In the Plan Participation section, click Enrollments and Adjustments, and click Transfer Balance from Pool.

If the worker loses eligibility or doesn’t consume the donated hours in the period specified by company policy, the HR
administrator can manually return the remaining balance from worker's pool plan enrollment back into the donation
pool fund. To do so, click Enrollments and Adjustments > Return Balance to Pool.

Related Topics

• Overview of Donation

• Options to Define Donation Plans

133

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 12
Donation

134

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

13  Absence Types, Reasons, and Categories

How Absence Components Work Together

Configure absence components such as types, categories, patterns, plans, reasons, and certifications to reflect the
absence management policy of your enterprise.

Component

Location in the Absences Work Area

Absence types

Use the Absence Types task to create absence types.

Absence categories

Use the Absence Categories task to create absence categories and associate them with absence types.

Absence patterns

Review these settings on the Display Features tab when you create an absence type.

Absence plans

Use the Absence Plans task to create absence plans.

Absence reasons

Use the Absence Reasons task to create absence reasons.

Absence certifications

Use the Absence Certifications task to set up a requirement. Then associate the requirement as an
action item with an absence type so that every absence associated with the absence type is subject to
that requirement.

135

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

This figure illustrates how the absence management components fit together.

Absence Type
When you create an absence type, such as sick leave, you include rules to determine when users record or manage
an absence of that type. For example, you can restrict workers so that they can record absences only of a particular
duration. An alert appears if the entered duration exceeds the maximum value.

Decide which fields or sections you want to show or hide for specific user roles when they record or approve a specific
absence type.

Absence Category
Create absence categories to group absence types for reporting and analysis. For example, you can create an absence
category called family leave and associate with it absence types, such as maternity, paternity, and child care.

Absence Pattern
An absence pattern contains a predefined set of rules that you can use as a starting point to create an absence type.
When you create an absence type, you must associate it with any of the following predefined patterns:

•

Illness or injury

• Childbirth or placement

• Generic absence

136

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

For example, you can select the Generic absence pattern to create an absence type to schedule vacation time using the
time accrued under a vacation accrual plan.

The pattern that you select determines:

• Whether special fields appear on the absence type pages

• The options available to display and process various aspects of absence recording

For example, the Childbirth or placement pattern displays a field for selecting whether the absence type applies for
childbirth or adoption placement.

Absence Plans
Create absence plans to define rules for accruing leave time and receiving payments during an absence period. You
must associate at least one absence plan with an absence type.

To schedule an absence using an absence plan, the unit of measure defined in the plan must match the unit of measure
defined in the associated absence type. If the unit of measure differs, you can define the conversion formula and attach
it to the absence type. This formula is applicable only if the unit of measure is hours or days for the absence type.

Absence Reasons
Create absence reasons to select from when scheduling an absence. Absence reasons are independent of absence
types. You can use the same reason for multiple absence types. When you create an absence type, you associate the
reasons with the type.

Absence Certifications
Create certification requirements for absences that require documentation to authorize an absence. For example,
in case of an absence due to illness, set up a requirement that workers must submit a doctor's certificate within a
stipulated period of time. This ensures they receive full payment for the absence duration.

Related Topics

• Create a Vacation Absence Type

• Create a Maternity Plan

• Create a Vacation Accrual Plan

• Create an Absence Certification Requirement

Absence Display and Processing Rules

When you create an absence type, you can configure various aspects of the absence type, such as processing rules, and
display of various fields.

You can configure the following in the absence type setup page:

• The display of various fields and sections on the absence recording pages for specific user roles

• Rules related to entry of information into specific fields. Based on the absence pattern that you select, all fields

and rules have default values, which you can configure on the Display Features tab.

137

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

You can configure the usage of the following sections:

Primary Details Configuration
Determine whether you want to show or hide the following fields in the Supplemental Details section on the absence
recording pages:

• Reasons

• Comments

• Attachments

Balance Display on Notification Configuration
Configure absence types to display plan balance as of the absence end date in any generated notification. Select the
Display balance in approval notification check box in the General Attributes section of the absence type setup page
to display the plan balance on absence notifications. You can display plan balances only for accrual, compensatory, and
donation plans.

Assignment Selection Configuration
Configure absence types for employees with multiple assignments so that managers, administrators, and employees
can enter absences that impact either all assignments or a specific assignment. Select the Allow assignment selection
at absence entry check box in the Type Attributes tab of Create/Edit absence type page to provide this option at
absence entry.

When adding an absence, if you select an absence type from the list that has been configured to allow assignment
selection during absence entry, the Business Title field appears. This is where you can select the assignment that
you want to add an absence for. If you choose a specific assignment, the absence will impact only that particular
assignment. But if you select the option All, the absence will impact all the assignments active as of the absence start
date.

Absence Bidding Configuration
Employees can request an absence by submitting a bid with two preferred absence dates, designating one as the first
preference and the other as the second preference. The manager can approve or reject these bids, depending on the
configured rules. Only approved bids are converted into absence requests. If the line manager is the only approver, then
the approved bid becomes a scheduled absence.

To enable bidding on an absence type, you need to select the Enable bidding check box in the General Attributes
section of the absence type setup page.

Qualified Entitlement Rule
Configure this rule to show or hide the Qualified Entitlements section on the absence recording pages for qualification
plans. When workers schedule an absence related to a qualification absence plan, the Qualified Entitlements section
displays payment percentages that apply during the absence period.

Approval and Processing Rules
Configure rules related to absence approvals and processing that are available to specific roles in the approval page.

138

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

Insufficient Balance Enforcement Rule
Configure this rule to show or hide the Projected Balances section on the absence recording pages. When workers
schedule an absence related to an accrual absence plan, an error message prevents workers from adding an absence if
there is insufficient accrual balance.

Dates and Duration Configuration
Control the processing and display of the date-related fields that appear on the absence recording pages. This section
covers the dates that are captured, calculated, and evaluated. The fields vary significantly by absence pattern.

Supplemental Details Configuration
Control the display of additional fields that collect additional information and support absence processing. The fields
vary based on the pattern selected.

Related Topics

• Examples of Start Date Validation Rule

• Absence Dates and Duration Rules

• Absence Approval and Processing Rules

• Options to Configure Display of Supplemental Details

Absence Approval and Processing Rules

When you create an absence type, you can configure the absence approval and processing rules.

The following table explains the absence approvals and processing rules:

Rule

Effect of Enabling

Approval processing

All absence submissions must be approved.

Approvals reset on update

When you update an already scheduled absence, it resets approvals and goes through manager
approval again. For example, the status changes from Scheduled to Awaiting approval.

Deferred processing

An absence that you schedule doesn't have any impact on accrual balance or entitlements until you
confirm the absence. You must run the Evaluate Absences process to confirm deferred absences.

Additional payload attribute

Helps you configure the absence approval flow according to your organization needs. This allows more
flexibility in routing approvals within your organization.

Concurrency

Enable workers to receive concurrent entitlements through different absence types for absences
scheduled for the same time and day.

139

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

Rule

Effect of Enabling

Payable after termination

Enable workers to receive qualification entitlements even after termination. For example, in some
legislations even though employment may end, the absence entitlement for maternity or adoption
leave may continue to be paid.

Absence Dates and Duration Rules

When you create an absence type, you can configure the processing and display of various date-related fields that
appear on the absence recording pages.

You can configure the following date-related fields:

• Absence start date: Configure this field to display the absence start date.

• Planned absence start date: Configure this field to determine the planned start date for an absence.

• Planned absence end date: Configure this field to determine the planned end date for an absence.

• Absence end date: Configure this field to display the absence end date.

• Occurrence limit rule: Configure this rule to set a limit on the duration and occurrence of an absence type.

• Open ended: Configure this rule to enable workers to submit an absence without entering an absence end date.

• Absence start date validation: For accrual plans, configure this rule to determine dates when workers can't
schedule an absence. For qualification plans, configure this rule to determine a specific date, based on the
absence start date, to process entitlements for the absence that the worker submitted.

• Advanced absence entry: This rule enables the Advanced mode option so that workers can schedule

discontinuous dates, a weekly recurring absence, or a half day absence.

• Override Daily Duration: This rule enables workers to override the start and end time of a particular day on

which they were absent.

• Matching date: For qualification plans, configure this rule to determine the date a child is matched with the

worker for adoption purposes. When the child is from another country, it's usually the date the child enters the
prospective parent's country. This field is applicable only when you select Placement as the event type.

• Expected date of event: Configure this field to determine the expected date of childbirth or adoption.

• Expected week of event: Configure this field to determine the expected week of childbirth or adoption.

• Actual date of event: Configure this field to enter the actual date of childbirth or adoption.

•

Intend not to return to work: Configure this rule for qualification plans where the worker doesn't intend to
return to work after the maternity absence.

Related Topics

• Examples of Start Date Validation Rule

140

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

Allow Daily Absence Duration Override

Use the Override Daily Duration rule to configure an absence type when the workers work variable hours and the
employer doesn't want to change the work schedule.

Configure an absence type that uses hours as the unit of measure to override the start and end time of a particular
absent day. A work schedule determines the times when a worker is available and unavailable for work based on the
defined daily working hours for the worker. So when the worker schedules an absence, the defined daily working hours
appear automatically on the absence request page. The Override daily duration rule enables the worker to modify the
defined daily duration to more than the availability hours when scheduling an absence.

Note:  If the employer changes the work schedule, and an absence is recorded with the same absence type that has
the override daily duration rule enabled, the duration of the absence doesn't change.

Here's how you enable the Override daily duration rule:

In the Absences work area Tasks panel tab, click Absence Types.
In the Search Results section, click Create to open the Create Absence Type dialog box.

1.
2.
3. Select the pattern.
4. Click Continue to open the Create Absence Type page.
5.
6. Select the legislative data group.
7. Select the Display Features tab.
8.
9. Click Save and Close to return to the Absence Types page.

In the Type Attributes tab, enter the name.

In the Dates and Duration section Override daily duration row, select Enabled.

Workers use the advanced absence entry page to override the automatically calculated absence duration.

Options to Configure Display of Supplemental Details

When you create an absence type, you can control the display of the following fields that appear in the Supplemental
Absence Details section on the absence recording pages:

• Authorized absence: Provides notification of an authorized absence.

• Authorization status updated: Determines the authorization status for an absence based on the certification

update.

• Block leave status: Enables workers to report a fixed period away from work deducted from the worker's

normal annual leave entitlement. For example, in financial organizations depending on the nature of work,
certain workers are required to take a block of leave every year so that finance watchdog organizations can
audit the financial transactions for any inconsistencies.

• Notification date: Determines the absence notification date.

• Late notification waiver date: Determines the waiver date when an absence notification qualifies as a late

notification.

• Late notification waived: Determines when an absence notification that qualifies as a late notification is

waived.

141

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

• Special conditions: Enables workers to select any special conditions relevant for the absence type. This field

appears when you select the Illness or injury or Childbirth pattern.

Examples of Start Date Validation Rule

The examples in this topic show you how to use the absence start date validation rule to restrict accrual plan related
absence entries to particular dates.

Use this rule rule to determine the date when you want to process entitlement calculations for a qualification plan
related absence. You configure the absence start date validation rule in the Display Features tab when you create or edit
an absence type.

Configuring the Rule for Accrual Plan Absences Using Two Conditions
Scenario:

• You want to enable workers to schedule an absence only if the absence start date is two days later than or equal

to the current date.

• You also want another condition that prevents workers from scheduling an absence too far in advance. You

want workers to schedule an absence only up to three months from the current date.

You configure the first condition of the absence start date validation rule with the following information.

Field

Value

Operation type

> (earlier than)

Reference date

System date

Operand

Time period

UOM

+

2

Calendar days

You configure the second condition of the absence start date validation rule with the following information.

Field

Value

Operation type

> (later than)

Reference date

System date

Operand

+

142

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

Field

Time period

UOM

Value

3

Months

Configuring the Rule for Qualification Plan Absences Using a Single
Condition
Scenario: You have defined a qualification plan for workers to schedule maternity absences. Although you want to
enable workers to submit the absence, you want to defer processing entitlements until thirty days after the absence
entry date.

You configure the absence start date validation rule with the following information.

Field

Operation type

Value

= (equal to)

Reference date

System date

Operand

Time period

UOM

+

30

Days

How HCM Assignment Security Works With Absences
Impacting Multiple Assignments

You can use the HCM assignment security feature to determine who gets access to the absence information of a worker
enrolled in multiple assignments.

You can decide whether managers or administrators get access to all the absence information of the employee, or
have restricted access to only the absence information pertaining to a specific assignment of the employee. HCM
Assignment Security impacts the usage of various aspects of absence components.

Plan Balances

143

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

When HCM Assignment Security Is
Disabled

When HCM Assignment Security Is Enabled

Managers can:

Managers can:

•

.View all the employee's assignments,
 during person search.

• View plan balances of enrollments of
all the employee's assignments.

• View only those employee assignments that they have access to, during person search.

•

.View plan balances of enrollments of only those employee assignments that they can access.

Administrators can:

Administrators can:

• View all the employee's assignments,

• View only those employee assignments that they have access to, during person search.

 during person search.

• View plan balances of enrollments of only the employee assignment that was selected in person

• View plan balances of all enrollments.

search.

• Do plan actions like transfer and

• Do plan actions like transfer and adjust balance on the enrollments of only the employee

adjust balance on any enrollment of
the employee.

assignment that was selected in person search.

Plan Balances Using REST

When HCM Assignment Security Is
Disabled

When HCM Assignment Security Is Enabled

Managers and administrators can
use resources to return plan balances
of enrollments of all the employee's
assignments.

Managers and administrators can use resources to return plan balances of enrollments of only those
assignments that they can access.

Disbursements and Donations

When HCM Assignment Security Is
Disabled

When HCM Assignment Security Is Enabled

Managers and administrators can:

Managers and administrators can:

•

•

•

.View all the employee's assignments,
 during person search

.View disbursements and donations
made from plans enrolled to any
assignment of the employee.

Initiate disbursement or donation
on behalf of the employee from
enrollments of any assignment of the
employee.

• View only those employee assignments that they have access to, during person search.

• View disbursements and donations made from plans enrolled to an employee assignment that

they have access to.

• View disbursements and donations made from plans enrolled to an employee assignment that

they have access to.

144

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

Absences Self-Service Pages, Administrator Page and Absences REST

When HCM Assignment Security Is
Disabled

When HCM Assignment Security Is Disabled

Managers and administrators can:

Managers and administrators can:

• View all the employee's assignments,

• View only those employee assignments that they have access to, during person search.

 during person search.

• Access all absences entered at the person-level which means that either assignment selection at

• View all the employee's assignments,

absence entry isn't enabled, or the absence was entered for "all" employee assignments.

 during person search.

• Create absences that impact any or
all the assignments of the employee
active as of the absence start date,
 depending on the absence type
configuration.

• Create absences that impact any or
all the assignments of the employee
active as of the absence start date,
 depending on the absence type
configuration.

• View absences entered for a specific employee assignment only if they have authority to access

that assignment.

• Enter absences for a specific employee assignment, only if they have authority to access that

assignment.

• View all absence certifications linked to a person-level absence. They can also View absence
certifications linked to an assignment-level absence, if they have access to the employee
assignment for which the absence was entered.

• View all qualification plan entitlements and entitlement agreements if they have access to the

person, as these are always at person level.

How You Configure Absence Types to Prevent Absences
From Impacting Multiple Assignments

You can use the Allow assignment selection at absence entry and Allow only one assignment per absence check
boxes to configure an absence type to ensure that all absences using that type will need to be entered for a specific
assignment.

You can use these check boxes in the absence type setup page's Multiple Assignment Rules section to ensure that:

• When you select both these check boxes, workers can only enter absences for specific assignments in the self-
service page. If the worker has only one assignment, or the manager has access to only one assignment, then
they can only select that assignment. If HCM Assignment Security is enabled, then the managers can see only
those assignments of the employee that they have access to in the Business Title. Similarly, on the absence
entry page available to the administrator, the assignment drop-down list displays only those assignments that
the administrator can enter an absence for. Workers can enter an absence only after they select an assignment.

• When you select only the Allow assignment selection at absence entry check box, workers can enter

absences for only a specific assignment or for all the assignments. When the employee or manager selects
the All option, the absence impacts all the assignments of the employee. Similarly, administrators can choose
to select a specific assignment or All option from the assignment drop-down list on the absence entry page
available to them.

If you don't select either of these check boxes, the application will continue its default behavior and won't allow the
entry of absences for specific assignments.

145

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

How You Configure Plans to Offer Concurrent
Entitlement

You define concurrent absence plans to ensure that workers receive payments from multiple plans simultaneously
during the absence period. Use the example in this topic to understand how to indicate plans that must offer concurrent
entitlement.

Statutory Plans and Occupational Plans
In accordance with government-mandated rules of your country, you want to enable workers going on maternity leave
to receive simultaneous payments from:

• A statutory qualification absence plan

• An occupational maternity absence plan

The occupational maternity plan contains rules defined by your enterprise that entitle workers to payment in addition to
the statutory payment rules.

When you create the statutory plan and the occupational plan, you must: select the Enable concurrent entitlement
check box in the Plan Attributes tab for both the plans.

1. Select the Enable concurrent entitlement check box in the Plan Attributes tab for both plans.
2. Associate these plans with the maternity absence type when you create that absence type.

Examples of Prioritizing Absence Plans for an Absence
Type

You prioritize absence plans associated with the absence type to determine the order in which the plans must process
accrual balances and entitlements. These examples show how to prioritize plans according to your requirement.

Prioritizing Multiple Accrual Plans
Scenario: You want to enable workers to use vacation time from two accrual absence plans. When workers exhaust time
from one plan, they must be able to use time from the other plan.

When you associate each of these plans with the absence type:

• Set a higher priority to the absence plan whose accrual balance workers must use first.

• Set a lower priority to the absence plan whose balance workers must use after they exhaust the other plan's

balance.

146

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

Prioritizing Multiple Qualification Plans
Scenario: In accordance with statutory rules, you want workers on long-term sickness absence to receive payments from
two plans in this sequence:

• Payments from a statutory plan

• Payments from an occupational sickness plan

When you configure the plans:

• Set a higher priority to the statutory plan so that workers are paid from that plan first.

• Set a lower priority to the occupational sickness plan so that payment rules in that plan are processed after the

statutory plan.

Examples of Configuring a Concurrent Absence Type

This example shows how you can configure the concurrency rule so that a worker can record a concurrent absence for
the same time period through multiple absence types. You configure the concurrency rule in the Display Features tab
when you create an absence type.

Configuring the Concurrency Rule for an Absence Type
Scenario: A worker falls ill during a vacation period. You want to enable the worker to record a sickness absence for
some dates overlapping with the vacation dates.

To ensure the worker can record a concurrent sickness absence, you must enable concurrency in the Display Features
tab for one of the absence types. When concurrency is enabled, depending on the rules defined by the worker's
enterprise, the worker can:

• Receive sickness entitlements

• Recover vacation days for those overlapping sickness days

Stop Sending ICS Calendar Invite Files in Absence
Notifications

Here’s how you can turn off the delivery of .ics files in the absence notification:

1.

In the Setup and Maintenance work area, click Search on the Tasks panel tab, search for and open the Manage
Common Lookups task.

2. On the Manage Common Lookups page, search for and open the ANC_PROC_CONFIGS lookup.
3. Add and enable a new lookup code, ANC_NO_ICS.

4. Click Save and Close.

What to do next

147

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

If you had previously configured AbsencesApprovalTask task in BPM Worklist to disable all absence attachments in
email notification, you can now revert that change. To do so you need to first create the ANC_NO_ICS lookup code as
described above, and then follow these steps:

In the Setup and Maintenance work area, click Search on the Tasks panel tab.

1.
2. Search for and open the Define Approval Management for Human Capital Management task list.
3. Select the Manage Task Configurations for Human Capital Management from the task list.
4. Select AbsencesApprovalsTask, and click Edit task in the BPM Worklist page.
5. Click Notifications.
6. Select the Send task attachments with email notifications checkbox.
7. Click Save.

After you do this, approvers will start receiving attachments in their email for absence approvals without the calendar
invite (.ics) file.

Schedule Hierarchy Start Point Options

When employees take time off, their work schedule determines the duration of the absence. For example, if an
employee takes 2 days of absence, and is currently on a 4-hour schedule, their absence duration will be 8 hours.

When you create an absence type, you can select a starting point to indicate which level the application should start
searching for a schedule. For example, if you select Published schedule, the application starts searching at that level and
continues down until it finds the schedule or relevant work hours.

1. Published schedule
2. Work schedule
3. Assignment hours details
4. Work pattern

You select one of these starting point options on the Absence Type setup page in the Schedule Hierarchy Start Point
field located under the Type Attributes tab.

Absences uses the schedule to determine the duration only if the absence type unit of measure is Hours or Days and
there's no conversion formula defined. The schedule isn't used for other units of measure.

If the absence type is linked to an absence plan that has an Alternate Schedule Category field defined, the duration is
generated using the plan schedule.

Related Topics

• How an Individual's Schedule Is Identified

Create a Vacation Absence Type

This example shows how to create an absence type to conform to a specific leave policy of an enterprise.

This table summarizes key decisions for this scenario.

148

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

Decisions to Consider

In This Example

What is the name of the absence type?

Vacation

The absence type must belong to which
absence pattern?

Generic absence

What unit of measure must workers use to
record an absence?

Days

What is the minimum absence duration
that workers must schedule to submit the
absence?

2 working days

Can workers schedule an absence whose
duration is less than the minimum limit?

Yes, but display a warning message before allowing users to submit the absence.

What is the maximum absence duration
that workers can schedule?

10 working days

Can workers schedule an absence whose
duration exceeds the maximum limit?

No. Display an error message that prevents users from submitting the absence

Can workers schedule partial-day
absences?

No

Who can update absence records after
submitting them?

Managers and workers only

Can workers record absences of this type
from a time card?

Yes

Can workers and managers use the
advanced absence entry method to record
discontinuous absence dates?

No. Only administrators can use the advanced absence entry method.

Create the vacation absence type on the Manage Absence Types page.

In this example, use this page to:

• Specify who can update absences of this type

• Set maximum and minimum duration limits

• Enable the advanced absence entry function during absence scheduling

Creating an Absence Type

In the Absences work area Tasks panel tab, click Manage Absence Types.

1.
2. Click Create.

149

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

3. On the Create Absence Type dialog box, complete the fields, as shown in this table. Use default values for fields

unless the steps specify other values.

Field

Value

Legislation

Select your legislation

Pattern

Generic absence

4. Click OK.
5. On the Create Absence Type page, Type Attributes tab, complete the fields, as shown in this table. Use default

values for fields unless the steps specify other values.

Field

Name

Status

UOM

Value

Vacation

Active

Days

Legislative data group

Select your legislative data group

Minimum Duration Alert

Warning

Minimum Duration

2

Maximum Duration Alert

Error

Maximum Duration

10

Partial Day Rule

Not allowed

Enable worker updates

Select

Enable manager updates

Select

6. Click the Display Features tab.

150

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

7.

In the Dates and Duration section, complete the following fields for the Advanced Absence Entry usage rule.

Field

Value

Employees

Not enabled

Managers

Not enabled

Administrators

Enabled

8. Click Save and Close.

FAQs

Why can't I see my absence type on the absence categories page?

Ensure that the absence type is active and effective on the current date.

Why can't I see my absence plans and absence reasons on the
absence types page?

Ensure that the absence plan and absence reason are active and effective on the current date.

How can I configure an absence type to include line managers of
relevant assignments for approval?

You can configure approvers from the Absence Record Maintenance section of the Absence Type setup page.

For employees with multiple assignments, select the Manager of all relevant assignments option from the approver
list. This will send the absence approval request to all the line managers of relevant assignments

How can I create an absence category?

You can create an absence category from the Absence Categories page in the Absences work area.

151

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 13
Absence Types, Reasons, and Categories

Click Create and enter the details of the absence category like name, legislation and effective end date. You then need
to select the absence type you want to associate with the absence category in the Associated Types section. Click Save
and Close to complete the process.

How can I configure an absence type to show absence reasons?

After you create an absence reason, you need to associate it with an absence type. To do that, add the absence reason
from the Absence Reasons section of the Absence Type setup page. People can select the reason from the Reason list
during absence entry for that absence type.

152

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 14
Absence Certifications

14  Absence Certifications

Options for Absence Certification Requirements

Configure absence certification requirements as action items that workers must complete to continue receiving
entitlements during an absence period. Requirement components include type, trigger, and actions.

Configuring absence certification is a two-step process in the Absences work area:

1. Configure the certification requirements using the Absence Certifications task.
2. Associate the certification requirements with an absence type on the Action Items tab of the Create Absence

Type page. When workers schedule an absence, they're subject to the certification requirements.

Absence certifications are supported only for absence types with the illness or injury and maternity absence patterns.

Certification Components
When you create a certification requirement, you configure the following aspects:

• Requirement type

• Requirement trigger

• Requirement phases and actions

• Requirement status during absence recording

• Entitlement reevaluations

Related Topics

• Create an Absence Certification Requirement

Absence Certification Requirement Types

Configure the certification requirements using the Absence Certifications task.

When you create a certification requirement, you must configure the following certification requirement types:

• Classification

• Absence Record Update Rule

Classification
Select one of the following to define an absence certification requirement:

Classification

Purpose

Documentation

Track documentation related to a worker's absence.

153

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 14
Absence Certifications

Classification

Purpose

Entitlement

Update payment percentages for qualification plans.

Absence Record Update Rule
Select one of the following to define an absence certification requirement:

Absence Record Update Rule

Description

Authorization

Select this rule if workers must complete an action item to receive entitlements.

For example, you can mandate workers to submit certain medical reports and other documents to
continue to receive entitlements for the absence period.

Timeliness

Select this rule to define the actions to take depending on when workers notify their managers about
their absence.

For example, you might want to revise entitlements for workers who have provided a late notification
of their absence.

Other

Select this rule if you want to consider other special requirements.

For example, you can define a certification requirement that HR specialists can initiate at any time to
retract absence entitlements for a worker whose employment ends.

Options to Trigger Certification Requirements

When you create an absence certification requirement, you must configure the certification requirement rules to
determine when the certification requirement takes effect.

Certification Requirement Trigger
Use one of the following rules to determine when the certification requirement takes effect:

Rule

On demand

Description

HR specialists add the certification requirement as an action item when they record an absence for a
worker on the Manage Absence Records and Entitlements page.

On the absence start date

The certification requirement appears as an action item in the Edit Absence dialog box on the Manage
Absence Records and Entitlements page.

154

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 14
Absence Certifications

HR specialists can set the status of the action item when the worker provides the required documents or other
information.

Options to Manage Actions For Certification Events

When a worker schedules an absence that's subject to a certification requirement, decide what actions to take in each of
the following phases of the requirement:

Phase

On creation

Description

When the certification requirement takes effect. Sometimes, your certification requirement might not
require any action from the worker to complete it.

For example, you might want to retract entitlements from a terminated worker when there is no further
action required from the worker. In that case, you can configure the certification requirement to
complete automatically when it becomes effective.

On passage of due date

When the certification requirement is past its due date.

On completion

When HR specialists evaluate the action item corresponding to the certification requirement and mark
it complete.

For each phase, you can perform the following actions:

• Set the certification status that appears during absence recording.

• Reevaluate entitlements.

Certification Status during Absence Recording
When you create an authorization requirement or a timeliness requirement, a corresponding Update Status field, known
as the target field appears in the Actions section. The following table shows the specific status field on the absence
recording page for each requirement type:

Requirement Type

Target Status Field

Authorization requirement

Primary Certification Authorized

Timeliness requirement

Late Notification Override

In the Actions section of page, you specify the update status value in the target field for each phase of the requirement.
For example, you can configure the target field on the absence recording page to display True when a worker provides
the required documents to complete a certification requirement.

155

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 14
Absence Certifications

Entitlement Reevaluations
Depending on the status of the certification requirement, you can reevaluate entitlements that a worker receives during
the absence period. Reevaluate entitlements as of the absence start date or the action date.

For example, you can change the worker's entitlement to half pay as of the absence start date when a certification
requirement has passed its due date. When the worker completes the requirement, you can recalculate the entitlements
from the absence start date or the completion date.

Use any of these rules to calculate entitlements:

Rule

Override

Description

Enables entry of a revised payment percentage that overrides the absence plan payment rules.

Recalculate

Calculates payments according to the absence plan payment rules.

Retract

Stops payments.

Related Topics

• Create an Absence Certification Requirement

Create an Absence Certification Requirement

This example contains steps to create an absence certification requirement for workers on long term sickness leave. The
following table summarizes key decisions for this scenario.

Decisions to Consider

In This Example

What action do you want workers to take
to complete the certification requirement?

What action do you want to take if workers
don't complete the requirement within the
stipulated time?

Submit a doctor's certificate to the manager within 14 calendar days of their absence start date.

Revise entitlement for the rest of the absence period to 75 percent of pay.

When do you want the certification
requirement to take effect?

On the absence start date

How do you want to configure the value of
the Primary Certification Authorized field
during absence recording?

Set status to True when the:

• Certification requirement initiates on the absence start date

• Worker completes the certification requirement

156

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 14
Absence Certifications

Decisions to Consider

In This Example

Set status to False when the due date of the certification requirement passes.

Creating a Certification Requirement

In the Absences work area Tasks panel tab, click Absence Certifications.

1.
2. Click Create.
3. On the Create Absence Certification page, complete the fields, as shown in this table.

Field

Name

Type

Status

Trigger

Value

Doctor's Certificate

Authorization

Active

On initial absence entry

Due Date Rule

Waiting period

Waiting Period Start Date

Absence start date

Duration

14

UOM

Calendar days

Classification

Entitlement

4.
5.

In the On Creation section, set the Target Field Update status to True.
In the On Passage of Due Date section, complete the fields, as shown in this table.

Field

Target Field Update

Value

False

Entitlement Reevaluation Rule

As of action date

Entitlement Update Rule

Override

157

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 14
Absence Certifications

Field

Value

Revised Payment Percentage

75

In the On Completion section, set the Target Field Update status to True.

6.
7. Click Save and Close.

158

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 15
Absence Processes

15  Absence Processes

Overview of Absence Processes

Use the Schedule and Monitor Absence Processes task in the Absences work area to run the following absence
processes:

Process Name

Purpose

When is the Process Run

Evaluate Absences

Calculates entitlements for unprocessed
absences based on absence plan rules

Automatically, when a user submits an absence,
 or under special conditions, such as:

• When you need to extend an open-ended

absence by 90 days

• When a work schedule changes and you
need to recalculate absence duration and
plan deductions

Evaluate Certification Updates

Checks whether certification requirements for
multiple employees are past their due dates

Administrators typically run this process daily to
check if certifications are overdue.

You run this process only if you use
certifications with due dates.

Update Accrual Plan Enrollments

Updates enrollments based on the new hire and
transfer events for multiple employees

Administrators typically run this process
daily to determine plan eligibility for multiple
employees.

Calculate Accruals and Balances

Calculates the accrual balances for multiple
employees under an accrual absence plan

Administrators typically run this process at
regular intervals. You can also run the process
for individual enrollments.

Withdraw Accruals and Balances

Withdraws accruals or deletes enrollments in
bulk for several employees

Generate Daily Breakdown of Absence Details

Generates the daily breakdown of absences
for absence. The included absences are for
absence types with Include in daily report
breakdown selected on the create or edit
absence type pages, Action Items tab

Administrators typically run this process when
there is an error in calculation or the dates and
they want to roll back the accrual balances to
correct the error.

Administrators typically run this process to view
the daily absence breakdown in the Absence
Calendar Real Time Entry Report.

159

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 15
Absence Processes

Related Topics

• Options for the Calculate Accruals and Balances Process

• Options for the Update Accrual Plan Enrollments Process

• Options for the Evaluate Absences Process

• Options for the Evaluate Certification Updates Process

Options for the Evaluate Absences Process

You calculate entitlements for unprocessed absences using the Evaluate Absences process in the Absences work area.
Use this process to evaluate absences marked for deferred processing and reevaluate absences that meet the process
parameters.

This process runs automatically when you submit an absence. To defer the process, select the rule Deferred processing
on initial entry in the Display Features tab of the Create Absence Type page.

Process Parameters
Use combinations of these parameters to control which person records are processed:

Parameter Name

Description

Effective Date

Evaluates and updates absence records that are effective on the specified date

This is a required parameter.

Person

Includes absences for only the specified person

When you select a person record, the Scheduled Absences parameter appears.

Scheduled Absences

Includes a particular future-scheduled absence for the selected employee

This parameter appears only when you select an employee in the Person parameter.

Business Unit

Includes employees in the selected business unit

Legal Employer

Includes employees assigned to the selected legal employer

Person Selection Rule

Includes specific employees identified by the person selection rule

You can use the Person Selection formula type to include specific employees who meet special
requirements for the absences batch process. You define the formula using the Manage Fast
Formulas task and select that formula in the Person Selection Rule field.

Payroll

Includes employees assigned to the selected payroll

160

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 15
Absence Processes

Parameter Name

Description

Legislative Data Group

Includes a group of one or more absence types that are associated with the legislative group that you
select

Work Schedule Rule

Includes employees assigned to a particular work schedule

Record Selection

Decides which absence records are selected for processing:

• Evaluate All Absences: Reprocesses all absence records that meet the other filtering options for

the process

• Evaluate Only Duration Changes: Reprocesses the absence records only if there is a change in

absence duration

• Evaluate Only Deferred Absences: Reprocesses deferred absences

• Evaluate Only Open-ended Absences: Reprocesses open-ended absences that require an

extension

Related Topics

• View Status and Other Details for Scheduled Processes

• Statuses of Scheduled Processes

Options for the Evaluate Certification Updates Process

You can check if certification requirements for multiple employees are past their due dates using the Evaluate
Certification Updates process in the Absences work area.

When a requirement is past the due date, the process updates the absence records and entitlements. You typically run
this process daily to check if certifications are overdue.

You run this process only when absence types have certification requirements and those requirements include actions
to take after due dates have passed. For example, you want to change the employee's entitlement to half pay as
of the absence start date when a certification requirement passes its due date. When the employee completes the
requirement, you can recalculate the entitlements from the absence start date or the completion date.

Process Parameters
Use combinations of these parameters to control which person records are processed:

Parameter

Description

Effective Date

Evaluates and updates certification requirements that are effective on the specified date

This is a required parameter.

Person

Includes absences for only the specified person

161

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 15
Absence Processes

Parameter

Business Unit

Description

Includes employees in the selected business unit

Legal Employer

Includes employees assigned to the selected legal employer

Person Selection Rule

Includes specific employees identified by the person selection rule

You can use the Person Selection formula type to include specific employees who meet special
requirements for the absences batch process. You define the formula using the Manage Fast
Formulas task and select that formula in the Person Selection Rule field.

Related Topics

• View Status and Other Details for Scheduled Processes

• Statuses of Scheduled Processes

Options for the Update Accrual Plan Enrollments Process

Update enrollments such as new hire, termination, and transfer events for multiple employees using the Update
Accrual Plan Enrollments process in the Absences work area. You typically run this process daily to determine plan
eligibility, and update plan enrollments and terminations for multiple employees.

Process Parameters
Use combinations of these parameters to control which person records are processed:

Parameter

Description

Effective Date

Evaluates and updates plan enrollments that are effective on the specified date

This is a required parameter.

Person

Includes absences for only the specified person

Business Unit

Includes employees in the selected business unit

Legal Employer

Includes employees assigned to the selected legal employer

Person Selection Rule

Includes specific employees identified by the person selection rule

You can use the Person Selection formula type to include specific employees who meet special
requirements for the absences batch process. You define the formula using the Manage Fast
Formulas task and select that formula in the Person Selection Rule field.

162

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 15
Absence Processes

Parameter

Description

Absence Plan

Processes enrollments for only the selected accrual plan

If you don't select an absence plan, you must select at least one of these parameters:

• Person

• Business Unit

• Legal Employer

• Person Selection Rule

The process updates accrual plan enrollments for each employee identified by the other parameters.

Plan Category

Includes a specific category, such as balance transfers

Changes since last run

Includes employees with changes, such as assignment updates or corrections since the last process
run

Payroll

Includes employees assigned to the selected payroll

Legislative Data Group

Includes only the absence types associated with the selected legislative data group

If you want to automatically enroll employees to corresponding accrual plans based on their legislative
data group, you need to define the following lookup type and lookup code:

• Lookup Type: ANC_PROC_CONFIGS

• Lookup Code: ENROLLMENT_PROCESS_LDG

So when you run the process, the application automatically enrolls employees to eligible absence
accrual plans associated with the legislative data group, even if you don't select this field.

Related Topics

• View Status and Other Details for Scheduled Processes

• Statuses of Scheduled Processes

Options for the Calculate Accruals and Balances Process

You can calculate accrual balances and update plan balances for multiple employees using the Calculate Accruals and
Balances process in the Absences work area. You typically run this process at regular intervals, such as daily or weekly.

You can also run the process for individual enrollments. The process transfers accrual balance data to Oracle Fusion
Global Payroll if the Transfer absence payment information for payroll processing option is selected for the absence
plan.

163

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 15
Absence Processes

Note:  If you run the Calculate Accruals and Balances process after deleting a person's enrollment into an accrual plan
and re-enrolling them into the same plan, the application won't display the absence information in the Plan Balances
region. You'll need to run the Evaluate Absence process to bring the absence information over.

Process Parameters
Use combinations of these parameters to control which person records are processed:

Parameter

Description

Effective Date

Calculates the accrual balance for only those plans that are effective on the specified date

This is a required parameter. You can select a past, current, or future date. The process only runs if a
plan enrollment exists for the employee on the effective date.

•

•

If you don't select an absence plan with this parameter, the process calculates the accrual balance
for multiple plans with differing accrual periods on the effective date.

If you select an absence plan, the process calculates the accrual balance for the accrual period of
the selected plan on the effective date.

Person

Includes absences for only the specified person

•

•

If you select a person but not an absence plan, the process calculates the accrual balance for all
plans in which the employee is actively enrolled in.

If you select a person and an absence plan, the process calculates the accrual balance for only the
selected plan, if the employee is actively enrolled in the plan.

Business Unit

Includes employees in the selected business unit

Legal Employer

Includes employees assigned to the selected legal employer

Person Selection Rule

Includes specific employees identified by the person selection rule

You can use the Person Selection formula type to include specific employees who meet special
requirements for the absences batch process. You define the formula using the Manage Fast
Formulas task and select that formula in the Person Selection Rule field.

Payroll

Includes employees assigned to the selected payroll

Payroll Relationship Group

Includes employees assigned to the selected payroll relationship group

You can define payroll relationship groups for a group of people in a single payroll or in multiple
payrolls.

Changes Since Last Run

Includes employees with either payroll or assignment updates or corrections since the last process run

If you select:

• Payroll events since last run: The process calculates the accrual balance for employees whose

payroll records have changed since the last scheduled run.

For example, an employee schedules five days off on January 25 and you run the process on
January 26. Due to an emergency, the employee returns to work on January 29, after being off

164

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 15
Absence Processes

Parameter

Description

just four days. The employee updates the absence record to reflect four days off instead of five.
If you schedule the process again on February 1 and select Payroll events since last run, it
generates the updated accrual balance for the employee.

• HR Assignment changes since last run: The process calculates the accrual balance for
employees whose assignment record last updated date is after the last scheduled run.

For example, the last scheduled run was on January 1 and you update an employee's assignment
on January 2. If you schedule the process again on January 3 and select HR Assignment
changes since last run, it generates the updated accrual balance for the employee.

Legislative Data Group

Includes only the absence types associated with the selected legislative data group

Absence Plan

Calculates accrual balances for only the selected accrual plan

When you select this option, the Repeating Period option appears.

If you don't select an absence plan, you must select at least one of these parameters

• Legislation

• Business Unit

• Legal Employer

• Person Selection Rule

• Person

• Payroll

• Payroll Relationship Group

• Changes Only

The process calculates accrual balances for each employee identified by the other parameters.

Repeating Period

Includes the selected accrual period for the selected plan

This option appears only when you select a value in the Absence Plan option.

Related Topics

• View Status and Other Details for Scheduled Processes

• Statuses of Scheduled Processes

Options for the Withdraw Accruals and Balances Process

You withdraw and update employee accrual balances and delete enrollments using the Withdraw Accruals and
Balances process. Run this process using the Schedule and Monitor Absence Processes task in the Absences work area.

You typically run this process to correct existing accrual data. You can also run the process for individual enrollments.

165

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 15
Absence Processes

Process Parameters
Use combinations of these parameters to control which person records are processed:

Parameter

Effective Date

Description

Withdraws the accrual balance or deletes enrollments for only those plans that are effective on the
specified date

This is a required parameter. You can select a past, current, or future date as the effective date.

Processing Option

Withdraws accrual balances or deletes enrollments

This is a required parameter.

Person

Includes absences for only the specified person

Legal Employer

Includes employees assigned to the selected legal employer

Person Selection Rule

Includes employees identified by the person selection rule

You can use the Person Selection formula type to include specific employees who meet special
requirements for the absences batch process. You define the formula using the Manage Fast
Formulas task and select that formula in the Person Selection Rule field.

Payroll

Includes employees assigned to the selected payroll

Payroll Relationship Group

Includes employees assigned to the selected payroll relationship group

You can define payroll relationship groups for a group of people in a single payroll or in multiple
payrolls.

Legislative Data Group

Includes only the absence types associated with the selected legislative data group

Absence Plan

Withdraws accrual balance or deletes enrollments for the selected accrual plan

Generate Daily Breakdown of Absence Details Process

You can view the absence details of employees on the absence calendar by generating the daily breakdown of absences
using the Generate Daily Breakdown of Absence Details process.

The absences that are processed belong to absence types that were configured to be included in the process. Use the
Include in daily report breakdown check box that's available in the Action Items tab of the absence type setup page
to configure the absence types for it. Run this process using the Schedule and Monitor Absence Processes task in the
Absences work area. View the results in the Absence Calendar Real Time Entry Report.

166

Oracle Fusion Cloud Human Resources
Implementing Absence Management

How You Run the Process
You can run this process in two ways.

Chapter 15
Absence Processes

• When you run the job by passing the absence start and end dates as input parameters, the process will consider
all absences that fall within that period for processing. The process ignores the effective date parameter in this
case.

• When you run the job without passing the absence start and end dates, and if it's the first time you're running

this job, the process will consider all absences that were created or updated on the effective date for processing.
On subsequent runs, the process will consider only those absences that were created or updated after the
previous run.

Note:  When you schedule the absence process to run at a specific time, the application uses this specified time
to calculate the effective date. For example, let's assume that you schedule the absence process to repeat every
ten minutes starting at 21:30 from 26 May to 14 June. Now this would mean that the absence process would still
be active on the morning of 15 June because the application considers it 14 June until the time 21:29. To avoid such
discrepancies, you need to ensure that your schedule starts at 00:00.

Ways to Control Which Absences are Processed
There are two ways to control which absences are included in the process:

• Configure the absence type to include or exclude absences.

• Add more parameters to the job, like person and business unit to process only those absences that meet all the

criteria you have specified.

You can schedule the job to run as often as required. The more often you run, the more up-do-date information will be
available to your manager when they check the Absence Calendar. Any new absences or changes to existing absences
that are made after running the job are synced up only in the subsequent run.

Process Parameters
Use combinations of these parameters to control which person records are processed:

Parameter

Description

Effective Date

Generates daily breakdown of absences for absence types that are effective on the specified date.

This is a required parameter.

Absence Start Date

Absence End Date

Includes absences whose start date falls on or after this specific date. If you enter this date, the process
ignores the Effective Date parameter.

Includes absences whose end date falls on or before this specific date. If you enter this date, the
process ignores the Effective Date parameter.

Person

Includes absences for only the specified person.

If you select a person but not an absence type, the process generates the daily breakdown of absences
meeting the eligibility criteria

167

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 15
Absence Processes

Parameter

Description

If you select a person and an absence type, the process generates the daily breakdown of absences for
only the selected absence type.

Business Unit

Includes employees in the selected business unit

Legal Employer

Includes employees assigned to the selected legal employer

Payroll

Includes employees assigned to the selected payroll

Legislative Data Group

Includes only the absence types associated with the selected legislative data group

Absence Type

Generates the daily breakdown for only the selected absence type

Create Event Processing Rules to Reprocess Absences

You can use HCM Events to configure absence types to automatically reprocess absences when an employee’s work
pattern or work schedule changes across HCM. This eliminates the need to schedule multiple absence processes to
manage such reprocessing across absences.

Create Event Condition
Here’s how:

In the My Client Groups tab, click the HCM Experience Design Studio quick action.

1.
2. Click the Event Conditions tab.
3. Click Add.
4. Enter the necessary details of the event. Based on your requirement, specify the entity as Work Pattern

Assignment, Work Pattern Break, or Work Pattern Shift. In the Condition Details section, enter the specific
details of the conditions of the event in which it will be triggered. You need to enter the details for how a
particular data changes from old to new.

5. Click Save and Close.

Configure Absence Type
Specify which absence types track that event and what needs to happen when that event is detected. Here’s how you
configure the absence type to respond to the event::

1. Click the newly added Additional Details tab in the absence type setup page.
2.
3.

In the Event Processing section, click Select and Add.
In the Select and Add Event Processing Rule window, select the event from the Event You can configure how an
absence plan responds when this event occurs by selecting an option from the Response option.

4. Click OK, then Save and Close.

168

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 15
Absence Processes

When you're done setting up the absence types, you can use the Process Events absence process to process all events.
You can find this process in the Schedule and Monitor Absence Processes page.

169

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 15
Absence Processes

170

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 16
Integrated Workbooks for Loading Absence Data

16  Integrated Workbooks for Loading Absence
Data

Integrated Workbooks for Absence Management

Use integrated Microsoft Excel workbooks to upload multiple records at one time for various Absence objects, such as:

• Absence records

• Absence plans

• Absence types

• Absence categories

• Absence reasons

• Absence certifications

Use the Initiate Spreadsheet Load task of the Data Exchange work area to use the absence spreadsheets.

All Absence Spreadsheets
You can only create absence business objects using the spreadsheets. You can't edit existing absence objects.

Absence Records Spreadsheet
You can create and load absence records only for the Generic absence and the Illness or injury pattern. You can't load
absence records for absence types with the Childbirth or placement pattern.

Absence Plans Spreadsheet
Consider the following points when you enter data in the spreadsheet:

• You must enter the start month and start date to define the plan term.

• You can associate only one eligibility profile with an absence plan.

• You can create only one accrual band for an accrual plan.

• You can associate only one qualification band and only one band detail with a qualification plan.

• When you enter adjustment reasons, you must enter their corresponding codes separated by commas.

• When you associate a rate definition with an absence plan, you must enter the corresponding rate definition ID.

Absence Types Spreadsheet
Consider the following points when you enter data in the spreadsheet:

• You must enter the legislative data group ID.

• You can associate a maximum of five absence plans with an absence type.

• You can associate a maximum of five absence certifications with an absence type.

171

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 16
Integrated Workbooks for Loading Absence Data

• Feature usages and rules for the absence type automatically upload with default values based on the absence

pattern that you enter.

• When you enter special conditions for a qualification plan, you must enter the corresponding condition codes

separated by commas.

Absence Categories Spreadsheet
You can associate a maximum of five absence types with an absence category.

Related Topics

• Update Absence Data Using HCM Spreadsheet Data Loader

Update Absence Data Using HCM Spreadsheet Data
Loader

You can use the Data Exchange work area to create absence data using spreadsheets and upload to Oracle Fusion
Absence Management using the HCM Spreadsheet Data Loader.

You can use the HCM Spreadsheet Data Loader to load the following business objects into spreadsheets:

• Absence Entry

• Absence Reason

• Absence Certification

• Absence Category

• Absence Accrual Plan Enrollment

• Absence Accrual Balance Component

• Absence Qualification Plan Entitlement

You can create, update and delete all the entities mentioned above.

Related Topics

• Generate Spreadsheets

•

Import Data to a Spreadsheet

• Manage Spreadsheet Data Sets

• Upload Data Using HCM Spreadsheet Data Loader

• How You Delete Data Using HCM Spreadsheet Data Loader

Set Up Desktop Integration for Excel

You can create or edit records and upload them to the application using integrated Excel workbooks. To use these
workbooks, you must install an Excel add-in.

172

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 16
Integrated Workbooks for Loading Absence Data

Note:  Every release of Oracle Fusion Cloud Applications is likely to have a new version of the Oracle ADF Desktop
Integration add-in. When prompted, install the latest version of the add-in.

•

•

For information on the new version, see the relevant What’s New document.

For information on the upgrade policy for the Oracle ADF Desktop Integration add-in, see: Add-In Upgrade
Policy for ADF Desktop Integration (DOC ID 2242879.1) on My Oracle Support.

Install or Upgrade the Desktop Integration Add-In
To install or upgrade the Oracle ADF Desktop Integration Add-In for Excel, you must have the appropriate Excel and
Windows version. See: Supported Platforms for ADF Desktop Integration (DOC ID 2242428.1) on My Oracle Support. Also,
make sure that you have the Download Desktop Integrator (ATK_DOWNLOAD_DESKTOP_INTEGRATOR_PRIV) privilege
to access the add-in installer.

1. Sign into your computer with your account.
2. Close Excel.
3. Click Navigator > Tools > Download Desktop Integration to download the installer file.
4. Run the adfdi-excel-addin-installer-current-user.msi installer just like you would run any program that you

install on your computer.

5. Run Excel once to complete the installation.

Note:  If you have administrator privileges, you can also install the add-in for all users. For more information, see: How
to install the ADF Desktop Integration Add-in for Excel (DOC ID 2681794.1) on My Oracle Support.

Related Topics

• Troubleshoot Desktop Integration for Excel

• Guidelines for Using Desktop Integrated Excel Workbooks

• Business User's Guide for ADF Desktop Integration

Guidelines for Using Desktop Integrated Excel
Workbooks

Where available, you can download a desktop-integrated Microsoft Excel workbook and use it to create or edit records.
Your edits in the workbook don't affect the application until you upload the records back into the application.

What You Must Not Do
To ensure that you successfully upload your changes to the application, avoid doing these tasks:

• Rename text from the integrated workbook, such as the worksheet names.

• Add columns.

• Delete any part of the template, such as columns.

• Hide required columns and status columns or headers.

173

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 16
Integrated Workbooks for Loading Absence Data

CAUTION:  Don't close Excel using the Windows Task Manager and clicking the End task button because that might
disable the add-in.

Conventions
Some column headers in the integrated workbook might include [..]. This means that you can double-click within any
cell in the column to open a dialog box, where you can select a value to insert into that cell.

Statuses
You can use Status Viewer to see the status of the entire integrated worksheet and the status of any row in a
worksheet. To use the status viewer, click Status Viewer on the Excel ribbon. You can see the status of the entire
integrated worksheet by default. To see the status of a row, click any table row in a worksheet. You can use the
information that appears on the Status Viewer to review and correct errors at the same time.

Searches
Some integrated workbooks include searches. To search within the workbook, you must first sign into the application.
When you click the Search button, the application prompts you to sign in if you haven't already done so.

Refreshes After Upload
If your changes aren't reflected after you upload the records back into the application, you can try out these options:

• Refresh the table

• Use a filter or search on the table to see your changes

Related Topics

• Set Up Desktop Integration for Excel

• Troubleshoot Desktop Integration for Excel

• How You Use Tables

Troubleshoot Desktop Integration for Excel

If you run into any issues with the integration, use the Client Health Check tool first to find out what integration issues
you might have and how to resolve them.

For more information, see: How to use the ADF Desktop Integration Client Health Check Tool (Doc ID 2010222.1) on My
Oracle Support.

If the health check tool doesn't resolve your issue, you can uninstall and reinstall the Oracle ADF Desktop Integration
add-in. For more information, see: Information Center: Troubleshooting Oracle ADF Desktop Integration (DOC ID
2012600.2) on My Oracle Support.

Note:  To check the version of Oracle ADF Desktop Integration, see: ADFdi Version Check (Doc ID 2012570.1) on My
Oracle Support.

174

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 16
Integrated Workbooks for Loading Absence Data

Uninstall the Desktop Add-In
Use the Microsoft Windows Settings to remove the ADF Desktop Integration add-in. After removing the add-in, you can
use the integrated Excel workbooks on this system only after you reinstall the ADF Desktop Integration add-in.

1. Open Windows Settings and go to Apps & features.
2. Select Oracle ADF Desktop Integration Add-In for Excel from the list of programs.
3. Click Uninstall from the toolbar at the top of the program list.
4. When prompted, click Uninstall to remove the Oracle ADF Desktop Integration add-in.

Note:  If you have installed the Oracle ADF Desktop Integration add-in on multiple user profiles using the current-user
installer, you must remove it from each user profile.

Related Topics

• Set Up Desktop Integration for Excel

FAQ

What's the difference between Export to Excel and desktop
integration for Excel?

You use the Export to Excel button or menu option to download data from your table as a Microsoft Excel file. You can
then use this file to view or analyze your data.

You use desktop integration for Excel to create or edit records in Excel workbooks, and then upload them back into the
application. This comes in handy when you have to work offline or make mass updates. In most cases, you download
the desktop integrated workbook from a link in a panel tab or your table.

Related Topics

• Guidelines for Using Desktop Integrated Excel Workbooks

175

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 16
Integrated Workbooks for Loading Absence Data

176

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 17
HCM Extracts for Absence Data

17  HCM Extracts for Absence Data

HCM Extracts for Absence Data

Extract past and future absences and open-ended absences using the Manage Extract Definitions task in the Data
Exchange work area.

You can extract absence data based on the effective date or start date. The effective date might not always be the right
option because you can make adjustments to existing and past absences.

Consider these aspects before you create an extract definition for absence data:

• Extract type

• Data groups

Extract Type
When you create an extract definition for absence data ensure that you:

• Select HR Archive from the Extract Type list.

• Select Yes in the Display column for Start Date in the Parameters section. The Effective Date is set to Yes by

default.

Data Groups
The absence data group available is ABS_EXT_ABSENCE_ENTRY_UE. You can select it as the root data
group. If you want person information such as first name and last name to appear, then you need to create a
PER_EXT_SEC_PERSON_UE (Person) data group. The Person data group doesn't need to be the root data group.

Related Topics

• Define Extracts

Define Extracts

This example shows the steps required to create an extract definition.

Before you create an extract definition, you should understand the following details:

•

Information that you want to extract.

• Structure in which the data must be extracted.

• How you want to deliver this data (including file format, delivery mechanism, and frequency information).

FAST Bank is a global organization with subsidiaries all over the world. As part of an external business reporting
requirement, FAST Bank is required to extract the department and employee details (grouped by department) across

177

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 17
HCM Extracts for Absence Data

the entire company. This information must be sent to a third party in an XML file and to HR Managers in a PDF file using
email. The following table summarizes the key decisions in this scenario:

Decisions to Consider

In This Example

How many extracts do I create to produce
this type of report?

You create one extract definition to define a headcount report.

How many data groups do I create?

There are 2 functional groups of information, therefore you create two data groups, one for the
department and one for employees.

How many records do I create?

You decide the number of records based on the subgroup of attributes within a data group. In this
example, you create two records for the department data group:

• Department Details

• Department Summary

You create one record for the employees' data group: Employee Details.

How many attributes do I create?

You decide the number of attributes based on the specific information required for that report. Create
the following attributes for the Department Details record:

• Department Name

• Department Location

For the Department Summary record, create the following attributes:

• Record Code

• Report Date

• Employee Count

For the Employees Details record, create the following attributes:

• Full Name

• Gender

• Date of Birth

• Salary

• Bonus

• Tax Rate

Do I create any fast formulas?

You can use fast formulas at the following levels:

• Extract Criteria level to decide certain conditions.

• Extract Rule level to derive attribute values.

• Extract Advanced Condition level to specify complex conditions.

• Extract Record level to automatically generate formulas using the Generate Formula option.

Create an Extract Definition

1. On the Extract Definitions page, click Add > Create New to open the Create Extract Definition page.

178

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 17
HCM Extracts for Absence Data

2. Select HR Archive and enter 01-Jan-2000 as the Session Effective Date. The session effective date is an

effective start date that applies to all date-effective interactions in the current session.

Field Name

Entry

Name

FAST Bank Extract

Note:

The application uses this name to generate the XML output file.

Start Date

01-JAN-2010

Consumer

Undefined

Note:

Selecting Report in the Consumer field indicates that the extract is used for reporting

purposes and that the data isn't interfaced with any external applications.

Note:

The Consumer field doesn't appear for the extract type Archive Retrieval.

Additional Details

HR Manager

Note:

The Additional Details field doesn't appear for the extract type Archive Retrieval and when

you select Report in the Consumer field.

Changes Only

No

179

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 17
HCM Extracts for Absence Data

Field Name

Entry

Note:  In the Consumer field you can include the consumer name or the external application to which the
data generated by the HCM Extracts is sent to or interfaced with. Also, you can add details in the Additional
Details field to capture the names of applications or consumers. The Consumer field has a list of values. If
the application or consumer name isn't found in the list, you can provide the name in the Additional Details
field. If you've a predefined extract that can be used as a template, select it from the Source Template list.

Note:  Capturing the consumer name or the external application to which the data is interfaced provides
information related to integration patterns and requirements from customers. This information can help
Oracle identify common integration patterns and deliver predefined templates, thus simplifying the Extract
creation and definition process.

3. Enter FAST Bank Extract as the name of the extract definition. The application automatically creates the tag

name based on the extract name and uses this name to generate the XML output file.

4. Click OK. The application saves the extract definition and automatically generates the parameters based on the

type of extract. The parameters control the output of an extract.

Configure Effective Date Defaulting Rule
When extracts are scheduled, the Effective Date parameter, which is a required attribute, needs to be specified for
defaulting appropriate values. For example, running an extract daily will require passing the effective date in context to
the date on which it's run. To configure the effective date rule:

In the Define tab, go to the Parameters region and select Advanced View from the Show list.

1. Open the extract for which you want to specify the Effective Date parameter.
2.
3. Select the value from the Parameter Basis list.
4. Click Save and Close.

Rename Extract Definitions
You can rename an extract when you want to import or migrate a later version of the extract with the same name.
Renaming will help references in external applications remain unaffected, while you can update the extract with a later
version.

In the Extract Definitions page, click Actions > Copy or Rename.

1.
2. Select Rename and enter the extract name.
3. Click OK. After renaming the extract, ensure that you run a new baseline if your extract is incremental.

Related Topics

• Extract Components

• Guidelines for Delivering Extracts

• Define the BI Publisher Template in HCM Extracts

180

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 17
HCM Extracts for Absence Data

Reconcile Absences and Payroll Info

You reconcile absence entries with absence payments by extracting a data file using the Absences and Payroll Info for
Reconciliation extract and ensure that people correctly paid for their time off. Here’s how you can access this extract:
My Client Groups > Data Exchange > HCM Extracts Section > Submit Extracts. The data file includes absence hours
reported in Oracle Global Absence Management and payroll info in Oracle Fusion Global Payroll Cloud Service.

The extract includes absence entries that belong to the current payroll period. Here’s the data that is extracted:

Person and Assignment Details (first

Absence Summary (Second row)

row)

Business Unit Name

Absence Plan

Person Number

Manager Name

Absence Plan Units

Absence Plan Units Difference

Assignment Number

Absence Plan Units in Payroll

Legal Employer Name

Absence Type

Employee Name

Current Retro Indicator

Location Name

Business Title

Department Name

Retro Absence Start Date

Units of Measure

If the absence plan units difference column shows 0, it signifies that the data is reconciled. If the difference is negative, it
means that some absence data wasn't transferred to Payroll.

181

Oracle Fusion Cloud Human Resources
Implementing Absence Management

Chapter 17
HCM Extracts for Absence Data

182

