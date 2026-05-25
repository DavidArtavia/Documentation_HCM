Oracle Fusion
Cloud Human
Resources

Implementing Time and Labor

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

G34726-01

Copyright © 2011, 2025, Oracle and/or its affiliates.

Author: Lynn Raiser

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Contents

Get  Help  ................................................................................................................................    i

1 Overview

1

Overview of Implementing Time and Labor .............................................................................................................................  1

Overview of Global Human Resources ......................................................................................................................................   3

Date-Effective Objects in Scheduling and Time and Labor .................................................................................................   4

2 Setup and Maintenance Tasks

5

Time Entry Setup and Maintenance Tasks ...............................................................................................................................  5

Time Processing Setup and Maintenance Tasks .....................................................................................................................  8

Time Collection Device Setup and Maintenance Tasks ........................................................................................................   11

3 Profile Options

15

Time and Labor Profile Options ................................................................................................................................................   15

Workforce Management Profile Options .................................................................................................................................   15

4 Workforce Management Lookups

19

Overview of Workforce Management Lookups .....................................................................................................................   19

Time and Labor Relative Ranges ..............................................................................................................................................   19

Change Audit Reason Lookup ...................................................................................................................................................   19

Time Collection Supplier and Supplier Device Event Lookups ..........................................................................................  20

Time Rule Classification Lookup ..............................................................................................................................................   20

Web Clock Properties Lookup ....................................................................................................................................................  21

5 Time Entry Configurations

23

Best Practices for Creating Time Entry Objects ....................................................................................................................   23

How Many Time Entry Layout Components, Categories, and Layout Sets to Create ...................................................   27

6 Absence, Payroll, and Project Costing Time Attributes

29

Time Attributes  .............................................................................................................................................................................    29

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Start and End Property Time Attributes .................................................................................................................................  29

Data Dictionary of Time Attributes ..........................................................................................................................................  30

Generate Data Dictionary Time Attributes .............................................................................................................................  30

Time and Labor Units of Measure ............................................................................................................................................  31

7 Custom Time Attributes

33

Overview of Custom Time Attributes ......................................................................................................................................   33

Create Value Sets to Use with Custom Time Attributes ......................................................................................................  34

Attribute Categories for Custom Time Attributes .................................................................................................................  35

Create Custom Time Attributes ................................................................................................................................................   35

8 Overview of Time Entry Layout Components

37

Overview of Layout Components for Time Entry .................................................................................................................   37

Single-Attribute Time Field ........................................................................................................................................................   37

Multiple-Attribute Time Field ....................................................................................................................................................   38

Web Clock Buttons .......................................................................................................................................................................  38

Dependent Time Field .................................................................................................................................................................  39

Delivered Time Card Fields ........................................................................................................................................................  39

Basic Time Entry Layout Component Configuration Process ...........................................................................................   40

9 Data Sources

43

Data Sources for Layout Components ....................................................................................................................................   43

Data Source Filters for Time Entry ..........................................................................................................................................   43

Data Source Filter Examples ......................................................................................................................................................  43

Data Source Types .......................................................................................................................................................................  44

10 Common Configuration Properties for Time Card Fields and Web Clock

Buttons

45

Best Practices for Configuring General Properties of Time Entry Layout Components ...............................................  45

Options to Configure Default Values for Time Card Fields ................................................................................................   45

Configure Field-Level Display Properties for Time Entry Layout Components .............................................................   46

11 Single-Attribute Time Card Fields

49

Configure the Single-Attribute Time Card Field Properties ...............................................................................................   49

Configure US Location Override Fields in the Unified Time Entry Experience ..............................................................   49

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Configure Labor Costing Override Fields in the Unified Time Entry Experience ............................................................  51

12 Dependent Time Card Fields in the Nonunified Time Entry Experience

53

Configure the Dependent Field Properties .............................................................................................................................  53

Availability Options for Dependent Time Card Fields ..........................................................................................................  54

Example of a Dependent Field That's Available After the Person Clicks a Specific Button ..........................................  55

Example of a Dependent Field That's Available After Specific Selections ......................................................................   56

Example of a Dependent Field That's Always Available ......................................................................................................  56

Configure Dependent Fields for US Location Overrides .....................................................................................................   57

Configure Dependent Fields for Labor Costing Overrides .................................................................................................   58

13 Dependent Time Card Field Configuration Examples

61

Create the Dependent Meal Override Rate and Rate Periodicity Fields ...........................................................................   61

Create the Dependent Department Field ...............................................................................................................................   62

Create the Dependent State, County, and City Fields ..........................................................................................................  63

14 Multiple-Attribute Time Card Field Configuration

67

Configure the Time Attributes for the Multiple-Attribute Time Card Field .....................................................................   67

Add and Configure Values for the Multiple-Attribute Time Card Field ...........................................................................   68

Configure the Time Type Attribute Field for Combined Absence, Payroll, and Project Costing Entries ....................   69

15 Web Clock Buttons Configuration

73

Configure the Web Clock Button Properties ..........................................................................................................................   73

Create Shift, Break, and Meal Web Clock Buttons ................................................................................................................  73

16 Time Attestations

77

Attestations for Oracle Web Clock and Time Cards .............................................................................................................   77

Configure Time Attestations ......................................................................................................................................................  77

Time Attestation Sets ..................................................................................................................................................................  78

17 Entries to Use in Time Totals and Processing

79

Time Categories ...........................................................................................................................................................................   79

Delivered Time Categories .........................................................................................................................................................  79

Condition Components in Time Categories ..........................................................................................................................   80

Compound and Grouped Conditions in Time Categories ...................................................................................................   81

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

How You Ungroup a Time Category Condition .....................................................................................................................  82

How You Embed an Existing Time Category in a New Category ......................................................................................   82

Create a Units-Based Time Category for a Specific Value ..................................................................................................  82

Create Time Categories Using Grouped Conditions and an Embedded Category ........................................................   83

18 Time Category Usages

85

How Time Categories Work in Time Layouts ........................................................................................................................   85

How Time Categories Work in a Time Attestation Set ........................................................................................................  85

How Time Categories Work in a Time Consumer Set .........................................................................................................   86

How Time Categories Work in a Time Allocation .................................................................................................................  86

How Time Categories Work in a Time Rules .........................................................................................................................  86

How Time Categories Work in a Time Rule Set ....................................................................................................................  87

19 Layout Sets

89

Time Layout Sets .........................................................................................................................................................................   89

Delivered Time Layout Sets .......................................................................................................................................................  92

Configure Time Layout Sets ......................................................................................................................................................   92

20 Layouts

93

Time  Layouts  .................................................................................................................................................................................    93

Time Entry, View, Review, Approval Notification, and Calendar Entry Layouts .............................................................   94

Manager Time Layouts ...............................................................................................................................................................  94

Responsive UI Layout for Time Cards .....................................................................................................................................  95

Cost Overrides Layout for Time Cards ....................................................................................................................................  95

Shift Layout for WFM Schedules ..............................................................................................................................................  96

Web Clock Layout ........................................................................................................................................................................   96

21 Unified Time Entry Layout Configuration

97

Overview of Unified Time Entry Layout Configuration .......................................................................................................   97

Layout Properties for Unified Time Entry ..............................................................................................................................   97

Time Card Fields for the Unified Time Entry Layout ...........................................................................................................  97

Time Totals for the Unified Time Entry Layout ....................................................................................................................   98

22 Classic Layout Configurations, Including Time Entry Formats

99

Time Entry, Review, View, Approval Notification, and Calendar Entry Layout Configurations ...................................   99

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

More Time Entry, Review, View, and Approval Notification Layout Configurations ....................................................  100

Time Totals Layout Configurations .........................................................................................................................................  101

Calendar Entry Layout Configurations ...................................................................................................................................  101

Considerations for Selecting the Time Entry Format .........................................................................................................  102

How You Let People Submit Time Cards Containing 0 Hours Entries ...........................................................................   103

Create a Nonunified Payroll Layout Set That Includes Absence and Override Fields .................................................   103

23 Responsive UI, Cost Overrides, Web Clock, and Shift Layouts

107

Configuration of the First Section on the Responsive UI Layout ....................................................................................   107

Entries Section Configuration of the Responsive UI Layout .............................................................................................  107

Cost Overrides Layout Configuration ....................................................................................................................................   108

Web Clock Layout Configuration ............................................................................................................................................   109

Shift Layout Configuration ........................................................................................................................................................  110

Create a Nonunified Responsive Payroll Layout Set That Includes Absence and Override Fields ..............................  111

24 Offline Web Clock Configuration

115

Overview of Configuring Web Clock for Offline Use ...........................................................................................................   115

Configure Web Clock for Offline Use ......................................................................................................................................  115

Functionality Differences Between Online and Offline Web Clock ..................................................................................   116

25 Time Processing Configurations

119

Best Practices for Creating Time Processing Objects .........................................................................................................   119

How Many Time Categories and Consumer Sets to Create ..............................................................................................   122

26 Repeating Time Periods

123

Repeating Time Periods ............................................................................................................................................................   123

Delivered Repeating Time Periods .........................................................................................................................................   124

Examples of Generated Repeating Time Periods ................................................................................................................  124

27 Time Consumer Validation, Approval, and Transfer

127

Time Consumer Sets ..................................................................................................................................................................  127

Delivered Time Consumer Sets ...............................................................................................................................................   129

Considerations for Creating Time Consumer Sets ..............................................................................................................  129

Approval Options in Time Consumer Sets ...........................................................................................................................   130

How Default Time Card and Time Entry Approvals Work .................................................................................................   132

Validation and Processing Rules by Time Card Action ......................................................................................................   134

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

28 Time Card and Entry Approval Workflows

137

Overview of Time Approval Workflows Configuration .......................................................................................................   137

Payroll Time Approval Workflow Tasks ..................................................................................................................................  138

Project Costing Time Approval Workflow Tasks ..................................................................................................................  139

Example of Payroll Time Approval Rules Using Payroll Values ........................................................................................  140

Example of Payroll Time Approval Rules Using Time Entry Source ................................................................................   141

Example of Payroll Time Approval Rules Using Reported Time and Cost Segment ....................................................  143

Example of Payroll Time Approval Rules Using Calculated Time and Cost Segment .................................................   144

Ensure Workers Get Only Completed Time Card Approval Notifications with Approval Comments .......................   146

29 Time Formulas and Rule Components

149

How Formulas and Time Rule Components Work Together ............................................................................................   149

Time Formula and Rule Types .................................................................................................................................................  152

Time Entry Owner and Internal Source in Calculation Rules ............................................................................................   152

30 Rule Template Options

155

Options to Configure Time Rule Templates .........................................................................................................................   155

Rule Classification Option for Time Rule Templates ...........................................................................................................  155

Default Allocation Option for Time Calculation Rule Templates ......................................................................................  156

Rule Execution Type Option for Time Calculation Rule Templates .................................................................................   156

Summation Level Option for Time Rule Templates ............................................................................................................  157

Reporting Level Option for Time Rule Templates ...............................................................................................................   157

Suppress Duplicate Messages Display Option for Time Rule Templates .......................................................................   158

Process Empty Time Card Option for Time Entry Rule Templates ..................................................................................  158

Time Card Actions That Trigger Rule Option for Time Entry and Calculation Rule Templates .................................   159

31 Rule Templates and Rule Parameters, Output, and Explanations

161

Formula Parameters in Time Rule Templates and Rules ...................................................................................................   161

Formula Outputs in Time Rule Templates and Rules .........................................................................................................  162

Formula Outputs Unique to Time Calculation Rule Templates and Rules .....................................................................   163

How You Group Outputs in Calculation Rule Templates and Rules ................................................................................   164

How You Configure Explanation Text in Time Rule Templates and Rules .....................................................................   165

Best Practices for Explanation Text That Includes Tokens ...............................................................................................   166

Processing Order in Time Calculation Rule Sets .................................................................................................................  166

Can I create absence entries using time calculation rules? ..............................................................................................   167

Why can't I edit some rule templates? ..................................................................................................................................   167

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Why can't I edit some rules? ....................................................................................................................................................  167

32 Time Rule Processing Details Analysis

169

How You Analyze Processing Details for Time Rules and Rule Sets ...............................................................................  169

Enable and Disable Time Rule Set and Rule Logging ........................................................................................................  169

Enable Time Rule Set and Rule Log Deletion ......................................................................................................................   170

Confirm Security Profile Setup to View Time Rule Set and Rule Log Files ....................................................................   172

Set Up the Data Role and Security Profile for the Analyze Rule Processing Details Task ...........................................   172

Set Up the Job Role for the Analyze Rule Processing Details Task .................................................................................   173

Delete Older Time Rule Set and Rule Log Files ...................................................................................................................   173

33 Rule Templates and Rules Configuration Procedures

175

Create Time Rule Templates ....................................................................................................................................................   175

Create Time Rules ......................................................................................................................................................................   176

Create Time Rule Sets ...............................................................................................................................................................   176

Create a Rule Template That Calculates the Threshold for Expenditure and Payroll Time Types .............................   177

Create a Rule That Calculates the Daily 8h Threshold for Expenditure and Payroll Time Types ...............................  179

Create the Projects and Payroll Time Calculation Rule Set ...............................................................................................  180

34 Automated Time Allocation to Cost Segments

181

Overview of Allocating Time to Cost Segments ..................................................................................................................   181

Before You Start Creating and Assigning Time Allocations ..............................................................................................   181

Create Time Allocations ............................................................................................................................................................   182

Time Allocation Assignment ....................................................................................................................................................   183

How You View and Override Time Allocation to Cost Segments ....................................................................................   184

Create the Cost Center, Program, and Fund Time Allocation ...........................................................................................  185

Create and Assign the Calculation Rule That Allocates Time to Cost Segments .........................................................   188

Assign the Cost Center, Program, and Fund Time Allocation Directly to a Group of People .....................................   189

35 Time and Compliance Exceptions and Alerts

191

Create Time Rules Sets and HCM Groups for Workforce Compliance Alerts .................................................................  191

How You Configure Resource Alert Notifications for Time Exceptions ..........................................................................   192

Alerts for Change Requests with an In Error Status ...........................................................................................................  192

36 Time Card Approval Reminders and Escalations

193

Overview of Time Card Approval Reminders and Escalations .........................................................................................   193

Basic Process to Configure Time Card Approval Reminders and Escalations ...............................................................  193

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

37 Time Entries That Span Midnight and Overtime Start

195

Setup to Handle Midnight-Spanning Time and Overtime Day Start ..............................................................................   195

When to Pay Time Entries That Span Midnight ..................................................................................................................  195

Day Start for Overtime Calculations ......................................................................................................................................   195

Start  Day  Rule  .............................................................................................................................................................................     196

Example of the Start Day Rule with a 90m Grouping Threshold ....................................................................................   197

Stop  Day  Rule  ..............................................................................................................................................................................     197

Split at Day Start Time Rule ....................................................................................................................................................   198

Spanning Days Rules and Grouping Threshold ..................................................................................................................   199

38 Database Items and Time Balances

201

Overview of How You Configure Database Items to Summarize Time ..........................................................................   201

Time Balance Dimensions ........................................................................................................................................................   201

Time Balance Definitions .........................................................................................................................................................   202

Sample Fast Formula with New Time Balance Database Item ........................................................................................   203

39 Time Collection Device Configurations

207

Overview of Time Collection Device and Web Clock Event Processing .........................................................................  207

How You Import Data from Time Collection Devices ........................................................................................................  209

Supplier-Related Choice Lists for Time Device Event Mappings ....................................................................................  209

Time Device Event Mappings ..................................................................................................................................................  210

Time Device Event Mapping Sets ...........................................................................................................................................  210

Examples of Mappings for Time Device Events ...................................................................................................................  211

Shift Limits in Time Processing ...............................................................................................................................................  212

40 How Many Time Device Processing Objects to Create

215

Best Practices for Creating Time Device Processing Objects ...........................................................................................   215

How Many Time Device Event Mappings and Web Clock Button Definitions to Create .............................................   216

How Many Time Device Event Mapping Sets and Web Clock Buttons to Create .........................................................   217

How Many Time Device Export Data Configurations to Create .......................................................................................   218

How Many Time Device and Submission Rule Sets to Create ..........................................................................................  218

How Many HCM Groups to Create for Time Device Processing Profiles ........................................................................  219

41 HCM Groups

221

Overview of Linking People to Time and Labor Objects ...................................................................................................   221

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Delivered HCM Groups .............................................................................................................................................................   224

Overview of HCM Group Membership ..................................................................................................................................   225

Evaluation Criteria and HCM Group Membership ..............................................................................................................   225

How You Lock HCM Group Membership ..............................................................................................................................  226

Embedded Group Priority in HCM Groups ...........................................................................................................................  226

How You Refresh HCM Group Membership .........................................................................................................................  227

How You View HCM Group Membership ..............................................................................................................................  228

Manually Maintained Audit and Excluded HCM Groups ...................................................................................................  228

42 HCM Group Examples

229

Create an HCM Group Using Evaluation Criteria ................................................................................................................   229

Create an HCM Group Using a Value Set .............................................................................................................................  229

Create an HCM Group by Embedding Other HCM Groups ..............................................................................................   230

43 Delivered Profiles and Time Entry Profiles

233

How Time Entry Profile Components Work Together ........................................................................................................  233

Delivered Time Entry and Processing Profiles ....................................................................................................................   235

How You Set Allowable Actions for Time Entry ..................................................................................................................   236

Manager Days Before and After Settings .............................................................................................................................  236

Time Collection Device and Web Clock Integration Options on Time Entry Profiles ..................................................   237

Configure Geofences for Web Clock ......................................................................................................................................  238

Schedule Option on Time Entry Profiles ..............................................................................................................................   238

Worker Attestation Options .....................................................................................................................................................   238

Cost Overrides Option on Time Entry Profiles ....................................................................................................................  239

44 Time Measures and Time Processing Profiles

241

Time Measure to Show Option ...............................................................................................................................................   241

How Time Processing Profile Components Work Together ..............................................................................................   241

Enable Resubmission of Future Time Cards Option ..........................................................................................................  243

Submit Time Cards for Scheduled Processing Option ......................................................................................................  244

Change Audit Options ..............................................................................................................................................................   244

Public Holidays on Time Cards Option .................................................................................................................................   245

On-Call Entries on Time Cards Options ...............................................................................................................................   246

45 Time Device Processing Profiles

247

How Time Device Processing Profile Components Work Together ................................................................................   247

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Time Attributes for In and Out Event Matching .................................................................................................................   249

46 Time Profile Assignments, Priorities, and Comparison

251

Group Assignments on Time Profiles ....................................................................................................................................   251

Priority of Time Profiles ............................................................................................................................................................   251

How Time Profiles Get Derived ...............................................................................................................................................  252

Compare Time Profiles .............................................................................................................................................................   252

47 Time and Labor Integration with Absence Management

253

Basic Process to Integrate Absence Management and Time and Labor .......................................................................   253

Compensatory Time and Time Cards ...................................................................................................................................   256

How You Set Up Compensatory Time in Absence Management ....................................................................................  257

How You Set Up Compensatory Time in Time and Labor ................................................................................................  257

How You Override the Work Location for Accurate Absence Accrual Calculations .....................................................   259

How You Configure Work Location Override ......................................................................................................................   260

48 Time and Labor Integration with Global Payroll

263

Basic Process to Integrate Global Payroll and Time and Labor .......................................................................................   263

Create Time Card Elements for Time Entries ......................................................................................................................  266

Generate Time Attributes and Time Card Fields for Your Elements ..............................................................................   268

Create the Units-Based Meals Taken Element for Time Entries .....................................................................................   269

49 Time and Labor Integration with Project Costing

271

Set Up Project Costing for Use with Time and Labor ........................................................................................................   271

Overview of Time Entry Configuration for Only Project Costing and Project Costing and Payroll Combined ......   272

Initial Assignment Info and Payroll Relationships Setup ..................................................................................................   274

Delivered Project-Specific Time Card Fields and Data Sources ......................................................................................   274

Choice List Filters for Project Costing Time Cards .............................................................................................................  277

Overview of Time Card Processing Configuration for Only Project Costing and Project Costing and Payroll Combined

.........................................................................................................................................................................................................     277

50 Best Practice Configurations for Time Entry and Processing

279

Time Configuration When Hire Today Is on the Same Day or a Future Day .................................................................  279

Time Configuration When Terminate Today Is on the Same Day or a Future Day .......................................................  281

Time Configuration When Terminate Today Is on an Earlier Date .................................................................................   283

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Time Configuration When Terminate Today Is on the Same Day or a Future Day, and Rehire Is a Future Day .....   285

Time Configuration 1: When Today Is After Termination and Before Rehire ................................................................   288

Time Configuration 2: When Today Is After Termination and Before Rehire ...............................................................   290

Time Configuration for Time Data Cleanup ........................................................................................................................   292

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

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
Implementing Time and Labor

Get Help

ii

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

1  Overview

Chapter 1
Overview

Overview of Implementing Time and Labor

You can address simple to complex time reporting for permanent and contingent employees using this rule-based time
management application.

•

Individuals can report time using time cards, calendar, and web clock. They can also use third-party time
collection devices, such as badge and biometric readers.

• Line managers can report, review, and submit time cards for their people, including delegates.

• Time and labor managers can report, review, and submit time for their people using time cards and processes

that generate mass time.

For web clock and third-party devices, the import process validates event-related time data and creates or completes
time entries. Time and labor managers resolve any badge and time entry exceptions identified during this validation.

When anyone saves or submits a time card, time entry rules run to validate reported time. Managers resolve any time
entry exceptions identified during this validation. Next, calculation rules run using the time data validated by the
time entry rules. Then, time consumer validation runs for the relevant calculated time data. Finally, time consumer
administrators transfer time data for further processing, such as payroll and project costing. Here's a summary of this
flow.

1

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 1
Overview

Time and Labor Task Lists
You access Time and Labor setup tasks in the Setup and Maintenance work area. The tasks are part of the Workforce
Deployment offering, Time, and Labor functional area.

If you already implemented Oracle Global Human Resources Cloud, required for Time and Labor processing, you've
completed many prerequisite tasks. If you pay worked time according to time card entries, you need to complete tasks
in the Elements and Formulas functional area too. The Implementing Global Human Resources guide explains these
tasks.

You need to show all Time and Labor setup tasks to complete these configurations:

• Time entry

• Time processing

• File processing for time collection devices

2

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 1
Overview

Related Topics

• Time Entry Setup and Maintenance Tasks

• Time Processing Setup and Maintenance Tasks

• Overview of Time Collection Device and Web Clock Event Processing

Overview of Global Human Resources

To start an implementation of Global Human Resources, a user with the Application Implementation Consultant role
(ORA_ASM_APPLICATION_IMPLEMENTATION_CONSULTANT_JOB) must opt into the offerings applicable to your
business requirements.

Refer to the Oracle Fusion Cloud Applications Using Functional Setup Manager guide to manage the opt-in and setup of
your offerings.

Workforce Deployment Offering
Use this offering to align resources and people with business objectives, and enter and maintain information related to
people, employment, and work structures.

The following table specifies the primary functional areas of this offering. For the full list of functional areas and
features in this offering, use the Associated Features report that you review when you plan the implementation of your
offering.

Functional Area

Description

Enterprise Profile

Manage geographies, file import, reference data, and data access for users.

Legal Structures

Manage information related to legal entities - jurisdictions, authorities, addresses, registration, and tax
profile.

Organization Structures

Manage business units and business unit set assignment.

Workforce Structures

HCM Data Loader

Manage work structures including legislative data groups, enterprise information, locations,
 departments, divisions, reporting establishments, department, position, and organization trees,
 disability organizations, grades, grade rates, grade ladders, jobs, and positions. You can also define
seniority dates, collective agreements, and worker unions.

Configure HCM Data Loader and HCM Spreadsheet Data Loader for bulk data loading. Import and load
data using HCM Data Loader. Manage access to spreadsheet templates, and configure spreadsheets to
suit business needs.

Workforce Information

Manage your workforce information including banks, actions, assignment statuses, checklist
templates, document types, and eligibility profiles.

Elements and Formulas

Define elements for base pay, absences, benefits, time and labor, and payroll. You can also define
formulas for specific areas such as payroll calculation.

3

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Functional Area

Description

Chapter 1
Overview

Payroll

Benefits

Manage payroll legislations, payroll and time definitions, fast formulas, and rate definitions.

Configure eligibility profiles for checklists.

Absence Management

Configure absence plans, types, categories, certifications, and reasons for employees, including
formulas, eligibility profiles, and rates.

HCM Data Extract

Define extract definitions for HCM.

Time and Labor

Define time entry, processing, and device processing configurations, including entry field and layouts,
 time categories and consumers, validation and calculation rules, groups and profiles.

Workforce Health and Safety Incidents

Define settings for environment, health, and safety.

Related Topics

• Plan Your Implementation

Date-Effective Objects in Scheduling and Time and
Labor

You can keep a history of configuration changes for these time and labor objects because they let you set effective
dates for the changes:

• Scheduler Profile

• Time Entry Rule Set

• Worker Time Entry Setup Profile

• Time Calculation Rule Set

• Worker Time Processing Setup Profile

• Time Device Rule Set

• Time Device Processing Profile

Related Topics

• Date Effectivity

• What's the difference between updating and correcting a date-effective object?

• Examples of Updating Date-Effective Objects

• Examples of Correcting Date-Effective Objects

• What happens when I end date an object?

4

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 2
Setup and Maintenance Tasks

2  Setup and Maintenance Tasks

Time Entry Setup and Maintenance Tasks

You can address simple to complex time reporting methods with your time entry configurations.

•

Individuals can report time using time cards, calendar, and web clock. Depending on your implementation, they
can also use third-party time collection devices, such as badge and biometric readers.

• Line managers can report, review, and submit time cards for their people, including delegates.

• Time and labor managers can report, review, and submit time for their people using time cards and processes

that generate mass time.

Configure time entry methods to support your policies by completing these tasks in the order listed. Unless otherwise
specified, the tasks are in the Setup and Maintenance work area, Workforce Deployment offering, Time and Labor
functional area.

Task

Description

Recommended Help

Elements
Functional area: Elements
and Formulas

Create the payroll elements required for payroll processing of
time data transferred to the Payroll time consumer. This includes
elements for public holidays, if you want to automatically create
holiday entries on people's time cards.

• Basic Process to Integrate Global Payroll

and Time and Labor

• Create Time Card Elements for Time

Entries

Generate Data Dictionary
Time Attributes

Link time attributes stored in the data dictionary to time card
elements. Also link them to any absence types enabled for time
entry. These attributes identify the time data for transfer to the
appropriate time consumer for processing.

• Generate Time Attributes and Time Card

Fields for Your Elements

• Generate Data Dictionary Time Attributes

The time card elements, such as Regular US, Overtime CAN, and
Public Holiday INDIA make up the drop-down list for the Payroll
Time Type attribute. The absence types make up the drop-down
list for the Absence Management Type attribute. You use these
drop-down list values when you create time card fields and web
clock buttons. Time reporters use them when they report time
worked and time off.

Generate Time Card Fields

Optionally generate multiattribute fields for the selected legislative
data group. You've the option to include absence types when
defining time card fields.

• Generate Time Attributes and Time Card

Fields for Your Elements

Time and Labor Value Sets

Optionally create value sets for your own data sources, such as
drop-down lists for custom time attributes. For example, you

• Create Value Sets to Use with Custom

Time Attributes

5

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 2
Setup and Maintenance Tasks

Task

Description

Recommended Help

create the Meal Taken custom time attribute with a data source
that contains these values: Breakfast, Lunch, and Dinner.

You can use them with time cards, calendar, web clock,
and processes that generate mass time based on business
requirements. You can't use them with third-party device files.
But, they can still apply to time cards and time entries created and
viewed by managers.

Optionally create your own time attributes to record more time
data to meet organization-specific requirements. For example,
record whether people took Breakfast, Lunch, or Dinner meal
breaks. Saving a custom time attribute adds it to the data
dictionary.

You can use them with time cards, calendar, web clock,
and processes that generate mass time based on business
requirements. You can't use them with third-party device files.
But, they can still apply to time cards and time entries created and
viewed by managers.

Create layout components or edit delivered components, such
as the Expenditure Type and Payroll Time Type fields. Layout
components let different groups of people report time using
different combinations of time attributes and values. For example,
 you configure the Worked Time field to include a Jury Duty option.
The option stores a value for the Payroll Time Type attribute and
the Absence Management Type attribute.

You don't create layout components for third parties with this task.
Here's how you can use the components:

• To configure time card layouts that managers use to resolve

device-related time exceptions.

• To configure the approval notification layout

Create time categories that classify the time entries to use on
the time totals tab of various time card and approval notification
pages. For example, you want to show totals for all reported
Straight Time, Training, and Vacation time for the week. Also create
the time categories to use in time attestation sets

Custom Time Attributes

Time Entry Layout
Components

Time Categories

Question Library,
 Questionnaire Templates,
 and Questionnaires

Optionally create time attestations that let you identify if people
comply with your time policies and various regulations. For
example, did they take their scheduled meal break.

Time Attestation Sets

Optionally create groups of related time attestations. You link
these groups to time entry profiles.

• Overview of Custom Time Attributes

• Attribute Categories for Custom Time

Attributes

• Best Practices for Creating Time Entry

Objects

• Create Custom Time Attributes

• Overview of Layout Components for Time

Entry

• Basic Time Entry Layout Component

Configuration Process

• Best Practices for Creating Time Entry

Objects

• How Many Time Entry Layout

Components, Categories, and Layout Sets
to Create

• Time Categories

• Best Practices for Creating Time Entry

Objects

• How Many Time Entry Layout

Components, Categories, and Layout Sets
to Create

• Attestations for Oracle Web Clock and

Time Cards

• Configure Time Attestations

• Best Practices for Creating Time Entry

Objects

• Best Practices for Creating Time Entry

Objects

• Time Attestation Sets

Time Layout Sets

Create a set of different layouts for the various time card, web
clock, and schedule shift pages used by individuals and managers.

• Time Layout Sets

6

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Task

Description

To change the appearance of a page, you delete and add layout
components and set various properties.

You don't create third-party device layouts with this task. Here's
how you can use the layouts:

• To configure the time card pages that managers use to

resolve device-related time exceptions.

• To configure the approval notification layout that managers
use to review and approve time cards created from time
device events.

Chapter 2
Setup and Maintenance Tasks

Recommended Help

• Time Layouts

• Configure Time Layout Sets

• How Many Time Entry Layout

Components, Categories, and Layout Sets
to Create

HCM Groups

Configure groups that identify the people who share common time
entry characteristics, such as hourly employees in the same job
and state.

Evaluate HCM Group
Membership

Build group membership for a specific date or range of dates. Run
this process regularly so that everyone always has the appropriate
time entry configuration.

During implementation, refresh the groups that we provide so that
you link everyone to a default time entry profile.

• Overview of Linking People to Time and

Labor Objects

• Best Practices for Creating Time Entry

Objects

• How You Refresh HCM Group Membership

Worker Time Entry Profiles

Create time entry profiles that directly link individuals, and
indirectly their managers, to the correct time entry configurations.
Also configure time entry access controls separately for individuals
and managers. For example, let individuals edit their time for the
past 7 days and let managers edit time cards for the past 31 days.

You don't create time entry layouts for third-party devices. But you
do use layouts to create the time cards that managers use to fix
exceptions.

• How Time Entry Profile Components Work

Together

• Best Practices for Creating Time Entry

Objects

• Time Collection Device and Web Clock

Integration Options on Time Entry Profiles

CAUTION:  If you plan to use geolocation with Web Clock, be
sure to test that the countries support generating the correct
addresses from the geolocation coordinates.

Security Reference
The tasks that people can do and the data that they can see depend on their roles, duties, and privileges. For
information about these factors, see these two guides:

• Securing HCM

• Security Reference for HCM

Related Topics

• How Time Entry Profile Components Work Together

• Best Practices for Creating Time Entry Objects

7

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 2
Setup and Maintenance Tasks

Time Processing Setup and Maintenance Tasks

Individuals can report time using time cards, third-party time collection devices, and Web Clock. Line managers manage
time cards and changes requests, as do time and labor managers. Time and labor managers can also generate time
using various processes.

Here's the high-level processing that happens for time reported with Web Clock and third-party devices:

1. The import process validates event-related time data and creates or completes time entries.
2. Time and labor managers resolve any badge and time entry exceptions identified during this validation.

Here's the high-level processing that happens for all time reporting and management methods:

1. Time entry rules that validate reported time run when people save time cards and submit them.
2. Managers resolve any time entry exceptions identified during this validation.
3. Calculation rules run using the time data validated by the time entry rules.
4. Time consumer validation runs for the relevant calculated time data.
5. Time consumer administrators transfer time data for further processing, such as payroll and project costing.

Retroactive changes to people's data can require recalculation and transfer of time card data. Examples of
retroactive changes are changes to the payroll relationship or overtime period.

Configure time processing that supports your policies by completing these configuration tasks, in the order listed. All
these tasks are in the Setup and Maintenance work area, Workforce Deployment offering, Time and Labor functional
area.

Task

Description

Recommended Help

Repeating Time Periods

Create repeating time periods, such as weekly from Monday to Sunday, to
use with time cards, approvals, accrual processing, overtime, and balances.
You can use the delivered periods or create your own, as appropriate.

• Repeating Time Periods

Workforce Management Value
Sets

Optionally review the delivered value sets that people can use when
creating time categories and rule templates. Create more value sets as
needed.

• Overview of Value Sets

Workforce Management
Lookups

Time Categories

Add reasons for audited time changes from time collection devices. Also
add reasons for exceptions for incomplete or in error data. Add more time
rule classifications, as appropriate. And add your suppliers and supplier
events for time collection devices so that people can create time device
event mappings.

• Overview of Workforce
Management Lookups

Identify the time entries to use in time rules, summaries, analytics, and
transfers according to your time processing policies. Delivered time
categories include All Absence Entries, All Payroll Entries, and All Project
Entries.

• Time Categories

• Best Practices for Creating Time

Processing Objects

8

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 2
Setup and Maintenance Tasks

Task

Description

Recommended Help

Time Consumer Sets

Enable informational workflow for everyone linked to the time consumer
set, for these processes:

• Mass submit and approve time cards

• Generate time cards

• Generate time entries

• Generate time cards from time collection devices

Specify for each time consumer what actions start validation, and what time
data to validate. And, select the approval period and the transfer rules to
use.

• How Many Time Categories and

Consumer Sets to Create

• Time Consumer Sets

• Best Practices for Creating Time

Processing Objects

• How Many Time Categories and

Consumer Sets to Create

Shift Properties

Optionally set shift limits, which you can include in various time rules. For
example, create rules that generate exceptions when people clock in late or
clock out early.

• Shifts Used in WFM Schedules

Time Allocations

Optionally allocate time automatically to specific cost segments, such as
Department, Fund, and Program, for payment.

• Overview of Allocating Time to

Cost Segments

Time Allocation Assignments

Optionally assign time allocations to individuals directly or using HCM
groups. Allocation assignments use effective dating to identify which
allocation to use in time rules applicable for the person and time card
period.

Workday Definitions

Optionally configure workday definitions that support your policies for
earned dates and the day start for overtime. Time processing uses these
definitions to derive and use the earned date for time entries that span
midnight.

Time Balance Dimensions

Optionally start creating your own database items to use as time balance
variables in fast formulas. Create time balance dimensions to specify the
level and time period to use when summarizing people's time balances.

• Best Practices for Creating Time

Processing Objects

• Create Time Allocations

• Time Allocation Assignment

• How You View and Override
Time Allocation to Cost
Segments

• Setup to Handle Midnight-

Spanning Time and Overtime
Day Start

• Time Balance Dimensions

Time Balance Definitions

Optionally finish creating your own database items to use as time balance
variables in fast formulas. Create time balance definitions to identify the
time data to add or subtract from the time balance.

• Time Balance Definitions

Fast Formulas

Optionally create formulas to use in place of, or in addition to, the delivered
workforce management formulas.

• Using Fast Formulas in Oracle

Help Center

Time Rule Templates

Create rule templates that support your time validation, calculation, and
submission policies. Use time categories in rule templates to identify the
time data to process.

You need to create rule templates for these conditions:

• You use your own formulas.

• Time and Labor Fast Formula

Reference Guides (document ID
1990057.1)

• How Formulas and Time Rule
Components Work Together

• Time Formula and Rule Types

• Create Time Rule Templates

9

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 2
Setup and Maintenance Tasks

Task

Description

Recommended Help

• You use multiattribute time card fields with more than one stored time

• Options to Configure Time Rule

attribute.

You can use delivered rule templates if the time card field or web clock
button stores a single time attribute.

Time Rules

Create time rules using the rule templates.

• Advanced time category rules identify time events and entries using
complex logic not available in the condition components of a time
category.

• Time entry rules validate time entries and generate messages.

• Time calculation rules generate calculated time, which transfers to

time consumers, such as payroll and project costing.

• Time device rules validate time events imported from time collection

devices, create or update time entries, and create time entry
exceptions.

• Time submission rules identify when to automatically save and

submit time card entries created with time events imported from time
collection devices.

Templates

• Formula Parameters in Time
Rule Templates and Rules

• Formula Outputs in Time Rule

Templates and Rules

• How Formulas and Time Rule
Components Work Together

• Create Time Rules

• Formula Parameters in Time
Rule Templates and Rules

• Formula Outputs in Time Rule

Templates and Rules

Time Rule Sets

Create collections of time submission, validation, and calculation rules and
rule sets.

• Best Practices for Creating Time

Processing Objects

• Create Time Rule Sets

HCM Groups

Create groups of people who share common time processing characteristics
to link to time processing profiles.

• Overview of Linking People to

Time and Labor Objects

• Best Practices for Creating Time

Processing Objects

Evaluate HCM Group
Membership

Build group membership for a specific date or range of dates. Run this
process regularly so that everyone always has the appropriate time
processing configuration.

• How You Refresh HCM Group

Membership

During implementation, refresh the groups that we provide so that you link
everyone to a default time processing profile.

Worker Time Processing
Profiles

Identify the rule sets, time consumer set, and time card periods to use to
validate, approve, and transfer time. Also, to automatically create public
holiday entries on people's time cards, set the default value to use for the
payroll time type attribute.

• How Time Processing Profile
Components Work Together

• Best Practices for Creating Time

Processing Objects

The profiles directly link individuals, and indirectly link their managers, to
time entry validation and calculation rules. These rules also apply to time
entries created using third-party device events and Web Clock events.

HCM Data Loader

Load WFM events and actions that automatically identify retroactive
changes to people's data that require the recalculation of their time card
data. Use these business objects, available under the product area Global
Payroll - Define:

•

Import and Load Data

• Event Group

10

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 2
Setup and Maintenance Tasks

Task

Description

Recommended Help

• Event Group Translation

• Event Action

• Event Action Translation

Manage Task Configurations
for Human Capital
Management

Optionally change default approval workflows to support your policies for
payroll and project costing time cards and entries.

• Overview of Time Approval
Workflows Configuration

• Payroll Time Approval Workflow

Tasks

• Project Costing Time Approval

Workflow Tasks

Security Reference
The tasks that people can do and the data that they can see depend on their roles, duties, and privileges. For
information about these factors, see these two guides:

• Securing HCM

• Security Reference for HCM

Related Topics

• Best Practices for Creating Time Processing Objects

• How Time Processing Profile Components Work Together

• Resubmit Time Cards Process

Time Collection Device Setup and Maintenance Tasks

For third-party collection methods, you need to complete the time entry and processing configuration tasks. To transfer
data and process events, you also need to complete these configuration tasks for your time collection devices.

Unless otherwise indicated, these tasks are in the Setup and Maintenance work area, Workforce Deployment offering,
Time and Labor functional area.

Task

Description

Recommended Help

Workforce Management
Lookups

Add the suppliers of your time collection devices to the ORA_HWM_
TCD_SUPPLIERS lookup and the supplier events to the ORA_HWM_
TCD_SUPPLIER_EVENTS lookup.

• Overview of Workforce Management

Lookups

• Supplier-Related Choice Lists for Time

Device Event Mappings

• Time Collection Supplier and Supplier

Device Event Lookups

Time Device Event
Mappings

Map time device events to time and labor application events. For
example, map a supplier Meal event to the application Out and In
event.

• Best Practices for Creating Time Device

Processing Objects

11

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 2
Setup and Maintenance Tasks

Task

Description

Recommended Help

• How Many Time Device Event Mappings
and Web Clock Button Definitions to
Create

• Time Device Event Mappings

Time Device Event Mapping
Sets

Create collections of device event mappings. For example, add
mappings for shift start, breaks, and shift stop to a set.

• Best Practices for Creating Time Device

Processing Objects

• How Many Time Device Event Mapping
Sets and Web Clock Buttons to Create

• Time Device Event Mapping Sets

Time Event resources and
request

Time Collection Device
Setup Data Export business
object services and service
data objects

Configure the appropriate REST resources and requests.

• REST API for Oracle Global Human

Configure the appropriate SOAP services.

Resources Cloud guide on Oracle Help
Center

• SOAP Web Services for Oracle HCM Cloud

guide on Oracle Help Center

Export Time Device Data
Configuration

Identify the person and employment data to export to the time
collection device.

• Best Practices for Creating Time Device

Processing Objects

Scheduled Processes task,
 Workforce Management
Time Device Export Data
process

Time Rule Templates, Time
Rules, and Time Rule Sets

• How Many Time Device Export Data

Configurations to Create

• Export Data to Time Collection Devices

Process

Schedule recurring exports of person and employment data to time
collection devices. This task is in the Time Management work area.

• Export Data to Time Collection Devices

Process

Validate and process time device and web clock events by creating
time device and submission rule templates, rules, and rule sets. The
import process runs these rules for both time device and web clock
events.

• How Formulas and Time Rule
Components Work Together

• Time Formula and Rule Types

• Create Time Rule Templates

• Create Time Rules

• How Many Time Device and Submission

Rule Sets to Create

• Create Time Rule Sets

• Options to Configure Time Rule

Templates

• Formula Parameters in Time Rule

Templates and Rules

• Formula Outputs in Time Rule Templates

and Rules

HCM Groups

Create groups of people who share common characteristics for time
device processing to link to time device processing profiles.

• Overview of Linking People to Time and

Labor Objects

• How Many HCM Groups to Create for

Time Device Processing Profiles

12

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 2
Setup and Maintenance Tasks

Task

Description

Recommended Help

Evaluate HCM Group
Membership

Build group membership for a specific date or range of dates. Run
this process regularly so that everyone always has the appropriate
configuration for time device processing.

• How You Refresh HCM Group Membership

During implementation, refresh the groups that we provide so that
you link everyone to a default time processing profile.

Time Device Processing
Profiles

Link device mappings, device and submission rules, and export
data to groups of people. You can also set time attributes that the
Generate Time Cards from Time Collection Device process uses
to match In and Out events. It uses the matched events to create
complete, valid time entries.

• How Time Device Processing Profile

Components Work Together

• Time Attributes for In and Out Event

Matching

Scheduled Processes task,
 Generate Time Cards from
Time Collection Device
process

Schedule onetime and recurring processes to validate imported
time device and Web Clock data. Generate time exceptions for any
invalid data, and create and update time cards with valid data at
appropriate intervals. This task is in the Time Management work
area.

• Generate Time Cards from Time

Collection Device Process

Security Reference
The tasks that people can do and the data that they can see depend on their roles, duties, and privileges. For
information about these factors, see these two guides:

• Securing HCM

• Security Reference for HCM

Related Topics

• How Time Device Processing Profile Components Work Together

• Overview of Time Collection Device and Web Clock Event Processing

• Generate Time Cards from Time Collection Device Process

13

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 2
Setup and Maintenance Tasks

14

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 3
Profile Options

3  Profile Options

Time and Labor Profile Options

To enable actionable and informational notifications about time cards, and to enable certain search features, configure
these profile options. To edit the site-level profile values, go to Setup and Maintenance > Tasks panel > Search >
Manage Administrator Profile Values.

Profile Option Code

Description

Default Value

BIP_EMAIL_NOTIFICATION_FIN_HXT

BIP_EMAIL_NOTIFICATION_HCM_HXT

BIP_ONLINE_NOTIFICATION_HCM_HXT

HXT_LOV_SEARCH_TIMECARDFIELDVALUES_STARTSWITH

HXT_LOV_SEARCH_TIMECARDS_STARTSWITH

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

Enable Oracle Business Intelligence Publisher
email notifications for time cards.

Enable Oracle Business Intelligence Publisher
email notifications for time cards.

Enable Oracle Business Intelligence Publisher
worklist notifications for Oracle Human Capital
Management Cloud applications.

Enable people to search for time card field
values that start with the specified characters.

Enable people to search for time cards that start
with the specified characters.

None

False

true

N

N

Workforce Management Profile Options

To enable various features, including whether people use classic, responsive, or enhanced time cards and Oracle Search,
use these profile options. To edit the site-level profile values, go to Setup and Maintenance > Tasks panel > Search >
Manage Administrator Profile Values.

Profile Option Code

Description

Default Value

HWM_MANAGER_RESPONSIVE_PAGES_ENABLED

HWM_MANAGER_SCHEDULES_RESPONSIVE_PAGES_ENABLED

Enable the mobile-responsive time card pages for managers.

Enable the mobile-responsive team schedule and worker calendar pages for managers.

HWM_TIME_AND_LABOR_MANAGER_RESPONSIVE_PAGES_ENABLED

Enable the mobile-responsive pages for time and labor managers and administrators.

HWM_TIME_AND_LABOR_MANAGER_SCHEDULES_RESPONSIVE_PAGES_ENABLED

Enable the mobile-responsive team schedule and worker calendar pages for time and labor managers.

Y

Y

Y

N

15

Chapter 3
Profile Options

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Profile Option Code

HWM_WORKER_RESPONSIVE_PAGES_ENABLED

HWM_WORKER_SCHEDULES_RESPONSIVE_PAGES_ENABLED

ORA_HWM_DECIMAL_ROUNDING_LIMIT

ORA_HWM_ELASTIC_SEARCH_ENABLED

ORA_HWM_ELASTIC_SEARCH_INITIAL_TC_INGEST_RGE

ORA_HWM_EVENT_INLINE_THRESHOLD

ORA_HWM_INTERNAL_TEST_FLAGS

ORA_HWM_MANAGER_VBCS_TC_SEARCH_ENABLED

ORA_HWM_PJC_VALIDATE_ONLY_UPDATED_ENTRIES

ORA_HWM_REQUEST_TIME_CHANGES_REDWOOD_PAGE_ENABLED

Enable the Redwood request time changes page.

ORA_HWM_RULES_LOG_LEVEL

ORA_HWM_RULES_LOG_MONTHS_TO_KEEP

Set the logging level for the processing of fast formulas in time repository rules. The default level is 300,

Incident

 which is the finest level.

Specify the number of months to retain log files generated when processing fast formulas in time

repository rules. The maximum retention is 24 months.

ORA_HWM_TIME_AND_LABOR_MANAGER_VBCS_TC_SEARCH_ENABLED

Enable time and labor managers to use the Visual Builder Studio time card search page.

ORA_HXT_GEN_TC_OFFLINE_SEARCH_ENABLED

ORA_HXT_MANAGER_VB_TC_UI_ENABLED

Enable time card generation with offline worker search.

Enable line managers to use the Visual Builder Studio time card grid.

ORA_HXT_TIME_AND_LABOR_MANAGER_VB_TC_UI_ENABLED

Enable time and labor managers to use the Visual Builder Studio time card grid.

None

ORA_HXT_TM_DSP

Enable the time data security policy for pages in the Time Management work area. For example, you've

No

someone who's both a time and labor manager and HR manager. For one group of people, they manage

time cards. For another group, they provide only HR management. The time data security policy limits

that person's time card access to only the group that they manage time cards for. They can't see the time

cards for the group they provide only HR management.

16

Description

Default Value

Enable the mobile-responsive time card pages for workers.

Enable the mobile-responsive calendar and team schedule pages for workers.

Specify the decimal precision that Workforce Management apps use in time calculations.

Enable the use of Oracle Search on time card pages.

For people to see search results, when you enable elastic search, you need to also define an HXT data

security policy.

If you don’t enable elastic search, the HXT data security policy isn't required. But if you use Oracle Search

for persons and the HR person LOV, you need to enable the ORA_HXT_TM_DSP profile option.

Pull all previous time cards with periods during the specified range, in months and up to 12, into the time

12

card search index. Also pull any applicable current and future time cards.

The maximum number of time record groups handled in a request for inline processing of the related

3

time record events.

Set internal flags to enable various processes in time repository.

WFM_TM_CACHE_JSERIAL_DISABLE

Change the value only when directed to by Oracle Support.

To delay the transfer of deleted time entries until the corresponding time

card is approved for the time consumer, set the value to:

WFM_TM_CACHE_JSERIAL_DISABLE WFM_XFR_DEL_ENTRY_ON_APPR_

ENABLED

Note:  There's a space separating the two WFM_ terms.

Enable line managers to use the Visual Builder Studio time card search page.

Identify which project costing time card entries to validate.

• No validates all entries.

• Yes validates only entries that changed since the last time card validation.

Y

Y

3

No

No

No

No

1

No

No

No

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Profile Option Code

Chapter 3
Profile Options

Description

time pages.

If you don't define a time data security policy and enable the related policy option, time and labor

managers won't see and can't search for anyone. No related time events, entries and cards appear on the

Default Value

ORA_HXT_WORKER_VBCS_TC_UI_ENABLED

Enable workers to use the Visual Builder Studio time card grid.

No

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

• HCM Data Roles

17

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 3
Profile Options

18

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 4
Workforce Management Lookups

4  Workforce Management Lookups

Overview of Workforce Management Lookups

Delivered lookups make up drop-down list values for various time and labor fields, including fields for change audit, rule
classification, and time collection devices.

To review and change these lookups according to your needs, go to Setup and Maintenance > Tasks panel > Search >
Workforce Management Lookups.

You can also review all the workforce management lookups and change the extensible lookups using these steps, as
appropriate for your policies:

1. On the Manage Common Lookups page in the Lookup Type field, enter ORA_HWM%.
2. Click Search.

Time and Labor Relative Ranges

Let line and time and labor managers quickly show only relevant time cards with relative range filters. Examples of
delivered relative ranges are Next week, Next 2 weeks, Previous 2 weeks, or Previous 3 months.

To enable the ranges that best support your managers, go to Setup and Maintenance > Tasks panel > Search >
Workforce Management Lookups and search for the ORA_HXT_RELATIVE_RANGES lookup type.

Change Audit Reason Lookup

When you enable change auditing for time cards, you can also have people give reasons for their changes. These
reasons show as read-only information in the change audit history of affected time cards.

To ensure consistency with your policies, people select their reasons from a drop-down list with values that come from
the ORA_HWM_CA_REASONS lookup type. The lookup type includes reasons for absences created and deleted in
Oracle Fusion Absence Management. The Evaluate Absences process applies these reasons to affected time cards
during reprocessing.

Related Topics

• Change Audit Options

19

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 4
Workforce Management Lookups

Time Collection Supplier and Supplier Device Event
Lookups

You create a list of the suppliers of your time collection devices, and the events their devices record using these lookups.

Suppliers
The values that make up the Supplier drop-down list on the Create Time Device Event Mappings page come from the
ORA_HWM_TCD_SUPPLIERS lookup. You need to add your suppliers to this lookup before you change the lookup for
the supplier device event. You do this because the lookup codes for device events need to start with the supplier lookup
code.

Supplier Device Events
The values that makes up the Supplier Device Event drop-down list on these pages come from the
ORA_HWM_TCD_SUPPLIER_EVENTS lookup:

• Create Time Device Event Mappings

• Generate Time Events

You need to start these lookup codes with the supplier lookup code. For example, if you've a supplier with the lookup
code ABC, start the lookup code for that supplier's device events with ABC_.

Related Topics

• Time Device Event Mappings

Time Rule Classification Lookup

You can identify the purpose of each time rule template using the Rule Classification list. Here are some example
purposes:

• Threshold

• Shift premium

• Meal or break

You can add classifications that support your time policies using the HWM_RULE_CLASSIFICATION lookup type. The tag
for each lookup code identify which template list includes the classification.

Tag

TAR

TCR

Template with the Classification

Time audit rule

Time calculation rule

20

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 4
Workforce Management Lookups

Tag

TDR

TER

TSR

WCR

Template with the Classification

Time device rule

Time entry rule

Time submission rule

Workforce compliance rule

You can't edit the rule-level classification, because it's inherited from the template.

Related Topics

• How Formulas and Time Rule Components Work Together

• Time Formula and Rule Types

Web Clock Properties Lookup

You can identify more properties for web clock or time device events using the ORA_HWM_CLOCK_PROPERTIES
lookup. For example, you can use delivered properties to identify when an event is the start or end of a shift or meal.

This lookup makes up the drop-down lists for the Start Property and End Property time attributes. You can add these
time attributes and select appropriate values as part of these tasks:

• Create web clock buttons

• Create time device event mappings

Related Topics

• Configure the Web Clock Button Properties

• Create Shift, Break, and Meal Web Clock Buttons

21

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 4
Workforce Management Lookups

22

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 5
Time Entry Configurations

5  Time Entry Configurations

Best Practices for Creating Time Entry Objects

You need to create separate time entry profiles for each unique combination of time entry objects, as shown in these
diagrams.

The more objects you create, the greater the ongoing maintenance effort. You want to find a balance between
optimizing the time entry experience for your time reporters and the effort required to maintain that experience.

Here's how the time entry components and time categories of layout sets work together. And how the layout and time
attestation sets of the time entry profile work together. The following sections provide some combination of guidelines,
considerations, questions, and examples to help you decide how many time entry objects to create.

23

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 5
Time Entry Configurations

24

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 5
Time Entry Configurations

Custom Time Attributes
Create as many custom time attributes as you need for people to record company-specific time information outside
of payroll, absences, and project costing. For example, you want people to record the type of break they take, such as
Breakfast or Tea.

25

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 5
Time Entry Configurations

Time Entry Layout Components, Time Categories, and Layout Sets
You've many considerations to factor when deciding how many time entry layout components, time categories, and
layout sets to create. For example, when you create layout components, you set a default field or button name. You
can elect to let people override those names when they configure layouts. This approach minimizes the number of
layout components you need to create because you can reuse them in different layouts. You create as many layouts as
you need to provide meaningful time entry, review, and approval pages for the people using them. Another topic has
questions, examples, and comments to help you assess how many of these objects you need.

Time Categories and Time Attestation Sets
Create as many time attestations sets as you need for the different groups of policy and regulations you need groups of
people to attest to. Also create as many time categories as you need to identify the web clock events and time entries
that cause the attestation questionnaires to appear.

Time Card Access Settings on Time Entry Profiles
Create one profile for each group of people when the different groups have these conditions:

• Different settings configurations for time card access

• The same settings configurations for time card access for different date ranges

If individuals and their managers have the same settings configuration for time card access, with the same date ranges,
create one profile per layout set. If subsets of managers have different configurations or use different date ranges, then
create one profile for each subset of managers and their people.

Schedule, Worker Attestation, and Cost Override Options on Time Entry
Profiles
Create one profile for each group of people with the same schedule, worker attestation, and cost override options.

HCM Groups
You link one or more HCM groups with each profile. Define separate groups wherever the characteristics are unique
across profiles or groups of profiles. For example, you group people into separate groups for these reasons:

• One group reports only payroll and absence time.

• Another group reports project costing, payroll, and absence time.

Related Topics

• Time Entry Setup and Maintenance Tasks

• How Time Entry Profile Components Work Together

• How Many Time Entry Layout Components, Categories, and Layout Sets to Create

26

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 5
Time Entry Configurations

How Many Time Entry Layout Components, Categories,
and Layout Sets to Create

Use these questions to help you figure out how many layout components, time categories, and layout sets you need to
create.

Question

Examples and Comments

What type of time do you want people to
report?

Examples: Project costing, payroll, absence, a combination, company-specific information

What layout components do people use to
report time?

Examples:

• Expenditure type, project ID or name, payroll time type, absence type, and cost center fields

• Start shift, end shift, and break web clock buttons

How often do people report time with the
fields? Regularly, infrequently, or does
frequency vary among different groups?

Example: You've a group of people who regularly reports payroll costing and another group who does
so infrequently. These configurations support both groups with a single field and two layout sets:

• Time card field: You add a payroll cost segment as a dependent field of the Payroll Time Type

field. You configure the dependent field to appear regardless of the selected value for the payroll
time type.

• Layout sets:

table.

◦ In one set, you configure the time entry layout so that the cost field shows as part of the main
◦ In another set, you configure the time entry layout so that the cost field appears in the entry-level

dialog box.

Should everyone see the same drop-
down list values for the time attribute or
only those values that apply to their time
entries? If you plan to differentiate drop-
down list values, how do you want to do
that?

Can you filter the drop-down list values by
creating a value set or using private view
objects delivered by Oracle Global Payroll
Cloud? Do you need to create different
fields?

You edit the display name in each layout set to show the name most expected by that group of people.

Examples of how you can differentiate the drop-down lists:

• Based on assignment

• Based on exemptions, such as overtime in the US

If you create value sets, you need to create time card fields to use those value sets. You can limit the
number of required value sets by creating table-defined value sets. Use the logic of the filter variable
to constrain the values available for each person according to values selected for the independent time
attribute.

You can filter values using values specified for related independent layout components that appear on
the time card or Web Clock. You can also use values from these places:

• The time card itself, such as time period start and end dates

• Hidden fields, such as Assignment

Values for hidden fields automatically populate based on these values:

• The person's primary assignment

• Values provided for related independent layout components

27

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 5
Time Entry Configurations

Question

Examples and Comments

Should everyone see the same name for
the layout component?

Example: You use the delivered Payroll Time Type time card field. You want certain people to see the
field name Type of Hours Worked and other people to see Time Type.

You can change the default display name of appropriately configured layout components when you
edit the layouts in a layout set.

Create different layout sets for different groups of people who use the same layout component but with
different names.

Should everyone see the same time totals? Example: You've reservists and you want their reservist time to show in their time totals. You want to

exclude reservist time totals for people who aren't reservists.

Create different layout sets for people with time totals from different time categories.

Do you want to automatically allocate time
entries to payroll cost segments? If yes, do
you want people to see these allocations?

Example: Allocate the person's daily hours evenly to the 1111 and 2222 departments.

You can create time allocations using just the dependent Payroll Time Type cost attributes and no time
entry fields. To view the allocations, you must create the dependent fields and add them to time card
layouts.

Related Topics

• Time Entry Setup and Maintenance Tasks

• How Time Entry Profile Components Work Together

• Best Practices for Creating Time Entry Objects

28

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 6
Absence, Payroll, and Project Costing Time Attributes

6  Absence, Payroll, and Project Costing Time
Attributes

Time Attributes

A time attribute reflects how time is paid, costed, billed, or recorded as an information entry. It also qualifies the linked
time event or time entry. Here's how you can use time attributes:

•

•

In the layout components that make up time card, calendar, and Web Clock layouts

In time calculation rules, categories, and approval rules

Here are examples of time attributes and values delivered by Oracle Global Payroll Cloud, Oracle Project Costing Cloud,
and Oracle Absence Management Cloud.

Integrating Application

Time Attribute

Attribute Description

Example Values

Global Payroll

Payroll Time Type

Project Costing

Expenditure Type

Absence Management

Absence Management Type

Identifies time for payroll
processing according to the value
selected

Regular US, Overtime CAN,
 Vacation US, Public Holiday US,
 and Public Holiday CAN

Identifies time for costing and
billing according to the value
selected

Identifies time for absence
processing according to the value
selected.

Billable and Nonbillable

Paid Maternity and Vacation

Related Topics

• Basic Process to Integrate Absence Management and Time and Labor

• Time and Labor Units of Measure

• Overview of Layout Components for Time Entry

• Create Time Card Elements for Time Entries

Start and End Property Time Attributes

You can identify if a time event is the start or end of a shift or meal. Depending on your policies, you can also identify
other start and end properties.

You can add your own values to the time attribute drop-down lists using the ORA_HWM_ CLOCK_PROPERTIES lookup.
You can add Start Property and End Property time attributes and select the appropriate values as part of these tasks:

• Create web clock buttons

• Create time device event mappings

29

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 6
Absence, Payroll, and Project Costing Time Attributes

Related Topics

• Overview of Workforce Management Lookups

• Time Device Event Mappings

• Configure the Web Clock Button Properties

• Create Shift, Break, and Meal Web Clock Buttons

Data Dictionary of Time Attributes

The data dictionary is the place with all possible attributes regardless of the source, such as Oracle Absence
Management Cloud or Oracle Global Payroll Cloud.

•

•

It includes the primary time attributes for projects, payroll, and absence time. You can load more payroll and
absence time attributes, and your own custom attributes.

It contains metadata that data sources and time consumers use to present time data in a meaningful way. Time
consumers also use it to process time data appropriately. Here are examples of the metadata:

◦ What attributes to store, such as storing the configured display names of time attributes and attribute

values as alternate names

◦ Where the repository physically keeps the attributes
◦ How to verify valid values

Related Topics

• Basic Process to Integrate Absence Management and Time and Labor

• Basic Process to Integrate Global Payroll and Time and Labor

• Overview of Layout Components for Time Entry

• Create Time Card Elements for Time Entries

Generate Data Dictionary Time Attributes

After you complete the payroll and absence setup tasks, you need to run the Generate Data Dictionary Time
Attributes process to create these attributes:

• Payroll-dependent attributes for all element input values, such as rate, rate code, state, city, and public holidays

• Payroll costing attributes

The process also updates the HWM_GENERATE_TIME_ATTR_DFF descriptive flexfield with the new and revised
attributes. Here's how you also make these attributes available in Oracle Transactional Business Intelligence (OTBI):

• Confirm that this flexfield has Deployment Status selected.

• Run the Import Oracle Fusion Data Extensions for Transactional Business Intelligence process.

30

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 6
Absence, Payroll, and Project Costing Time Attributes

You also need to run the Generate Data Dictionary Time Attributes process after changing any time elements. Changes
include adding or deleting elements, editing input values, or editing element eligibility records. If you don't run the
process, you might negatively affect these actions:

• Setup of time card fields

• Validation of payroll time types

• Transfer of time to payroll

Currently, this process doesn't create any attributes for project costing time.

Related Topics

• Basic Process to Integrate Absence Management and Time and Labor

• Time and Labor Units of Measure

• Overview of Layout Components for Time Entry

• Create Time Card Elements for Time Entries

Time and Labor Units of Measure

You can create payroll and custom time attributes to store and display quantities as hours, days, or units.

• Use hours-based time entries to reflect how to pay, cost, and bill worked and calculated time. For example:

◦ 8 hours of regular time per workday
◦ 8 hours of public holiday time for what would otherwise be a regular workday
◦ 10 hours of regular time per workday that calculation rules converted into 8 hours of regular time and 2

hours of overtime

◦ 7 hours of regular time per workday spent on project A, and 1 hour of regular time spent on

miscellaneous administration

◦ 8 hours of regular time per workday for 2 days, and 8 hours of absence for 3 days
• Use days-based time entries to measure absences, for example, 4 days of personal time off.

• Use units-based time entries to assign people a flat payment amount. For example:

◦ Pay people 25 USD for each meal taken, up to three meals per day.
◦ Pay people an extra 100 USD for each worked shift where they were in charge and handled related duties.

Here are the units of measure that you can include on various time layouts:

• You can include both hours-based and units-based time card fields on these layouts: time entry, review, view,

approval notification, calendar entry, and responsive UI.

• You can use only hours-based time attributes to create the web clock buttons on the web clock layout. You can

optionally include hours-based and units-based fields on the web clock layout.

• You can include only hours-based fields for the shift layout.

31

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 6
Absence, Payroll, and Project Costing Time Attributes

Related Topics

• Time Attributes

• Create Custom Time Attributes

32

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 7
Custom Time Attributes

7   Custom Time Attributes

Overview of Custom Time Attributes

You can create custom time attributes that store company-specific information in the time repository and add them
on people's time cards. You can also link dependent attributes to these independent custom attributes. Then use this
information in rules and reports.

For example, you want to record the type of break people take when they report time for the Break payroll time type.
You start by creating a value set with these values to link to your custom attribute:

• Standard 10-minute break

• Special 15-minute break

• 2 combined 10-minute breaks

• Lunch break

• Combined lunch break and 10-minute break

• Combined lunch with 10-minute breaks to leave early

You then create your custom time attribute, which you can use with the Break time card field or web clock button.

Note:  You can't delete custom time attributes after you create them. And, the attribute values don't transfer to payroll
or project costing.

Value Sets
Before you create your custom time attributes, create at least one value set for each independent and dependent time
attribute.

•

If your list of values is the same for both the setup tasks and time entry, you can create just one value set. Use
that value set with both the unfiltered data source and the filtered data source.

• To limit the drop-down lists for time entry to valid values for each individual, create both an unfiltered and a

filtered value set.

CAUTION:  Updating an existing value set for a custom time attribute linked to time entry layout components already
used on time card layouts causes errors. You need to create a new value set, new custom time attribute, and new
layout component instead. Then, replace the existing layout component with the new component in the appropriate
layouts.

Attribute Categories
You can use attribute categories to group multiple custom time attributes together, to help when people add time
attributes as part of setup tasks. For example, you can use the delivered Custom category to identify time attributes not
delivered as part of the application. You can also use these categories in reports.

33

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 7
Custom Time Attributes

Related Topics

• Data Dictionary of Time Attributes

• Data Sources for Layout Components

• Attribute Categories for Custom Time Attributes

• Create Value Sets to Use with Custom Time Attributes

• Create Custom Time Attributes

Create Value Sets to Use with Custom Time Attributes

Create unfiltered value sets for your administrators to use during setup tasks, such as creating time categories. To limit
drop-down lists to only valid values for each worker, also create filtered value sets for workers to use when reporting
time.

If your list of values is the same for both setup tasks and time entry, you can create just one value set.

CAUTION:  You'll get errors if you update an existing value set for a custom time attribute used on time card layouts.
You need to create a new value set, new custom time attribute, and new layout component instead. Then, replace the
existing layout component with the new component in the appropriate layouts.

1. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time and Labor Value Sets.

2. Create the value set.

In the Module field, select Time and Labor Web Entry Configurations.

a.
b. Select one of these validation types: Format Only, Independent, or Table. Typically, you want to use a

table-validated set as the filtered data source for a time card field.

c. Select the appropriate data type for the values in the set.
d. For a table-validated value set, use the SQL WHERE clause to add filter variables that limit the valid values

to a subset of values. When you create time card fields, you map these filter variables to time attributes that
limit drop-down lists to valid values for each individual.

e. Save and close your configuration. The task maintains the values that you want to use in an application

table.

3. Add values. How you add them to the value set depends on the validation type.

◦ Independent validation: On the Create Value Sets page, click Manage Values to add values.
◦ Table-validated: You don't have to define or maintain values because the reference view or table manages

them.

Related Topics

• Overview of Custom Time Attributes

• Delivered Project-Specific Time Card Fields and Data Sources

• Overview of Value Sets

• Validation Type Options for Value Sets

• Considerations for Planning Value Sets

34

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 7
Custom Time Attributes

Attribute Categories for Custom Time Attributes

An attribute category can include a limited number of time attributes. This limit depends on the data type of the time
attribute, as shown here.

Data Type

Maximum Number of Time Attributes Supported

Text

Number

Date

40

40

20

If you've more than the specified number of attributes, you need to create another category. To retain the relationship
between the categories for reports, you might want to use the same category name with an appended number.

You create attribute categories for the ORA_HWM_ATTR_CATEGORY lookup type using the Manage Common Lookups
task in the Setup and Maintenance work area. The attribute categories are available for use when you create time
attributes.

Related Topics

• Overview of Custom Time Attributes

Create Custom Time Attributes

You can create custom time attributes that store company-specific information in the time repository and add them
on people's time cards. You can also link dependent attributes to these independent custom attributes. Then use this
information in rules and reports.

1. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Custom Time Attributes.

2. Create a custom time attribute.

35

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 7
Custom Time Attributes

3. On the Create Time Attribute page, complete these steps:

a. Enter a name and description.
b. Select the classification type, which indicates if the attribute has dependent attributes.
c. Select the data type of the attribute. It need to match the data type of the linked value set.
d. Optionally, select the unit of measure used for payroll and reporting purposes.
e. Select the data source value sets that appear first in the data source lists when your administrators

configure time card fields with these attributes.

f. Select an attribute category value to group time attributes for reporting purposes. You create your own

attribute categories as lookup type values.

When you select an attribute category, the data dictionary location that stores the custom time attribute
appears. The location value also indicates the number of times this attribute category was used to group
time attributes.

g. To add dependent time attributes, go to the next section. Otherwise, save your changes and close the page.

Saving your time attribute adds it to the data dictionary.

4. If you're using the nonunified time entry experience and you selected the classification type With dependent

attributes, you need to add the dependent time attributes. Here's how to do that:

a. On the Create Custom Attributes page, in the Dependent Time Attributes section, click Create.
b. Select the data type. It needs to match the data type of the selected data sources.
c. Select the data source value sets that need to appear first in the data source lists when your administrators

configure the dependent fields.

d. Save your changes and close the page. Saving your time attribute and any dependent attributes adds them

to the data dictionary.

If you're using the unified time entry experience, you can create the related single-attribute time card fields instead
of dependent fields. Then add the custom attribute and related single-attributes fields to the appropriate layouts in
the layout sets, in the display sequence that makes the appropriate list values available.

Related Topics

• Data Dictionary of Time Attributes

• Overview of Custom Time Attributes

• Attribute Categories for Custom Time Attributes

• Create Value Sets to Use with Custom Time Attributes

36

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 8
Overview of Time Entry Layout Components

8  Overview of Time Entry Layout Components

Overview of Layout Components for Time Entry

You specify how a time attribute appears on classic calendar pages, classic and responsive time card and web clock
pages, and enhanced time card pages. Also specify how the attributes transfer to the time consumer with these layout
components.

To manage time entry layout components, use the Time Entry Layout Components task in the Setup and Maintenance
work area. The task is part of the Workforce Deployment offering, Time and Labor functional area.

Related Topics

• Time Attributes

• Data Dictionary of Time Attributes

• Availability Options for Dependent Time Card Fields

• Delivered Project-Specific Time Card Fields and Data Sources

• Basic Time Entry Layout Component Configuration Process

Single-Attribute Time Field

A single-attribute time field has only one time attribute linked to it. For example, Task is a single-attribute field with the
TaskID time attribute.

You use single-attribute fields most often with lists of values that are dynamic and update automatically as new values
are added for the attribute. Because the list is dynamic, some values might not be relevant to the people reporting time.

If you've the unified time entry experience enabled, you create single-attribute fields with dependent time attributes
from payroll element values. Examples of element values are rate override, location override, and costing segments. The
people who can see the field, and where they see it depends on how you configure the field and the layouts that include
it.

If you've the nonunified time entry experience, you configure dependent attributes as part of the create single-attribute
field guided process.

Related Topics

• Time Attributes

• Data Dictionary of Time Attributes

• Basic Time Entry Layout Component Configuration Process

37

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 8
Overview of Time Entry Layout Components

Multiple-Attribute Time Field

A multiattribute field has one or more time attributes linked to it. It stores multiple values internally, but people see only
one value. For example, when someone selects the Hours Type value Regular, the save action stores the Regular payroll
time type and Billable expenditure type.

Multiattribute fields also let you identify HCM groups whose members can see the value. And you can specify whether
workers, line managers, and time and labor managers can edit or only read the value.

You use multiattribute fields most often with payroll time attributes because they're relatively static. And you can
change the name of the attribute value that people see. For example, a payroll time type value might be US Reg Hr and
you set the display name to Regular Pay.

The unified time entry experience uses layout-level maximums for time card field data types, including multiattribute
fields. The nonunified time entry experience uses a site-level maximum of 20 multiattribute fields across all layouts. So
if you've the nonunified experience, plan carefully the fields to create and the layouts to add them to.

1. Use the allowed actions and HCM groups in each row to create one multipurpose field.
2. Use the field in various layout sets across many groups of workers, managers, and time and labor managers.

Related Topics

• Time Attributes

• Data Dictionary of Time Attributes

• Basic Time Entry Layout Component Configuration Process

Web Clock Buttons

Each web clock buttons layout component typically contains multiple web clock buttons. Each button has one or more
attributes linked to it.

The button stores the multiple values internally, but people see only one value. For example, when someone clicks
Clock Out, it stores the Out application event and Regular payroll time type.

The create buttons page automatically includes the Clock Event time attribute in the button definition table. The
attribute values are In, In and Out, Out and In, and Out.

Related Topics

• Time Attributes

• Data Dictionary of Time Attributes

• Basic Time Entry Layout Component Configuration Process

38

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 8
Overview of Time Entry Layout Components

Dependent Time Field

Optionally define dependent time card fields as part of the guided processes to create single-attribute and
multiattribute time card fields, and web clock buttons. A dependent field is always a single-attribute field that's related
to an independent field or button.

Generally, you identify dependent time attributes from payroll element values, such as rate override, location override,
and costing segments. For example, you configure a field so that people need to select a Payroll Time Type value before
they can select the dependent State value.

When and where the dependent field appears on the time card or Web Clock depends on the related independent field
or button. It also depends on the availability setting. The availability setting specifies whether the field always appears
with the independent field or only after people select specific values.

If you've the unified time entry experience enabled, you create single-attribute fields. Instead of just independent time
attributes, the Time Attributes drop-down list includes both independent and dependent attributes. The people who
can see the field, and where they see it depends on how you configure the field and the layouts that include it. It doesn’t
depend on any value selected for the corresponding independent time attribute because the unified experience doesn't
let you do this configuration.

Note:  If you need fields to appear only after workers select specific attribute values, then continue to use the
nonunified environment. You can also post your requirement in Idea Lab.

Related Topics

• Time Attributes

• Data Dictionary of Time Attributes

• Availability Options for Dependent Time Card Fields

• Delivered Project-Specific Time Card Fields and Data Sources

• Basic Time Entry Layout Component Configuration Process

Delivered Time Card Fields

Time and Labor include delivered single-attribute absence, payroll, and project fields, many of them used in the
delivered layout sets.

Delivered project fields include fields to track grant-related information, such as funding sources and expenditure
organizations for sponsored projects. You need to finish configuring the delivered multiattribute Time Type field before
you can use it.

To quickly find these fields, search for Delivered in the Description field. If you need to create your own fields, you can
search for and duplicate the delivered field that most closely matches the field you need. Then, edit the duplicate field to
support your time reporting policies.

39

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 8
Overview of Time Entry Layout Components

CAUTION:  For the delivered fields to work properly, you need to complete Absence Management, Global Payroll, and
Project Costing setup and integration task. Then, you need to generate the time attributes in the data dictionary.

Related Topics

• Overview of Layout Components for Time Entry

• Delivered Project-Specific Time Card Fields and Data Sources

• Choice List Filters for Project Costing Time Cards

• Overview of Time Entry Configuration for Only Project Costing and Project Costing and Payroll Combined

Basic Time Entry Layout Component Configuration
Process

You use time entry layout components on classic calendars, classic and responsive time cards shift dialog boxes, and
Web Clock, and enhanced time cards.

1. Make sure that the payroll and absence time attributes exist in the data dictionary, and any custom time attributes.

2. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Entry Layout Components.

3. Create the time card field.

4. Complete the Field Definition page. If you've the unified time entry experience enabled, this is the only page

available.

a. Enter the general properties.
b. Configure the time attributes, data sources, and filters for the filtered data source, as appropriate. For
multiattribute fields, you do this when you add a time attribute to the attributes definition table.

c. Configure the reported time options for workers, line managers, and time and labor managers. This section

is available only if you've the unified time entry experience enabled.

- All options apply only where the field is used to report time. They're ignored where the field is used to

show calculated time and on other, nonreported time pages.

- Any Filtered Data Source for Time Entry selection that you make for line managers and time and

labor managers overrides the selection in the Time Attribute and Data Source section. You only need
to do this when managers need a less granular filter than workers.

d. Add and configure each row in the attributes definition table. This step doesn't apply to single-attribute

fields.

e. Optionally, configure a value to default for the field when it appears on classic and responsive time cards.

The enhanced time card ignores the default value.

f. Configure the field-level display properties.

If you've the nonunified time entry experience enabled, continue to the next step.

40

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 8
Overview of Time Entry Layout Components

5. Optionally complete the Dependent Field Definition page. This step is available only if the independent time attribute

you selected on the previous page has dependent attributes defined in the data dictionary.

a. Create the dependent field. Each dependent field that you create appears as a row in the table on the

Dependent Field Definition page.

b. Optionally, edit the dependent field properties, as appropriate.
c. Select the data sources for the dependent time attribute and add filters for the filtered data source, as

appropriate.

d. Optionally, configure a default value for the dependent field.
e. Configure the field-level display properties for the dependent field.

You can also create all dependent fields first, step 1, then select a field in the table and complete steps 2 through 5.
You keep selecting a field and completing steps 2 through 5 until you completely configure all the dependent fields.

6. Complete the Review page.

On this page of the guided process, you review and save your definition details. If any details aren't right, you can go
back and fix them before you save the component.

Related Topics

• Best Practices for Configuring General Properties of Time Entry Layout Components

• Configure the Single-Attribute Time Card Field Properties

• Configure the Time Attributes for the Multiple-Attribute Time Card Field

• Configure the Web Clock Button Properties

• Configure the Dependent Field Properties

41

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 8
Overview of Time Entry Layout Components

42

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

9  Data Sources

Chapter 9
Data Sources

Data Sources for Layout Components

When you define single-attribute, multiattribute, and dependent fields, you select a filtered data source and an
unfiltered data source for the specified time attribute. When you define web clock buttons, you select the unfiltered data
source for each time attribute.

Typically, the most appropriate filtered and unfiltered data source is the first value in the list.

Related Topics

• Overview of Custom Time Attributes

• Create Value Sets to Use with Custom Time Attributes

• Overview of Value Sets

• Validation Type Options for Value Sets

• Payroll Cost Allocation Key Flexfield Setup

Data Source Filters for Time Entry

Oracle Absence Management Cloud, Oracle Global Payroll Cloud, and Oracle Project Costing Cloud provide filtered
data sources for many of their independent time attributes. They don't provide filtered data sources for many of their
dependent time attributes.

When the filtered data sources include filter variables, you need to select the filter input attribute for each filter variable.
A filter input attribute supplies the value that filters the field data source. For example, the person's assignment ID
identifies their choices for the Payroll Time Type attribute. Lists for the filter variable and input attribute values of
multiattribute fields contain all the values from all the filtered data sources, for all the time attributes.

Data Source Filter Examples

Both a single-attribute field and multiattribute field use the Payroll Time Type time attribute. The multiattribute field
also uses the Expenditure Type time attribute. Here are the filter variables provided by the filtered data source for each
time entry field.

Single-Attribute Filter Variables

Multiattribute Filter Variables

• pAssignmentID

• pEffectiveDate

• pProjectUnitId

• pEffectiveDate

• pAssignmentID

43

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 9
Data Sources

Single-Attribute Filter Variables

Multiattribute Filter Variables

• pStartTime

• pStopTime

The Filter Variables drop-down list includes pEffective Date only once, even though it's provided by the
filtered data sources for both time attributes.

Data Source Types

Data sources are either private view objects or value sets.

• A private view object is an Oracle component that simplifies querying and working with business object

rows. Values for private view objects appear on the time card, in the lists of the time attributes. Global Payroll
provides separate private view objects for the filtered and unfiltered data sources.

• A value set is a collection of values that appear in the lists of the time attributes. Project Costing provides the

same value set for both the filtered and unfiltered data sources. You can create value sets to use as lists for any
custom time attributes that you create.

For unified single-attribute time card fields, the filtered data sources for line managers and time and labor managers
must store the same data type and data as the worker filtered data source. When the worker delivered data source is a
private view object, the corresponding manager value sets that you create must include the same values as the private
view object.

Related Topics

• Overview of Custom Time Attributes

• Create Value Sets to Use with Custom Time Attributes

• Overview of Value Sets

• Validation Type Options for Value Sets

• Payroll Cost Allocation Key Flexfield Setup

44

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 10
Common Configuration Properties for Time Card Fields and
Web Clock Buttons

10  Common Configuration Properties for
Time Card Fields and Web Clock Buttons

Best Practices for Configuring General Properties of
Time Entry Layout Components

When you create any time entry layout component, configure the name and description according to these best
practices.

Name
Enter a unique short name, possibly using agreed on abbreviations, such as PTT for payroll time type. This name
appears in the Name list on the Edit Layout dialog box, Time Card Matrix page. That list shows only the first 15
characters.

Description
Provide a concise but complete description of the purpose of the time card field or web clock buttons. It really helps
people who are configuring time layouts to know which components to add or delete. Here's an example description
for a multiattribute time card field with dependent fields: Absence and payroll values with dependent meals,
department, and US location fields.

Related Topics

• Basic Time Entry Layout Component Configuration Process

• Configure the Dependent Field Properties

• Configure the Single-Attribute Time Card Field Properties

• Configure the Time Attributes for the Multiple-Attribute Time Card Field

• Configure the Web Clock Button Properties

Options to Configure Default Values for Time Card Fields

When you create time card fields, you can optionally specify values to default for new time entries on classic,
responsive, and enhanced time cards. You can also specify values to default for dependent fields that appear on Web
Clock.

Note:  You don't configure default values for web clock buttons.

45

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 10
Common Configuration Properties for Time Card Fields and
Web Clock Buttons

People add fields to a time card when they open the time card, add an attribute row, or add an entry. You don't configure
default values for web clock buttons.

Select the population method for new field entries from these options:

• No default value: Don't automatically populate the new field with an entry.

• Specific value: Automatically populate the new field with the specified value. These sources populate the

Specific Display Value list:

◦ For single-attribute fields, the unfiltered data source that you selected earlier
◦ For multiattribute fields, the display names in the Display Name and Multiple Attribute Definition section

Optionally, populate new entries based on another time card field. For example, if you select the Expenditure
Type time attribute, you can specify to populate new entries based on the Expenditure Type Name attribute
value.

Note:  This option works only with classic time cards. Responsive and enhanced time cards ignore this
population method.

• Function: Automatically populate the new field with the value derived by the selected function, such as Based
on primary assignment. The function uses the filtered data source. This option is available only if the time
attribute has delivered functions.

Note:  Any default value that you specify is ignored by My Client Groups > Team Time Cards > Generate
Time Cards. It uses the attribute values specified on that page instead. Enhanced time cards also ignore
default values.

Related Topics

• Basic Time Entry Layout Component Configuration Process

• Configure the Dependent Field Properties

• Configure the Single-Attribute Time Card Field Properties

• Configure the Time Attributes for the Multiple-Attribute Time Card Field

• Data You Can Include When Generating Time Cards

Configure Field-Level Display Properties for Time Entry
Layout Components

The actual combination of field-level display properties that you can configure varies by the type of time entry layout
component. For example, you can't configure the Display Type property for web clock buttons.

1. Select the display type, such as Text box, Smart choice list, or Hidden field. Hidden fields never appear on the time
card. If you've the unified time entry experience, the list doesn’t include Read Only option. You handle this instead in
the Reported Time section, with the Read only option.

2. Edit the display name, as appropriate. This name is the default column header of the tables on classic time card

entry, review, view, and approval notification pages. It’s the default column header of the tables on the enhanced

46

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 10
Common Configuration Properties for Time Card Fields and
Web Clock Buttons

time card pages. It's also the default field name on responsive time card pages, Web Clock, and time card and
calendar dialog boxes.

Note:  To fully render the display name on time card, calendar, and web clock pages and dialog boxes, limit the
name to 70 characters or less.

3. Enable or disable override on layouts. Enabling the override lets people set different, meaningful display names in

various layout sets that use the same layout component.

4. Specify whether the time card field is required. Required fields always appear on the page or dialog box and people

need to provide a value.

Tip:  To keep people from submitting time cards with no entries, make sure that at least one time card field on the
time layout is required.

The validation that checks for values in the required fields runs when people save or submit classic and enhanced
time cards. It also runs when people click OK after editing an entry on a responsive time card. It doesn't run when
people save or submit responsive time cards. If people don't edit responsive time card entries that include required
fields, they can submit time cards that are missing required values.

Related Topics

• Basic Time Entry Layout Component Configuration Process

• Configure the Dependent Field Properties

• Configure the Single-Attribute Time Card Field Properties

• Configure the Time Attributes for the Multiple-Attribute Time Card Field

• Configure the Web Clock Button Properties

47

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 10
Common Configuration Properties for Time Card Fields and
Web Clock Buttons

48

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 11
Single-Attribute Time Card Fields

11  Single-Attribute Time Card Fields

Configure the Single-Attribute Time Card Field
Properties

Here's how you configure the time attribute, data sources, and filters for single-attribute time card fields. The process
applies for both nonunified and unified time entry experiences.

1. On the Create Time Card Field: Field Definition page, select the time attribute, such as Payroll Time Type.

2. Select the filtered data source and unfiltered data source for the specified time attribute. Typically, the most

appropriate source for the selected attribute is the first value in the list.

3. Add any filters for the filtered data source by selecting the filter variable and corresponding input attributes. For
example, here are the filter variables and filter input attributes provided by the Payroll Time Type attribute data
source.

Filter Variables

Filter Input Attributes

pAssignmentID

pEffectiveDate

Assignment

Start Time

Not all filtered data sources have filters.

Related Topics

• Time Attributes

• Data Dictionary of Time Attributes

• Data Sources for Layout Components

• Basic Time Entry Layout Component Configuration Process

• Configure the Dependent Field Properties

Configure US Location Override Fields in the Unified
Time Entry Experience

Let people enter location override information when they report time worked somewhere other than their normal work
location. You can set up only a single location level, such as State, or multiple location levels, such as State, County, and
City.

Set up each location level as a single-attribute time card field.

49

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 11
Single-Attribute Time Card Fields

1. Prepare the location time attributes. You can use the location time attributes we provide. They have data sources and
list filters, and transfer to payroll after final approval. Or you can prepare your own location attributes using this basic
process:

a. Create payroll elements using the Time Card category, with the necessary input values for location by

legislative data group.

b. Generate the location time attributes Generate Global Payroll Time Attributes for the Data Dictionary for the

data dictionary.

2. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Entry Layout Components.

3. Create the single-attribute time card field, such as State, County, or City.

4. Complete the general properties.

5.

In the Time Attribute field, search for and select the appropriate location attribute, such as State, County, or City.

6. Select the unfiltered data source and filtered data source for the time attribute.

Time Attribute

Data Source

State

One of these options:

◦ ORA_HRX_US_EARN_STATE
◦ List of values for payroll US county field for Geocode

County

One of these options:

◦ ORA_HRX_US_EARN_COUNTY
◦ List of values for payroll US county field for Geocode

City

Filtered, one of these options:

◦ ORA_HRX_US_EARN_CITY
◦ List of values for payroll US county field for Geocode
Unfiltered: List of values for payroll US city field for administrator

7. Add the filter variables and input attributes for the filtered data source. If you use multiple location levels, you

configure the data source filters as shown in this US example.

Time Attribute

Filter Variable Variable Input

Available Values

Attribute

State

NA

NA

All values in the State data source

County

pCodeLevel1

State

All counties in the selected State

City (step 1)

pCodeLevel1

State

None

City (step 2)

pCodeLevel2

County

All cities in the selected County in the selected State

8. Add the location fields to the appropriate layouts in the layout sets, in the display sequence that makes the

appropriate list values available. For example, when city values depend on the selected state and county values, you
display the State field first, followed by County, and then City. If you display the City field first, the list is empty.

50

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 11
Single-Attribute Time Card Fields

Configure Labor Costing Override Fields in the Unified
Time Entry Experience

Let people enter payroll costing information by creating the appropriate single-attribute fields.

1. Prepare cost segment time attributes for use in time card fields using this basic process:

a. Create payroll value sets using the Payroll Value Sets task.
b. Set up the cost allocation key flexfield using the Cost Allocation Key Flexfield task.
c. Set up the cost allocation key flexfield usage to be available at the element entry level.
d. Generate the costing time attributes for the data dictionary.

2. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Entry Layout Components.

3. Create the single-attribute time card field.

4. Complete the general properties.

5.

In the Time Attribute field, search for and select the appropriate general or common payroll cost segment.

6. Add the data sources and filters.

a. Select the unfiltered data source and filtered data source for the cost attribute. Typically, the most

appropriate source is the first value in the list.

b. Add the filter variables and input attributes for the filtered data source.

7. Add the costing field to the appropriate unified time entry layout.

51

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 11
Single-Attribute Time Card Fields

52

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 12
Dependent Time Card Fields in the Nonunified Time Entry
Experience

12  Dependent Time Card Fields in the
Nonunified Time Entry Experience

Configure the Dependent Field Properties

You can define dependent fields in the nonunified time entry experience. You do this in the optional second step of the
guided processes for creating time entry layout components.

If you've the unified experience, you create dependent fields as single-attribute time card fields. Then you add the fields
to the appropriate time layouts in the appropriate order for filters and processing. For example, the State field needs to
come before the County field. This way the County list has only the counties for the selected state and not all counties
for all 50 states.

Dependent time card fields that you created before the unified experience was enabled continue to work in unified
layouts that include the corresponding independent layout component.

You can create and configure dependent fields in the nonunified experience using either of these methods:

• Create all your dependent fields and then select each field in turn to add the data sources and filters.

• Create a dependent field, add the data sources and filters, and then repeat for the remaining dependent fields.

Note:  To add dependent fields to a single-attribute payroll field, duplicate and edit the delivered Payroll Time Type
field. Don't directly edit the delivered field to avoid possible issues with future upgrades.

1. Configure the entire attribute definition table on the Field Definition page. You do this because the attribute values

that you select in that table make up the Independent Attribute Value list.

2. On the Dependent Field Definition page, click the Create button.

3. On the Create Dependent Time Card Field dialog box, complete the general properties:

a.

In the Name field, enter a unique short name, possibly using agreed on abbreviations, such as PTT for
payroll time type. Also, you can select a dependent time attribute from either the general or detailed level.
For example, at the general level you can select Rate Amount. At the detailed level, you can select Rate
Amount for US Regular or Shift Premium. To help with accurate layout configurations, we recommend
that you include an appropriate suffix, such as D or G, for example, RateG or DeptOTD.

This name appears in the Name list on the Edit Layout dialog box, Time Card Matrix page. That list shows
only the first 15 characters.

53

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 12
Dependent Time Card Fields in the Nonunified Time Entry
Experience

b.

In the Description field, document the purpose of the dependent field. Here are some examples:

- Override rate amount to provide as the payroll input value
- Override rate amount to provide as the payroll input value for the US Regular time attribute
- Department for the reported time
- Department for the worked overtime
- County for the reported time, provided as the payroll input value
- County code for the reported time, provide for the US Hourly costing segment

c. Select the dependent time attribute for the specified independent time attribute, such as Overtime_City

for location or Department for payroll costing.

d. Configure the availability of the dependent time attribute:

i. Select the availability of the dependent time attribute. See the Availability Options for Dependent

Time Card Fields topic for key considerations about these options.
If you select For specific independent time attribute values, add the specific values.

ii.
e. Click OK.

4. Select the filtered data source and unfiltered data source for the specified time attribute. Typically, the most

appropriate source is the first value in the list.

5. Add any filters for the filtered data source. Many filtered data sources for dependent absence management, payroll,

and project costing attributes don't have filters.

Related Topics

• Availability Options for Dependent Time Card Fields

• Create the Dependent Department Field

• Create the Dependent State, County, and City Fields

• Create the Dependent Meal Override Rate and Rate Periodicity Fields

Availability Options for Dependent Time Card Fields

When you define dependent time fields, you specify the availability of the dependent field in relation to the independent
time attribute. You indicate whether it's available with all values of the independent time attribute or just specific values.

Considerations
Your availability selection affects where you can configure the dependent field on layouts. The selection also affects
when people see the dependent field on time cards and Web Clock. Here are some key considerations for when you're
deciding which availability option to select for the dependent field.

Consideration

Available for All Independent Values

Available for Selected Independent Values

Can I use the dependent field on the calendar?

Yes

No.

When does the dependent field appear?

It always appears, as configured in the time
card matrix or a dialog box, when the layout
configuration includes the independent
attribute.

It appears only after the person selects one of
the specified values.

54

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 12
Dependent Time Card Fields in the Nonunified Time Entry
Experience

Consideration

Available for All Independent Values

Available for Selected Independent Values

Where can I display the dependent field on the
time card layout?

•

•

In the matrix

In the dialog box for row-level or entry-
level details

• On the calendar dialog box

Only on the dialog box for row-level or entry-
level details.
You need to add the independent time attribute
in the matrix of the layout before you can add
the dependent field.

In what scenarios is each availability option
recommended?

When people use the dependent field often:

When you want it to appear in the time card
matrix, on the calendar, on Web Clock, or a
combination

When people use the dependent field
infrequently

When you don't want it to ever appear in the
time card matrix or on the calendar

What are the drawbacks of each availability
option?

The list values for the dependent field might be
inappropriate or missing

The time card matrix and calendar can't display
the dependent field

The dependent field could be available but
there isn't a corresponding input value on the
payroll element for some independent attribute
values

When can I use dependent fields on Web Clock? When the dependent field applies to all defined

web clock buttons

When the dependent field applies to only one
or a subset of web clock buttons

When you create single-attribute fields in the unified time entry experience that depend on other fields, it’s the same as
selecting Available for all independent values.

Related Topics

• Example of a Dependent Field That's Always Available

• Example of a Dependent Field That's Available After Specific Selections

• Example of a Dependent Field That's Available After the Person Clicks a Specific Button

• Configure the Dependent Field Properties

Example of a Dependent Field That's Available After the
Person Clicks a Specific Button

You want people to select a department on Web Clock after they click Transfer.

Setup
You specify that the dependent Department field is available for only the Transfer button. You then add the Department
field on the web clock layout.

Results
The Department field appears when people click Transfer on Web Clock.

55

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 12
Dependent Time Card Fields in the Nonunified Time Entry
Experience

Related Topics

• Availability Options for Dependent Time Card Fields

Example of a Dependent Field That's Available After
Specific Selections

You want people to select a department after they select Overtime in the Payroll Type field. They use this dependent
field infrequently so you want it to appear only in the dialog box with row-level details.

Setup
You specify that the dependent Department field is available only when people select Overtime for the independent
Payroll Time Type attribute.

Results
If the people select Overtime, the Department field appears in the dialog box with row-level details and they can select
a department. If people select Regular, the Department field doesn't appear anywhere on the page, including dialog
boxes, and they can't select a department.

Related Topics

• Availability Options for Dependent Time Card Fields

Example of a Dependent Field That's Always Available

You want people to always select the department after they select a payroll time type. They should easily find the
dependent field in the time card matrix or on the calendar.

Setup
You specify that the dependent Department field is available for all independent Payroll Time Type attribute values.

Results
The Department field always appears in the time card matrix and on the calendar, regardless of the selected payroll time
type. People can always select a department.

Related Topics

• Availability Options for Dependent Time Card Fields

56

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 12
Dependent Time Card Fields in the Nonunified Time Entry
Experience

Configure Dependent Fields for US Location Overrides

You can let people enter location override information when they report time worked somewhere other than their
normal work location.

You can capture only a single location level, such as State, or multiple location levels, such as State, County, and City. Set
up each location level as a dependent time card field of the independent Payroll Time Type attribute.

1. Prepare the location time attributes. You can use the location time attributes we provide. They've data sources and

list filters, and transfer to payroll after final approval. Or you can prepare your own location attributes using this basic
process:

a. Create payroll elements using the Time Card category, with the necessary input values for location by

legislative data group. Use the Elements task in the Elements and Formula functional area.

b. Generate the location time attributes using the Generate Data Dictionary Time Attributes task in the Time

and Labor functional area.

2. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Entry Layout Components.

3. Create or edit an independent time card field or web clock buttons definition that has the Payroll Time Type time

attribute.

4. Create the dependent field.

◦ Be sure to set the independent attribute to Payroll Time Type.
◦ Remember, your availability selection decides what display options people have when they configure time

layouts.

You can repeat step 2 as many times as needed to create all the dependent fields first. Then, add the data sources
and filters to each field. Or, you can create a field and add the sources and filters before you create the next field.

5. Select the unfiltered data source and filtered data source for the location attribute.

Time Attribute

Data Source

State

One of these options:

◦ ORA_HRX_US_EARN_STATE
◦ List of values for payroll US county field for Geocode

County

One of these options:

◦ ORA_HRX_US_EARN_COUNTY
◦ List of values for payroll US county field for Geocode

City

Filtered, one of these options:

◦ ORA_HRX_US_EARN_CITY
◦ List of values for payroll US county field for Geocode
Unfiltered: List of values for payroll US city field for administrator

57

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 12
Dependent Time Card Fields in the Nonunified Time Entry
Experience

6. Add the filter variables and input attributes for the filtered data source. If you use multiple location levels, you

configure the data source filters as shown in this US example.

Dependent Field

Filter Variable

Variable Input Attribute

State

County

City (step 1)

City (step 2)

NA

pCodeLevel1

pCodeLevel1

pCodeLevel2

NA

State

State

County

Available Values for Dependent
Field

All values in the State data source

All counties in the selected State

None

All cities in the selected County in
the selected State

7. Add the dependent location fields to the appropriate layouts in the layout sets, in the display sequence that makes
the appropriate list values available. For example, when city values depend on the selected state and county values,
you display the State field first, followed by County, and then City. If you display the City field first, the list is empty.

The availability setting that you selected when you create the dependent field decides your display options in time
card layouts.

Related Topics

• Availability Options for Dependent Time Card Fields

• Time Layout Sets

• Create Time Card Elements for Time Entries

• Create the Dependent Meal Override Rate and Rate Periodicity Fields

• Configure the Dependent Field Properties

Configure Dependent Fields for Labor Costing Overrides

You can let people enter payroll cost information by creating dependent fields for the independent Payroll Time Type
time attribute.

Set up cost fields as dependent time card fields of the related independent Payroll Time Type time attribute.

1. Prepare cost segment time attributes for use in time card fields using this basic process:

a. Create payroll value sets using the Payroll Value Sets task.
b. Set up the cost allocation key flexfield using the Cost Allocation Key Flexfield task.
c. Set up the cost allocation key flexfield usage to be available at the element entry level.
d. Generate the costing time attributes using the Generate Data Dictionary Time Attributes task.

2. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Entry Layout Components.

3. Create or edit an independent time card field that has the Payroll Time Type time attribute.

58

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

4. Create the dependent field.

Chapter 12
Dependent Time Card Fields in the Nonunified Time Entry
Experience

◦ Be sure to set the independent attribute to Payroll Time Type.
◦ Remember, your availability selection decides what display options people have when they configure time
layouts. Here's the appropriate availability selection for legislative data groups that do and don't share
costing structures.

Shared by LDGs

Availability Setting

Yes

No

You can make the costing structure available to all independent attribute values.

You must create multiple dependent fields and specify the independent attribute values for

each dependent field.

5. Add the data sources and filters to the field selected in the General Properties section.

a. Select the unfiltered data source and filtered data source for the cost attribute. Typically, the most

appropriate source is the first value in the list.

b. Add the filter variables and input attributes for the filtered data source.

6. Add the dependent costing fields to the appropriate layouts in the layout set. The availability setting that you

selected when you create the dependent field decides your display options in time card layouts.

Related Topics

• Availability Options for Dependent Time Card Fields

• Configure the Dependent Field Properties

• Create the Dependent Department Field

• Payroll Cost Allocation Key Flexfield Setup

• Payroll Cost Allocation Key Flexfield Structure

59

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 12
Dependent Time Card Fields in the Nonunified Time Entry
Experience

60

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 13
Dependent Time Card Field Configuration Examples

13  Dependent Time Card Field Configuration
Examples

Create the Dependent Meal Override Rate and Rate
Periodicity Fields

You want to let managers override the meal allowance as appropriate, so you create two dependent fields for the
independent Payroll Time Type attribute.

The Meal Override Rate field lets them override the person's default rate. The Meal Rate Periodicity field ensures proper
processing after the overridden rate transfers to Global Payroll.

1. Create the Meals Taken element.

2. Create both dependent rate fields by completing these steps twice, once for each field.

In the General Properties section, click the Create icon.

a.
b. On the Create Dependent Time Card Field dialog box, complete these steps:

i.

ii.
iii.

In the Name field for the first field you're creating, enter MealOvrrdRt. For the second field you're
creating, enter MealRtPdcty.
In the Independent Time Attribute field, select Payroll Time Type.
In the Dependent Time Attribute field, click Search.

a. On the Search and Select: Time Attributes dialog box, in the Name field, enter Rate. The

default search results level is General, which is what you want for these attributes.
In the search results section, select Rate Amount of the collection InputValue.

b.
c. Click OK.

iv. On the Create Dependent Time Card Field dialog box, enter the description.

Dependent Field

Description

MealOverrdRt

Override the default meal allowance.

MealRtPdcty

Rate periodicity for the override rate of the meal allowance.

In the Availability section, select For specific independent time attribute values.
In the Independent Time Attribute Value field, select Meals Taken.

v.
vi.
vii. Click OK.

61

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 13
Dependent Time Card Field Configuration Examples

3. Define the data sources and display properties.

Repeat steps a through c twice, once for each dependent field.

In the General Properties section, select the dependent field that you're defining.

a.
b. Select the data sources, as shown here.

Dependent Field

Filtered Data Source for Time Entry

Unfiltered Data Source for Setup Tasks

MealOvrrdRt

MealRtPdcty

Default format value set for number

Default format value set for number

HR Lookup Type PVO

HR Lookup Type PVO

c. Complete the display properties, as shown here.

Field

MealOvrrdRt

MealRtPdcty

Display Type

Display Name

Text box

Hidden

Meal Override Rate

Meal Rate Periodicity

d. For MealOvrrdRt, select Enable override on layouts.
e. For MealOvrrdRt, in the Required on the Time Card field, select No.
f. Repeat steps 1 through 3 once, to define these properties for the dependent MealRtPdcty field.

4. Click Next to open the Review page.

Related Topics

• Availability Options for Dependent Time Card Fields

• Create the Units-Based Meals Taken Element for Time Entries

• Configure the Dependent Field Properties

• Configure the Time Type Attribute Field for Combined Absence, Payroll, and Project Costing Entries

Create the Dependent Department Field

Certain groups of people can work in different departments during their shifts and you want to track the time they work
in each department. So you create a dependent Department cost segment field for the independent Payroll Time Type
attribute.

The cost segment was created as part of the Global Payroll setup.

1.

In the General Properties section, click the Create icon.

2. On the Create Dependent Time Card Field dialog box, complete these steps:

a.
b.
c.

In the Name field, enter Department.
In the Independent Time Attribute field, select Payroll Time Type.
In the Dependent Time Attribute field, click Search.

i. On the Search and Select: Time Attributes dialog box, in the Name field, enter Depart. The default

search results level is General, which is what you want for this attribute.

62

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 13
Dependent Time Card Field Configuration Examples

In the search results section, Cost costing collection, select Department.

ii.
iii. Click OK.

d. On the Create Dependent Time Card Field dialog box, in the Description field, enter Department where the

time was worked.
In the Availability section, select For all independent time attribute values.

e.
f. On the Warning dialog box with the message that the dependent field always appears on the time card with

the independent attribute, click Yes.

g. On the Create Dependent Time Card Field dialog box, click OK.

3. Define the data sources.

a. On the Create Time Card Field: Dependent Field Definition page, in the Filtered Data Source for Time Entry

field, select the first source. This data source doesn't have any filters to add.
In the Unfiltered Data Source for Setup Tasks field, select the first source.

b.

4. Define the display properties.

In the Display Type field, select Smart choice list.

a.
b. Select the Enable override on layouts option.
c.

In the Required on the Time Card field, select No.

5. Click Next to open the Review page.

Related Topics

• Availability Options for Dependent Time Card Fields

• Configure the Time Type Attribute Field for Combined Absence, Payroll, and Project Costing Entries

• Configure the Dependent Field Properties

Create the Dependent State, County, and City Fields

Certain people regularly travel among regional locations, even crossing state lines. You want them to identify where
they worked their reported time. So you create the dependent State, County, and City location fields for the independent
Payroll Time Type attribute.

63

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 13
Dependent Time Card Field Configuration Examples

1. Create all the dependent location fields by completing steps a through b three times, once for each field.

In the General Properties section, click the Create icon.

a.
b. On the Create Dependent Time Card Field dialog box, complete these steps:

i.

ii.
iii.

In the Name field, enter the name of the current location field that you're creating, either State,
County, or City.
In the Independent Time Attribute field, select Payroll Time Type.
In the Dependent Time Attribute field, click Search.

a. On the Search and Select: Time Attributes dialog box, in the Name field, enter the current

attribute name, either State, County, or City. The default search results level is General, which
is what you want for these attributes.
In the search results section, select the dependent time attribute for the current field, either
State, County, or City, that's in the InputValue collection.

b.

c. Click OK.

iv. On the Create Dependent Time Card Field dialog box, enter the description.

Dependent Field

Description

State

County

City

State where the hours were worked

County where the hours were worked

City where the hours were worked

In the Availability section, select For all independent time attribute values.

v.
vi. On the Warning dialog box with the message that the dependent field always appears on the time

card with the independent attribute, click Yes.

vii. On the Create Dependent Time Card Field dialog box, click OK.

c. Repeat steps a through b twice, to create the dependent County and City attributes.

2. Define the data sources, filters, and display properties.

a. On the Create Time Card Field: Dependent Field Definition page, in the General Properties section, select

the dependent field that you haven't defined yet.

b. Select the filtered data source for time entry.

Location Level

Filtered Data Source

State

County

List of values for payroll US state field for Geocode

List of values for payroll US county field for Geocode

64

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 13
Dependent Time Card Field Configuration Examples

Location Level

Filtered Data Source

City

List of values for payroll US city field for user

c. For the County and City fields, click Add Filters. The State field doesn't have any filters.

i. On the Add Time Entry Data Source Filters dialog box, complete these steps for both the County and

City fields:

In the Filter Variable field, select pCodeLevel1.
In the corresponding Filter Input Attribute field, enter State.

a.
b.
c. Press Enter.
d. On the Search and Select: Time Attributes dialog box, complete these steps:

In the Collection field, select Payroll input value.

In the search results section, select State.

1.
2. Click Search.
3.
4. Click OK.

ii. On the Add Time Entry Data Source Filters dialog box, complete these steps for the City field:

In the Filter Variable field, select pCodeLevel2.
In the corresponding Filter Input Attribute field, enter County.

a.
b.
c. Press Enter.
d. On the Search and Select: Time Attributes dialog box, complete these steps:

In the Collection field, select Payroll input value.

In the search results section, select County.

1.
2. Click Search.
3.
4. Click OK.

iii. On the Add Tim Entry Data Source Filters dialog box, click OK.

d. On the Create Time Card Field: Dependent Field Definition page, select the unfiltered data source for setup

tasks.

Location Level

Unfiltered Data Source

State

County

City

List of values for payroll US state field for Geocode

List of values for payroll US county field for Geocode

List of values for payroll US city field for administrator

In the Display Type field, select Smart choice list.
In the Required on the Time Card field, select No.

e.
f.
g. Repeat steps a through f until you defined the data sources and display properties for all three location

fields.

3. Click Next to open the Review page.

65

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 13
Dependent Time Card Field Configuration Examples

Related Topics

• Availability Options for Dependent Time Card Fields

• Configure the Time Type Attribute Field for Combined Absence, Payroll, and Project Costing Entries

• Configure the Dependent Field Properties

66

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 14
Multiple-Attribute Time Card Field Configuration

14  Multiple-Attribute Time Card Field
Configuration

Configure the Time Attributes for the Multiple-Attribute
Time Card Field

You create a multiple-attribute time card field by adding, for example, a combination of absence, payroll, and project
costing time attributes as table columns.

1. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Entry Layout Components.
2. Create a multiple-attribute time card field.

3. On the Create Time Card Field: Field Definition page, click Add Time Attribute.

4. On the Add Time Attribute dialog box, complete these steps:

a. Set the attribute display sequence to specify where the column appears in the table.
b. Select the time attribute, such as Payroll Time Type.
c. Select the unfiltered data source and filtered data source for the specified time attribute. Typically, the

appropriate source is the first value in the list.

d. Specify whether the structure definition requires the time attribute.
e. Click OK.

5. Repeat steps 1 and 2 until you add all the time attributes for this field definition. Be sure to include the Identifier time

attribute so that you can uniquely identify rows that otherwise have the same attribute values.

6. Add up to five of the filters provided by the filtered data sources, for the time attributes in the attribute definition
table. For example, these are the filter variables and input attributes provided by the Expenditure Type and Payroll
Time Type attribute data sources.

Filter Variables

Filter Input Attributes

pAssignmentID

pEffectiveDate

pProjectUnitID

pStartTime

pStopTime

Assignment

Start Time

Project Unit

Start Time

Stop Time

Related Topics

• Start and End Property Time Attributes

• Basic Time Entry Layout Component Configuration Process

• Configure the Time Type Attribute Field for Combined Absence, Payroll, and Project Costing Entries

67

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 14
Multiple-Attribute Time Card Field Configuration

Add and Configure Values for the Multiple-Attribute
Time Card Field

After you create the attribute definition structure, you define the field values by completing these steps for each row
that you add to the table:

1. Enter the display value that people see in the field list, such as Paid holiday US, Nonproject work, or Regular

professional.

2. Select the time attribute values that the time repository stores, such as the Public Holiday US or Regular US

payroll time type. Or select attribute value combinations. For example, select the Professional Straight Time US
expenditure type name and the Regular US payroll time type.

Expenditure types are derived from the project unit. The selected project identifies the expenditure type values that
people see in this field list. Changing the project won't affect the payroll or absence values that people see in the list.

CAUTION:  If you use Absence Management and Global Payroll or Project Costing attributes, or all three, in the
absences rows, select values for only the absence management attributes. This way payroll and project time data
routes to the appropriate approvers and transfers to the appropriate time consumers. If you extract time data to
use with external applications, you can combine absence data with payroll or project data, or both.

3. Optionally specify that people can override the cost segment linked to the specified payroll time type. For example,
the default cost segment for the Regular US payroll time type is Standard. This default is fine for your help center
staff. But, your field technicians often need to override the cost segment according to the type of work they do.

If you enable cost override, be sure to include and configure the Cost overrides layout in the appropriate payroll or
payroll and project layout sets.

4. Specify the worker and manager actions allowed for reported time entries. The default action for both is Edit.

◦ When a time attribute value is read-only for everyone, the value appears in only the calculated time. The

value doesn't show up in any reported time entries.

◦ Calculated results are always read only for both workers and managers.
◦ Managers with the Time Attribute Full Access privilege can edit reported time values, even if the manager

allowed action is Read only.

5. Optionally filter the values that people see by assigning one or more HCM groups. Click the Show All Groups icon to

do this row by row. You can also select multiple rows, and on the Actions menu, select Assign to HCM Group.

◦ If you assign groups to specific values, group membership identifies if workers and managers can even see

the value in their list.

◦ If you don't assign groups to specific values, everyone can see all the values in their list.

Related Topics

• Start and End Property Time Attributes

• Basic Time Entry Layout Component Configuration Process

• Configure the Time Type Attribute Field for Combined Absence, Payroll, and Project Costing Entries

68

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 14
Multiple-Attribute Time Card Field Configuration

Configure the Time Type Attribute Field for Combined
Absence, Payroll, and Project Costing Entries

So that the delivered layouts for combined absence, payroll, and project costing time can work correctly, finish
configuring the delivered Time Type time card field.

Add as many rows as appropriate for the combined time that people should be able to report. For this example,
complete these steps eight times to add and configure all the table rows.

1. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Entry Layout Components.

2. Add and configure each field value in the attribute definition table.

a. On the Edit Time Card Field: Field Definition page, click the Add icon.
b. Configure the fields for each row, as shown here. Note that the absence rows have values for only absence
management attributes. This way payroll and project time data routes to the appropriate approvers and

69

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 14
Multiple-Attribute Time Card Field Configuration

transfers to the appropriate time consumers. If you extract time data to use with external applications, you
can combine absence data with payroll or project data, or both.

70

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 14
Multiple-Attribute Time Card Field Configuration

71

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 14
Multiple-Attribute Time Card Field Configuration

After time processing, Absence Management retrieves the attribute values from the rows with display
sequences 1, 2, 8, and 9. Global Payroll transfers the attribute value from the rows with display sequences 5
and 6. And, Project Costing and Global Payroll transfer their respective attribute values from the rows with
display sequences 3, 4, and 7.

3. Click Next.

4. On the Create Time Card Field: Dependent Field Definition page, you can also define dependent fields for the

independent Absence Management Type and Payroll Time Type time attributes. Other examples provide details
on how you can create dependent rate, cost segment, and location fields for the independent Payroll Time Type
attribute.

5. Click Next.

6. On the Create Time Card Field: Review page, review the definition details for the independent and any dependent

fields. If you need to, go back and make any necessary changes.

7. When the configuration is correct, click Save and Close.

8. On the Confirmation dialog box, click OK.

Related Topics

• Configure the Time Attributes for the Multiple-Attribute Time Card Field

• Create the Dependent State, County, and City Fields

• Create the Dependent Department Field

• Create the Dependent Meal Override Rate and Rate Periodicity Fields

72

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 15
Web Clock Buttons Configuration

15  Web Clock Buttons Configuration

Configure the Web Clock Button Properties

You create groups of web clock buttons by adding a combination of absence, payroll, and project costing time attributes
as table columns. You select specific attribute values in the table rows.

1. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Entry Layout Components.

2. Create attribute definition table structure, which automatically includes the Clock Event attribute.

a. On the Create Web Clock Buttons: Button Definition page, click Add Time Attribute.
b.

In the Add Time Attribute dialog box, complete these steps:

i. Set the attribute display sequence to specify where the column appears in the table.
ii. Select the time attribute, such as Payroll Time Type or Start Property.
iii. Select the unfiltered data source for the specified time attribute. Typically, the correct value for the

selected attribute is the first value in the list.

iv. Specify whether the definition structure requires the time attribute.
v. Click OK.

c. Repeat steps a and b until you add all the time attributes for the definition of these buttons.

3. After you finish the attribute definition structure, add and configure each row of the attribute definition table.

a. Enter the button label that people see on Web Clock. For example, Start Shift, Take Break, Back from

Break, or Take Meal.

b. Select the time attribute values, which the time repository stores.

CAUTION:  If you use Absence Management and Global Payroll or Project Costing attributes, or all three,
in the absence rows, select values for only the absence management attributes. This way payroll and
project time data routes to the appropriate approvers and transfers to the appropriate time consumers.
If you extract time data to use with external applications, you can combine absence data with payroll or
project data, or both.

Related Topics

• Time Attributes

• Start and End Property Time Attributes

• Basic Time Entry Layout Component Configuration Process

• Create Shift, Break, and Meal Web Clock Buttons

• Configure the Dependent Field Properties

Create Shift, Break, and Meal Web Clock Buttons

You want people to use Web Clock to report time for 8-hr shifts that include short breaks and a meal break. So you
create web clock buttons that store values for the related clock event and Payroll Time Type attribute.

73

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 15
Web Clock Buttons Configuration

You can reuse the short break buttons, so you only create them once.

1. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Entry Layout Components.
2. Create the web clock buttons.

a. On the Create Layout Component dialog box, select Web clock buttons.
b. Click OK.

3. Enter the general properties.

a. On the Create Web Clock Buttons: Buttons Definition page, in the Name field, enter 8-Hr Shift Clock

b.

Events.
In the Description field, enter Uses the independent Payroll Time Type, Start Property, and End
Property attributes, and the dependent Department time attribute.

4. Add the time attributes, data sources, and filters.

a. On the toolbar, click Add Time Attribute.
b. On the Add Time Attribute dialog box, complete the fields for the Payroll Time Type time attribute, as

shown here. Use default values unless otherwise specified.

Field

Payroll Time Type

Start Property

End Property

Attribute Display Sequence

10

15

20

Time Attribute

Payroll Time Type

Start Property

End Property

Unfiltered Data Source for

List of Payroll Time Types for

ORA_HWM_CLOCK_

ORA_HWM_CLOCK_

Setup Tasks

Administrator

PROPERTY_V

PROPERTY_V

Time Attribute Required

No

No

No

c. Click OK.
d. Repeat steps a through c until you added all three time attributes to the attribute definition.

5. On the Create Web Clock Buttons: Buttons Definition page, add rows to the attribute definition and complete the

fields, as shown here.

Button Label

Clock Event

Payroll Time
Type In

Payroll Time
Type Out

Start Property
In

Start Property
Out

End Property
In

End Property
Out

Clock In

In

Regular US LDG

Start of shift

Out for Break

Out and In

Paid Break US
LDG

Regular US LDG NA

Back from
Break

Out and In

Regular US LDG Paid Break US

NA

LDG

Out for Meal

Out and In

Unpaid Meal

Regular US LDG Start of meal

Back from Meal Out and In

Regular US LDG Unpaid Meal

Start of shift

Clock Out

Out

NA

Regular US LDG NA

NA

NA

NA

NA

NA

NA

NA

NA

NA

NA

NA

NA

NA

NA

NA

End of shift

End of meal

End of shift

74

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 15
Web Clock Buttons Configuration

6. In the Display Properties section, select Enable override on layouts.

The remaining steps apply only if you’re in a nonunified time entry experience. If you've a unified experience, click
Create.

7. Click Next.

8. On the Create Web Clock Buttons: Dependent Field Definition page, you can also define dependent fields for the
independent Payroll Time Type time attribute. Other examples provide details on how you can create dependent
rate, cost segment, and location fields for this independent time attribute.

9. Click Next.

10. On the Create Time Card Field: Review page, review the definition details for the independent and any dependent

fields. If you need to, go back and make any necessary changes.

11. When the configuration is correct, click Save and Close.

12. On the Confirmation dialog box, click OK.

Related Topics

• Create the Dependent Meal Override Rate and Rate Periodicity Fields

• Configure the Web Clock Button Properties

• Configure the Dependent Field Properties

• Create the Dependent State, County, and City Fields

• Create the Dependent Department Field

75

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 15
Web Clock Buttons Configuration

76

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 16
Time Attestations

16  Time Attestations

Attestations for Oracle Web Clock and Time Cards

You can identify if people are complying with time policies and various regulations. You do this by having people attest
to more information when they report time using Web Clock or responsive time cards.

You can configure these attestations to appear for the time card. For example, you've an attestation that prompts
workers to attest they took their meal break if they worked more than 5 hours. Or you can configure attestations to
appear when specified events or actions occur. For example, show a meal attestation when someone clocks out at the
end of their shift, or when they save their time card. You can also have attestations appear when certain conditions get
met. For example, show an attestation after a specific elapsed Web Clock duration, for a specified time entry duration,
or for specific time attributes.

Time-card level attestations appear every time the worker submits their time card for approval and the attestation
display conditions are met. Detail-level and day-level attestations appear only once. Submitted attestations are viewable
only in attestation history opened from the time card.

Configure Time Attestations

Here are the setup tasks that you need to complete in the Setup and Maintenance work area to configure time
attestations: The tasks in steps 2 through 4 are part of the Workforce Deployment Offering, Time and Labor functional
area.

1. Create your attestations using the Question Library, Questionnaire Templates, and Questionnaires tasks.

2. Create time categories using the Time Categories task. For more complex logic, you can create an advanced time

category rule and link it to the time category. Use the Time Rule Templates and Time Rules tasks.

3. Create groups of related attestations using the Time Attestation Sets task.

4. Link the time attestation set to people on their time entry profiles using the Worker Time Entry Profiles task.

Related Topics

• Time Categories

• How Time Categories Work in a Time Attestation Set

• Time Attestation Sets

• Worker Attestation Options

• Questionnaires

77

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 16
Time Attestations

Time Attestation Sets

Identify if people are complying with time policies and various regulations using time attestations sets. You can link an
attestation set to a time entry profile so that people with shared compliance characteristics for time entry can make
appropriate attestations.

Questionnaires
Link existing questionnaires to a time attestation set for people with similar attestation requirements. For example,
teenagers need to attest that when they work unscheduled time, their managers authorized the work beforehand. And,
they need to attest to whether they took meal breaks. If they didn't take a meal break, they need to specify why for
regulatory compliance.

Initiating Events
Specify when to check whether to show the questionnaire. For example, you can check only when someone clocks in or
out, saves or submits their time card, or some combination of events and actions.

Time Category
Identify what conditions the web clock events or time card entries need to meet for the questionnaire to actually appear.
For example, when someone has a web clock event or time card entry with unscheduled time, show the overtime
attestation questionnaire.

Display Level
Specify when to show the questionnaire. For example, show it when an entry that meets the time category conditions
added to the time card. Or, show it when the person submits their time card.

Related Topics

• Attestations for Oracle Web Clock and Time Cards

• How Time Categories Work in a Time Attestation Set

• Worker Attestation Options

• Questionnaires

78

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 17
Entries to Use in Time Totals and Processing

17  Entries to Use in Time Totals and
Processing

Time Categories

A time category has conditions that the time entry must meet to be included. A category can include only hours-based,
days-based, units-based time entries, or a combination.

For example, the delivered All Payroll Entries time category includes all time entries with Payroll Time Type attribute
values, regardless of their units of measure. You create categories using the Time Categories task in the Setup and
Maintenance work area. It's part of the Workforce Deployment Offering, Time and Labor functional area.

Tip:  To create a category with a combination of measures, leave the Unit of Measure field blank.

You can configure a single condition, compound conditions, or both. Here are some examples:

• A units-based category includes any time entry with the Payroll Time Type attribute value Meals Taken.

• An hours-based category includes any time entry with these specific Payroll Time Type attribute values: Regular

US or Training US or Travel US.

• A days-based category includes any time entry with the Absence Management Type attribute values measured

in days, such as Vacation Days, and not those measured in hours.

You can include other time categories in a category as long as they've the same unit of measure. Here's an example:

• The hours-based Statutory Time for OT category identifies entries with these specific Payroll Time Type

attribute values: Regular US or Training US or Travel US.

• The hours-based Union Time for OT category includes the Statutory Time for OT category. It also has another

OR condition that identifies entries with the Payroll Time Type attribute value Jury Duty US.

Related Topics

• Condition Components in Time Categories

• Compound and Grouped Conditions in Time Categories

• Delivered Time Categories

• Create Time Categories Using Grouped Conditions and an Embedded Category

Delivered Time Categories

Here are the delivered time categories used in delivered layout sets, time consumer sets, and time rule templates. You
can also use them in your own time entry and processing configurations.

79

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 17
Entries to Use in Time Totals and Processing

Delivered Category

Description

All Absence Entries

Identifies all the reported time entries with absence management attributes

Ignores absence entries with only compensatory time attributes

All Compensatory Time Entries

Identifies all the reported time entries with compensatory time attributes

Ignores absence entries with no compensatory time attributes

All Payroll Entries

All Project Entries

Identifies all the reported time entries with payroll time type attributes

Identifies all the reported time entries with the Project, Task, or Expenditure Type project time
attributes

Ignores project entries with only grant-related attributes for sponsored projects

To quickly find these categories, in the Description field, search for Delivered. To include other conditions to support
how you identify and group time entries, you need to create more categories.

Related Topics

• Time Categories

• How Time Categories Work in Time Layouts

• How Time Categories Work in a Time Consumer Set

Condition Components in Time Categories

A time category condition has a time attribute, value type, and operator.

• The time attribute identifies the type of time, such as Payroll Time Type, Task, and Expenditure Type. The unit

of measure that you select filters the available time attributes.

• The value type is the classification of the time category value. You can use these value types to define time

categories.

Value Type

Any value

Blank value

Description

Include the time entries that have any value for the time attribute in the category.

Include the time entries that have no value for the time attribute in the time category.

Specific value

Include the time entries that have the specified value for the time attribute in the time category.

Value set

Include the time entries that have an attribute value that's in the specified value set, in the time

category.

To see only attribute values that you can save and use in balance definitions and reports, select Track Usage.

80

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 17
Entries to Use in Time Totals and Processing

• The operator lets you combine multiple conditions to further filter the time entries to include in the category.

Use an AND operator to include entries only if they meet both conditions. Use an OR operator to include entries
if they meet either condition.

Related Topics

• Time Categories

• Compound and Grouped Conditions in Time Categories

• Create Time Categories Using Grouped Conditions and an Embedded Category

• Create Value Sets to Use with Custom Time Attributes

Compound and Grouped Conditions in Time Categories

You can use parentheses and operators to create compound and grouped conditions in time categories.

• Connect two or more conditions using the logical AND or OR operations to create a compound condition.

• Group two or more conditions inside parentheses to form a separate statement, or group, within a compound

condition.

• Group a condition within another grouped condition.

For example, you create a time category that includes a compound condition with these components and values:

Component

Value

Single condition

Logical operator

Grouped condition

(Payroll Time Type = Regular)

AND

(Expenditure Type = Overtime
OR

Expenditure Type = Billable)

The time category includes all the time entries that match the first condition and either of the two grouped conditions.

Related Topics

• Time Categories

• Condition Components in Time Categories

• Create Time Categories Using Grouped Conditions and an Embedded Category

• Create Value Sets to Use with Custom Time Attributes

81

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 17
Entries to Use in Time Totals and Processing

How You Ungroup a Time Category Condition

Select any one of the conditions in that group and click the Remove Parentheses icon to ungroup all the conditions.
You can then regroup conditions as appropriate.

How You Embed an Existing Time Category in a New
Category

Use the Embed Time Category icon to insert the condition of an existing time category. The embedded category
appears in read-only format, along with its time attributes and attribute values.

Create a Units-Based Time Category for a Specific Value

You plan to use meal-related time entries in rules that calculate meal allowances and in reports. So you create this time
category to identify the Payroll Time Type time attribute value Meals Taken US.

1. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Categories.

2. Create a time category.

3. On the Create Time Category page, complete the fields, as shown here:

Field

Name

Description

Track Usage

UOM

Value

Meals Taken US

Identifies time entries with the Meals Taken US payroll value

Yes

Units

4. Complete the condition row, as shown here:

Time Attribute

Value Type

Payroll Time Type

Specific Value

Attribute Value

Meals Taken US

5. Save your category and return to the Time Categories page.

82

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 17
Entries to Use in Time Totals and Processing

Create Time Categories Using Grouped Conditions and
an Embedded Category

You need to include certain payroll time in overtime calculation rules to be compliant with statutory rules. You need to
use these same entries, plus another entry in overtime calculation rules to be compliant with a union contract.

1. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Categories.

2. To identify time entries with the Regular US, Training US, or Travel US value, create the Statutory Time for US OT

category.

a. On the Create Time Category page, complete the fields, as shown here:

Field

Name

Value

Statutory Time for OT

Description

Identifies time entries with the Regular US LDG, Training US LDG, and Travel US LDG payroll

UOM

values

Hours

b. Complete three condition rows, as shown here:

Time Attribute

Value Type

Attribute Value

Operator

Payroll Time Type

Specific Value

Regular US

Payroll Time Type

Specific Value

Training US

OR

OR

Payroll Time Type

Specific Value

Travel US

c. Select the newly created condition rows.
d. On the toolbar, click the Add Parentheses icon.
e. Save the category and return to the Time Categories page.

3. To identify time entries with the Jury Duty US value or that meet the Statutory Time for US OT conditions, create the

Union Time for OT category.

a. On the Create Time Category page, complete the fields, as shown here:

Field

Name

Value

Union Time for OT

Description

Identifies time entries with the Regular US, Training US, Travel US, and Jury Duty US payroll

UOM

values

Hours

83

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 17
Entries to Use in Time Totals and Processing

Field

Value

b. On the toolbar, click the Embed a Time Category icon.
c. On the Embed Time Category dialog box, search for and select the Statutory Time for OT time category.
d. On the Create Time Category page, in the Travel US LDG row, select the OR operator.
e. Add the fourth condition, as shown here:

Time Attribute

Value Type

Attribute Value

Payroll Time Type

Specific Value

Jury Duty US

f. Delete the blank rows. Press and hold Ctrl and select the blank rows, then click the Delete icon.
g. Save the category and return to the Time Categories page.

84

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 18
Time Category Usages

18  Time Category Usages

How Time Categories Work in Time Layouts

Provide relevant hours, days, and units totals on time entry, review, view, approval notification, and responsive UI
layouts. Do this by adding time categories on the Time Totals tabs. On the responsive UI layout, you add them on the
initial section.

For example, you have a group of people who want to see these totals on each of their time cards:

• Reported regular hours

• Calculated overtime hours, if any

• Reported on call allowance units

• Time totals for absences measured in days

You can change the name that people see for each category on the layout to names that are meaningful to them. For
example, on one layout, calculated overtime is Overtime. On another layout, it's Premium Time.

How Time Categories Work in a Time Attestation Set

You need to select a time category for each questionnaire you add to a time attestation set. The category identifies the
web clock events or time card entries that the questionnaire applies to.

Example
You create an advanced time category rule to identify when people have payroll time events or entries when they're not
scheduled to work. You then create the Entry When Not Scheduled time category and link the advanced time category
rule to it. In a time attestation set, you've a questionnaire about overtime attestation. You link the Entry When Not
Scheduled time category to that questionnaire. Depending on the display level you select in the set, the questionnaire
appears when someone reports time that matches the time category conditions.

Related Topics

• Time Categories

• How Formulas and Time Rule Components Work Together

• Attestations for Oracle Web Clock and Time Cards

• Time Attestation Sets

85

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 18
Time Category Usages

How Time Categories Work in a Time Consumer Set

You need to select a time category for each time consumer that you select in a time consumer set. Here's what the time
category identifies:

• Which time entries the validation rules of the time consumer apply to

• Which time entries make up the time data transferred to the time consumer.

Typically, you use the delivered All Project Entries and All Payroll Entries time categories with these respect time
consumers: Project Costing and Payroll. The All Payroll Entries time category includes both hours-based and units-
based time data.

Related Topics

• Time Categories

• Time Consumer Sets

• Considerations for Creating Time Consumer Sets

How Time Categories Work in a Time Allocation

You need to select a time category for every source that you include in a time allocation. The time category identifies
which time entries the time calculation rule with the allocation uses to calculate the corresponding allocation outputs.

For example, allocate all time entries with a payroll attribute value of Regular as follows:

• 25 percent to department 1001

• 35 percent to department 1002

• 40 percent to department 1003

You can use only hours-based time categories in time allocations.

Related Topics

• Time Categories

• Overview of Allocating Time to Cost Segments

How Time Categories Work in a Time Rules

When you create time rules, you select the time category that identifies which time entries to use in validations,
calculations, and submissions. Here are examples of what the time category identifies:

• The end and start entries to compare with the defined rest period

• The entries to compare with the person's total scheduled hours

86

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 18
Time Category Usages

• The entries to allocate across the specified cost segments

• The entries to use when dividing reported daily or period time by the specified threshold value to calculate

regular and overtime hours

• The entries that cause the rule that automatically saves or submits the time card to run

Related Topics

• How Formulas and Time Rule Components Work Together

• Time Formula and Rule Types

• Time Categories

• Create Time Categories Using Grouped Conditions and an Embedded Category

• Create a Units-Based Time Category for a Specific Value

How Time Categories Work in a Time Rule Set

When you create a time rule set, you can optionally select a time category for one, multiple, or all time rule set
members. You want to add time categories at this level only when the category criteria apply to the entire time card.

For example, you set the Statutory Time for OT time category on the rule set member.

• Time cards that contain entries for only Regular US, Training US, and Travel US cause this rule set member to

run.

• Time cards with different, or more entries don't cause this rule set member to run.

Related Topics

• How Formulas and Time Rule Components Work Together

• Time Categories

• Create Time Categories Using Grouped Conditions and an Embedded Category

• Create a Units-Based Time Category for a Specific Value

87

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 18
Time Category Usages

88

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

19  Layout Sets

Time Layout Sets

Chapter 19
Layout Sets

You specify the appearance of various time card, calendar, Web Clock, and shift pages and dialog boxes by generating
and editing a collection of layouts. You also specify the time entry identifiers used in change audits.

You generate different layout sets for groups of people with different requirements. Here's a summary of how time
attributes, layout components, and categories make up the layout sets in the nonunified time entry experience.

89

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 19
Layout Sets

90

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 19
Layout Sets

Here's a summary of how time attributes, layout components, and categories make up the layout sets in the unified
time entry experience.

Related Topics

• Time Entry Setup and Maintenance Tasks

• Delivered Project-Specific Time Card Fields and Data Sources

91

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 19
Layout Sets

Delivered Time Layout Sets

Here are the delivered layout sets used in the delivered time entry profiles. You can also use them in your own time
entry profiles. You can't edit them, but you can duplicate them and edit the copies.

• Payroll Layout Set

• Projects and Payroll Layout Set

• Projects Layout Set

• Projects Layout Set Filtered by Project Team Members

• Projects Team Membership and Payroll Layout Set

CAUTION:  You need to finish configuring the multiattribute Time Type time card field for the layout set that
combines project and payroll time reporting to work.

All these layout sets filter the values in field drop-down lists according to people's primary assignments. The project
team layout sets also filter the drop-down list values in project costing and task number fields according to team
membership. The Projects and Payroll Layout Set includes absence fields to record and store absence data for transfer
to the Project Execution Management time consumer.

To quickly find these layout sets, in the Description field, search for Delivered.

Related Topics

• Delivered Time Card Fields

• Delivered Time Categories

• Time Layout Sets

Configure Time Layout Sets

The basic process to create your own layout set has two or three steps.

1. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Layout Sets.

2.

In the nonunified experience, select any more layouts that are appropriate. This step doesn't apply if you're in the
unified experience.

3. Select one or more time consumers and generate a set of delivered layouts for the time consumers. You can't delete

layouts from a layout set.

4. Configure the generated layouts.

92

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

20  Layouts

Time Layouts

Chapter 20
Layouts

Each nonunified or unified time layout set that you generate includes essential layouts and any selected optional
layouts.

Here are all the possible layouts in a nonunified layout set.

Here are the three layouts in a unified layout set.

93

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Related Topics

• Time Layout Sets

Chapter 20
Layouts

Time Entry, View, Review, Approval Notification, and
Calendar Entry Layouts

The worker versions of these classic, nonunified layouts are essential layouts and all layout sets automatically include
them unless the HWM_WORKER_RESPONSIVE_PAGES_ENABLED profile option is enabled. If it's enabled, here's what
happens:

• Only time and labor managers can see the time entry, review, view, and approval notification layouts.

Individuals see the responsive UI layout.

• The generated layout set doesn't include the calendar entry layout.

Both nonunified classic and responsive layouts can include unified time card fields.

When you save your configurations to the time entry layout, you've the opportunity to apply your edits to all related
layouts. You can then edit the other layouts to refine their configurations as appropriate for your policies.

Note:  People can't submit monthly time cards created with these layouts. Managers can generate monthly time cards
with these layouts and the generate time cards process. And, they can approve these monthly time cards. But, they
can't open these monthly time cards to see the details.

Related Topics

• Time Entry, Review, View, Approval Notification, and Calendar Entry Layout Configurations

• More Time Entry, Review, View, and Approval Notification Layout Configurations

Manager Time Layouts

Manager versions are available for all classic and responsive nonunified time layouts except the calendar entry and web
clock layouts. The manager versions are optional and included in layout sets only when you select the Manager layout.

When you don't select the Manager layout option, managers get the worker layout configurations. When you do
include the manager versions of the layouts, they automatically inherit your worker configurations. You can optionally
make more edits to manager versions that individuals don't see, or see as read-only.

Related Topics

• Time Entry, Review, View, Approval Notification, and Calendar Entry Layout Configurations

• More Time Entry, Review, View, and Approval Notification Layout Configurations

94

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 20
Layouts

Responsive UI Layout for Time Cards

The nonunified responsive UI layout merges time entry, review, and view layouts. It's an optional layout that's included
in layout sets only when you select the Responsive UI layout.

•

Individuals see responsive time cards only after the HWM_WORKER_RESPONSIVE_PAGES_ENABLED profile
option is enabled.

• Line managers see the responsive time cards for their teams only after the

HWM_MANAGER_RESPONSIVE_PAGES_ENABLED profile option is enabled.

• Time and Labor managers see the responsive time cards for their client groups only after the

HWM_TIME_AND_LABOR_MANAGER_RESPONSIVE_PAGES_ENABLED profile option is enabled.

This layout can include unified time card fields.

Note:  People can create and submit monthly time cards with this layout. And, managers can open the monthly time
cards to review details.

Related Topics

• Configuration of the First Section on the Responsive UI Layout

• Entries Section Configuration of the Responsive UI Layout

Cost Overrides Layout for Time Cards

The nonunified cost overrides layout lets people override the cost segment for any time card field with a payroll value
with cost override enabled. For example, let people override the cost for Regular payroll entries but not Sick absence
entries.

This layout is optional and included in layout sets when you select the Cost overrides layout. You need to select the
Responsive UI layout before you can select this layout. You also need to enable cost override for the appropriate payroll
values configured in multiattribute time card fields.

Related Topics

• Cost Overrides Layout Configuration

• Cost Overrides Option on Time Entry Profiles

• Configure Dependent Fields for Labor Costing Overrides

95

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 20
Layouts

Shift Layout for WFM Schedules

The shift layout is optional and included in nonunified layout sets only when you select the Shift layout. It’s
automatically included in unified layout sets.

• The manager version lets you identify time attribute values that time and labor managers can configure when

the create and edit shifts.

• The worker version identifies the time attributes and values that individuals see when they view shift details.

Related Topics

• Shift Layout Configuration

• Shifts Used in WFM Schedules

Web Clock Layout

The web clock layout is optional and included in nonunified layout sets only when you select the Web clock layout. No
manager version exists for this layout. The layout is automatically included in unified layout sets.

Related Topics

• Web Clock Layout Configuration

• How Many Time Device Event Mapping Sets and Web Clock Buttons to Create

• Functionality Differences Between Online and Offline Web Clock

• Configure the Web Clock Button Properties

• Configure Web Clock for Offline Use

96

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 21
Unified Time Entry Layout Configuration

21  Unified Time Entry Layout Configuration

Overview of Unified Time Entry Layout Configuration

The unified time entry layout is essential and all unified layout sets automatically include it. Configure responsive,
classic, and enhanced time cards with this layout. Use the Layout Sets task in the Time Management work area.

You can also use the Layout Sets task in the Setup and Management work area. The task is part of the Workforce
Deployment offering, Time and Labor functional area.

Layout Properties for Unified Time Entry

Here are the layout properties that you can configure. They apply to the pages and dialog boxes that the layout defines.

• Specify the time entry and date formats, and the precision of time display using decimal places.

• Specify the default view for responsive time cards.

• Enable the entry of negative time and time spanning midnight.

• Display the unit of measure column.

• Enable editing of time and durations with time change requests.

• Enable time entry and time card comments.

• Display scheduled hours header row on enhanced time cards

Time Card Fields for the Unified Time Entry Layout

You can replace the default fields and add more nonunified and unified fields that you want to appear on the time card.
By default any fields that you add apply to both reported and calculated time.

Note:  Dependent time card fields continue to work in unified layouts that include the corresponding independent
layout component.

You can also change display names. If you want the complete names to appear, limit them to 70 characters or less. The
display names appear here:

• On existing time card pages in the Time work area

• On the Report Time dialog box opened from the Time work area calendar

• On team time card pages in the Time Management work area of for My Team

• As column headers in the time entry and calculated time tables

97

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 21
Unified Time Entry Layout Configuration

The display sequence of the fields is important for data filter dependencies and processing. For example, your layout
includes location fields. You need to select a state before you can select a county. And, you need to select the county
before you select a city.

You can select the fields that together uniquely identify time entries on responsive time cards and on dialog boxes for
change audit. People open these dialog boxes from classic time cards and see these fields and their values for each
changed time entry. Or you can include them in the Addition Attributes of responsive and enhanced time cards. You can
also specify where the time card fields appear on classic time cards, such as the main time card matrix, or row-level or
entry-level details.

The Users column shows you the roles that can see the field on time cards. The Exclude option is set as part of the time
card field configuration. You can’t override it while configuring the layout.

You can use the Actions > View By > Users or Locations options to filter the fields that you see while configuring the
time entry layout. The filter doesn’t affect the actual time cards.

Time Totals for the Unified Time Entry Layout

You can add time categories measured in hours and units and specify where they appear on classic, responsive, and
enhanced time cards. You can also make the category display names more meaningful to the people who use the time
cards.

These delivered hourly totals will always appear before all other time categories that you add. You can change the order
in the layout and all time totals will appear in the order that you specify.

Delivered Time Category

Description or Calculation

Total Hours

All Hours - On-Call Time Category from Worker Time Processing Profile

Equivalent Hours for Absence Days

Converts absences measured in days using the worker’s defined day. For example, a worker who works
8-hour days has a 3-day absence. The calculated equivalent hours are 24.

Scheduled Hours

Pulled from the worker’s schedule, excluding on-call shifts.

Schedule Deviation

Total Hours (All Hours - On-Call Time Category from Worker Time Processing
Profile) + Equivalent Hours for Day Entries - Scheduled Hours

On-Call Scheduled Hours

Pulled from only the worker’s on-call schedule.

On-Call Schedule Deviation

Absence Hours

Total of absences entries measured in hours.

Related Topics

• How an Individual's Schedule Is Identified

98

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 22
Classic Layout Configurations, Including Time Entry
Formats

22  Classic Layout Configurations, Including
Time Entry Formats

Time Entry, Review, View, Approval Notification, and
Calendar Entry Layout Configurations

The time entry, review, view, and approval notification layouts are essential layouts and all classic and nonunified layout
sets automatically include them. They include the calendar entry layout only when you don't select the Responsive UI
layout.

Configure these layouts using the Layout Sets task in the Time Management work area.

Time Card Fields
You can replace the default fields and add more nonunified and unified fields that you want to appear on the time card.
Also change display names. If you want the complete names to appear, limit them to 70 characters or less. The display
names appear here:

• On existing time card pages in the Time work area

• On the Report Time dialog box opened from the Time work area calendar

• On team time card pages in the Time Management work area

• As column headers in the time entry and calculated time tables

The sequence of the fields is important for data filter dependencies. For example, your layout includes location fields.
You need to select a state before you can select a county. And, you need to select the county before you select a city. To
set field sequence for classic layouts, you need to use Personalization. Otherwise, classic time card pages ignore field
positions in the time card matrix table. To set field sequence for unified layouts, you need to enable the unified time
entry experience.

You can select the fields that together uniquely identify time entries on dialog boxes for change audit. People open
these dialog boxes from classic time cards and see these fields and their values for each changed time entry.

On the time review layout, you can also whether to display the owner and entry source as column headers on time
review pages.

Time Entry Properties
Here are the time entry properties that you can configure. The specific properties vary by the layout that you're editing
and apply to the pages and dialog boxes that the layout defines.

• Enable the entry of negative time and time spanning midnight.

• Display the unit of measure column and the option to highlight overtime periods.

• Specify the time entry and date formats, and the precision of time display using decimal places.

99

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 22
Classic Layout Configurations, Including Time Entry
Formats

Related Topics

• Availability Options for Dependent Time Card Fields

• Considerations for Selecting the Time Entry Format

• Time Layouts

• Create a Nonunified Payroll Layout Set That Includes Absence and Override Fields

More Time Entry, Review, View, and Approval
Notification Layout Configurations

Here are more edits that you can make to the classic, nonunified time entry, review, view, and approval notification
layouts. On the Edit Layout dialog box, click Next to move from one page of the guided process to the next.

Row-Level Details
You can add nonunified and unified fields that you want people to see in a separate, row-level dialog box. They open
this dialog box from the time entry, review, view, and approval notification pages. For example, you configure the
Additional Attributes dialog box to include the dependent Department field whenever someone selects Premium in the
Time Entries table.

You can change the display names so that they're meaningful to the people who use the layout. If you want people to
see the whole name, limit each name to 70 characters or less.

Comments
Specify whether the time card pages should include the Comments column. Further specify if the column should be in
the Time Entry and Calculated Time tables or on the entry-level details dialog box.

Entry-Level Details
Add nonunified and unified fields that you want people to see in a separate, entry-level dialog box. They open this
dialog box from the time entry, review, view, and approval notification pages. You can change the display names so that
they're meaningful to the people who use the layout. If you want people to see the whole name, limit each name to 70
characters or less.

On the time review layout, you can also specify whether to display the owner and source columns. This information
can be useful to who report time with multiple methods, such as badge reader, Web Clock, and time card. It can also be
useful to managers who review time cards with time entries from various owners and sources.

• Examples of time entry owners are WFM or Web Clock.

• Examples of internal sources are Manager entry, Absence entry, or Calculated entry.

Related Topics

• Availability Options for Dependent Time Card Fields

• Time Layouts

• Create a Nonunified Payroll Layout Set That Includes Absence and Override Fields

100

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 22
Classic Layout Configurations, Including Time Entry
Formats

Time Totals Layout Configurations

You can add time categories measured in hours and units to the Time Totals tab. This tab appears on the classic,
nonunified time entry, review, view, and approval notification layouts.

• Hours: You can add time categories measured in hours. The Time Totals tab of classic time card pages shows

the hours-based time totals for the specified time categories.

• Units: You can add time categories measured in units. The Time Totals tab of classic time card pages shows the

units-based time totals for the specified time categories.

On both Hours and Units pages, you can also make the category display names more meaningful to the people who use
the time cards. And, you can configure time entry properties.

Related Topics

• Availability Options for Dependent Time Card Fields

• Create a Nonunified Payroll Layout Set That Includes Absence and Override Fields

Calendar Entry Layout Configurations

Here's what you can edit on the classic, nonunified calendar entry layout.

Drag and Drop Values
You can select up to five nonunified or unified field values to display at the top of the calendar page in the Time work
area. If you want people to see the whole field name, limit each name to 70 characters or less.

Time Totals
Optionally, select the time category that identifies the time entries to include in overtime calculations. The total
calculated overtime hours appear on the overtime bar of the calendar page in the Time work area.

You can also specify the precision, in decimal places, to use when displaying time on the calendar page.

Related Topics

• Availability Options for Dependent Time Card Fields

• Time Layouts

• Create a Nonunified Payroll Layout Set That Includes Absence and Override Fields

101

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 22
Classic Layout Configurations, Including Time Entry
Formats

Considerations for Selecting the Time Entry Format

Specify whether people enter time as number of hours, start and stop times, or both when you configure time layouts.
You need to include the correct formats in the layouts to ensure the accuracy of reported and calculated time.

You configure the layouts using the Layout Sets task in the Time Management work area. You specify the time entry
format on the Edit Layout dialog box, in the Time Entry Properties section.

Time Entry Formats
Here are the available time entry formats.

Time Entry Format

Appearance on Time Card for Each
Day

Time Entry by Time Reporters

Display hours only

One column, labeled Hours

Enter the number of hours.

Display start and stop time

Two columns, labeled Start and Stop Enter clock times.

Display hours and times

Three columns, labeled Start, Stop,
 and Hours

Enter either the number of hours or clock times for each time card row.
Entering both times and hours in a single time card row results in an
error message.

Time Entry Format for Calculated Time
For the classic, nonunified time review, view, and approval notification layouts, you need to configure two sections:

• Reported Time

• Calculated Time

If your time entry layout includes Start and Stop columns, your Calculated Time sections need to use the time entry
format Display hours and times. Calculated time always displays totals as a number measured in hours, in the summary
row.

Absence and Payroll Time Entry Format
Absence entries resolve according to the person's schedule. Select the time entry format supported for the schedule
type applicable to people who use the layout set. Here are the different schedule types with the correct formats for each.

Schedule Type

Time Entry on the Time Card

Time Entry Format to Select on the Layout

Work Schedule

Absence start and end times

Either Display start and end time or Display hours and times

Elapsed or Duration Schedule

Number of absence hours

Either Display hours only or Display hours and time

102

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Related Topics

Chapter 22
Classic Layout Configurations, Including Time Entry
Formats

• Time Entry, View, Review, Approval Notification, and Calendar Entry Layouts

• Entries Section Configuration of the Responsive UI Layout

• Create a Nonunified Payroll Layout Set That Includes Absence and Override Fields

How You Let People Submit Time Cards Containing 0
Hours Entries

Make sure that the time entry format is Display hours and time.

• To edit the time entry format, use the Layout Set task.

• To link the layout set to relevant profiles, use the Worker Time Entry Profiles task.

Both tasks are in the Time Management work area.

Create a Nonunified Payroll Layout Set That Includes
Absence and Override Fields

You want to configure how people report, change, submit, and approve payroll and absence time. You also want to let
managers include time attributes as part of shift details.

1. Complete these tasks:

a. Create the Meals Taken element and calculation components. Use the Elements task in the Elements and

Formula functional area.

b. Generate the absence management and payroll time attributes in the data dictionary. Use the Generate

Data Dictionary Time Attributes task.

c. Create the AbsencePayrollTime multiattribute field with the dependent meal, department, state, county,

and city fields. Use the Time Entry Layout Components task.

d. Create the Statutory Time for OT, Overtime, and Meals Taken US time categories. Use the Time Categories

task.

The examples in the Related Links section at the end of this topic tell you how to create the element and dependent
fields.

2. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Layout Sets.

3. Create the Absence and Payroll layout set.

a. On the Generate Layout Set page, select Responsive UI, Manager, Shift, and Payroll.
b. Make sure that Project Costing isn't selected.
c. Click Generate Layout Set.
d. On the Define Layout Set page, in the Name field, enter Payroll and Absences.
e.

In the Description field, enter Includes the row-level department field for the time entry, review,
view, and approval layouts. Includes entry-level location fields for the time entry, review, view, and

103

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 22
Classic Layout Configurations, Including Time Entry
Formats

approval layouts and meals rates on the manager layouts. Includes time and hours sliders on the
calendar layout and location fields for the shift layout.

f. Click Save.

104

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

4. Configure the time entry layout for workers.

Chapter 22
Classic Layout Configurations, Including Time Entry
Formats

a. On the Define Layout Set page, in the Time Entry Layout row, click Configure Layout.
b. On the Configure Time Entry Layout page, click the Worker tab.

Tip:  Edit the worker layout first so that the manager layout inherits the edits, which you can then revise
as required. The worker layout doesn't inherit any manager layout edits.

In the Time Entry section, click Edit Layout.

c.
d. On the Edit Layout dialog box, Time Card Matrix page, make these edits:

i. Replace the Payroll Time Type field with AbsencePayrollTime.
ii.

In the Time Entry Properties section, select these options: Enable time to span midnight and
Display unit of measure.

iii. Make sure that the time entry format is Display hours and time because it best supports the

reporting of both absence and payroll time.
In the Date Format field, select Mon,Jan 01.

iv.
v. Click Next.

e. On the Row Level Details page, make these edits:

i. Add the Department field.
ii. Change the Label on the Time Card value to Department Details.
iii. Click Next.

f. On the Comments page, make these edits:

i. Make sure that Comments column in the time card is selected.
ii. Change the Label on the Time Card value to Row-Level Comments.
iii. Click Next.

g. On the Entry Level Details page, make these edits:

i. Add these fields in the order listed: Default Payroll Rate, State, County, and City. The location fields

need to go from broadest geographic area to narrowest for time attribute filters to work.

In the Date Format field, select Mon,Jan 01.

ii. Change the Label on the Time Card value to Daily Pay Details.
iii.
iv. Click Save and Close.
v. On the Warning message asking if you want to copy your edits to the other layouts in the set, click

Yes.

Tip:  Only edits to the fields in the time card matrix and time entry properties copy to the calendar
entry and shift layouts. Edits on the row-level and entry-level pages don't copy. To include these
edits on the time review, view, and approval notification layouts, repeat the edits on the relevant
Reported Time and Calculated Time sections.

vi. On the Confirmation message, click OK.

h. On the Configure Time Entry Layout page, click the Time Totals tab.
i.
In the Time Totals section, click Edit Layout.
j. On the Edit Layout dialog box, make these edits:

In the Date Format field, select Mon,Jan 01.

i. On the Hours page, add these time categories: Statutory Time for OT and Overtime.
ii.
iii. On the Units page, add the Meals Taken US time category.
iv.
v. Click Save and Close.

In the Date Format field, select Mon,Jan 01.

105

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 22
Classic Layout Configurations, Including Time Entry
Formats

vi. On the Warning message asking if you want to copy your edits to the other layouts in the set, click

Yes.

vii. On the Confirmation message, click OK.

5. Configure the time entry layout for managers.

a. On the Configure Time Entry Layout page, click the Manager tab.
b.
c. On the Edit Layout dialog box, Entry Level Details page, make these edits.

In the Time Entry section, click Edit Layout.

i. Add the Meal Override Rate field.
ii. Select the Worker layout read only display option.
iii. Add the hidden Meal Rate Periodicity field.
iv. Click Save and Close.
v. On the Warning message asking if you want to copy your edits to the other layouts in the set, click

Yes.

vi. On the Confirmation message, click OK.

6. Configure the calendar entry layout for workers.

a. On the Configure Time Review Layout page header, in the layout list, select Calendar Entry Layout.
b. On the Configure Calendar Entry Layout page, Worker tab, click Edit Layout.
c. On the Edit Layout dialog box, select these options: Display hours slider and Display time slider.
d. Click Save and Close.

7. Configure the shift layout.

a. On the Configure Calendar Entry Layout page header, in the layout list, select Shift Layout.
b. On the Configure Shift Layout page, Worker tab, click Edit Layout.
c. On the Edit Layout dialog box, add these time card fields, in the order listed: State, County, and City. The
location fields need to go from broadest geographic area to narrowest for time attribute filters to work.

d. Click Save and Close.
e. On the Configure Shift Layout page, click Save and Close.
f. On the Edit Layout Set: Absence and Payroll page, click Save and Close.
g. On the Confirmation message, click OK.
h. On the Layout Sets page, click Done.

Related Topics

• Create the Units-Based Meals Taken Element for Time Entries

• Create the Dependent Meal Override Rate and Rate Periodicity Fields

• Create the Dependent State, County, and City Fields

• Create Time Categories Using Grouped Conditions and an Embedded Category

106

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 23
Responsive UI, Cost Overrides, Web Clock, and Shift
Layouts

23  Responsive UI, Cost Overrides, Web Clock,
and Shift Layouts

Configuration of the First Section on the Responsive UI
Layout

You can affect what people see when they show details in the first section of the nonunified responsive time card page.
Make these changes when you edit the section.

• Specify whether to show the person's start time from their assigned workday definition, if they've a definition.

• Show only the delivered time totals that are appropriate for the people using this layout. And add more time

categories to provide relevant totals for reported and calculated time.

Tip:  The Scheduled Hours total comes from the individual’s current schedule or work hours.

• Optionally change the display name and time entry properties. You can include the unit of measure in display

names, as appropriate.

Related Topics

• Time Layouts

• How an Individual's Schedule Is Identified

Entries Section Configuration of the Responsive UI
Layout

You can configure the default view, time card fields, and time entry properties for individuals and managers. Do this by
editing the Entries section of the nonunified responsive UI layout.

Default View
When individuals open a responsive time card page, by default they see the Reported Time detailed view by entry date.
When managers open a responsive time card, by default they see the Reported Time summary view by entry date. In
the Entries section, you can change these default views, for example, so managers start by seeing the calculated times.

Tip:  The Add button appears on only the Reported Time view.

107

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 23
Responsive UI, Cost Overrides, Web Clock, and Shift
Layouts

Time Card Fields
On the Reported Time and Calculated Time tabs of the layout, you can replace the default fields on the responsive time
card. You can add more nonunified and unified fields that you want to appear. And you can change display names. If
you want the complete names to appear, limit them to 70 characters or less.

You can also identify which fields to use to uniquely identify time entries tracked as part of change audits. You can
identify the fields to show in the additional attributes area of completed entries, instead of in the main area. And, you
can identify the fields that people can edit when they create change requests.

Note:  People need to edit absences using the Existing Absences task instead of the Request Change task. So, the Edit
with Change Request option is unavailable for fields with absence time attributes.

If the layout set also includes the Cost overrides layout, be sure to include the multiattribute fields with cost override
enabled for appropriate payroll values. Include the fields on the Reported Time tab so that you can configure the
dependent cost segments on the Cost overrides layout. Include the fields on the Calculated Time tab so that people can
see how calculations applied the cost overrides to calculated time entries. You can't add the cost segments themselves
to the Reported Time tab. You can add them on Calculated Time tab of the same layout or in the Cost overrides layout.

Optionally, display the entry owner and internal source. This information can be useful to people who report time
with multiple methods, such as badge reader, Web Clock, and time card. It can also be useful to managers who review
time cards with time entries from various owners and sources. Examples of time entry owners are WFM or Web Clock.
Examples of internal sources are Manager entry, Absence entry, or Calculated entry. You can also change display names.
If you want the complete names to appear, limit them to 70 characters or less.

Effect on the Responsive Time Card Page
Here's what the fields and properties you configured do:

• Form the entries on the Reported Time and Calculated Time tabs

• Group time entries in summary views

•

Identify the owner and source of individual or grouped time entries

• Appear in the expandable Additional Attributes entry area

• Comments appear as part of responsive Time Card page entries and expanded Additional Attributes area.

Related Topics

• Availability Options for Dependent Time Card Fields

• Time Layouts

• Considerations for Selecting the Time Entry Format

Cost Overrides Layout Configuration

You can configure the dependent cost override fields that appear on the nonunified cost override page that opens from
a responsive time card entry. You can also configure time entry properties.

108

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 23
Responsive UI, Cost Overrides, Web Clock, and Shift
Layouts

Add the dependent cost override fields that are linked to payroll values for the multiattribute fields you added to the
responsive UI layout. Optionally, you can change the display names. If you want the complete names to appear, limit
them to 70 characters or less.

The sequence of the fields is important for data filter dependencies. For example, your layout includes department and
fund fields. And people need to select the department to see the corresponding funds.

Optionally, you can set the time entry format, decimal precision, and date format.

Related Topics

• Time Layouts

• Configure the Dependent Field Properties

• Create the Dependent Department Field

Web Clock Layout Configuration

You can optionally let individuals report time and view daily time events using Web Clock. You configure the nonunified
and unified web clock layout using the Layout Sets task in the Time Management work area.

Web Clock Layout Configuration
You can edit the layout to make these configuration changes.

Configuration Options

Usage Description

Hide or show seconds on the clock

The digital clock appears on the web clock page with or without seconds showing.

Enable the button logic rule

Individuals either can or can't click earlier buttons after they click a button later in the sequence.

Restart sequence after last button

Either make all the buttons available again after the person clicks the last button in the sequence, or
keep the buttons unavailable.

Allow manual entry of missing In event

Individuals either have or don't have the option to manually enter the missing In event when they're
clocking out.

Enable viewing of daily time events

Individuals either can or can't see the corresponding time events in the Daily Time Events section after
they click a button. When enabled, they can see the events for the current day and day-by-day for up to
7 previous days.

Specify whether to use device or server
time

When individuals' layouts configurations use device time, validate whether the device time is within
the allowable difference with server time. If it isn't, then the time event uses server time and saves the
device time as additional event information.

Enable editing of clock time with change
request

Instead of letting individuals edit their time cards directly, let them request changes to their time and
corresponding attributes.

Buttons
You add the buttons that you want to include on the Web Clock page and optionally select an icon for each button. You
can also change the display label. If you want all the label text to show, limit the labels to 70 characters or less.

109

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 23
Responsive UI, Cost Overrides, Web Clock, and Shift
Layouts

Individuals see these button labels and icons on their Web Clock. The device that they use to open Web Clock
dynamically identifies how many buttons they see per row. For example, if they open Web Clock on their smart phones,
they probably see one button per row in portrait mode. If they use a tablet in landscape mode, they might see three or
four buttons.

Time Card Fields
Optionally, you can add any nonunified and unified time card fields that individuals need to complete. And again, you
can change the display names. If you want all the names to show, limit them to 70 characters or less.

CAUTION:  When the selected web clock buttons and fields have the same time attributes, the time repository stores
the field value and ignores the button value.

The sequence of the fields is important for data filter dependencies. For example, your layout includes location fields.
You need to select a state before you can select a county. And, you need to select the county before you select a city.

Individuals see these fields on their Web Clock, in addition to the buttons. They and their managers also see these fields
on the corresponding pages of the time cards generated from the clock events.

If individuals submit change requests instead of directly editing the corresponding time card, you also identify the
fields where they can change the values. Individuals can edit their time data for the enabled fields when they open the
Request Change page from Web Clock.

Related Topics

• Availability Options for Dependent Time Card Fields

• Time Layouts

• Create a Nonunified Payroll Layout Set That Includes Absence and Override Fields

Shift Layout Configuration

Optionally include time attributes on people's shifts by adding nonunified and unified time card fields to the shift layout.
For example, include the Department and Payroll Time Type attribute values for the shifts that use this layout.

You can also change the display labels. If you want all the names to show, limit them to 70 characters or less. Use the
Layout Sets task in the Time Management work area.

The sequence of the fields is important for data filter dependencies. For example, your layout includes location fields.
Managers need to select a state before they can select a county. And, they need to select the county before they select a
city.

Managers can enter values for these fields when they create shifts in the Time Management work area. Individuals see
the values that their managers entered when they view shift details for their team schedule in the Time work area.

Related Topics

• Time Layouts

• Availability Options for Dependent Time Card Fields

• Create a Nonunified Payroll Layout Set That Includes Absence and Override Fields

110

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 23
Responsive UI, Cost Overrides, Web Clock, and Shift
Layouts

Create a Nonunified Responsive Payroll Layout Set That
Includes Absence and Override Fields

You want to configure how people report, change, submit, and approve payroll and absence time on responsive time
cards. You also want to let managers include time attributes as part of shift details.

1. Complete these tasks:

a. Create the Meals Taken element and calculation components. Use the Elements task in the Elements and

Formula functional area.

b. Generate the absence management type and payroll time type attributes in the data dictionary. Use the

Generate Data Dictionary Time Attributes task.

c. Create the AbsencePayrollTime multiattribute field with the dependent meal, department, state, county,

and city fields. Use the Time Entry Layout Components task.

d. Create the Statutory Time for OT, Overtime, and Meals Taken US time categories. Use the Time Categories

task.

The examples in the Related Links section at the end of this topic tell you how to create the element and
dependent fields.

2. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Layout Sets.

3. Create the layout set with the responsive UI layout.

a. On the Generate Layout Set page, select Responsive UI, Manager, Shift, and Payroll.
b. Make sure that Project Costing isn't selected.
c. Click Generate Layout Set.
d. On the Define Layout Set page, in the Name field, enter Responsive Payroll and Absences.
e.

In the Description field, enter Includes the additional attribute department and location fields for the
responsive UI layouts. Includes meal rate fields on the manager layout. And includes location fields
for the shift layout.

f. Click Save.

4. Configure the top section of the responsive UI layout.

a. On the Define Layout Set page, in the Responsive UI Layout row, click Configure Layout.
b. On the Configure Responsive UI Layout page, click the Worker tab.

Tip:  Edit the worker layout first so that the manager layout inherits the edits, which you can then revise
as required. The worker layout doesn't inherit any manager layout edits.

In the top section, click Edit Layout.
In the Overtime Day Start Time section, select Show.
In the Decimal Places field, select 2.
In the Hourly Totals section, add these time categories: Statutory Time for OT and Overtime.
In the Unit Totals section, add the Meals Taken US time category.

c.
d.
e.
f.
g.
h. Click Save and Close.

111

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 23
Responsive UI, Cost Overrides, Web Clock, and Shift
Layouts

5. Configure the Entries section of the responsive UI layout for workers.

a.
b.
c.

In the Entries section, click Edit Layout.
In the Default View section, select Reported summary by entry date.
In the Time Card Fields section, make these edits:

In the Assignment Number and AbsencePayrollTime rows, select Time Entry Identifier.

i. Replace the Payroll Time Type field with AbsencePayrollTime.
ii.
iii. Add the Meal Rate Department field and select Show in Additional Attribute.
iv. Add these location fields in the order listed: Default Payroll Rate, State, County, and City. The location

fields need to go from broadest geographic area to narrowest for time attribute filters to work.
In all the location rows, select Show in Additional Attribute.

v.

d.

In the Time Entry Properties section, make these edits:

i. Select these options: Enable time to span midnight and Display unit of measure.
ii. Ensure that the time entry format is Display hours and time because it best supports the reporting

of both absence and payroll time.
In the Other fields section, make these edits:

e.

i.
ii.

In the Owner and Internal Source rows, select Display and Show in Additional Attribute.
In the Comments row, select Display and Show In Detail List View.

f. Click Save and Close.
g. On the Warning message asking if you want to copy your edits to the calculated time tab, click Yes.

6. Configure the responsive UI layout for managers.

a. On the Configure Responsive UI Layout page, click the Manager tab.
b.

In the top section, click Edit Layout.

In the Overtime Day Start Time section, select Show.

i.
ii. Click Save and Close.

In the Entries section, click Edit Layout.

c.
d. On the Edit Layout dialog box, in the Default View section, select Calculated summary by entry date.
e.

In the Time Card Fields section, make these edits:

i. Add the Meal Override Rate field.
ii. On the Configure Time Card Field Display Option dialog box, select Worker layout read only.
iii. Click OK.
iv. On the Edit Layout dialog box, add the hidden Meal Rate Periodicity field.
v. On the Configure Time Card Field Display Option dialog box, click Cancel.
vi. Click Save and Close.
vii. On the Warning message asking if you want to copy your edits to the calculated time tab, click Yes.

7. Configure the shift layout.

a. On the Configure Responsive UI Layout page header, in the layout list, select Shift Layout.
b. On the Configure Shift Layout page, Worker tab, click Edit Layout.
c. On the Edit Layout dialog box, add these time card fields, in the order listed: State, County, and City. The
location fields need to go from broadest geographic area to narrowest for time attribute filters to work.

d. Click Save and Close.
e. On the Edit Layout Set: Responsive Absence and Payroll page, click Save and Close.
f. On the Confirmation message, click OK.
g. On the Layout Sets page, click Done.

112

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Related Topics

Chapter 23
Responsive UI, Cost Overrides, Web Clock, and Shift
Layouts

• Create the Units-Based Meals Taken Element for Time Entries

• Create the Dependent Meal Override Rate and Rate Periodicity Fields

• Create the Dependent State, County, and City Fields

• Create Time Categories Using Grouped Conditions and an Embedded Category

113

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 23
Responsive UI, Cost Overrides, Web Clock, and Shift
Layouts

114

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 24
Offline Web Clock Configuration

24  Offline Web Clock Configuration

Overview of Configuring Web Clock for Offline Use

You can optionally configure Web Clock to also work offline after you configure it to work online. For example, you've
people who work remotely, so you set them up to report their time using Web Clock on their mobile devices.

They aren't always able to connect to the server when it's time for them to clock in or out. So you also let them use Web
Clock when they're offline. Their devices store their time data locally until they connect to the internet again. Then, the
local data gets synced to the time repository and processed accordingly.

Related Topics

• Time Entry Setup and Maintenance Tasks

• Web Clock Layout Configuration

• Configure the Web Clock Button Properties

• Create Shift, Break, and Meal Web Clock Buttons

Configure Web Clock for Offline Use

Here's how you can extend your Web Clock configuration so people can also use it offline.

1. Add these 2 privileges to your custom employee roles for the relevant workers:
◦ HXT_REST_SERVICE_ACCESS_TIME_LAYOUT_SETS_RO_PRIV
◦ HXT_REST_SERVICE_ACCESS_WEB_CLOCK_EVENTS_PRIV

2. Make sure that the HCM Mobile Enable Offline Web Clock profile option has the site-level profile value set to Yes.

3. Specify timeouts for authentications using these profile options:

◦ HCM Mobile Idle Timeout: Specify how many seconds workers have to sign back into the app using local

authentication. For example, if it should be 5 minutes, you'd set the site-level profile value to 300.
◦ HCM Mobile Session Timeout: Specify how many seconds workers have before they need to re-

authenticate with the server to get a new, valid online or offline session. For example, if it should be every 7
days, you'd see the site-level profile value to 604,800.

4. Have workers install the Oracle HCM Cloud app on their mobile device from either the Goggle Play Store or the Apple

Apps Store.

5. Make sure that everyone who will use Web Clock offline use it first on their device while they're online and connected

to the server. Starting online makes sure that each device successfully completes the initial data sync and can
complete future syncs.

Workers see appropriate notifications on their online Web Clocks when the sync finishes. They can then use Web
Clock online and offline to report their time. When they're online, any stored offline time data automatically syncs to
the time repository for time processing.

115

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 24
Offline Web Clock Configuration

Related Topics

• Time Entry Setup and Maintenance Tasks

• Web Clock Layout Configuration

• Configure the Web Clock Button Properties

• Create Shift, Break, and Meal Web Clock Buttons

Functionality Differences Between Online and Offline
Web Clock

Some functionality acts differently depending on whether Web Clock is online or offline.

Elapsed Time Counter
The counter for time elapsed since the most recent button tap is accurate when Web Clock is online. The counter
isn't accurate when offline. People who are offline can't use the elapsed time to make sure they're complying with
regulations. For example, they can't tell if they rested for the required periods between work periods.

Button Logic
Enabled button logic applies only when Web Clock is online. This means that when people are online the earlier buttons
they tapped are now unavailable. When they're offline, the buttons are still available. People can inadvertently tap the
same button multiple times during a day, which can cause time entry errors. People need to fix these errors before
submitting the corresponding time card. You can use time entry profiles to identify if individuals, their managers, or
both can correct the errors.

Time to Use for Clock Events
If the layout has server time enabled, it applies to only online clock events. When Web Clock is offline, the clock events
always use device time. This difference in the time used might lead to time entry errors that people need to fix before
they submit the corresponding time card.

More Fields
If the layout includes more fields for specific buttons, when Web Clock is online, people can see the fields. When Web
Clock is offline, they can't. The corresponding time card might be incomplete or in error if people don't complete these
more fields.

Data Sync Time
The time it takes to sync data between the device and the time repository is completely dependent on the device,
network bandwidth, and connection stability. To keep time events on Web Clock current, people need to let the data
sync completely when they're back online. Then they use Web Clock to report their latest time.

116

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 24
Offline Web Clock Configuration

Related Topics

• How You Set Allowable Actions for Time Entry

• Overview of Configuring Web Clock for Offline Use

• Configure Web Clock for Offline Use

117

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 24
Offline Web Clock Configuration

118

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 25
Time Processing Configurations

25  Time Processing Configurations

Best Practices for Creating Time Processing Objects

You need to create separate time processing profiles for each unique combination of the time processing objects, as
shown in this diagram. To automatically add public holiday entries to time cards, you also need separate profiles for
each LDG.

The more processing objects that you create, the greater the ongoing maintenance effort. You want to find a balance
between optimizing the time processing experience for your employees and the effort required to maintain that
experience.

Here's how the components of the time processing profile work together. The following sections provide some
guidelines and considerations to help you decide how many time processing objects to create.

119

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 25
Time Processing Configurations

The number of time consumer sets that you need depends on the time consumers needed and the unique
configurations of these options for each consumer:

• Validate on time card actions

• Time category

• Approval period

Time Consumer Sets and Time Card, Approval, and Overtime Periods
You need a separate time consumer set for each unique combination of time card, approval, and overtime periods. The
approval periods of the time consumer set need to match the time card period of the time processing profile. Each time
consumer requires a separate time processing profile.

Time Consumer Sets and Time Categories
What type of time--such as project costing, payroll, absence, or a combination--do your people report and how
often? The type of time and the reporting frequency affect how you configure time categories and time consumer

120

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 25
Time Processing Configurations

sets. Because you can link only one time category to a time consumer, we recommend that you use these delivered
categories: All Project Entries and All Payroll Entries. The delivered category All Payroll Entries includes both hours-
based and units-based time entries.

The more time categories and time consumer sets that you create, the greater the maintenance effort. Another topic
has scenarios and suggested configurations to help you assess how many of these objects you need.

Time Consumer Sets and Validate on Time Card Actions
Create one consumer set for each group of people with different settings for the time card actions that run validation for
the same time consumer. Here are examples of how you might create different Payroll time consumers depending on
the Validate on Time Card Action selection.

• Save and Submit: For people who report time every day of a time card period, or whose entries you want to

report on during the week.

• Submit only: For people who create and submit time cards at the end of their week and for time and labor

managers who correct time exceptions.

Time Categories and Time Allocations
Create as many time categories as you need to identify the time entries that you want to allocate to various cost
segments.

Time Entry and Time Calculation Rule Sets
You can link only one time entry and one time calculation rule set to a time processing profile. But, you can add as many
rules and rule sets to a rule set as appropriate for the people linked to the rule set. Use rule sets to link rules to groups of
people who have similar requirements for vacation, time validation, and time processing.

The number of rule sets you need depends on the different ways that you validate reported time and calculate time.
Here are some examples:

• You generate validation exceptions for a group of people when their total reported time exceeds 42 hours for

the week. You generate validation exceptions for another group when their total reported time exceeds 10 hours
a day.

• You pay people an overtime rate of 1.5 times their regular pay. For people working in California, the overtime
rate applies every worked hour over 8 hours in a 24-hour period. For people working in Florida, the overtime
rate applies for every hour worked over 40 hours in a 7-day period.

Change Audit and Public Holiday Settings
Create one profile for each group of people with different change audit settings. Also create one profile for each group
of people who use the same payroll element to automatically create their public holiday entries. Typically, this means
creating at least one profile for each LDG. For example, create one profile for people who use the Public Holiday US
element. Create another profile for people who use the Public Holiday CAN element. You can have more than one profile
per LDG, depending on how many unique settings you've for the other profile options.

121

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 25
Time Processing Configurations

HCM Groups
You link one or more HCM groups to each profile. Define separate groups wherever the characteristics are unique across
profiles or groups of profiles. For example, you group people into separate groups for these reasons:

• One group has people who work in states that calculate overtime daily.

• Another group has people who work in states that calculate overtime weekly.

Related Topics

• Repeating Time Periods

• Considerations for Creating Time Consumer Sets

• Validation and Processing Rules by Time Card Action

How Many Time Categories and Consumer Sets to
Create

Use these scenarios to help you figure out how many time categories and consumer sets you need to create.

Scenario

Time Category

Time Consumer Sets

Some people always report only payroll
and absence time.

Some people always report only project
costing and absence time.

Use the delivered category All Payroll Entries or your category
of relevant payroll time attributes. Absence time entries
automatically transfer to Absence Management and don't
transfer to Payroll.

Use the delivered time category All Project Entries or your
category of relevant project time attributes. Absence time
entries automatically transfer to Absence Management and
don't transfer to Project Costing.

Create a time consumer set with only
Payroll selected.

Create a time consumer set with only
Project Costing selected.

Some people regularly, but not always,
 report project costing time and always
report payroll and absence time.

Use the delivered time categories All Payroll Entries and All
Project Entries or your categories of relevant project and payroll
time attributes, respectively. Absence time entries automatically
transfer to Absence Management and don't transfer to either
Payroll or Project Costing.

Create a single time consumer set
with both Project Costing and Payroll
selected.

Some people always report only payroll
and absence time and always or often
track the number of meals that they
take.

Use the delivered category All Payroll Entries, which includes
both hours-based and units-based time entries, or your
category of relevant payroll time attributes. Absence time
entries automatically transfer to Absence Management and
don't transfer to Payroll.

Create a time consumer set with only
Payroll selected.

Related Topics

• Best Practices for Creating Time Processing Objects

• Time Processing Setup and Maintenance Tasks

122

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 26
Repeating Time Periods

26  Repeating Time Periods

Repeating Time Periods

Many organizational tasks need continually generated time periods, such as a weekly period that starts every Sunday.
You can't edit delivered periods. After saving your own periods, you can edit only the name and description.

To configure these periods, go to Setup and Maintenance > Workforce Deployment > Time and Labor > Repeating
Time Periods.

Period Usages
Here are descriptions of the repeating period usages. It also identifies the pages where the usage decides which
configured repeating periods the period lists include.

Usage

Time cards

Description

Page Where the Usage Filters Period Choices

How often people need to submit their time
card.

Worker Time Processing Profiles

When you configure a time processing profile,
you select a repeating time period as the time
card period. All time card layouts support
weekly and 2-week repeating periods. The
responsive layout also supports a monthly
repeating period.

Approvals

The date range when approvers can approve a
submitted time card, including monthly.

Time Consumer Sets

When you configure a time consumer set, you
select a repeating time period as the approval
period.

Accrual Processing

The interval when people accrue time, such as
every 2 weeks within an annual accrual term.

Manage Absence Plans

Use these periods when you create absence
plans.

Overtime

The date range used to calculate overtime.

Worker Time Processing Profiles

A person's overtime period can match or
differ from the time card period. For example,
 your people report time using time cards
with a weekly period that starts on Saturdays.
You calculate their overtime using a weekly
overtime period that starts on Mondays.

123

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 26
Repeating Time Periods

Usage

Balances

Description

Page Where the Usage Filters Period Choices

The date range used to calculate time balances.
For example, add 6 hours to a vacation balance
every pay period.

Time Balance Dimensions

Related Topics

• Delivered Repeating Time Periods

Delivered Repeating Time Periods

Delivered time consumer sets and time processing profiles use delivered repeating periods. You can also use them in
time processing configurations.

Name

Usages

Period Type

Period Length

Biweekly Starting Monday

Time Card

Weekly

Biweekly

Approval

Accrual Processing

Daily

Balances

Monthly Accrual Processing Period Accrual Processing

Payroll Weekly Starting Monday

Time Card

Projects and Payroll Weekly
Starting Monday

Approval

Accrual Processing

Projects Weekly Starting Monday
Weekly Starting Sunday

Daily

Monthly

Weekly

1 Day

Calendar month

1 week

Semimonthly

Accrual Processing

Semimonthly

Related Topics

• Repeating Time Periods

Examples of Generated Repeating Time Periods

You use repeating time periods with time cards, approvals, accrual processing, overtime, and balances. The combination
of period usage, type and length, and sample start date decide the generated periods.

124

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 26
Repeating Time Periods

Create these periods using the Repeating Time Periods task in the Setup and Maintenance work area. The task is part of
the Workforce Deployment offering, Time and Labor functional area.

These examples show you how the sample start date works with the period type and length to generate repeating
periods within the preview period dates. The preview start dates let you review your repeating period configuration
without generating the actual repeating time periods. The first preview period generated might or might match the
sample start date. It depends on how you configured the preview period.

Weekly Period with a Biweekly Length
The sample start date is 05/01/12 and the preview period start and end dates are 01/01/12 and 05/31/12. The period
generation logic generates periods every 14 days from the sample start date. All periods start on the same day of the
week, for example:

• 01/10/23 to 01/23/12

• 01/24/12 to 02/06/12

• 02/07/12 to 02/20/12

• 02/21/12 to 03/05/12

• 03/06/12 to 03/19/12

• 03/20/12 to 04/02/12

• 04/03/12 to 04/16/12

• 04/17/12 to 04/30/12

• 05/01/12 to 05/14/12

• 05/15/12 to 05/28/12

Monthly Period with a Calendar Month Length
The sample start date is 05/04/12 and the preview period start and end dates are 01/01/12 and 07/31/12. The period
generation logic generates periods from a specified day in 1 month up to that day in the following month, for example:

• 01/04/12 to 02/03/12

• 02/04/12 to 03/03/12

• 03/04/12 to 04/03/12

• 04/04/12 to 05/03/12

• 05/04/12 to 06/03/12

• 06/04/12 to 07/03/12

Semimonthly Period
The sample start date is 05/04/12 and the preview period start and end dates are05/01/12 and 07/31/12. The period
generation logic generates periods using a pattern:

• The first of the semimonthly periods starts on the numeric day of the pattern starting date and lasts for 15 days.

• The second period starts the day after the first period ends. It lasts through the day before the numeric day of

the pattern starting date in the next month.

125

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Here are examples:

• 05/05/12 to 05/18/12

• 05/19/12 to 06/03/12

• 06/04/12 to 06/18/12

• 06/19/12 to 07/03/12

• 07/04/12 to 07/18/12

Chapter 26
Repeating Time Periods

126

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 27
Time Consumer Validation, Approval, and Transfer

27  Time Consumer Validation, Approval, and
Transfer

Time Consumer Sets

Typically, other applications use, or consume, your time data in their processes. These are the other Oracle Cloud
products and offering that consume time data from Time and Labor:

• Global Payroll, to pay people

• Project Costing, to bill customers for time worked on projects

• Project Execution Management offering of Project Portfolio Management, to figure out staffing for projects

You identify the consumers that consume time data for specific groups of people using a time consumer set. The set
is also how you configure the consumer validation rules, approval periods, and transfer rules that apply for the linked
groups. Link a time consumer set with groups using time processing profiles, as shown here.

127

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 27
Time Consumer Validation, Approval, and Transfer

Tip:  You can't edit any time consumer sets associated with a worker time processing profile. Also, after you save
a new time consumer set, you can't include new time consumers in the set. And you can't exclude existing time
consumers from it.

Related Topics

• Delivered Time Consumer Sets

• Considerations for Creating Time Consumer Sets

128

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 27
Time Consumer Validation, Approval, and Transfer

Delivered Time Consumer Sets

The delivered time processing profiles use these delivered time consumer sets. You can also use them in your own time
processing profiles.

Delivered Consumer Set

Description

Payroll Only

Applies to only time entries identified by the delivered All Payroll Entries time category

Project Execution Management Only

Applies to only time entries identified by the delivered All Absence Entries time category

Projects and Payroll

Applies to only time entries identified by the delivered All Project Entries time category for Project
Costing

Applies to only time entries identified by the delivered All Absence Entries time category for Project
Execution Management

Applies to only time entries identified by the delivered All Payroll Entries time category for Payroll

Projects Only

Applies to only time entries identified by the All Project Entries time category

To quickly find these time consumer sets, in the Description field, search for Delivered. To save time when creating
your own consumer sets, duplicate the delivered set that most closely meets your needs. Then, edit the duplicate set to
support your time processing policies.

Related Topics

• Time Consumer Sets

• Delivered Repeating Time Periods

• Delivered Time Categories

Considerations for Creating Time Consumer Sets

To create time consumer sets, go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time
Consumer Set.

Time Consumer
Start by selecting the relevant time data consumers.

• Global Payroll, to pay people

• Project Costing, to bill customers for time worked on projects

• Project Execution Management offering of Project Portfolio Management, to figure out staffing for projects

129

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 27
Time Consumer Validation, Approval, and Transfer

Enable Informational Workflow for Bulk Time Card Submission
Specify whether to notify everyone affected across the selected time consumers when managers generate or submit
and approve bunches of time data at one time. You might want to select No if you regularly submit and approve many
time cards at one time.

Time Category
Select the time category that identifies the time data to transfer to the time consumer. For example, payroll doesn't want
time data with project attributes, so you select a time category that identifies only payroll-related data. Project execution
management automatically uses the All Absence Entries category.

Validate on Time Card Actions
You specify the time card actions that start consumer validations for the time data identified by the selected time
category.

• Submit Only: This default selection validates relevant time data when someone clicks Next on classic time cards

or Submit on responsive time cards. Validation doesn't run when they click Save.

• Submit and Save: This selection validates relevant time data when someone clicks and of these actions on a

time card: Save, Save and Close, Next, or Submit.

For Project Costing, we recommend that you select this option. That way people working on time cards know
immediately if they're saving time entries to closed projects.

Required Time Card Status
This option is for reporting purposes.

• Select Yes to report on missing time cards for the people linked to this consumer set, and who regularly submit

them.

• Select No if the consumer set is for groups of people who submit time cards sporadically, such as to report

absences, training, and other exceptions.

Related Topics

• Validation and Processing Rules by Time Card Action

Approval Options in Time Consumer Sets

Here are the various approval options you configure when you create time consumer sets.

Watch video

130

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 27
Time Consumer Validation, Approval, and Transfer

Enable Informational Approval Workflow for Workers
You can send people approval notifications that let them approve or reject their time card. Their approval or reject is
acceptance or repudiation of the time card data. This worker approval workflow is separate from the manager approval
task and doesn't affect the time card status or processing.

Absence Approval Routing
Specify how you want to handle approvals for absence entries on time cards. The setting applies to all selected time
consumers.

• Absence approval rules: The approval process uses the absence approval task to approve absence entries. It

uses the time card approval task to approve worked time entries. The process approves the time card after both
approval tasks complete.

• Time approval rules: The approval process uses the time card approval tasks to approve all time card entries,
including absences. To include absences from time cards with only project and absence attributes, you also
need to select the Payroll and Project Execution Management time consumers. The time card approval
workflow for payroll handles absence approvals. And, all absence data transfers only to project execution
management. No absence data transfers to project costing.

Approval Period
To define the approval period for the time consumer, select a repeating time period. For example, you want approvers to
approve the time card once every week, so you select a repeating period with a weekly definition.

CAUTION:  The approval period that you select for each consumer must match the time card period set in the time
processing profile containing the consumer set. Otherwise, you might get errors when you try to link groups to the
profile.

Entry-Level Approval
If you want approvers to see only the time card entries that they need to approve, select this option. If you want
approvers to see all time card entries, even those that they can't approve, don't select this option.

Time Data for Approval Rules to Evaluate
Specify the time card data that approval rules should evaluate, either reported time or calculated time with reported
absences. If you select entry-level approval for the time consumer, then approval rules can only evaluate reported time.

Required Approval Configuration
Specify whether other time consumers in the set must approve the time card before the time data can transfer to this
time consumer. For example, the payroll department wants only the payroll time data approved by both project costing
and payroll time approvers.

131

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 27
Time Consumer Validation, Approval, and Transfer

Related Topics

• Overview of Time Approval Workflows Configuration

• How Default Time Card and Time Entry Approvals Work

• Considerations for Creating Time Consumer Sets

• Validation and Processing Rules by Time Card Action

How Default Time Card and Time Entry Approvals Work

When you submit a time card that has project, payroll, or project and payroll data, you start approval workflows. These
workflows are for either the time card or the time card entries, depending on the corresponding time processing
configuration.

Time Card Level Approvals
Here's what happens with the default approval workflows for time cards:

• For project time data, the workflow tries to figure out the appropriate project manager. If it can figure out who
that person is, it routes the data to them to review and approve or reject. If it can't figure who that person is, it
routes the data to the individual's line manager to review and approve or reject.

• For payroll time data, the workflow checks the total payroll time. If it's up to or 40 hours, the workflow

automatically approves the data. If it's more than 40 hours, it routes the data to the individual's line manager to
review and approve or reject.

Here's how the default workflow handles approvals, rejections, and notifications:

•

•

•

It changes the time card status to Approved after all approvers approve the time card. The relevant time card
data is ready for transfer to Project Costing or Payroll.

It changes the time card status to Rejected if at least one of the approvers rejects the time card.

It lets the individual know whether the approver approved or rejected their time card.

132

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 27
Time Consumer Validation, Approval, and Transfer

Here's a workflow diagram that shows you the default approval behavior for time cards.

133

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 27
Time Consumer Validation, Approval, and Transfer

Time Entry Level Approvals
These default approval workflows for time card entries are similar, but not identical to the time-card-level workflows.
The big difference is when the time data is ready for transfer to project costing and payroll.

• For project time data, the workflow tries to figure out the appropriate project manager. If it can figure out who
that person is, it routes the data to them to review and approve or reject. If it can't figure who that person is, it
routes the data to the individual's line manager to review and approve or reject.
Approved data is ready for transfer to Project Costing.

• For payroll time data, the workflow routes the data to the individual's line manager to review and approve or

reject. The applicable approvers need to approve all entries for the time card period before the data is ready for
transfer to Payroll.

Related Topics

• Repeating Time Periods

• Overview of Time Approval Workflows Configuration

• Considerations for Creating Time Consumer Sets

• How You Define Approvals for Human Capital Management

• How You Manage HCM Approval Transactions

Validation and Processing Rules by Time Card Action

Time consumers, such as absence management, payroll, and project costing, deliver validation rules that apply to time
card data. For example, absence validations make sure that absence entries are for only those absence types that the
person is eligible for.

Here's the validation and processing associated with the main time card buttons.

Button

Next

Validation and Processing Description

• Validates absence, payroll, and project time entries

• Applies time entry rules, as specified by rule configuration

• Applies time calculation rules, including any allocation rules, as specified by rule configuration

• Generates calculated time entries

Save

Save and Close

• Always starts the delivered absence validations

• By default, doesn't start the delivered project and payroll validations

You configure validation on the save buttons using the Time Consumer Sets task. In the Validate on
Time Card Actions field, select Submit and save. Validations on the save buttons are then identical to
those described for the Next button.

For Project Costing, we recommend that you select Submit and save. That way people working on
time cards know immediately if they're saving time entries to closed projects.

Submit

Sets the time card status to Submitted and starts the approval workflow

134

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 27
Time Consumer Validation, Approval, and Transfer

135

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 27
Time Consumer Validation, Approval, and Transfer

136

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 28
Time Card and Entry Approval Workflows

28  Time Card and Entry Approval Workflows

Overview of Time Approval Workflows Configuration

Send time card data for project costing or payroll to the appropriate approvers using approval workflow tasks. Configure
the workflows to support your approval policies using these tasks in the Define Approval Management for Human
Capital Management task list:

• Manage Task Configurations for Human Capital Management: You configure the associated rules and rule sets
on the Assignees tab. On the Configuration tab, the Once per stage task aggregation ensures that the approval
process sends only one notification per approver.

• Manage Approval Groups: By default, the actionable time card approval workflow tasks route time cards using
the dynamically decided supervisor hierarchy. You can identify specific approvers to route to instead using this
task. The informational workflow task sends the notification to the individual on the time card.

To search for the task list, on the Setup and Maintenance work area, Tasks panel tab, click Search.

Stages and Layers
Workflow tasks for time approval have two stages and the payloads have two layers. These stages and layers link to
header-level and line-level approvals, respectively.

• Header-level approvals have the ApprovalTimeRecordHeader payload layer and the Serial participant type. The

approvals include the total number of hours.

• Line-level approvals have the ApprovalTimeRecordGroup payload layer and the Parallel participant type. So,
the line-level rules always run in parallel for each line. The approvals include individual hours and time-card-
related attributes, such as Expenditure Type or Payroll Time Type. ApprovalTimeRecordGroup attribute values
vary by implementation. To figure out your value mapping, create your own data model report in the Reports
and Analytics work area using this query:

select * from FUSION.hxt_tm_col_attr_map where LOCATION like 'Approval' and ENTERPRISE_ID = <ent_id>;

Related Time Object Configurations
These time objects include settings that affect approval workflow:

• Worker Time Entry Profile: You specify when people can change time cards during approval processing.

• Repeating Time Periods: You also configure time periods that continually generate, such as weekly periods that

start on Sunday. You can use these periods with time data approvals.

• Time Consumer Sets: You can specify whether to notify everyone affected across the selected time consumers
when managers submit and approve bunches of time data at one time. Also specify which time card actions
start checks and rules. For example, specify which time category, approval period, and transfer rules to use. And
specify whether to handle approvals at the time card or time entry level.

137

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 28
Time Card and Entry Approval Workflows

Related Topics

• Payroll Time Approval Workflow Tasks

• Project Costing Time Approval Workflow Tasks

• Considerations for Creating Time Consumer Sets

• How You Define Approvals for Human Capital Management

• How You Manage HCM Approval Transactions

Payroll Time Approval Workflow Tasks

Time consumer sets with Payroll selected start these approval tasks. The ELA task starts when the payroll consumer
configuration uses entry-level approval.

Here's what the actionable tasks do:

TimeCardApproval

TimecardApprovalELA

Supports header-level and line-level
approval configurations that use payroll
data on the time card, for the specified
individual and time card period.

Notifies the configured approvers to
approve or reject the time entries that
they're responsible for. The approvers see
all payroll time data, even the data that
they don't approve.

Notifies specified recipients based on
time card status, for example, notifies
individuals when approvers approve or
reject their time cards.

Supports line-level approval configurations that use payroll data on the time card, for the specified
individual and time card period.

Notifies the configured approvers to approve or reject only the time entries that they're responsible for.
Approvers see only the payroll time data that they approve. Payroll data for the time card isn't ready for
transfer until all time card entries are approved.

Notifies specified recipients based on time entry status, for example, let's individuals whether
approvers approved or rejected their time entry.

By default, the TimeCardApproval task evaluates payroll time entries only when the entire time card is ready for
approval.

CAUTION:  To avoid issues with approval routing for the TimeCardApproval task, TimeEntryApprovalRuleSet and
TimecardApprovalRules must each have either an active rule or call IgnoreParticipant.

The TimeCardApprovalFYI task notifies individuals when approvers approve or reject their time entries for the specified
time card period. You can disable this task so that individuals don't get notified about approved or rejected time cards.
Because this task isn't rule based, you can't configure it to disable only one notification. For example, you can't disable
the notification about approved time cards while keeping enabled the notification about rejected time cards.

How to Set Ignore Participant
Here's how you set Ignore Participant:

1. On the Assignees tab, click the appropriate participant.
2.

In the participant configuration pane at the bottom, click Advanced.

138

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 28
Time Card and Entry Approval Workflows

3. Select Ignore Participant.
4. On the Tasks to be configured header, click Save.

Related Topics

• Overview of Time Approval Workflows Configuration

• Example of Payroll Time Approval Rules Using Payroll Values

• Example of Payroll Time Approval Rules Using Time Entry Source

• Example of Payroll Time Approval Rules Using Reported Time and Cost Segment

• Example of Payroll Time Approval Rules Using Calculated Time and Cost Segment

Project Costing Time Approval Workflow Tasks

Time consumer sets with Project Costing selected start these approval tasks. The ELA task starts when the project
costing consumer configuration uses entry-level approval.

The approval flow builds the list of project approvers using the project managers defined in Project Portfolio
Management. Here's what these approval tasks do.

ProjectTimeCardApproval

ProjectTimecardApprovalELA

Supports header-level and line-level
approval configurations that use project
data from the time card, for the specified
individual and time card period.

Notifies the configured approvers to
approve or reject the time entries that
they're responsible for. The approvers see
all project time data from the time card,
 even the data that they don't approve.

Notifies specified recipients based on
time card status, for example, notifies
individuals when approvers approve or
reject their time cards.

Supports line-level approval configurations that use project data on the time card, for the specified
individual and time card period.

Notifies the configured approvers to approve or reject only the time entries that they're responsible for.
Approvers see only the project time data that they approve. Project data for the time entry is ready to
transfer as soon as the approver approves the entry.

Notifies specified recipients based on time entry status, for example, lets individuals whether
approvers approved or rejected their time entries.

By default, the ProjectTimeCardApproval task evaluates project time entries only when the entire time card is ready for
approval.

CAUTION:  To avoid issues with approval routing for the ProjectTimeCardApproval task, TimecardApprovalRuleSet,
ProjectTimecardApprovalRules, and ProjectTimeCardLineManagerRuleset must each have either an active rule or the
call IgnoreParticipant.

How to Set Ignore Participant
Here's how you set Ignore Participant:

1. On the Assignees tab, click the appropriate participant.
2.

In the participant configuration pane at the bottom, click Advanced.

139

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 28
Time Card and Entry Approval Workflows

3. Select Ignore Participant.
4. On the Tasks to be configured header, click Save.

Related Topics

• Overview of Time Approval Workflows Configuration

• Payroll Time Approval Workflow Tasks

Example of Payroll Time Approval Rules Using Payroll
Values

You want line managers to review and approve any time cards with overtime hours. And you want to automatically
approve any time cards with only regular hours.

Here are the key configuration assumptions for this scenario:

• The environment has the Payroll Time Type attribute value Overtime.

• The relevant time consumer set has one of these rule configurations for payroll approval:

◦ Uses reported time data when individuals can report overtime hours
◦ Uses calculated time data when calculating overtime from other reported time

1. For the delivered TimecardApproval workflow task, TimeEntryApprovalRuleSet, click the Assignees tab.

2. Create the rule to manually approve overtime.

a. Create this IF expression:

ApprovalTimeRecordGroup.measure more than 0 and ( ApprovalTimeRecordGroup.attributeChar5 is
 "Overtime" )

b. Complete the THEN fields, as shown in this table.

THEN Field

Value

List Builder

Response Type

Supervisory

Required

This response type makes the notification actionable, instead of informational.

Number of levels

1

Starting Participant

Top Participant

HierarchyBuilder.getManager("supervisory",
Task.payload.process.Requester,-1,null,null)

HierarchyBuilder.getManager("supervisory",
Task.payload.process.Requester,-1,null,null)

Auto Action Enabled

False

140

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 28
Time Card and Entry Approval Workflows

THEN Field

Auto Action

Rule Name

Value

null

ManApproveOT

3. Create the rule to automatically approve time cards with only regular hours.

a. Create this IF expression:

ApprovalTimeRecordGroup.attributeChar5 isn't "Overtime"

b. Complete the THEN fields, as shown in this table.

THEN Field

Value

List Builder

Response Type

Supervisory

Required

Number of levels

1

Starting Participant

Top Participant

HierarchyBuilder.getManager("supervisory",
Task.payload.process.Requester,-1,null,null)

HierarchyBuilder.getManager("supervisory",
Task.payload.process.Requester,-1,null,null)

Auto Action Enabled

True

Auto Action

Rule Name

"APPROVE"

AutoApproveReg

Related Topics

• How Default Time Card and Time Entry Approvals Work

• Overview of Time Approval Workflows Configuration

• Approval Options in Time Consumer Sets

• Payroll Time Approval Workflow Tasks

Example of Payroll Time Approval Rules Using Time
Entry Source

You want to automatically approved time cards where all entries come from a time collection device. And you want two
levels of managers to review and approve any time cards with entries that don't come from time collection devices.

1. For the delivered TimecardApproval workflow task, TimeEntryApprovalRuleSet, click the Assignees tab.

141

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 28
Time Card and Entry Approval Workflows

2. Create the rule to automatically approve time cards with entries from only time collection devices.

a. Create this IF expression:

ApprovalTimeRecordGroup.attributeChar18 is "ORA_HWM_TIME_COLLECTION_DEVICE"

b. Complete the THEN fields, as shown in this table.

THEN Field

Value

List Builder

Response Type

Supervisory

Required

Number of levels

1

Starting Participant

Top Participant

HierarchyBuilder.getManager("supervisory",
Task.payload.process.Requester,-1,null,null)

HierarchyBuilder.getManager("supervisory",
Task.payload.process.Requester,-1,null,null)

Auto Action Enabled

True

Auto Action

Rule Name

"APPROVE"

AutoApproveTCD

3. Create the rule to manually approve time cards with entries that don't come from time collection devices.

a. Create this IF expression:

ApprovalTimeRecordGroup.attributeChar18 isn't "ORA_HWM_TIME_COLLECTION_DEVICE"

b. Complete the THEN fields, as shown in this table.

THEN Field

Value

List Builder

Response Type

Supervisory

Required

Number of levels

2

Starting Participant

Top Participant

Auto Action Enabled

Auto Action

Rule Name

HierarchyBuilder.getManager("supervisory",
Task.payload.process.Requester,-1,null,null)

HierarchyBuilder.getManager("supervisory",
Task.payload.process.Requester,-1,null,null)

False

null

ManApproveNonTCD

142

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 28
Time Card and Entry Approval Workflows

Related Topics

• How Default Time Card and Time Entry Approvals Work

• Overview of Time Approval Workflows Configuration

• Approval Options in Time Consumer Sets

• Payroll Time Approval Workflow Tasks

Example of Payroll Time Approval Rules Using Reported
Time and Cost Segment

You want to send line managers actionable notifications to review and approve time card entries. And you want to send
department managers informational notifications for any time entries associated with their departments.

Key configuration assumption: The relevant time consumer set configuration has payroll approval rules set to use
reported, instead of calculated, time data.

1. For the delivered TimecardApproval workflow task, imeEntryApprovalRuleSet, click the Assignees tab.

2. Create the actionable notification rule for line managers.

a. Create this IF expression:

1 is 1

b. Complete the THEN fields, as shown in this table.

THEN Field

Value

List Builder

Response Type

Supervisory

Required

This makes the notification actionable, instead of informational.

Number of levels

1

Starting Participant

Top Participant

Auto Action Enabled

Auto Action

Rule Name

HierarchyBuilder.getManager("supervisory",
Task.payload.process.Requester,-1,null,null)

HierarchyBuilder.getManager("supervisory",
Task.payload.process.Requester,-1,null,null)

False

null

ActionLineMgrs

143

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 28
Time Card and Entry Approval Workflows

3. Create the informational notification rule for relevant department managers.

a. Create this IF expression:

ApprovalTimeRecordGroup.entryDepartmentManager ins't ""

b. Complete the THEN fields, as shown in this table.

THEN Field

Value

List Builder

Supervisory

Response Type

Number of levels

Starting Participant

Top Participant

Auto Action Enabled

Auto Action

Rule Name

FYI

1

HierarchyBuilder.getPrincipal
(ApprovalTimeRecordGroup.entryDepartmentManager,-1,"","")

HierarchyBuilder.getPrincipal
(ApprovalTimeRecordGroup.entryDepartmentManager,-1,"","")

False

null

InfoDeptMgrs

Related Topics

• How Default Time Card and Time Entry Approvals Work

• Overview of Time Approval Workflows Configuration

• Approval Options in Time Consumer Sets

• Payroll Time Approval Workflow Tasks

Example of Payroll Time Approval Rules Using Calculated
Time and Cost Segment

You want to send line managers actionable notifications to review and approve calculated time card entries. And you
want to send department managers informational notifications for any reported time entries associated with their
departments.

Key configuration assumption: The relevant time consumer set configuration has payroll approval rules set to use
calculated, instead of reported, time data.

1. For the delivered TimecardApproval workflow task, TimeEntryApprovalRuleSet, click the Assignees tab.

144

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 28
Time Card and Entry Approval Workflows

2. Create the actionable notification rule for line managers using calculated time data.

a. Create this IF expression:

1 is 1

b. Complete the THEN fields, as shown in this table.

THEN Field

Value

List Builder

Response Type

Supervisory

Required

This response type makes the notification an actionable, rather than informational,

 notification.

Number of levels

1

Starting Participant

Top Participant

Auto Action Enabled

Auto Action

Rule Name

HierarchyBuilder.getManager("supervisory",
Task.payload.process.Requester,-1,null,null)

HierarchyBuilder.getManager("supervisory",
Task.payload.process.Requester,-1,null,null)

False

null

ActionLineMgrsCalcTime

3. Create the informational notification rule for relevant department managers.

a. Create this IF expression:

ApprovalTimeRecordGroup.entryDepartmentManager isn't ""

b. Complete the THEN fields, as shown in this table.

THEN Field

Value

List Builder

Supervisory

Response Type

Number of levels

Starting Participant

Top Participant

FYI

1

HierarchyBuilder.getPrincipal
(ApprovalTimeRecordGroup.entryDepartmentManager,-1,"","")

HierarchyBuilder.getPrincipal
(ApprovalTimeRecordGroup.entryDepartmentManager,-1,"","")

Auto Action Enabled

False

145

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 28
Time Card and Entry Approval Workflows

THEN Field

Auto Action

Rule Name

Value

null

InfoDeptMgrsReptTime

Related Topics

• How Default Time Card and Time Entry Approvals Work

• Overview of Time Approval Workflows Configuration

• Approval Options in Time Consumer Sets

• Payroll Time Approval Workflow Tasks

Ensure Workers Get Only Completed Time Card Approval
Notifications with Approval Comments

By default, workers get the delivered TimecardApprovalFYI notification when their time cards are approved or rejected.
Those notifications don’t include approval comments. Here’s how they can get only an approval or rejection notification
with approver comments.

1. Go to Setup and Maintenance > Tasks panel Search >  Manage Task Configurations for Human Capital

Management.

2. On the BPM Worklist page, make sure Task Configuration is selected.

3.

In the Search field, enter Time (no space after the term).

4. Run the search. Here are the approval tasks you should see listed.

Time Consumer

Approval Task

Information

Payroll

Payroll

TimecardApproval

When ELA isn't enabled for the assigned Time Consumer

TimecardApprovalELA

When ELA is enabled for the assigned Time Consumer

Project Costing

ProjectTimecardApproval

When ELA isn't enabled for the assigned Time Consumer

Project Costing

ProjectTimecardApprovalELA

When ELA is enabled for the assigned Time Consumer

Worker FYI Notification

TimecardApprovalFYI

Delivered FYI notification that can be set Inactive so workers only get
the completed approver notification that contains approval comments

5. So workers see only the completed notification with approval comment, disable the delivered Worker FYI notification.

That notification doesn't include any approval comments. Here's how to disable the FYI notification:

a. Select TimecardApprovalFYI. When the task is selected, the task displays in the right region of the page.
b. On the search toolbar, click the Edit icon.
c. On the Assignees tab, select the SoaOlabel.Time box. The box turns blue when selected.
d.
e. Select the Ignore Participant option.

In the SoaOlabel.Timecard Submitter section, click Advanced.

146

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 28
Time Card and Entry Approval Workflows

f. Save icon your changes and optionally enter a comment.
g. To complete the update to the task, commit your changes.

6. Enable the approval notification to route the completed approval notification with comments to the approval
initiator. For time card approval purposes, the initiator is always the worker the time card is for. Here's how:

a. On the BPM Worklist page, search for and select the task, such as TimecardApproval.
b. On the search toolbar, click the Edit icon.
c. On the Notifications tab, in the table, add a row.
In the Task Status column, select Complete.
d.
e.
In the Recipient column, select Initiator. The row then shows as Complete and Creator.
f. Save your changes.
g. Optionally enter a comment about the changes.
h. Commit your changes.

147

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 28
Time Card and Entry Approval Workflows

148

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 29
Time Formulas and Rule Components

29  Time Formulas and Rule Components

How Formulas and Time Rule Components Work
Together

One way that you can configure time validation, processing, and compliance is with fast formulas. You create rules
based on formulas using rule templates. Then, you group rules of the same type into rule sets.

Here's what this relationship among formulas, rule templates, rules, and rule sets look like.

149

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 29
Time Formulas and Rule Components

150

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 29
Time Formulas and Rule Components

Formula
Formulas contain the logic for processing time. You can associate a formula with more than one rule template. For
example, in the diagram the Hours Rounding rule template uses the Rounding formula. And, the Daily Summation and
Time-Card Level Summation rule templates use the Threshold formula.

Rule Templates
Rule templates are tools that simplify the adaptation of formulas into rules. A template exposes the exact parameters
that the associated formula requires and the outputs that the formula uses to return results. For example, a time
calculation rule template can have an overtime threshold parameter. And, it can return Payroll Time Type attributes,
such as Regular and Overtime, as outputs.

You can use one formula with multiple rule templates by varying the template configuration. For example, the diagram
shows how the Daily Summation rule template uses the Threshold formula to calculate daily totals. The Time-Card Level
Summation template uses the same formula to calculate totals for the time card period.

Rules
When you create a rule, you select a template to use rather than a formula. For example, in the diagram, the Round To
Nearest Hour rule was created with the Hours Rounding template. The template automatically populates the description
of all outputs and helps you enter correct parameter values.

You can create multiple rules from a single template, varying the parameter and output values of each rule. For example,
the diagram has two rules, 8h Daily Threshold and 12h Daily Threshold, that were created with the Daily Summation
template.

Rule Sets
You create a collection of rules and rule sets of the same type. You then assign these rule sets to groups of people with
similar requirements for vacation, time validation, and time processing. For example, in the diagram the Nearest Hour,
8h Daily Threshold rule set has the Round To Nearest Hour and 8h Daily Threshold rules. The 8h, 12h, Daily Thresholds
rule set has the 8h and 12h daily threshold rules. And, the 8h, 12h, 40h Thresholds rule set has the 2 daily and 1 weekly
threshold rules.

You assign rule sets to an individual or group of people using worker time entry, processing, and device processing
profiles.

References
To access the Workforce Management database items spreadsheet and information about array processing formula,
including annotated examples, see the Time and Labor Fast Formula References (document ID 1990057.1).

Related Topics

• Time Formula and Rule Types

• Overview of Allocating Time to Cost Segments

• How You Configure Resource Alert Notifications for Time Exceptions

151

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 29
Time Formulas and Rule Components

Time Formula and Rule Types

You configure time validations, processing, and compliance using these types of formula, rule templates, rules, and rule
sets.

Formula and Template Type

Description

Example Rule Usages

Advanced time category

Time calculation

Time device

Time entry

Time submission

Workforce compliance

Defines advanced conditions that you then
associate with a time category.

Create rules to find time events or time entries
that don't match published schedule times.

Creates or updates time card entries and uses
the data to create calculated results based on
formula logic.

Handle overtime or premium pay by updating
reported time or creating more calculated time.

Evaluates time events imported from time
collection devices and creates time entry
exceptions.

Create exceptions for time entries with start
time, or stop time, or both outside the specified
grace periods.

Validates time card entries and generates a
message with a defined severity.

When reported time exceeds a specified weekly
maximum, display the specified message.

Identifies when to automatically save and
submit time card entries created with time
events imported from time collection devices.

Identifies upcoming compliance exceptions by
reviewing time card data and unprocessed time
events to help you prevent or quickly fix any
exceptions.

Automatically save a time card after each Out
event. Automatically submit a time card after
receiving the Out event for the last scheduled
shift of the week.

Notify managers when young people are
approaching mandated worked time limits.

References
To access the Workforce Management database items spreadsheet and information about array processing formula,
including annotated examples, see the Time and Labor Fast Formula References (document ID 1990057.1).

Related Topics

• Formula Contexts for Workforce Management

• Workforce Management Functions

•

Input Attributes for Workforce Management Fast Formulas

Time Entry Owner and Internal Source in Calculation
Rules

When you create time calculation rules, you can specify whether the calculated time should keep the owner and internal
source from the reported time.

152

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 29
Time Formulas and Rule Components

For example, a person badges in at the start of the workday. Then they badge out 2 hours later than their schedule has
them stopping for the day. Here's what the associated calculation rules do:

• A rule reduces the regular time to account for the standard 1 hour, unpaid meal break. Another rule converts the
remaining 2 hours of regular time to overtime. Both rule configurations keep the original source, even though
the rules are calculating the entries from the reported time.

• Yet another rule adds 1 hour of premium time. This rule configuration overwrites the original source to show

that the entry is a calculation result.

Type of Time

Start Time

End Time

Quantity

Payroll Time Type

Internal Source

Reported

8:00a

Calculated

8:00a

5:00p

NA

7:00p

5:00p

7:00p

11h

8h

2h

1h

Regular

Regular

Overtime

Premium

TCD

TCD

TCD

Calculated entry

To keep or change the owner and internal source, the selected calculation rule template needs these attributes
configured in the relevant output groups. You can't add these attributes to calculation rule templates already in use, but
here's what you can do:

1. Check your existing rule to see what template it was created with.
2. Duplicate the original template.
3. On the Outputs page of the new template, add the Owner, Internal Source, or both attributes as user-defined

rows in the relevant output groups.

4. Create the rule again, this time using the new template and specifying whether to change or keep the

appropriate output.

153

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 29
Time Formulas and Rule Components

154

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 30
Rule Template Options

30  Rule Template Options

Options to Configure Time Rule Templates

You configure various options when you create time rule templates. Go to My Client Groups > Time Management >
Rule Templates.

Here are the options that you can configure for each template type.

Option

Template Type with the Option

Rule Classification

Default Allocation

All except advanced time category

Time calculation after you select a time allocation formula

Rule Type Execution

Time calculation if the selected formula references it

Summation Level

Reporting Level

Time calculation, device, entry, and submission if the selected formula references it

Time device, time entry, and workforce compliance if the selected formula references it

Suppress Duplicate Messages Display

Time device, time entry, and workforce compliance if the selected formula references it

Process Empty Time Card

Time entry if the selected formula references it

Time Card Events That Trigger

Time calculation and entry

Related Topics

• How You Analyze Processing Details for Time Rules and Rule Sets

• Formula Parameters in Time Rule Templates and Rules

• Formula Outputs in Time Rule Templates and Rules

Rule Classification Option for Time Rule Templates

The optional rule classification is the subtype within the template type. The list values vary among the template types.
Examples include Business message, Comparison validation, Variance, Supplier event, and Hours entered.

You can set the rule classification for all template types except Advanced time category.

Related Topics

155

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 30
Rule Template Options

Default Allocation Option for Time Calculation Rule
Templates

For time calculation rules, you can optionally select a default time allocation created using My Client Groups > Time
Management > Time Allocations.

Here's what you can do when creating allocation rules from calculation rule templates:

• Select an allocation, if the parent rule template doesn't have a default allocation.

• Leave the default allocation, if already selected in the template.

• Override the default allocation selected in the template.

Related Topics

Rule Execution Type Option for Time Calculation Rule
Templates

To specify whether rules created with time calculation templates either create more hours or update existing hours,
select a Rule Execution Type option.

Example
Scenario: Threshold 8 Overtime is a time calculation rule that compares reported time to a defined daily threshold of 8
hours. Time worked over the scheduled 8 hours pays at 1.5 times the regular rate of 10 USD per hour.

Results: Here are the calculation details for both rule execution types when reported time is 10 hours.

Rule Execution Type

Calculation Description

Calculation Example

Create

Rule processing calculates total time of 12 hours, which is 2 hours
more than the reported time.

(10 hours * 10 USD) + (2 hours *5 USD) = 110
USD

•

•

It keeps the 10 hours of regular time at the regular hourly rate.

It creates 2 hours of premium time at .5 times the regular hourly
rate.

Update

Rule processing calculates total time of 10 hours, which matches
the reported time. Processing adjusts the pay rate for 2 of the 10
reported hours.

(8 hours * 10 USD) + (2 hours *15 USD) = 110
USD

• 8 hours of regular time at the regular hourly rate.

• 2 hours of overtime at 1.5 times the regular hourly rate.

156

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Related Topics

Chapter 30
Rule Template Options

Summation Level Option for Time Rule Templates

Time calculation, device, entry, and submission rule templates might reference the Summation Level option. When they
do, you can specify the level to apply the rule.

Here's the rule logic for each option:

Summation Level

Rule Logic

Details

Day

Time Card

Related Topics

Apply the rule to all time entries that match the time category conditions.

Apply the rule to all the hours for the entire day that match the time category conditions.

Apply the rule to all the hours for the entire period that match the time category conditions.

Reporting Level Option for Time Rule Templates

Time device, time entry, and workforce compliance rules might reference the Reporting Level option. When they do, you
can specify the level to display the rule message results.

Here's the rule logic for each option:

Reporting Level

Rule Logic

Details

Day

Time Card

Related Topics

Display rule results for all time entries that match the time category conditions.

Display rule results for all the hours for the entire day that match the time category conditions.

Display rule results for all the hours for the entire period that match the time category conditions.

157

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 30
Rule Template Options

Suppress Duplicate Messages Display Option for Time
Rule Templates

Time entry and device rules might generate repeated messages for the same condition. It depends on the time card
action settings in the rule template. Workforce compliance rules might also generate repeated messages for the same
condition.

• To display the message just once, in the Suppress Duplicate Messages Display field, select Yes.

• To display the message every time an entry or rule meets the condition, select No.

This option works with the Reporting Level option.

Example
A time entry rule produces a warning message when people report more than 20 worked hours for a week. When they
save, submit, and resubmit their time cards, they apply the rule.

Someone reports working for 10 hours per day for 5 days and saves the time card each day. Here's how often messages
would appear according to the reporting level and whether you suppress duplicate messages.

Reporting Level

Suppress Duplicate Messages Display

Message Display Frequency

Time Card

Either Yes or No

Once

Day

Day

No

Yes

Related Topics

3 successive days after reported time exceeds the 20-hour
maximum

Once, on the third day when the reported time for the week
exceeds the 20-hour maximum

Process Empty Time Card Option for Time Entry Rule
Templates

For only time entry rule templates, you can specify whether the rule applies to time cards that contain days with no time
entry values. If you select Yes, then the rule applies to all entries, not just those with hours.

Related Topics

158

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 30
Rule Template Options

Time Card Actions That Trigger Rule Option for Time
Entry and Calculation Rule Templates

You can select the time card actions--Save, Submit, Resubmit, and Delete--that cause the time calculation or entry rule
to run. Here are the default selections for each template type.

Template Type

Default Selections

Time calculations

Submit and Resubmit You can't edit these selections. But, you can select Save. You can edit this
selection in rules that you create with this template type.

Time entry

None

You can edit any selections in rules created with this template type. Here's what people typically select:

• Save for rules with details and daily summation levels, such as when a rule validates a daily

minimum

• Submit and Resubmit with the summation level of time card, such as when a rule validates a

weekly maximum

Related Topics

159

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 30
Rule Template Options

160

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 31
Rule Templates and Rule Parameters, Output, and
Explanations

31  Rule Templates and Rule Parameters,
Output, and Explanations

Formula Parameters in Time Rule Templates and Rules

Formulas contain parameters that time repository rules use to provide actual values to the formulas. You configure
formula parameters when you create rule templates. Your settings affect the values people select or enter when creating
rules with the rule template.

Display Sequence
You can specify the order that the parameters appear when people create rules with the template. The lower the
number, the higher the parameter appears in the list. The actual values set in the template don't show when people
create rules.

Formula Parameter Name
The name of the formula parameter that you see in the rule template comes from the formula. You can't change the
parameter name because it uniquely identifies the parameter in the formula.

Parameter Type
The parameter type specifies the expected format of the value set in rules created with the template. You type
selections include value set; fixed text, number, and date; time category; exclude; and message. If you don't want the
parameter to appear in rules created with the template, select Exclude.

Required
You specify whether rules created with the template need to use the parameter. You select Yes or No when you create
the rule template. People creating rules with the template see your selection as a read-only value.

Value Set
You can see the Value Set parameter setting only if Parameter Type is Value set. The value set that you select decides
the values that people can select from when they create rules with the template. They see the values that make up the
parameter list, but they don't see the name of the value set. For example, the available value set HRC_YES_NO includes
the values Yes and No. People creating rules see those values in the parameter list. They don't see HRC_YES_NO
anywhere in the Rule Parameters section.

Display Name
The display name is the read-only name for the parameter in rules created with the template. By default, the
display name is the formula parameter name. For example, many time formulas have a parameter named
WORKED_TIME_CONDITION of type Time category. This parameter identifies which time entries the formula should
consider as part of the validation or processing. People creating rules with the template select a time category from a

161

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 31
Rule Templates and Rule Parameters, Output, and
Explanations
list. It might make more sense for them to see the display name Time Category or Time to Consider instead of the actual
parameter name WORKED_TIME_CONDITION.

Value
People creating rules with the template select or enter the actual value that parameter passes to the formula depending
on your parameter settings. For example, if a parameter uses the HRC_YES_NO value set, one rule created with the
template could have the parameter pass the value Yes. Another rule created with the same template could have the
parameter pass the value No.

Related Topics

• Formula Outputs in Time Rule Templates and Rules

Formula Outputs in Time Rule Templates and Rules

Formulas contain outputs that they use to return results to the time repository rule. You configure outputs when
creating rule templates. Your settings affect the values that people select or enter when they create rules with the rule
template.

Display Sequence
You can specify the order that the outputs appear when people create rules with the template. The lower the number,
the higher the output appears in the list. The actual values set in the template don't show when people create rules.

Output Name
The name of the formula output that you see in the rule template comes from the formula. You can't change the output
name because it uniquely identifies the output in the formula.

Message Severity
You can specify the default exception type for time entry and time card exceptions by setting the message severity to
Information, Warning, or Error. For example, you want to identify anyone who starts or stops outside their specified
grace period, but during their start and end early and late periods. So, you set a default severity of Warning. People
creating rules with the template can change this default severity as appropriate.

Display Name
The display name is the read-only name for the output in rules created with the template. By default, the display name's
the formula output name. For example, many time formulas have the OUT_MSG output, which returns the selected
message severity. It might make more sense for people creating rules to see the display name Message Severity instead
of the actual output name.

Related Topics

• Formula Parameters in Time Rule Templates and Rules

162

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 31
Rule Templates and Rule Parameters, Output, and
Explanations

Formula Outputs Unique to Time Calculation Rule
Templates and Rules

Formulas contain outputs uses to return results to the time repository rule. You configure these outputs when creating
time calculation rule templates. Your settings affect the values that people select or enter when creating time calculation
rules with the template.

Output Group
You use output groups to link outputs from the formula to specific time attributes for calculation processing. For
example, you add the PayrollTimeType attribute once to Output Group 1 and once to Output Group 2. Here's what you've
after you finish:

• Output Group 1 has the OUT_MEASURE_UNDER output from the formula and your added PayrollTimeType

attribute.

• Output Group 2 has the OUT_MEASURE_OVER output from the formula and your added PayrollTimeType

attribute.

Even though both groups have the same payroll time attribute, the values that people set when they create rules with
the template will be different. For example, the payroll value for hours below the measure is typically a regular pay rate.
The payroll value for hours over the measure is typically an overtime or premium pay rate.

You select the output group when you create the calculation template. People can see, but not change your selection
when they create calculation rules with the template.

Time Attribute
You need to specify the type of time attribute for each output. For all measure outputs, such as OUT_MEASURE_UNDER
and OUT_MEASURE_OVER, select the Measure time attribute. As with output groups, people can see, but not change,
your selection when they create calculation rules with the template.

Value Type
You specify whether the people creating rules with the template enter or select the time attribute value. For example,
people enter a value for Measure attributes, such as 8 for a daily threshold or 40 for a weekly threshold. If you select
Data source or Value set, people select a value from the corresponding list. If you select fixed number, text, or date,
then people enter the value.

Value Set
You can see the Value Set output setting only if Value Type is Value set. The value set that you select decides the values
that people can select from when they create rules with the template. They see the values that make up the output list,
but they don't see the name of the value set. For example, the available value set HRC_YES_NO includes the values Yes
and No. People creating rules see those values in the output list. They don't see HRC_YES_NO anywhere in the Rule
Outputs section.

163

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 31
Rule Templates and Rule Parameters, Output, and
Explanations

Output Source
The output source identifies whether the output came from the formula linked to the template or a person added it. You
see this setting when you create calculation rule templates. People who create rules with the template don't see it.

Value
People creating rules with the template select or enter the actual time attribute value for the output results. For example,
you create a calculation template with the Under Pay Rate and Over Pay Rate payroll attributes. A rule created with the
template calculates daily overtime. Another rule created with the same template calculates daily premium time. Both
rules have Under Pay Rate set to Regular. The first rule has Over Pay Rate set to Overtime and the second rule has it set
to Premium.

Related Topics

• Formula Parameters in Time Rule Templates and Rules

How You Group Outputs in Calculation Rule Templates
and Rules

When creating time calculation rule templates, use output groups to identify the time attributes that store outputs. The
associated formula provides the outputs and groups, one group for each output.

You select the output values for the time attributes as you create rules using the rule template. In the Time Management
work area, create templates using the Rule Templates task and rules using the Rules task.

Scenario
You create a rule template that calculates time data weekly based on the
WFM_THRESHOLD_TIME_CALCULATION_RULE formula, which has these 2 outputs:

• OUT_MEASURE_UNDER

• OUT_MEASURE_OVER

The Output Group list contains these values:

• Output Group 1

• Output Group 2

Grouping Structure
On the Outputs page, you complete these actions:

• For OUT_MEASURE_OVER, change the output group to Output Group 2.

• For the time attribute of each measure outputs, select Measure.

• Add one time attribute output to each output group, as shown in this table:

164

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 31
Rule Templates and Rule Parameters, Output, and
Explanations

Output Name

Time Attribute

Output Group

Display Name

PAY_TYPE_UNDER

Payroll Time Type

Output Group 1

Pay for Below Threshold

PAY_TYPE_OVER

Payroll Time Type

Output Group 2

Pay for Over Threshold

On the Outputs section toolbar:

• Use Grouping Structure to review your output groups in a hierarchy format.

• Use Reorder to edit the display sequence.

Time Attribute Values in the Rule
You create a rule using this template. For the PAY_TYPE_UNDER and PAY_TYPE_OVER payroll time types, select Regular
and Overtime, respectively. The rule sets calculated hours below the threshold value to regular time. And it sets the
hours over the threshold value to overtime.

Related Topics

• Formula Outputs in Time Rule Templates and Rules

• Create a Rule Template That Calculates the Threshold for Expenditure and Payroll Time Types

• Create a Rule That Calculates the Daily 8h Threshold for Expenditure and Payroll Time Types

How You Configure Explanation Text in Time Rule
Templates and Rules

You describe the business purpose of the time rule template and any rules created with the template on the Create Rule
Template Explanation page.

You can include message tokens as placeholders for parameter and output values. When people create rules with the
template, the specific values they set replace these message tokens in the rule explanation text.

By default, the values in the Message Tokens list are the parameter and output names from the linked formula. If you
configure display names for the parameters and outputs in the rule template, then the list values are the display names.

Example
You create a time calculation rule template. It evaluates all reported time that meets the specified conditions. And, it
identifies the appropriate Payroll Time Type attribute to store the calculated hours depending on a defined limit. You
then use the template to create a rule that evaluates total reported time for all payroll time entries against a 40-hour
threshold. It stores time below the threshold with the Regular time attribute. And it stores time over the threshold with
Overtime.

Here's an example of how explanation text that includes tokens changes from the rule template to a rule created with
the template.

• Template: Compare the total reported hours in the {WORKED_TIME_CONDITION} time category
to the threshold of {DEFINED_LIMIT} hours. Store the calculated hours below the threshold with

165

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 31
Rule Templates and Rule Parameters, Output, and
Explanations

the {OUT_PAY_TYPE_UNDER} pay attribute. Store any calculated hours over the threshold with
{OUT_PAY_TYPE_OVER}.

• Rule: Compare the total reported hours in the All Payroll Entries time category to the threshold of 40 hours.

Store the calculated hours below the threshold with the Regular pay attribute. Store any calculated hours over
the threshold with Overtime.

Best Practices for Explanation Text That Includes Tokens

Here are some best practices to keep in mind when you write text that includes tokens:

•

Include abbreviations in tokens that are easy to recognize.

• Qualify tokenized text by inserting a word or phrase just before or after the token that describes what the token

is.

• Ensure that the qualifier text and the token name make sense together, as shown here.

Example of Incorrect Pairing

Examples of Correct Pairings

The time card was approved by the

The approver {APPROVER_NAME} approved the time card.

approver {STATUS}.

The invoice was approved and now has a {STATUS} status.

• Read your explanation text without the token to check if the explanation makes sense.

• Use tokens for numbers carefully. Qualify tokens for numbers that are objects, such as number of hours or time
type. If a token represents an amount that could be singular or plural, the text needs to support both scenarios.

Related Topics

• How You Configure Explanation Text in Time Rule Templates and Rules

Processing Order in Time Calculation Rule Sets

You determine the order that time calculation rules run when you create time calculation rule sets. The processing order
is important because later rule calculations might use results from earlier rule calculations.

Example
Here are the processing orders defined in three different rule sets.

Processing Order

Rule Set A

Rule Set B

Rule Set C

1

Rule 1

Rule 1

Rule 1

166

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 31
Rule Templates and Rule Parameters, Output, and
Explanations

Processing Order

Rule Set A

Rule Set B

2

3

4

Rule 2

NA

NA

Rule 2

NA

NA

Here's the order that rules run in Rule Set C:

Rule Set C

Rule Set B

Rule 2

Rule Set A

1. Rule C1
2. Rule B1
3. Rule B2
4. Rule C2
5. Rule A1
6. Rule A2

Can I create absence entries using time calculation rules?

No. You need to manually create absence entries for time cards.

Why can't I edit some rule templates?

You can't edit templates that were used to create rules. It doesn't matter whether these rules link to time processing or
time device processing profiles.

Why can't I edit some rules?

You can't edit rules that were linked to time processing or time device processing profiles.

167

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 31
Rule Templates and Rule Parameters, Output, and
Explanations

168

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 32
Time Rule Processing Details Analysis

32  Time Rule Processing Details Analysis

How You Analyze Processing Details for Time Rules and
Rule Sets

You can analyze the formulas, rules, and rule sets used to validate and process a person's time card. To review the
processing logs and diagnose any errors, go to My Client Groups > Time Management > Tasks panel > Analyze Rule
Processing Details.

Watch video

• To view details of the time repository rule that includes the parameter and output values, click Rule Definition.

• To view the processing logs that help you diagnose processing issues, click Rule Processing Log or Rule Set

Processing Log.

• To view details of the formula associated with the rule templates, click Formula Details.

Correct any errors using the relevant task. For example, if you find errors when processing a rule template, use the Rule
Template task to fix them.

Related Topics

• When to Pay Time Entries That Span Midnight

Enable and Disable Time Rule Set and Rule Logging

To troubleshoot issues with time and workforce compliance rules by analyzing process details, you must enable rule set
and rule logging.

1. Sign in as an application administrator.

2. Go to Setup and Maintenance > Tasks panel > Search > Manage Administrator Profile Values.

3. Search for the profile option code ORA_HWM_RULES_LOG.

4. Select ORA_HWM_RULES_LOG_LEVEL.

5.

In the Site level row, select the profile value from the options described in this table.

Log Level

Rule Set Logs

Rules Log

Incident

No, unless status is Failed

No, unless status is Failed

Finest

Finer

Yes

Yes

Yes

Yes for time calculation and entry rules

No for time device, workforce compliance, and time submission
rules

169

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 32
Time Rule Processing Details Analysis

Log Level

Rule Set Logs

Rules Log

Fine

Yes for time calculation and entry rule sets

No

No for time device, workforce compliance, and time
submission rule sets

Enable Time Rule Set and Rule Log Deletion

To manage performance, you can set a logging duration and automatically delete old log files.

1. Sign in as an application administrator.
2. Go to Setup and Maintenance > Tasks panel Search > Manage Administrator Profile Values.

3. Search for the profile option code ORA_HWM_RULES_LOG.

4. Select ORA_HWM_RULES_LOG_MONTHS_TO_KEEP.

170

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 32
Time Rule Processing Details Analysis

5.

In the Site profile level row, enter a profile value from 0 to 24. The number indicates the age, in months, that a log file
can reach before you delete.

◦ The default value is 6.
◦ Entering 0 deletes all entries.
◦ The rules engine doesn't keep logs older than 24 months, so any entry over 24 automatically adjusts to 24.

What to do next

Delete Older Time Rule Set and Rule Log Files

171

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 32
Time Rule Processing Details Analysis

Confirm Security Profile Setup to View Time Rule Set and
Rule Log Files

The Analyze Rule Processing Details task is here: My Client Groups > Time Management > Task panel. If you haven't
used the task before, first confirm that your sign in has the correct security.

If not, follow the instructions to set up the relevant data role. Then you can analyzing rule set and rule processing
details. And you can delete rule set and rule log files that are older than the specified months to keep.

On the Analyze Rule Processing Details page, in the Search section, show the Worker list.

•

•

If the list is empty, then the data role is missing or incorrectly configured.

If the list isn't empty, the data role is correctly configured for you to view rule set and rule log files.

Set Up the Data Role and Security Profile for the Analyze
Rule Processing Details Task

Here's how you set up security so that the appropriate people can use My Client Groups > Time Management >
Analyze Rule Processing Details.

1. Go to Setup and Maintenance > Tasks panel Search > Manage Data Role and Security Profiles

2. Create a data role.

3. On the Create Data Role: Select Role page, complete the fields as shown here.

Field

Data Role

Job Role

Role Code

4. Click Next.

Value

Time and Labor Administrator Role-TL1

Time and Labor Administrator

ORA_HXT_TIME_AND_LABOR_ADMINISTRATOR_JOB

5. On the Create Data Role: Security Criteria page, select the View All… option in each list.

For example:

◦ In the Organization Security Profile field, select View All Organizations.
◦ In the Position Security Profile field, select View All Positions.
◦ In the LDG Security Profile field, select View All Legislative Data Groups.
◦ In the Person section, Person Security Profile field, select View All People.
◦ In the Public Person section, Person Security Profile field, select View All People.

6. Click Next.

172

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 32
Time Rule Processing Details Analysis

7. On the Assign Security Profiles to Role: Organization Security… page, in the Organization Security Profile field, select

View All Organizations.

8. Click Next repeatedly, until you open the Create Data Role: Review page.

9. Click Submit. Don't click Review.

10. On the Manage Data Roles and Security Profiles page, click Done.

Set Up the Job Role for the Analyze Rule Processing
Details Task

Here's how you set up the job role so that the appropriate people can use My Client Groups > Time Management >
Analyze Rule Processing Details.

1. Go to Setup and Maintenance > Tasks panel  > Search > Manage Job Roles.
2. Click the Users task tab.

3. On the User Accounts page, search for and click the appropriate user name.

4. On the User Account Details page, click Edit.
5. Add the Time and Labor Administrator Role-TL1 role.

6. On the Edit User Account page, save your changes and close the page.

7. Sign out of the app.

8. Sign in to the app.

9. Go to My Client Groups > Time Management > Tasks panel > Analyze Rule Processing Details and confirm that

you can now see values in the Worker list.

Delete Older Time Rule Set and Rule Log Files

You can delete log files older than the number of months entered for the site-level profile value of the
ORA_HWM_RULES_LOG_MONTHS_TO_KEEP profile option. To do so, on the Analyze Rule Processing Details page, click
Actions > Delete Older Log Files.

173

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 32
Time Rule Processing Details Analysis

174

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 33
Rule Templates and Rules Configuration Procedures

33  Rule Templates and Rules Configuration
Procedures

Create Time Rule Templates

Rule templates are tools that simplify the adaptation of formulas into rules. A template exposes the exact parameters
that the associated formula requires and the outputs that the formula uses to return results.

1. Go to My Client Groups > Time Management > Tasks > Rule Templates.

2. Create a template.

3. On the Create Rule Template dialog box, select the template type and formula. The template type filters the formulas

that you can select from.

4. On the Create Rule Template: Definition page, configure the basic information.

5.

In the Time Card Events that Trigger Rule section, select the time card actions that start the rule. This step isn't
applicable to time device and submission rule templates.

Tip:  You can edit the Save setting when creating time calculation rules. You can edit all action settings when
creating time entry rules.

6. On the Create Rule Template: Parameters page, configure the parameters provided by the selected formula.

7. On the Create Rule Template: Outputs page, configure the outputs provided by the selected formula.

Tip:  The bundled time allocation formula doesn't contain any outputs. You specify rule outputs in time allocation
configurations that you create using the Time Allocation task.

In time calculation rule templates, for measure outputs, select the Measure time attribute. Optionally, you can add
time attributes. If you don't add time attributes, then the rules created with the template use the time attribute for
the reported time. For example, you use the same payroll attribute value as the reported time to store the calculated
hours for regular time entries. You use a different attribute value to store any calculated overtime hours. So, you add
the Payroll Time Type attribute to the output group for outputs over the threshold.

8. On the Create Rule Template: Explanation page, enter the business purpose of the rule template. To have the rule

explanation include the specific values set in that rule, include message tokens.

9. On the Create Rule Template: Review page, review your template settings.

10. When you're ready, save and close the template.

11. Create Time Rules.
12. Create Time Rule Sets.

Related Topics

• Formula Parameters in Time Rule Templates and Rules

• Formula Outputs in Time Rule Templates and Rules

• How You Group Outputs in Calculation Rule Templates and Rules

• How You Configure Explanation Text in Time Rule Templates and Rules

175

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 33
Rule Templates and Rules Configuration Procedures

Create Time Rules

When you create a rule, you select a template to use rather than a formula. The template automatically populates the
description of all outputs and helps you enter correct parameter values.

1. Create Time Rule Templates.

2. Go to My Client Groups > Time Management > Tasks > Rules.

3. Create a rule.

4. On the Create Rule dialog box, enter a descriptive rule name, and select the template type and rule template.

5. On the Create Rule page, in the Basic Information section, include a description of what the rule does.

6. In the Time Card Events that Trigger Rule section, check whether the default values from the selected template
match your rule requirements. The time device and time submission rule templates don't include this section.

7.

In the Rule Parameters section, enter or select values for the parameters from the selected rule template.

8. In the Outputs section, select values for the outputs from the selected rule template. The bundled time allocation

formula doesn't contain any outputs. You specify rule outputs in time allocation configurations that you create using
the Time Allocation task.

9. When you're ready, save and close your rule.

Tip:  Every time you create a time submission rule, you automatically create a corresponding rule set because the
rule set can have only one rule.

10. Create Time Rule Sets.

Related Topics

• How Formulas and Time Rule Components Work Together

• Formula Parameters in Time Rule Templates and Rules

• Formula Outputs in Time Rule Templates and Rules

• How You Group Outputs in Calculation Rule Templates and Rules

• Create a Rule That Calculates the Daily 8h Threshold for Expenditure and Payroll Time Types

Create Time Rule Sets

You create a collection of rules and rule sets of the same type. You then assign these rule sets to groups of people with
similar requirements for vacation, time validation, and time processing.

1. Create Time Rule Templates.

2. Create Time Rules.

3. Go to My Client Groups > Time Management > Tasks > Rule Sets.

4. Create a rule set.

5. On the Create Rule Set dialog box, enter the rule set name, select the type, and edit the effective date, as needed.
The default date is the current device date. If you change the date, be sure to select a date that coincides with the
start of a time card period.

176

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 33
Rule Templates and Rules Configuration Procedures

6. On the Create Rule Set page, in the Basic Information section, enter a description.

7. Edit the effective date to control when the new rule or rule edits take effect.
8. In the Rule Set Members section, add the rules and rule sets that you want to include. The lower the processing

sequence, the higher the processing priority.

9. When you're ready, save and close the rule set.

Related Topics

• How Formulas and Time Rule Components Work Together

• Processing Order in Time Calculation Rule Sets

• How Time Categories Work in a Time Rule Set

• Create the Projects and Payroll Time Calculation Rule Set

Create a Rule Template That Calculates the Threshold for
Expenditure and Payroll Time Types

You want to create a time calculation rule template that calculates regular and overtime hours.

Rules created with this template should run whenever people save, submit, or resubmit time cards. And, the rules
should update, or reapportion, the calculated hours, rather than create more hours. Also, you want to use hours-based
PJC_EXPENDITURE_TYPE_NAME and PayrollTimeType attributes to store the calculated hours that are below and over a
specific threshold.

1. Go to My Client Groups > Time Management > Tasks > Rule Templates.

2. Create the rule template.

3. On the Create Rule Template dialog box, complete these steps:

In the Template Type field, select Time calculation rule.
In the Formula Name field, select WFM_THRESHOLD_TIME_CALCULATION_RULE.

a.
b.
c. Click Continue.

4. On the Create Rule Template: Definition page, complete these steps:

a.
b.

c.
d.

In the Name field, enter Threshold for Expenditure and Pay Types.
In the Description field, enter Calculates hours to store for specific expenditure and payroll types using
time category and threshold parameters.
In the Rule Classification field, select Threshold.
In the Rule Execution Type field, select Update to handle overtime by splitting the reported hours between
two Payroll Time Type attribute values.
In the Summation Level field, select Day.
In the Time Card Events that Trigger Rule section, select Save.

e.
f.
g. Click Next.

5. On the Create Rule Template: Parameters page, complete these steps:

a.
b.

In the DEFINED_LIMIT row, set Parameter Type to Fixed number and Display Name to Threshold.
In the WORKED_TIME_CONDITION row, set Parameter Type to Time category and Display Name to Time
to Consider.

c. Click Next.

6. On the Create Rule Template: Outputs page, complete these steps:

177

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 33
Rule Templates and Rules Configuration Procedures

a. On the Outputs toolbar, click Add four times to insert four table rows.
b. Complete the two existing and four new outputs, as shown here. In this example, you store the calculated

hours in different project and payroll attributes than those of the reported time.

Note:  After inserting the four rows, the first time that you click a field, a comprehensive message about
all the missing required values appears. Click OK to close the message and complete the fields.

Display Sequence

Output Name

Output Group

Time Attribute

Value Type

Display Name

1

2

3

4

5

6

OUT_MEASURE_

Output Group 1

Measure

NA

Below Calculated

UNDER

Hours

EXPEND_

Output Group 1

PJC_

Data source

Below Expenditure

ATTRIBUTE_UNDER

EXPENDITURE_

TYPE_NAME

Type

PAY_ATTRIBUTE_

Output Group 1

PayrollTimeType

Data source

Below Pay Type

UNDER

OUT_MEASURE_

Output Group 2

Measure

NA

OVER

Over Calculated

Hours

EXPEND_

Output Group 2

PJC_

Data source

Over Expenditure

ATTRIBUTE_OVER

EXPENDITURE_

TYPE_NAME

Type

PAY_ATTRIBUTE_

Output Group 2

PayrollTimeType

Data source

Over Pay Type

OVER

c. On the Outputs section toolbar, click Reorder.
d. On the Reorder Display Sequence dialog box, reorder the display sequence as specified in the preceding

table.
e. Click OK.
f. On the Create Rule Templates: Outputs page, click Next.

7. On the Create Rule Template: Explanation page, in the Explanation section, add this explanation. To insert

placeholders, select the appropriate tokens from the Message Tokens list.

Compare the total hours in the {WORKED_TIME_CONDITION} time category with the threshold of
{DEFINED_LIMIT} hours. Store calculated hours under the threshold, with the {EXPEND_ATTRIBUTE_BELOW}
expenditure type and the {PAY_ATTRIBUTE_BELOW} pay type. Store calculated hours over the threshold with
the {EXPEND_ATTRIBUTE_OVER} expenditure type and the {PAY_ATTRIBUTE_OVER} pay type.

8. Click Next.

9. On the Create Rule Template: Review page, review your template settings. Make sure that the outputs display

sequence is what you want.

10. Click Save and Close.

What to do next

Create a Rule That Calculates the Daily 8h Threshold for Expenditure and Payroll Time Types and Create the Projects and
Payroll Time Calculation Rule Set

178

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 33
Rule Templates and Rules Configuration Procedures

Related Topics

• Create a Rule That Calculates the Daily 8h Threshold for Expenditure and Payroll Time Types

• Create the Projects and Payroll Time Calculation Rule Set

Create a Rule That Calculates the Daily 8h Threshold for
Expenditure and Payroll Time Types

You want to calculate daily regular and overtime hours to store with expenditure and payroll types.

This rule uses an 8-hour threshold and updates reported time by adjusting calculated results, rather than creating
more hours. It stores calculated hours below the threshold with the Professional Straight Time expenditure type and the
Regular pay attribute value. It stores calculated hours over the threshold with the Professional Overtime expenditure
type and the Overtime pay attribute.

1. Create a Rule Template That Calculates the Threshold for Expenditure and Payroll Time Types.

2. Go to My Client Groups > Time Management > Tasks > Rule
3. Create the rule.

4. On the Create Rule dialog box, complete these steps:

In the Name field, enter Daily Threshold 8h Update TCR.
In the Template Type field, select Time calculation rule.
In the Rule Template Name field, select Threshold for Expenditure and Pay Types.

a.
b.
c.
d. Click Continue.

5. On the Create Time Calculate Rule: Daily 8h Threshold for Expenditure and Pay Types page, complete these steps:

a.

In the Basic Information section, Description field, enter this text: Calculates daily regular time and
overtime for expenditure and payroll types using all time entries and an 8-hour threshold.
In the Rule Parameter section, Daily Overtime Threshold row, set the Value to 8.
In the Time to Consider row, set Value to All Payroll Entries.
In the Outputs section, Below Expenditure Type row, set Value to Professional Straight Time.
In the Below Pay Type row, set Value to Regular.
In the Over Expenditure Type row, set Value to Professional Overtime.
In the Over Pay Type row, set Value to Overtime.

b.
c.
d.
e.
f.
g.
h. Click Save and Close.

6. Create the Projects and Payroll Time Calculation Rule Set.

Related Topics

• Create a Rule Template That Calculates the Threshold for Expenditure and Payroll Time Types

• Create the Projects and Payroll Time Calculation Rule Set

179

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 33
Rule Templates and Rules Configuration Procedures

Create the Projects and Payroll Time Calculation Rule Set

You want to create a time calculation rule set that contains two rules. One rule handles overtime for a specified daily
threshold and the other allocates time to specific cost segments.

1. Create a Rule Template That Calculates the Threshold for Expenditure and Payroll Time Types.

2. Create a Rule That Calculates the Daily 8h Threshold for Expenditure and Payroll Time Types.

3. Go to My Client Groups > Time Management > Tasks > Rule Sets.

4. Create the rule set.

5. On the Create Rule Set dialog box, complete these steps:
In the Name field, enter US Writers.
In the Rule Set Type field, select Time calculation rule.
In the Effective Start Date field, select January 1 of this year.

a.
b.
c.
d. Click Continue.

6. On the Create Rule Set: US Writers page, complete these steps:
In the Basic Information section, enter a description.
In the Rule Set Members section, click the Add icon twice to add two rule members.

a.
b.
c. Complete the fields for the two rule members, as shown here.

Rule

First

Second

Processing Sequence

Member Type

Member Name

1

2

Rule

Rule

Daily 8h Threshold for

Expenditure and Pay Types

Start Time Allocations

d. Click Save and Close.

Related Topics

• Create a Rule Template That Calculates the Threshold for Expenditure and Payroll Time Types

• Create a Rule That Calculates the Daily 8h Threshold for Expenditure and Payroll Time Types

180

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 34
Automated Time Allocation to Cost Segments

34  Automated Time Allocation to Cost
Segments

Overview of Allocating Time to Cost Segments

To support your payment policies, automatically allocate people's time to specific cost segments, such as Department
and Program. For example, allocate their daily time evenly to the 1111 and 2222 departments. Assign time allocations
directly or using time calculation rules.

Basic Process to Create and Assign Time Allocations

1. Create the time allocation.
2. Assign the time allocation to one or more people, groups, or both.
3. Create a time calculation rule that allocates the time.
4. Link the time calculation rule to groups of people.

Related Topics

• Time Allocation Assignment

• Create the Cost Center, Program, and Fund Time Allocation

• Create Time Allocations

• How You View and Override Time Allocation to Cost Segments

Before You Start Creating and Assigning Time
Allocations

You need to complete these setup tasks before you create and assign time allocations.

1. Go to Setup and Maintenance > Workforce Deployment

2. Configure the time entry objects.

a. To prepare costing attributes for use in time card fields, complete these tasks:

i. Create payroll value sets using the Manage Value Sets task. On the Tasks panel tab, use Search to find

this task.

ii. Set up the cost allocation key flexfield using the Cost Allocation Key Flexfield task.
iii. Set up the cost allocation key flexfield usage to be available at the element entry level.
iv. Generate the costing time attributes using the Generate Data Dictionary Time Attributes task.
b. To uniquely identify regular and on call hours, create payroll elements and calculation components for time

cards using the Elements task.

c. To let people report relevant time, create time entry fields using the Time Entry Layout Components task.
d. To identify the regular and on call time entries, create time categories using the Time Categories task.

181

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 34
Automated Time Allocation to Cost Segments

e. To automatically generate relevant time entries, create time calculation rules using the Time Rules and

Time Rule Sets tasks.

f. To identify the people to link to the time allocations, create groups using the HCM Groups task.

3. To view and override time allocations, configure the appropriate layout sets and time entry profiles.

a. Add the dependent fields for the cost segments to time review, view, and approval notification layouts in a

layout set. Use the Time Layout Sets task.

b. Link the layout set to the relevant individuals and their managers using the Worker Time Entry Profiles task.

4. Create Time Allocations.

5. Time Allocation Assignment.

6. How You View and Override Time Allocation to Cost Segments.

Related Topics

• Overview of Allocating Time to Cost Segments

• Time Entry Setup and Maintenance Tasks

• Time Processing Setup and Maintenance Tasks

• How You View and Override Time Allocation to Cost Segments

Create Time Allocations

Here's what you need to do for each source row:

1. Before You Start Creating and Assigning Time Allocations.

2. Go to My Client Groups > Time Management > Tasks panel > Time Allocations.

3. Complete one or more source rows.

a. Specify whether to allocate someone's hours by percentages, hours, or equally. For hours-type allocations,

further specify whether to summarize hours by day or period.

b. Specify the time category that time allocation rules use to identify the person's hours to include and

exclude.

Here's a sample configuration of a source row.

Processing Sequence

Allocation Type

Summation Level

Time Category

1

Hours

Day

Union Time for OT

The processing sequence identifies in what order the allocation rules evaluate time category conditions.
You can enter your source rows in any order and reorder them as required to get the expected allocation
output.

4. Configure the output columns by adding all relevant time attributes.

182

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

5. Complete one or more output rows.

Chapter 34
Automated Time Allocation to Cost Segments

Here's a sample configuration of output columns and rows for the sample source row.

Processing Sequence

Hours

Department

Fund

1

2

3

20

20

999

1111

2222

3003

The processing sequence identifies in what order to generate the allocation output. You can enter your output rows
in any order and reorder them as required to get the expected allocation output.

Tip:  When the summation level is Day, the total hours should equal or exceed 24 hours. When the summation
level is Time card, the total hours should equal or exceed the time card period. For example, if the period is weekly,
the total hours should equal or exceed 168. A final hourly value of 999 safely covers any overflow for all summation
levels because a blank value isn't valid.

6. Time Allocation Assignment.

7. How You View and Override Time Allocation to Cost Segments.

Related Topics

• Overview of Allocating Time to Cost Segments

• Create the Cost Center, Program, and Fund Time Allocation

Time Allocation Assignment

After you create a time allocation, you can assign it to people directly or with rules.

Direct Assignment
You can directly assign time allocations using the Allocation Assignments task in the Time Management work area. Set
a specific date range for the assignment or leave the end open by specifying only a start date.

Rule and Time Processing Profile Assignment
You can assign time allocations to all members of one or more HCM groups using rules. Here's what you need to do
using tasks in My Client Groups > Time Management.

1. To specify a default allocation, create one or more time calculation rule templates using the Rule Templates

task. Use the bundled OFA_WFM_TCR_ALLOCATION_TIME_AP formula or create your own.

2. Create time calculation rules using the Rules task. You can use the bundled template Time Allocation Template
or your rule templates. When you create the rule, you can optionally associate a time allocation with the rule.
Or, you can override a default allocation set in the selected rule template.

3. Create a time calculation rule set that includes the relevant allocation rule or rules using the Rule Sets task.

183

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 34
Automated Time Allocation to Cost Segments

4. Associate the time calculation rule set with time processing profiles using the Worker Time Processing Profiles

task.

Assignments from Both Methods
When you assign time allocations to people with both methods, the direct allocation assignment takes priority over
assignments derived from the time processing profile. We recommend that you create a default time allocation and
assign it to the appropriate people through time processing profiles. Then, assign more specialized allocations for
specific people and HCM groups using the Allocation Assignments task.

Time Allocation
For the assigned time allocation to actually allocate time, here's what you need to do:

1. Create a time allocation rule even if you don't specify an allocation name.
2.

Include the allocation rule in the time calculation rule set associated with the time processing profile.

Related Topics

• Create Time Allocations

• Create Time Rule Templates

• Create Time Rules

• Create the Cost Center, Program, and Fund Time Allocation

How You View and Override Time Allocation to Cost
Segments

Here's how you can view and override time allocation outputs on time cards.

1. Go to Setup and Maintenance > Workforce Deployment > Time and Labor.

2. Create dependent cost fields for the independent Payroll Time Type attribute that correspond to the cost time

attributes in the allocation. Use the Time Entry Layout Components task.

3. Add the dependent cost fields to layouts using the Layout Sets task.

◦ To let workers and managers override allocations, add the fields to their time entry layouts. To let only
managers override allocations, add the fields to only the manager layouts. Show the override values to
workers as read only or not at all.

◦ To let workers and managers view allocation outputs, edit the Worker tab, in the Calculate Time section.

Add the fields to the time card matrixes of these layouts: time view, review, and approval notification. To let
only managers view allocation outputs, edit the Manager tab, in the Calculate Time section. Add the fields
to the time card matrixes of these layouts: time view, review, and approval notification.

4. Link the layout sets to people using the Worker Time Entry Profiles task.

184

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 34
Automated Time Allocation to Cost Segments

Related Topics

• Time Layout Sets

• Configure Dependent Fields for Labor Costing Overrides

• Create Time Rule Templates

• Create Time Rules

• Create the Cost Center, Program, and Fund Time Allocation

Create the Cost Center, Program, and Fund Time
Allocation

You want to automatically allocate time entries linked to regular payroll time attributes, to different cost centers,
programs, and funds.

These allocations use hours-based, daily thresholds. The allocation also automatically allocates 100 percent of time
entries linked to on-call payroll time attributes, to a specific cost center.

1. Create the Cost Center, Program, and Fund cost segments and the RN in CA on Primary Assign HCM group.

2. Go to My Client Groups > Time Management > Tasks > Time Allocations.

3. Create the time allocation.

a. On the Create Time Allocation page, in the Allocation Name field, enter Cost Center, Program, Fund.
b.

In the Description field, enter Allocates regular, holiday premium, and on call hours among Cost Center,
Program, and Fund cost segments.
In the Source section, create and complete rows, as shown here.

c.

Processing Sequence

Allocation Type

Summation Level

Time Category

1

2

Hours

Percentage

Daily

NA

Regular

On Call

d. Configure the output for the first source by completing these steps:

i.
ii.

In the Source section, select the first row, which contains the Regular time category.
In the Output section, add the time attributes, as shown here.

Attribute Display Sequence

Time Attribute

1

2

Cost Center

Program

185

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 34
Automated Time Allocation to Cost Segments

Attribute Display Sequence

Time Attribute

3

Fund

iii. Complete the output rows, as shown here.

Processing Sequence Hours

Cost Center

Program

Fund

1

2

3

8

16

24

2210

3320

4430

1000

2000

3000

1110

1120

1130

e. Configure the output for the second source by completing these steps:

In the Source section, select the second row, which contains the On Call time category.
In the Output section, add the Cost Center time attribute.

i.
ii.
iii. Complete the output row, as shown here.

Processing Sequence

Percentage

Cost Center

1

100

5000

f. Click Save and Close.
g. On the Time Allocations page, click Done.

4. Assign the time allocation directly to a group of people.

a. On the Tasks panel tab, click Allocation Assignments.
b. On the Allocation Assignments page, click the Create icon.
c. On the Create Allocation Assignment: Assignment Definition page, complete these steps:

In the Allocation Name field, search for and select Cost Center, Program, Fund.

i.
ii. Add an assignment range with the start date of today.
iii. Click Next.

d. On the Create Allocation Assignment: Person Assignments page, complete these steps:

In the Group Name field, select RN in CA on Primary Assign.

i.
ii. Click Search.
iii. To assign the allocation to all RN in CA on Primary Assign group members, click Next.

e. On the Create Allocation Assignment: Review page, complete these steps:

i. Review the assignment definition and ranges, and the person assignments.
ii. Click Save and Close.

f. On the Allocation Assignments page, click Done.

186

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 34
Automated Time Allocation to Cost Segments

5. Create the calculation rule that allocates time to cost segments.

a. On the Tasks panel tab, click Rules.
b. On the Rules page, click the Create icon.
c. On the Create Rule dialog box, complete these steps:

i. Complete the fields, as shown here.

Field

Name

Value

Start Time Allocations

Template Type

Time calculation rule

Rule Template Name

Time Allocation Template

ii. Click Continue.

d. On the Create Rule: Start Time Allocations page, complete these steps:

i.

Field

Value

Description

Start any time allocation calculations assigned to employees with time processing

profiles containing this rule

Match Total Allocated Hours with

Yes

Hours Identified by the Allocation

ii. Click Save and Close.

e. On the Rules page, click Done.

6. Link the time calculation rule that allocates time to cost segments, to people.

a. Add the Start Time Allocations rule to the appropriate time calculation rule sets using the Rule Sets task. If
you use other time calculation rules to calculation regular and on call hours, position this rule after them in
the rule set processing sequence.

b. Add the time calculation rule sets to appropriate worker time processing profiles using the Worker Time

Processing Profiles task.

Related Topics

• Overview of Allocating Time to Cost Segments

• Time Layout Sets

• Create Time Rules

• Create an HCM Group Using Evaluation Criteria

187

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 34
Automated Time Allocation to Cost Segments

Create and Assign the Calculation Rule That Allocates
Time to Cost Segments

To allocate time to cost segments, you need to create and run at least one time calculation rule. To run the rule, add it to
a time calculation rule set and add the rule set to worker time processing profiles.

1. Go to My Client Groups > Time Management > Tasks > Rules.

2. Create the time calculation rule to allocate time to cost segments.

a. On the Create Rule dialog box, complete these steps:

i. Complete the fields, as shown here.

Field

Name

Value

Start Time Allocations

Template Type

Time calculation rule

Rule Template Name

Time Allocation Template

ii. Click Continue.

b. On the Create Rule: Start Time Allocations page, complete these steps:

i. Complete the fields, as shown here.

Field

Value

Description

Start any time allocation calculations assigned to employees with time processing

profiles containing this rule

Match Total Allocated Hours with

Yes

Hours Identified by the Allocation

ii. Click Save and Close.

c. On the Rules page, click Done.

3. Link the time calculation rule to people.

a. Add the Start Time Allocations rule to the appropriate time calculation rule sets using the Rule Sets task. If
you use other time calculation rules to calculation regular and on call hours, position this rule after them in
the rule set processing sequence.

b. Add the time calculation rule sets to appropriate worker time processing profiles using the Worker Time

Processing Profiles task.

188

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 34
Automated Time Allocation to Cost Segments

Related Topics

• Overview of Allocating Time to Cost Segments

• Time Layout Sets

• Create Time Rules

• Create an HCM Group Using Evaluation Criteria

Assign the Cost Center, Program, and Fund Time
Allocation Directly to a Group of People

Here's how you directly assign the Cost Center, Program, Fund time allocation to a group of people.

1. Go to My Client Groups > Time Management > Tasks > Allocation Assignments.

2. Create the allocation assignment.

3. On the Create Allocation Assignment: Assignment Definition page, complete these steps:
In the Allocation Name field, search for and select Cost Center, Program, Fund.

a.
b. Add an assignment range with the start date of today.
c. Click Next.

4. On the Create Allocation Assignment: Person Assignments page, complete these steps:

In the Group Name field, select RN in CA on Primary Assign.

a.
b. Click Search.
c. To assign the allocation to all RN in CA on Primary Assign group members, click Next.

5. On the Create Allocation Assignment: Review page, complete these steps:

a. Review the assignment definition and ranges, and the person assignments.
b. Click Save and Close.

6. On the Allocation Assignments page, click Done.

Related Topics

• Overview of Allocating Time to Cost Segments

• Before You Start Creating and Assigning Time Allocations

• Create Time Allocations

189

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 34
Automated Time Allocation to Cost Segments

190

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 35
Time and Compliance Exceptions and Alerts

35  Time and Compliance Exceptions and
Alerts

Create Time Rules Sets and HCM Groups for Workforce
Compliance Alerts

You can prevent time exceptions by checking compliance outside of the time management process using workforce
compliance time rule sets and HCM groups.

1. Go to Setup and Maintenance > Workforce Deployment > Time and Labor.
2.

If the delivered fast formulas don't meet your requirements, create your own formulas using the Fast Formulas task.
The delivered fast formulas identify missing time attestations, card, and entries, and dangling In and Out events.
There's also a reminder escalation formula.

3. Review the bundled lookup values for time collection device exceptions using the Workforce Management Lookups

task. Add more lookup codes to the ORA_HWM_TCD_EXCEPTION_TYPE lookup type, as needed.

4. Create and edit workforce compliance rule templates using the Time Rule Templates task. Use time categories in the

templates to summarize time and compare different categories of time.

5. Create and edit workforce compliance rules with your compliance rule templates using the Time Rules task.

6. Create and edit collections of workforce compliance rules and rule sets using the Time Rule Sets task.

7. Create and edit groups to identify the people you want to link to workforce compliance rules using the HCM Groups

task. You use these groups when you prepare the Generate Time Exceptions from Compliance Rules process.

You can reuse the existing HCM groups that are part of your Worker Time Entry Profiles. Or you can create as
many HCM groups to identify time exceptions as makes sense for your organization. For example, you could create
separate groups for each department, legislative data group (LDG), or business unit. You can also create a list of
specific individuals.

8. Schedule the Generate Time Exceptions from Compliance Rules process to run either once or regularly. You use this

process to send managers and workers notices of noncompliance.

Related Topics

• ORA_WFM_WCR_MISSING_TIME_CARD_AP Fast Formula

• ORA_WFM_WCR_IN_OUT_DANGLERS_AP Fast Formula

• ORA_WFM_WCR_ATTESTATION_ANSWER_NOTIFY_MGR_AP Fast Formula

• WORKFORCE_MANAGEMENT_WORKFORCE_COMPLIANCE_RULES Formula Type

191

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 35
Time and Compliance Exceptions and Alerts

How You Configure Resource Alert Notifications for Time
Exceptions

To alert managers and workers about time exceptions, you can use the delivered HWM Time Exceptions from
Compliance Rules event alert notification template. You can also configure your own resource alert notifications.

In the Alerts Composer work area, add resource alerts that use either the timeRecords or timeRecordGroups resource.
You schedule when the alert gets sent while you add the resource alert.

Related Topics

• Overview

Alerts for Change Requests with an In Error Status

You can notify individuals and their managers about errors that occurred when the manager approved a change
request. For example, the change request included a stop time before the start time, or there was an issue with the
environment.

You notify them using the Alerts Composer tool and the delivered HWM Time Change Request In Error alert. The alert
includes two alert templates, that are both enabled by default:

• Notify Individuals of In Error Change Request

• Notify Managers of a Subordinate's In Error Change Request

192

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 36
Time Card Approval Reminders and Escalations

36  Time Card Approval Reminders and
Escalations

Overview of Time Card Approval Reminders and
Escalations

You can send approval reminders for submitted time cards to an individual and their manager. You can also send
approval escalations to other managers in the manager's supervisor hierarchy.

You can configure parameters, such as these:

• The approval type, such as Worker Approval and Time Card Approval

• The maximum management level to escalate the approval to

•

If delegates receive reminders and escalations

• When reminders should start

• When escalations should start

Automated notifications pause for people who are part of the manually maintained exclusion group.

Basic Process to Configure Time Card Approval
Reminders and Escalations

Here's the basic process to configure approval reminders and escalations for submitted time cards.

1. Create a workforce compliance rule template. Use the Rule Templates task and the delivered

ORA_WFM_WCR_APPR_REMIND_ESCALATE_AP formula.

2. Create a rule with the new compliance rule template using the Rules task.

3. Create a compliance rule set with your new rule using the Rule Sets task.

4. Review the delivered notifications for the HWM Time Approval Reminders and Escalations alert and adjust them as

needed using the Alerts Composer tool.

5. Configure the Generate Time Exceptions from Compliance Rules process to automatically run at appropriate

intervals. Use the Scheduled Processes task.

Click the Advanced button to set up the recurring schedule. Make sure that you select the Send alert immediately
option so that the alerts start correctly.

193

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 36
Time Card Approval Reminders and Escalations

194

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 37
Time Entries That Span Midnight and Overtime Start

37  Time Entries That Span Midnight and
Overtime Start

Setup to Handle Midnight-Spanning Time and Overtime
Day Start

Here are the setup tasks that you need to complete to derive and use the earned date for time entries that span
midnight. It's also how you specify and use the overtime day in overtime calculations.

1. Configure workday definitions that support your policies for earned dates and the day start for overtime. Go to

Setup and Maintenance > Workforce Deployment > Time and Labor > Workday Definitions.

2. Assign a workday definition to each person whose time entries can span midnight or who has a nonstandard

overtime day. On the Employment Info page for your team or client groups, use the Assignment Hours Details icon.
The icon is next to the Working Hours field.

3. Create time rules to calculate overtime using time entry earned dates. Use the Rule Templates, Rules, and Rule Sets
tasks. To link these rules to the appropriate groups of people, use the Worker Time Processing Profiles task. Both
tasks are in My Client Groups > Time Management.

Related Topics

• Time Formula and Rule Types

When to Pay Time Entries That Span Midnight

If you have groups of people whose time entries span midnight, including on-call entries defaulted from Workforce
Scheduling, you need to identify the earned date. Payroll uses it as the pay date for the calculated time entries.

Related Topics

• Time Formula and Rule Types

• Reported Time

Day Start for Overtime Calculations

To support your overtime policies, you can specify the day start time for overtime, including whether the time is for the
current or next day.

By default, the day start time for overtime is 12:00a of the current day. Overtime calculations split single time entries
that span the day start time into two entries. The first entry ends at the day start time and the second entry starts then.

195

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 37
Time Entries That Span Midnight and Overtime Start

Related Topics

• Time Formula and Rule Types

Start Day Rule

You can configure workday definitions to use the Start day spanning days rule on classic, responsive, and enhanced
time card entries that span midnight. The rule includes on-call entries defaulted from Oracle Fusion Cloud Workforce
Scheduling.

With this rule, the earned and reference dates for the entry are the start date of the entry. For grouped time entries, it's
the start date of the oldest time entry in the group.

Entry Spans 2 Periods
It's possible that an entry group includes the last entry of a time card period and the first entry on the next period.
These entries both appear on the first time card because the earned and reference dates are in that time card period.
The entry from the next period appears as an another day on the first time card.

Here's an example with a time card period of April 5 to 11. The person has a grouping threshold of 90 minutes because
you want to keep entries before and after a break together as a single shift. The person works a regular or on-call shift
that starts on April 11 and ends on April 12.

Time Card Period

Date

Start Time

Stop Time

Complete Time Entry

April 5 to 11

April 12 to 18

April 11

April 12

April 12

6:30p

NA

12:30a

11:30p

NA

5:30a

6:30p to 11:30p

12:30a to 5:30a

NA

Their two time entries are from 6:30p to 11:30p on April 11 and from 12:30a to 5:30a on April 12. Normally, the time
card wouldn't show the April 12 time entry because it's part of the next time card period. But because the entries are
grouped, the rule adds the April 12 entry to the April 5 to 11 time card.

Also, the entries get processed together as part of the April 5 to 11 time card period. If time card, absence accrual, and
pay periods are the same, then the entries also accrue and get paid in that period.

Related Topics

• When to Pay Time Entries That Span Midnight

196

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 37
Time Entries That Span Midnight and Overtime Start

Example of the Start Day Rule with a 90m Grouping
Threshold

You configure the person's workday definition with the Start day spanning days rule and a 90-minute grouping
threshold.

Hours Paid and Absences Accrued
Here's how the time on a classic, responsive, or enhanced time card gets paid and accrued for the 2 periods April 5 to 11
and 12 to 18.

Shift

Day Reported

Reported Time

Earned and Reference Day Hours Paid and Accrued

Wednesday

4, period 1

6:30p to 11:30p

Thursday

Friday

Saturday

5

5

6

6

7

7

12:30a to 5:30a

6:30p to 11:30p

12:30a to 5:30a

6:30p to 11:30p

12:30a to 5:30a

6:30p to 11:30p

1, period 2

12:30a to 5:30a

4

5

6

7

10

10

10

10

The final entry for the Saturday regular or on-call shift is reported on Sunday, April 12, which is part of the second
period. But because of the grouping threshold, it appears on the April 5 to 11 time card. The hours also get paid and
accrue as part of that first period.

Related Topics

• Start Day Rule

Stop Day Rule

You can configure workday definitions to use the Stop day spanning days rule on classic, responsive, and enhanced time
card entries that span midnight.

With this rule, the earned and reference dates for the entry are the stop date of the entry. For grouped time entries, it's
the stop date of the newest time entry in the group.

197

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 37
Time Entries That Span Midnight and Overtime Start

Entry Spans 2 Periods
An entry can start on the last day of a time card period, and end on the first day of the next period. When this happens,
the entry appears on the time card with the time card period that includes the entry stop date. The entry also gets
processed as part of that time card period.

Here's an example with the time card periods April 5 to 11 and 12 to 18.

Time Card Period

Date

Reported Time

April 5 to 11

April 12 to 18

April 11

April 12

10:30p

6:30a

After Applying Workday
Definition

10:30p to 6:30a

NA

The entry starts on April 11 at 10:30p and stops on April 12 at 6:30a. So, it appears on the April 5 to 11 time card and gets
processed as part of that time card period.

When the time card, absence accrual, and pay periods are the same, the entry accrues and gets paid in the period that
includes the entry stop date. So in this example, the entry accrues and gets paid as part of the April 12 to 18 period.

Tip:  To ensure that all time card entries get paid in the same pay period, start your time card period 1 day before your
pay period. Using the preceding example, if your time card period is April 5 to 11, your pay period is April 6 to 12.

Related Topics

• When to Pay Time Entries That Span Midnight

Split at Day Start Time Rule

You can configure workday definitions to use the spanning days rule Split at day start time, on time entries that span
midnight. The time entries can be on classic, responsive, or enhanced time cards.

Time entries can include on-call entries defaulted from Oracle Fusion Cloud Workforce Scheduling.

This rule splits the entry into two entries, an entry that stops at midnight and an entry that starts at midnight. The
earned and reference dates for each of the two entries match the entry start dates.

Entry Spans 2 Periods
In this example, the reported entry that starts on April 11 at 10:30p and ends on April 12 at 6:30a becomes two reported
entries:

Time Card Period

Date

Start Time

Stop Time

Complete Time Entry

April 5 to 11

April 12 to 18

April 11

April 12

10:30p

NA

NA

6:30a

10:30p to 12:00a

12:00a to 6:30a

198

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 37
Time Entries That Span Midnight and Overtime Start

The earned and reference dates for these entries are April 11 and April 12, respectively. When the time card, absence
accrual, and pay periods are the same, the entries get processed, accrue, and get paid in the same period.

Related Topics

• When to Pay Time Entries That Span Midnight

Spanning Days Rules and Grouping Threshold

For certain rules, such as Start day, you can also set a grouping threshold. The grouping threshold, measured in
minutes, lets you link time entries together to identify the earned or reference date.

For example, you want to treat the entries just before and after a meal break as one shift. So, you set a grouping
threshold of 90 in the person's workday definition.

• They start work at 6:30p on April 11 and break for lunch at 11:30p.

• They return from lunch at 12:30a on April 12 and stop for the day at 5:30a.

The earned and reference dates for both entries are April 11 because less than 90 minutes separates the stop and start
times.

Time entries can include on-call entries defaulted from Oracle Fusion Cloud Workforce Scheduling.

Related Topics

• When to Pay Time Entries That Span Midnight

• Example of the Start Day Rule with a 90m Grouping Threshold

199

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 37
Time Entries That Span Midnight and Overtime Start

200

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 38
Database Items and Time Balances

38  Database Items and Time Balances

Overview of How You Configure Database Items to
Summarize Time

You can include relevant time data in fast formulas that include people's balances, such as absence accruals, by creating
your own database items.

Database items are formula language variables with values resulting from database queries. They make formulas
simpler to write and maintain because you avoid writing and updating complex queries to access the database. To
create your own database items, you create balance dimensions and then time balance definitions.

Related Topics

• Time Balance Dimensions

• Time Balance Definitions

• Sample Fast Formula with New Time Balance Database Item

Time Balance Dimensions

To specify the level and time period to use when summarizing time for people's balances, you create time balance
dimensions.

Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Balance Dimensions. You can also use
this task to view bundled balance dimensions.

Summary Levels

• Assignment summarizes them by the person's assignment.

• Person summarizes them across all the person's assignments.

Period Types

• Absence accrual time period: The time period set in the absence accrual calculation.

• Profile overtime period: The repeating period with the Overtime usage associated with the person's

assignment. Otherwise, the overtime repeating period selected on the person's worker time processing profile.
The profile selection is optional, so there's no guarantee that the profile provides this period.

• Repeating time period: The repeating time period with the Balances usage selected.

201

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 38
Database Items and Time Balances

Dimension Level and Period Type Working Together
Here are examples of how the dimension level and period type work together:

• A balance dimension summarizes time for people across all their assignments using the overtime period set in

time processing profiles.

• Another balance dimension summarizes time for people by each of their assignments using a specified

repeating time period with the Balances usage.

Dimension Suffix
Saving the newly created dimension automatically generates a dimension suffix based on the dimension name,
grouping, and time period values. This dimension suffix forms part of the automatically generated definition name of
the balance definition. For example, you create a time balance dimension with this configuration:

Field

Name

Example Configuration Value

Reg Hrs by Person

Dimension Level

Person

Period Type

Time Period

Repeating Period

Biweekly Starting Sunday

The application-generated suffix, which forms part of the database item name, is _REG_HRS_BY_PERSON_PER_RP.

Related Topics

• Overview of How You Configure Database Items to Summarize Time

• Time Balance Definitions

• Sample Fast Formula with New Time Balance Database Item

Time Balance Definitions

Time balance definitions consist of one balance dimension and one or more time categories. The time categories
identify the time data to add or subtract from the time balance.

When you create balance definitions, you must select a unit of measure, either Hours or Units. This selection constrains
the time categories that you can select.

To create balance definitions, go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time
Balance Definitions.

Definition Name
After you enter a name for the balance definition and select the balance dimension, the application automatically
generates the definition name. This automatically generated definition name, which includes the automatically

202

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 38
Database Items and Time Balances

generated dimension suffix, is the database item name. You can use the database item name in your fast formulas that
include time balances. For example, you create a time balance dimension with this configuration:

Field

Name

Example Configuration Value

Reg Hrs Time Bal Def

Entry Unit of Measure

Hours

Balance Dimension

Reg Hrs by Person

This selection associates the dimension suffix (_REG_HRS_BY_PERSON_PER_RP) with the time balance
definition.

Effective Start Date

January 1, 2018

Time Category Name

Add or Subtract

Reg Hrs

Add

The application-generated dimension, or database item, name is
REG_HRS_TIME_BAL_DEF_REG_HRS_BY_PERSON_PER_RP.

Related Topics

• Overview of How You Configure Database Items to Summarize Time

• Time Balance Dimensions

• Sample Fast Formula with New Time Balance Database Item

Sample Fast Formula with New Time Balance Database
Item

This sample formula includes the new database item created from these example time configurations.

Example Balance Dimension Configuration
Here's the balance dimension configuration used in the sample formula:

Field

Name

Example Configuration Value

Reg Hrs by Person

Dimension Level

Person

Period Type

Time Period

Repeating Period

Biweekly Starting Sunday

203

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 38
Database Items and Time Balances

The application-generated suffix, which forms part of the database item name, is _REG_HRS_BY_PERSON_PER_RP.

Example Balance Definition Configuration
Here's the balance definition configuration used in the sample formula:

Field

Name

Example Configuration Value

Reg Hrs Time Bal Def

Entry Unit of Measure

Hours

Balance Dimension

Reg Hrs by Person

This selection associates the dimension suffix (_REG_HRS_BY_PERSON_PER_RP) with the time
balance definition.

Effective Start Date

January 1, 2018

Time Category Name

Add or Subtract

Reg Hrs

Add

The application-generated dimension, or database item, name is
REG_HRS_TIME_BAL_DEF_REG_HRS_BY_PERSON_PER_RP.

Sample Formula
Here's the sample formula that uses the example balance definition:

DEFAULT FOR HWM_CTXARY_RECORD_POSITIONS is EMPTY_TEXT_NUMBER
DEFAULT FOR StartTime is EMPTY_DATE_NUMBER
DEFAULT FOR StopTime is EMPTY_DATE_NUMBER

default FOR REG_HRS_TIME_BAL_DEF_REG_HRS_BY_PERSON_PER_RP is 0

INPUTS ARE HWM_CTXARY_RECORD_POSITIONS, measure ,StartTime ,StopTime
ffs_id = GET_CONTEXT(HWM_FFS_ID, 0)
rule_id = GET_CONTEXT(HWM_RULE_ID, 0)

NullDate = '01-JAN-1900'(DATE)
NullText = '**FF_NULL**'

groupTypeID = 101
out_msg_ary = EMPTY_TEXT_NUMBER

ctxPersonId = GET_CONTEXT(HWM_RESOURCE_ID, 0)
ctxPeriodEndTime = GET_CONTEXT(HWM_CTX_PERIOD_END_DATE, NullDate)

pMaxHr = get_rvalue_number (rule_id ,'DEFINED_LIMIT', 0)
pMsgCd = ger_rvalue_text (rule_id ,'MESSAGE_CODE', 'HWM_FF_TER_PERIOD_GT_MAX_WRN')

tcRecCount = HWM_CTXARY_RECORD_POSITIONS.count

if (tcRecCount > 0 ) then
(
 balValueCurCHANGE_CONTEXTS(EFFECTIVE_DATE = ctxPeriodEndTime, PERSON_ID = ctxPersonId, GRP_TYPE_ID =
 groupTypeId) = 0

204

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 38
Database Items and Time Balances

 (

 IF (REG_HRS_TIME_BAL_DEF_REG_HRS_BY_PERSON_PER_RP WAS NOT DEFAULTED) THEN
 (
 balValueCur = REG_HRS_TIME_BAL_DEF_REG_HRS_BY_PERSON_PER_RP
 rLog = add_rlog (ffs_id, rule_id, 'Balance Value: ' || TO_CHAR(balValueCur) ||
 ' = DBI_CONTEXTS: EFFECTIVE_DATE= '||
 TO_CHAR( GET_CONTEXT(EFFECTIVE_DATE, nullDate) ) ||
 ', PERSON_ID=' || TO_CHAR( GET_CONTEXT(PERSON_ID, 0) ) ||
 ', GRP_TYPE_ID=' || TO_CHAR( GET_CONTEXT(GRP_TYPE_ID,0) ) )
 )
 ) /* Change Context */

 if (balValueCur > pMaxHr ) then (
 out_msg_ary[tcRecCount] = get_output_msg1 ( 'FND ,pMsgCd ,'DEF_LIMIT' , TO_CHAR( pMaxHr ) )
 )
)

RETURN out_msg_ary

205

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 38
Database Items and Time Balances

206

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 39
Time Collection Device Configurations

39  Time Collection Device Configurations

Overview of Time Collection Device and Web Clock Event
Processing

You can process time reported with time collection devices, such as badge or biometric readers. Or process time
reported with Web Clock. Here's the basic ongoing process of collecting events through to creation or completion of
time entries.

1. You regularly export person and employment data to third-party time devices and import time device and web clock

events.

2. The import process runs validations of the imported time data and identifies any badge and time entry exceptions

for resolution by time and labor managers.

207

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 39
Time Collection Device Configurations

3. The import process uses valid events to create or complete time entries.

208

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 39
Time Collection Device Configurations

Related Topics

• How Time Device Processing Profile Components Work Together

• Time Collection Device Setup and Maintenance Tasks

How You Import Data from Time Collection Devices

You transfer time data from a third-party time device using the Time Event REST service. Typically, the time collection
device performs time event transfers in regularly scheduled batches.

The process handles imported time events using one of these methods, depending on the verification results:

• Returns inaccurately formed resources in an error status

• Saves accurately formed resources to the time repository for further functional validations

For details on configuring the Time Event resources and requests, see REST API for Oracle Global Human Resources
Cloud in Oracle Help Center.

Related Topics

• Time Collection Device Setup and Maintenance Tasks

• How Time Device Processing Profile Components Work Together

• Overview of Time Collection Device and Web Clock Event Processing

Supplier-Related Choice Lists for Time Device Event
Mappings

When you create time device event mappings, you identify the supplier and supplier device event using drop-down lists
generated from these lookups.

• ORA_HWM_TCD_SUPPLIERS: the companies supplying the time collection devices

• ORA_HWM_TCD_SUPPLIER_EVENTS: the time events recognized by the time collection device supplier, such as

Clock In or Meal Out

These event lookup codes need to start with the supplier lookup code. For example, if you've a supplier lookup
code ABC, start the lookup codes for those supplier device events with ABC_.

To create values for these lookup types and edit existing values, use the Workforce Management Lookups task in the
Setup and Maintenance work area. The task is part of the Workforce Deployment offering, Time and Labor functional
area.

209

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 39
Time Collection Device Configurations

Related Topics

• Overview of Workforce Management Lookups

• Time Device Event Mappings

• Examples of Mappings for Time Device Events

• Overview of Time Collection Device and Web Clock Event Processing

Time Device Event Mappings

To process events imported from time collection devices, map the supplier device events to time and labor application
events. Also identify the time attributes and default attribute values for each device event, such as Payroll Time Type
and Regular.

Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Device Event Mappings.

Here are descriptions of the four application event values.

Application Event

Description

In

In and Out

Out and In

Out

Used with the specified time attributes to create the start time event for an
activity.

Used with the specified time attributes to create the start time event for one
activity and the stop time event for another activity.

Start break and stop shift

Used with the specified time attributes to create the stop time event for one
activity and the start time event for another activity.

Stop shift and start break

Used with the specified time attributes to create the stop time event for an
activity.

Stop shift

Example

Start shift

Related Topics

• Examples of Mappings for Time Device Events

• Start and End Property Time Attributes

• Overview of Time Collection Device and Web Clock Event Processing

• Generate Time Cards from Time Collection Device Process

Time Device Event Mapping Sets

To group time device event mappings for a specific supplier device and the people who use the device, create mapping
sets.

Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Device Event Mapping Sets.

You can get unpredictable processing results if you include multiple mappings for the same supplier device event in a
single mapping set. For example, you map the same device event to these combinations of pay type and costing time

210

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 39
Time Collection Device Configurations

attributes: Regular and Administration, and Regular and Engineering. You include both mappings in the same mapping
set. The import process has no logic that decides which mapping the process uses for each imported time device event.
For best results, name and describe your device event mappings so that you include only one mapping per supplier
device event in each mapping set.

Related Topics

• Time Device Event Mappings

• Examples of Mappings for Time Device Events

• Overview of Time Collection Device and Web Clock Event Processing

• Generate Time Cards from Time Collection Device Process

Examples of Mappings for Time Device Events

You want to create mappings between PPR Mint Company supplier device events and time and labor application events.
You also want to include Payroll Time Type attribute values in the mappings.

Event Mapping Scenario
You've hourly workers who use badge readers from PPR Mint Company to record when they start and stop shifts,
breaks, and meals. You pay shifts and breaks at regular rates, while meals are unpaid.

Event Mapping Set
Here are the individual mappings you plan to add to a mapping set for PPR Mint Company.

Event Mapping Name

Supplier Device Event

Application Event

Time Attribute

Default Values

PPRMint Start Shift

Start Shift

In

Payroll Time Type

Regular

PPRMint Stop Shift, Start
Break

PPRMint Stop Break, Start
Shift

PPRMint Stop Shift, Start
Meal

PPRMint Stop Meal, Start
Shift

Start Break

Out and In

Payroll Time Type

Stop Break

Out and In

Payroll Time Type

Start Meal

Out and In

Payroll Time Type

Stop Meal

Out and In

Payroll Time Type

Out: Regular
In: Paid Break

Out: Paid Break
In: Regular

Out: Regular
In: Unpaid Meal

Out: Unpaid Meal
In: Regular

PPRMint Stop Shift

Stop Shift

Out

Payroll Time Type

Regular

211

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 39
Time Collection Device Configurations

Analysis
To make sure that there aren't any gaps when people take breaks and meals during a shift, select the Out and In
application event. Although there's one application event in this instance, the Generate Time Cards from Time
Collection Device import process creates two time events. The first time event is an Out event that's immediately
followed by an In event. For example, in the PPRMint Stop Shift, Start Break mapping, the Out event corresponds to
stopping the shift. The In event corresponds to starting the break.

Payroll elements created for use with time cards provide the default values for the Payroll Time Type time attribute.

Resulting Time Card Entries
Here are the time entries that the Generate Time Cards from Time Collection Device import process creates as someone
badges in and out.

Time Attribute Values

Wednesday Start

Wednesday End

Regular

Paid Break

Regular

Unpaid Lunch

Regular

Paid Break

Regular

08:00

10:00

10:15

12:00

13:00

15:00

15:15

Related Topics

• Time Device Event Mappings

10:00

10:15

12:00

13:00

15:00

15:15

17:00

Shift Limits in Time Processing

Shift limits identify acceptable deviations from scheduled shift starts and stops. And they help time device rules identify
the shift to use when evaluating time device or web clock events.

To set shift limits, go to My Client Groups > Time Management > Tasks > Manage Shift Properties.

Grace Period
A grace period is the number of minutes that individuals can deviate from their published scheduled start and stop
times without getting attendance violations. This deviation applies both before and after the scheduled time. For
example, when a shift with a 15-minute grace period starts at 8:00, the valid start period is 7:45 to 8:15.

212

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 39
Time Collection Device Configurations

Start and End Early and Late Periods
Early and late periods are ranges of time in minutes, before and after scheduled start and end times. These periods help
time device rules evaluate time device and web clock events using identified shift start or stop times. For example, a
scheduled shift starts at 8:00. It has a 15-minute grace period, a 45-minute start early period, and a 30-minute start late
period.

• The 45-minute start early period includes the 15-minute grace period. So, the start early period is 7:15 to 8:00.

• The 30-minute start late period includes the 15-minute grace period. So, the start late period is 8:00 to 8:30.

213

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 39
Time Collection Device Configurations

Violation Types
Time device rules create time entry exceptions for time device or web clock events in the specified start and end early or
late periods. They can also create exceptions for events outside of the grace period, depending on how you set up the
shift limits.

Time entry exceptions include an exception type of Information, Warning, or Error, which specifies what message the
time and labor manager reviewing the exception sees. A device rule uses the violation type that you set for the shift
limits as the exception type for the time entry. If you don't set a violation type, it uses the message severity set in the
rule. For example, the violation type for the start early period is Warning. The message severity in the device rule is
Error. When the rule generates an exception, it sets the type as Warning. If there wasn't any violation type for the start
early period, the rule would generate an Error exception.

Time event processing also uses the rule message severity for time events outside of any specified start and end early
and late periods. For example, the rule generates Error exceptions for time before start and end early periods, and after
start and end late periods.

Related Topics

• How Time Device Processing Profile Components Work Together

• Overview of Time Collection Device and Web Clock Event Processing

214

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 40
How Many Time Device Processing Objects to Create

40  How Many Time Device Processing
Objects to Create

Best Practices for Creating Time Device Processing
Objects

You need to create separate time device processing profiles for each unique combination of device processing
components, as shown here. You link these profile people who share similar time entry and processing requirements for
third-party time devices and web clock.

The more device processing objects that you create, the greater the ongoing maintenance effort. You want to find
a balance between optimizing the device processing experience for people and the effort required to maintain that
experience.

215

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 40
How Many Time Device Processing Objects to Create

Related Topics

• Time Collection Device Setup and Maintenance Tasks

How Many Time Device Event Mappings and Web Clock
Button Definitions to Create

Use these questions to help you decide how many time device event mappings or web clock button definitions you
need to create.

216

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 40
How Many Time Device Processing Objects to Create

Question

Examples and Comments

What events do you record with your
time collection devices or web clock, for
example shift start, break, meal, and shift
end?

To ensure accurate time event validation and processing, there can't be any ambiguity about the time
events that each device provides. They must clearly and consistently map to an In, Out, In and Out, or
Out and In application event. For example:

• You identify when employees start their work using the Start Shift time device event, which maps

to the In application event.

• You identify when employees take a break using either of these methods. Map one time device
event, Break, to the Out and In application event. Or, map two time device events, Shift End and
Break In, to the Out and In application events, respectively.

What are the time attributes and attribute
values that correspond to the time device
or web clock events?

For example, the Start Shift, Break, and Meal time device events all map to the Payroll Time Type time
attribute. But, the events each have different attribute values.

• Shift Start: Regular

• Break: Paid Break

• Meal: Unpaid Meal

Using discrete time attributes enables you to report in greater detail, but might require more event
mappings and mapping sets or web clock buttons. For example, because you pay breaks and shifts
at the same rate, you could use the same Payroll Time Type attribute value for both. Because you
don't pay for meals, you could decide not to associate any time attribute. Time device rules could still
validate the event but time calculation rules would ignore it.

Related Topics

• Time Collection Device Setup and Maintenance Tasks

How Many Time Device Event Mapping Sets and Web
Clock Buttons to Create

When you create a layout component for Web Clock, you can define as many buttons as you want. If your people use
Web Clock, you can optionally, link web clock events with a time device processing profile, as needed:

1. Link a web clock layout with groups of people using time entry profiles.
2. Assign the same groups of people to a time device processing profile that doesn't include an event mapping set

or time device export data.

You can link only one time device event mapping set to a time device processing profile. But, you can link as many
mappings to a mapping set as you want.

Use these questions to help you decide how many event mapping sets or web clock buttons and button definitions you
need to create.

• Are there unique events for time collection devices or web clocks in different areas, buildings, or regions?

• Are there events that are relevant only in certain years, for example, some time attributes relate to a location

that you closed?

• Do you group certain events from time devices or web clock together for payroll eligibility? For example, some

payroll-related time attributes are effective for only certain date ranges.

217

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 40
How Many Time Device Processing Objects to Create

Related Topics

• Time Collection Device Setup and Maintenance Tasks

How Many Time Device Export Data Configurations to
Create

You can link only one time device export data configuration to each device processing profile. Create a separate export
data configuration for each unique combination of data that you regularly send to the time collection device.

Examples of export data are:

• Person identification data, such as first and last name and badge ID

• Other data, such as payroll time types and published WFM schedules

Use these questions to help you decide how many export data configurations you need to create:

• What data does the time device require to provide complete time event records?

• What data, if any, do people require when they report time using the device? For example, you require people to

select their location when they report time.

Because Web Clock is part of the standard Time and Labor solution, you don't have to create and send export data to
provide relevant information.

How Many Time Device and Submission Rule Sets to
Create

You can link only one time device and one time submission rule set to a device processing profile.

Use rule sets to link rules to people with similar validation and submission requirements for events from third-party
time devices or Web Clock. You can link as many time device rules to a rule set as you want. When you create a time
submission rule, you also automatically create the corresponding rule set because each submission rule set can contain
only one rule.

Use these questions to help you decide the rules that you require:

• Do you want to validate time device or web clock events against published employee schedules and designated
shift limits? Or do you want to accept all time entries automatically? Shift limits consist of a grace period, start
and end early and late periods, and start and end early and late violation types.

• Do you want to validate that certain employee groups satisfy a specified minimum rest period between shifts?

• Do you want to automatically save time card entries created with the time device or web clock events and

submit the time cards? What conditions, such as the type or number of events cause an automatic save? What
conditions, such as number of events, duration, or schedule, cause an automatic submission? For example,
automatically submit time cards after the eighth time event on the last day of the time card period.

218

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 40
How Many Time Device Processing Objects to Create

Related Topics

• Time Collection Device Setup and Maintenance Tasks

How Many HCM Groups to Create for Time Device
Processing Profiles

You can link one or more HCM groups with each time device processing profile.

Define separate groups wherever the member characteristics are unique among time profiles or groups of profiles. For
example, you group your people according to the country where they work.

Related Topics

• Time Collection Device Setup and Maintenance Tasks

219

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 40
How Many Time Device Processing Objects to Create

220

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

41  HCM Groups

Chapter 41
HCM Groups

Overview of Linking People to Time and Labor Objects

You link individuals and their managers to time entry, processing, and device processing objects using HCM groups and
profiles.

To create groups, go to Setup and Maintenance > Workforce Deployment > Time and Labor > HCM Groups.

HCM Groups and Time Entry Objects
Payroll, project, absence, and custom time attributes make up layout components for time entry. These layout
components, which are either time card fields or web clock buttons, and time categories make up the layouts in a layout
set. You link individuals with layout sets using time entry profiles and HCM group assignments.

221

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 41
HCM Groups

222

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 41
HCM Groups

Tip:  You can't edit groups linked to a time entry profile.

HCM Groups and Time Processing Objects
Time consumer sets include time categories. You can also link time categories with rules and rule sets that make up
time entry or time calculation rule sets. Time card periods, consumer sets, optional overtime periods, and rule sets
make up time processing profiles. You link individuals and their managers with these objects using time processing
profiles and HCM group assignments.

HCM Groups and Time Device Processing Objects
Time device event mappings make up mapping sets. Time device rules and a single submission rule make up respective
rule sets. These mapping and rule sets and a device export data configuration make up time device processing profiles.
You link individuals and their managers with these sets and export data objects using time device processing profiles
and HCM group assignments.

223

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 41
HCM Groups

Related Topics

• Delivered HCM Groups

• Overview of HCM Group Membership

• Create an HCM Group Using Evaluation Criteria

Delivered HCM Groups

Here are the delivered HCM groups used in delivered time entry and processing profiles. You can also use them in your
own time profiles. But you can't edit them. All employees in your organization are members of each group.

224

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Delivered Group

Description

Chapter 41
HCM Groups

Payroll Usage

Used in the delivered time entry and processing profiles for the payroll time consumer

Project Execution Management Usage

Used in the delivered time processing profile for the project execution management time consumer

Projects and Payroll Usage

Used in the delivered time entry and processing profiles for combined payroll and project costing time
consumers

Projects Usage

Used in the delivered time entry and processing profiles for the project costing time consumer

To quickly find these groups, in the Description field, search for Delivered.

Related Topics

• Overview of Linking People to Time and Labor Objects

• Overview of HCM Group Membership

Overview of HCM Group Membership

You can create groups of people with similar characteristics by defining membership conditions and including or
excluding individuals, value sets, or other groups.

A group might have a fixed number of people or you might update the members on a defined basis. Also, an individual
can belong to more than one group. Go to Setup and Maintenance > Workforce Deployment > Time and Labor >
HCM Groups.

Related Topics

• Overview of Linking People to Time and Labor Objects

Evaluation Criteria and HCM Group Membership

You can use personal and employment criteria to define conditions that people need to meet to get included in a group
or excluded.

Here are some personal criteria you can use:

• Person Type

• Date of Birth

• Full Name

Here are some employment criteria you can use:

• Assignment Status

• Bargaining Unit

• Collective Agreement

• Department Name

225

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

• Job Name

• Labor Union

• Location

Chapter 41
HCM Groups

Example
You create the Associate Marketers group, which includes hourly individuals in the Marketing department. You define
the conditions, as shown here.

Field

Condition 1 Value

Condition 2 Value

Evaluation Criteria

Department Name

Operator

Value

Logical Operator

Related Topics

Equal to

Marketing

AND

• Overview of Linking People to Time and Labor Objects

• Create an HCM Group Using Evaluation Criteria

Job Name

Equal to

Associate Marketer

NA

How You Lock HCM Group Membership

So that you can always use the same set of individuals in time processing, prevent group membership refreshes. Do this
by setting Locked to Yes. For example, you lock the Senior Managers group membership as of June 12, 2022.

Note:  Locking group membership is a permanent action and you can't reverse it.

Related Topics

• Overview of Linking People to Time and Labor Objects

Embedded Group Priority in HCM Groups

When you embed groups within another group, an individual can exist in more than one group. In such a case, the
priority numbers assigned to the embedded groups decide the group membership. The lowest number has the highest
priority.

Example
Joe Smith is a member of these two groups. The Marketing group has them embedded with these statuses:

226

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 41
HCM Groups

Priority

1

2

Group Name

Promotions

Advertising

Status

Exclude

Include

The Marketing group excluded Joe Smith because the Promotions group, his highest priority embedded group, has the
Exclude status.

Related Topics

• Overview of Linking People to Time and Labor Objects

How You Refresh HCM Group Membership

You can evaluate the membership of existing HCM groups and update the list of members. To configure and submit the
Evaluate Group Membership process, go to Setup and Maintenance > Workforce Deployment > Time and Labor >
HCM Groups and click Refresh Group Membership.

Use the View Evaluation Status action to see the processing status for group membership refreshes.

You can schedule regular refreshes for the HCM group using advanced options. You can also regularly refresh the
membership of all HCM groups that meet both of these conditions:

• The group definition has the Include in Refresh All Groups Process option selected.

• At least one time entry, processing, or device processing profile configuration includes the group.

To include active and suspended assignments, select the Include assignments with an HR status of active or suspended
option. To include only active assignments, deselect the option.

Tip:  To refresh all groups that meet both conditions, when you configure the process, be sure to leave the HCM Group
and Person fields blank.

To maintain group membership for large populations or because of frequent hiring, schedule the Evaluate Group
Membership process using the As of run date parameter and a daily frequency. The process automatically increments
the Evaluation Date parameter using the first run date. Because we aren't sure at what time on what day the Wait runs,
we change the Evaluation Date only when the process runs. For example, server loads can delay when the process
actually runs. Also, using the original time during the Wait status helps you identify the original process because you
can have multiple processes scheduled.

Here's how the Evaluate Group Membership process decides the final membership status of each worker as of the
specified evaluation date.

Membership Evaluation

Membership Status When True

1. Is the worker directly included in or
excluded from the group?

2. Is the worker part of multiple child
groups or value sets with different
membership statuses?

Include or exclude the worker as appropriate.

Use the child group or value set that the worker is part of, with the highest priority, to include or
exclude the individual as appropriate.

227

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 41
HCM Groups

Membership Evaluation

Membership Status When True

3. Is the worker part of only one child
group or value set that's included in or
excluded from the parent group?

4. Does the worker match evaluation
criteria that has attributes, relational
operators, and logical operators?

Include or exclude the worker as appropriate.

Include the worker.

By default, these delivered groups include everyone:

• Payroll Usage

• Projects and Payroll Usage

• Project Execution Management Usage

• Projects Usage

How You View HCM Group Membership

After you create an HCM group, view the membership by clicking View Group Membership on the HCM Groups page.
Enter a membership evaluation date to get a list of the individuals who are group members as of that date.

The listed members can change as you change the evaluation date, depending on whether they meet membership
conditions on the specified date.

Manually Maintained Audit and Excluded HCM Groups

You can identify people who must not get worker approval reminders for a certain period. And, you can identify people
to include in Oracle Transactional Business Intelligence (OTBI) audit reports.

Use these tasks in the Time Management work area:

• Manually Maintained Excluded Members

• Manually Maintained Audit Members

You can also use the corresponding quick actions in My Client Groups.

The Actions menu has templates that you can use to merge and delete members if you prefer to maintain member
using spreadsheets.

Related Topics

• Overview of HCM Group Membership

228

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 42
HCM Group Examples

42  HCM Group Examples

Create an HCM Group Using Evaluation Criteria

Here's how you can create an HCM group that uses evaluation criteria to find the members.

1. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > HCM Groups.

2. Create the HCM group.

a. Enter a name, such as RN in CA on Primary Assign.
b. Enter a description, such as People with the Registered Nurses collective agreement, in a labor union,

in California.
In the Evaluation Criteria section, click the Create icon.

c.
d. On the Evaluation Criteria dialog box, add all your evaluation criteria. For example, to create these three

rows of criteria, complete the substeps three times.

i. Add a row of criteria.

Employment Attributes

Operator

Value

Logical Operator

Collective Agreement

Equal To

Registered Nurses

Labor Union

Equal To

Yes

Location Components

Equal To

(State) California

And

And

NA

ii. After adding each of the first 2 rows, click Apply and Add Another. After adding the third row, click

Save and Close.

e. Optionally group the criteria into a single condition.

i. On the Create Group page, in the Evaluation Criteria table, select all 3 rows.
ii. Click the Add Parentheses icon.
iii. Save your changes and close the page.

3. Refresh the group membership.

a. Select the group to refresh.
b.
c. Submit the refresh process.

In the Evaluation Date field, select the current date.

Create an HCM Group Using a Value Set

Here's how you can create an HCM group using a value set.

1. Create the value set. For example, you create the All Part-Time Workers with an Annual Salary Basis value set that

includes this query:

 SELECT ASG.PERSON_ID

229

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 42
HCM Group Examples

 FROM PER_ALL_ASSIGNMENTS_M ASG
 , CMP_SALARY SAL
 , CMP_SALARY_BASES SB
 , HR_LOOKUPS EMP_CAT
 WHERE ASG.ASSIGNMENT_ID = SAL.ASSIGNMENT_ID
 AND SAL.SALARY_BASIS_ID = SB.SALARY_BASIS_ID
 AND SYSDATE BETWEEN ASG.EFFECTIVE_START_DATE AND ASG.EFFECTIVE_END_DATE
 AND SYSDATE BETWEEN Sal.Date_From AND SAL.DATE_TO
 AND ASG.PRIMARY_FLAG = 'Y'
 AND ASG.EMPLOYMENT_CATEGORY = EMP_CAT.lookup_code
 and emp_cat.lookup_type = 'EMP_CAT'
 and emp_cat.lookup_code = 'PR'
 and sb.name = 'Annual Basis'

In this query, 'PR' identifies the Part-Time Regular employment category.

Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time and Labor Value Sets.

2. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > HCM Groups.

3. Create the HCM group.

a. Enter a name, such as All PTE with Annual.
b. Enter a description, such as Uses a value set to find all part-time equivalent employees with an annual

salary basis.
In the Include or Exclude Groups section, click the Add Value Set icon to insert a value set table row.

c.
d. Select the value set, such as All Part-Time Individuals with an Annual Salary Basis.
e. Specify whether to include or exclude members identified by the value set.
f. Save your changes and close the page.

4. Refresh the group membership.

a. Select the group to refresh.
b.
c. Submit the refresh process.

In the Evaluation Date field, select the current date.

Create an HCM Group by Embedding Other HCM Groups

Here's how you create an HCM group with embedded groups.

1. Create the groups to embed in this group. For example, you create the RN in CA on Primary Assign group and the All

PTE with Annual groups.

2. Go to Setup and Maintenance > Workforce Deployment > Time and Labor > HCM Groups.

230

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

3. Create the HCM group.

Chapter 42
HCM Group Examples

a. Enter a name, such as RN in CA on Primary Assign and All PTE with Annual.
b. Enter a description, such as Individuals with the Registered Nurses collective agreement, in a labor

c.

union, in California. And all part-time equivalent individuals with an annual salary basis.
In the Include or Exclude Groups section, embed the applicable groups and set the priorities. Here's an
example.

Priority

Group

1

2

RN in CA on Primary Assign

All PTE with Annual

When you embed groups within another group, a worker can exist in more than one group. The priority
numbers assigned to the embedded groups decide the group membership.

d. Specify whether the embedded group includes or excludes members. When the worker is a member of

multiple embedded group, the status of the highest-priority group decides whether the worker is included
or excluded.

e. Save your changes and close the page.

4. Refresh the group membership.

a. Select the group to refresh.
b.
c.
d. Submit the refresh process.

In the Evaluation Date field, select the current date.
In the Remove Future-Dated Group Members field, select No.

231

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 42
HCM Group Examples

232

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 43
Delivered Profiles and Time Entry Profiles

43  Delivered Profiles and Time Entry Profiles

How Time Entry Profile Components Work Together

A time entry profile specifies how linked individuals report, review, and submit time using time cards, calendar, and Web
Clock. It also specifies how their managers report, review, and submit time cards on behalf of individuals.

To create these profiles, go to Setup and Maintenance > Workforce Deployment > Time and Labor > Worker Time
Entry Profiles.

233

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 43
Delivered Profiles and Time Entry Profiles

Here's how the profile components work together.

Layout Sets
A layout set is a collection of layouts that decide the appearance of time card, calendar, Web Clock, and shift pages.
It also decides the time entry identifies used in change audits. For example, one layout set has layouts for people
who have the same payroll characteristics. Another layout set has layouts for people who have the same project

234

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 43
Delivered Profiles and Time Entry Profiles

costing characteristics. And a third layout set has layouts for people who have the same payroll and project costing
characteristics.

Time Attestation Sets
A time attestation set is a collection of questionnaires and their initiating events and time categories. The attestation
set lets you gather more information about reported time to make sure that people are complying with time policies and
various regulations. For example, you can have people who work when they aren't scheduled attest that they obtained
authorization beforehand.

Groups
An HCM group identifies people who share the same characteristics. All group members and their managers inherit the
layouts in the layout set of their assigned time entry profile. They also inherit the time attestation set, if selected. You
can assign each HCM group to only one time entry profile at a time.

Related Topics

• Time Attributes

• Overview of Layout Components for Time Entry

• Time Layout Sets

• Overview of HCM Group Membership

Delivered Time Entry and Processing Profiles

By default, all employees in an organization are members of delivered HCM groups linked to delivered time entry and
processing profiles. These delivered profiles apply to all employees.

The delivered time entry profiles use delivered time card fields, layout sets, and HCM groups. The delivered time
processing profiles use delivered repeating periods, time categories, time consumer sets, and HCM groups.

Delivered Time Entry Profiles

Delivered Time Processing Profiles

Description

Payroll Time Entry Profile

Payroll Time Processing Profile

For only the payroll time consumer

Projects and Payroll Time Entry Profile

Projects and Payroll Time Processing Profile

For the project costing, project execution
management, and payroll time consumers

Project Execution Management Time
Processing Profile

For only the project execution management
time consumer

Projects Time Entry Profile

Projects Time Processing Profile

For only the project costing time consumer

These delivered profiles don't include any time rules because the time repository includes only delivered time rule
templates. You use these delivered templates to create any rules and rules sets that you want to link to your own
profiles.

To save time when creating your own profiles, you can duplicate the delivered profile that most closely matches the
profile you need. Then, edit the duplicate profile, including the effective date, to support your time reporting policies.

235

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 43
Delivered Profiles and Time Entry Profiles

For example, to create a profile that uses the delivered Projects Layout Set Filtered by Project Team Members layout set,
duplicate Projects Time Entry Profile.

Related Topics

• How Time Entry Profile Components Work Together

• How Time Processing Profile Components Work Together

How You Set Allowable Actions for Time Entry

You can specify the actions that individuals, lines managers, and time and labor managers can do by time card status.
You can also set the number of days into the past and future they can do the enabled actions.

You make these configurations using the Worker Time Entry Profiles task.

Actions by Status
Enable individuals, line managers, and time and labor managers to create, view, edit, and delete time cards according
to your time card policies. For example, you've individuals who report time using Web Clock and correct any time
exceptions and issues by submitting change requests. So, you let them only view their Entered, Saved, Submitted,
Rejected, and Approved time cards. You've other individuals who report time with time collection devices and you
want them to fix any incomplete or in error issues. So, you enable them to edit only incomplete entries on classic and
responsive time cards with an Incomplete or In error status. If they’re using enhanced time cards and you enable these
edits, individuals can also edit or add entries.

To let individuals edit time entries generated from device events, be sure to also select the Allow edits to times
generated from device events option.

Days Before and After
You can optionally set the number of days before and after today that people can do the action for the enabled status.
For example, your policy is to let individuals edit submitted time cards up to 5 days before the current date. If that day
falls in a prior time card period, they can edit the current and previous time cards if the status is still Submitted.

If you don't set any number of days, people can always do the entry action on their time cards with the enabled statuses.
For example, you let individuals edit entered and saved time cards but don't set any number of days before or after.
They can edit their entered and saved time cards, regardless of how many time card periods the time cards are in the
past or future. But, as soon as the time card status changes to Submitted, they can't edit the time card.

Related Topics

• How Time Entry Profile Components Work Together

Manager Days Before and After Settings

Consider prior period ranges for allowable adjustments to time data when setting days before values for allowable time
entry actions on the Line Manager and Time and Labor Manager tabs.

236

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 43
Delivered Profiles and Time Entry Profiles

For example, to limit adjustments for all actions and statuses to the last quarter and next month, enter 90 days before
and 30 days after. The configuration on the manager tabs apply to all managers of individuals associated with the
profile. We recommend that you configure the managers tabs to support your typical adjustment policies for time cards.

Here's how you can handle exceptions that fall outside the typical adjustment periods:

1. Edit the relevant profile to remove the relevant days before or after values.
2. Make your time card adjustments.
3. Edit the relevant profile to re-enter the relevant days before or after values.

Time Collection Device and Web Clock Integration
Options on Time Entry Profiles

You can specify whether people can edit the time entries generated for them from their time collection devices,
including Web Clock. You can also enable geolocation and geofencing for Web Clock.

Geolocation
The collected geolocation information includes the Web Clock device used to report the time, such as Desktop, Mobile
Offline, or Mobile Online. It also includes the latitude and longitude accuracy in meters, and any exceptions, such as
rejected location requests.

Note:  You can record geolocation information and generate geolocation addresses for most, but not all countries. We
recommend that you test the countries where you work with geolocation information to make sure you can generate
the correct addresses from the geolocation coordinates.

GPS is a country-specific service. A time reporter's location, device, and other factors decide the accuracy and
availability of their geolocation information. For most exact information, we recommend that you enable this
functionality for people who use Web Clock on mobile devices because they've dedicated GPS sensors. Because desktop
devices don't have GPS sensors, their location is derived from the network, and it's likely to be less exact. Desktops that
use VPN connections are most likely to provide incorrect location information. Oracle HCM Cloud app versions that
support geolocation are 11.13.23.01.01 or later.

Note:  People with these time entry profiles are prompted to grant Location access when they use Web Clock on
mobile devices or in browsers on any supported device.

Geofencing
When you enable geofencing, you set the validation mode.

• Record and report: Shows the worker a message letting them know that their manager was notified that they

reported time outside their geofence. It also records the clock event with an exception.

• Restrict: Won't allow the worker to record web clock events outside the primary assignment work location.

If overriding the geolocation coordinates, you need to use the decimal Latitude, Longitude format, such as
17.449654755550803, 78.3741768166791. Web Clock geofences ignore the regional format set for numerals on the device
used to enter the overriding coordinates.

237

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 43
Delivered Profiles and Time Entry Profiles

Configure Geofences for Web Clock

To review existing geofences and create needed fences, go to My Client Groups > Show More > Geofences for Web
Clock.

Add one of more geofences around a location by adding a name and description, and selecting a location. The address
and derived coordinates are then populated from the selected location.

You can create more than one geofence around a work location. When a worker’s assignment has a work location, Web
Clock lets the worker use any of the geofences defined for the location when they report time.

Here's how you override the derived coordinates and create more work location geofences:

1. Copy the address to a clipboard and use your preferred map provider to search for the address.

2. Copy the geolocation coordinates from that provider and enter them, in Latitude, Longitude format, in the

Coordinates for Override Location field.

3. Set the Radius in Meters value for the location.

Schedule Option on Time Entry Profiles

You can specify whether schedulers can create shifts and edit shift properties for individuals linked to the scheduler
profile or only view existing shift details. By default, schedulers can edit shift properties.

You set this option using the Worker Time Entry Profiles task.

Note:  The configuration of this option on imported schedule events overrides the configuration on the time entry
profile. For example, you configure a profile to allow edits and import schedule events configured to not allow edits.
Schedulers can't edit those imported schedule events.

Related Topics

• How You Plan and Publish WFM Schedules

Worker Attestation Options

To identify if people are complying with time policies and various regulations, link a time attestation set to the time
entry profile. For example, have people who work when they aren't scheduled attest that they obtained authorization
beforehand.

You can optionally set the number of days before and after today that people can edit their attestations. For example,
your policy is to let people edit their attestations up to 5 days before the current date. If that day falls in a prior time
card period, they can edit the attestations for the current and previous time cards. If you don't set any number of days,

238

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 43
Delivered Profiles and Time Entry Profiles

people can always edit their attestations. It doesn't matter how many time card periods the time cards are in the past or
future.

Related Topics

• Time Attestation Sets

Cost Overrides Option on Time Entry Profiles

If the layout set that you link to the time entry profile includes the Cost overrides layout, you need to enable the cost
overrides option.

Doing this turns on the Override Costs option of the time entry level Actions menu on responsive time cards. The
people linked to the profile use the action to open the Cost Overrides page.

Related Topics

• Entries Section Configuration of the Responsive UI Layout

• Cost Overrides Layout Configuration

• Add and Configure Values for the Multiple-Attribute Time Card Field

239

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 43
Delivered Profiles and Time Entry Profiles

240

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 44
Time Measures and Time Processing Profiles

44  Time Measures and Time Processing
Profiles

Time Measure to Show Option

You can specify for classic and responsive time pages whether to show time measures in hours and minutes or set a
decimal place.

For example, enter and show quantities on time card pages in the format Hours, Minutes (HH:MM). On certain pages,
read-only quantities and durations in this format can appear in the format Hh Mm, for example, 15h 30m.

Enhanced, unified time pages use only decimal place options.

Hours decimal options specify the number of places to show to the right of the decimal. Your selection applies to pages
where time layouts don't control the appearance. For example, your selection applies to time measures on the Existing
Time Cards and Team Time Cards pages. It doesn't apply to the Create Time Card or Add Time Card pages.

By default, time card layouts, such as time entry, review, view, approval notification, and responsive UI, have Decimal
Places set to 2. You can edit the layouts to change this default, as appropriate. We recommend that you review all the
pages that correspond to any layouts in a layout set where you changed the default value. Make sure that the number of
decimal places that you see on each page is what you expect.

Time Entry Rules
Time entry rules can specify output messages that include the number of hours. Unchanged formulas and rule
templates delivered before 2020 use the decimal format. To create your own formulas that use the Hours format,
delivered reference the delivered formula ORA_TER_PERIOD_MAX_WITH_MSG_FORMAT_OPTION_AP.

Basic Process for Defining Time Measures

1. On the Worker Time Processing Profile page, Actions menu, select Define Time Measures.
2. On the Time Measure Properties page, select the measure to show.

Note:  Your selection applies across the entire Oracle Fusion Cloud Time and Labor environment. It isn't specific to the
individuals linked to a specific time processing profile, nor the managers acting on their behalf.

How Time Processing Profile Components Work
Together

A time processing profile identifies the time card period and time entries to use in linked validation, calculation,
approval, and transfer rules. It also identifies whether to audit time changes and when to start the audit.

241

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 44
Time Measures and Time Processing Profiles

To create these profiles, go to Setup and Maintenance > Workforce Deployment > Time and Labor > Worker Time
Processing Profiles.

Here's how the components that make up a time processing profile work together.

Repeating Time Periods
Repeating time periods, such as weekly, biweekly, or monthly periods, make up the choices for the time card period and
optional overtime period. They’re also selected as approval periods in time consumer sets. The approval period needs to
match the selected time card period. Otherwise, you might get errors when you try to link groups to the profile.

Time Category
A time category identifies the time entries to use in time rules, summaries, analytics, and transfers. For example, use all
payroll and absence entries or only all payroll entries.

242

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 44
Time Measures and Time Processing Profiles

Time Consumer Set
A time consumer set identifies the time data to validate for linked individuals. It also identifies the approval period
that applies to the linked individuals, and what data approval rules should use. And, it specifies when to transfer the
validated time data. For example, for the Payroll consumer validates all payroll time entries whenever linked individuals
or their managers save or submit their time cards. Transfer the validated payroll time data whenever someone runs the
Load Time Card Batches or Transfer Time Cards from Time and Labor process. The linked individuals have a weekly
approval period and approval rules evaluation calculated and absence time data. And, payroll approval is required
before the time data can transfer.

Time Calculation Rule Set
A time calculation rule set collects related calculation rules and rule sets that support time processing policies. For
example, automatically allocate time across cost segments or grants and calculate daily and weekly overtime for the
linked individuals. The rules in the selected rule set also apply to time entries created using web clock events and third-
party device events.

Time Entry Rule Set
An entry rule set contains time entry rules and rule sets that support time validation policies. For example, enforce
minimum and maximum worked hours and generate exceptions when linked individuals start or stop their shifts too
early or late. The rules in the selected rule set also apply to time entries created using web clock events and third-party
device events.

HCM Group
An HCM group identifies people who share common characteristics. All group members and their managers inherit the
repeating periods, the consumer set, and the rule sets in their assigned processing profile. You can assign each HCM
group to only one time processing profile at a time.

Related Topics

• Repeating Time Periods

• Time Categories

• Approval Options in Time Consumer Sets

• Time Formula and Rule Types

• Overview of HCM Group Membership

Enable Resubmission of Future Time Cards Option

A person's information, such as the payroll relationship or assignment status, can change retroactively. These
information changes can also change the person's associated layout set, time card period, or both. And, the person can
add absences to and change absences on existing time cards.

To include future time cards for linked individuals when the Resubmit Time Cards process runs, select the Enable
Resubmission of Future Time Cards option. This option is on time processing profiles.

243

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 44
Time Measures and Time Processing Profiles

Related Topics

• Resubmit Time Cards Process

Submit Time Cards for Scheduled Processing Option

By default, when people click Submit on time cards, the applicable time consumer validation and time entry and
calculation rules run immediately.

If your company has complex calculation rules or people with monthly time cards, we encourage you to submit time
cards for scheduled processing. This way, the time consumer validation, time entry, and time calculation rules for the
linked individuals run in the background. These individuals and their managers can review any issues and calculated
time data results later, after the process completes.

You set this option on time processing profiles.

• When you select this option and linked individuals click Submit on their time cards, their Existing Time Cards
page opens. The page has a submission pending message over the submitted time card. When managers
click Submit on a time card, their Team Time Cards page opens with the same message. After time entry and
calculation processing completes, other messages replace the submission pending message. The messages
could be about exceptions that need fixing. Or, if there aren't any exceptions, the new message indicates that
approval is pending for the time card.

• When you don't select this option, the linked time entry and calculation rules run immediately. Messages about

any exceptions appear on the time card, which is still open. If the rules don't generate any exceptions, the
Existing Time Cards or Team Time Cards page opens. The time card shows with the message that approval is
pending.

Related Topics

• Submit Queued Time Cards Process

Change Audit Options

You can track who did what classic, responsive, or enhanced time card action--such as save, submit, and approve--and
when. You can also track who changed time entries, including absences, and when and why.

Go to Setup and Maintenance > Workforce Deployment > Time and Labor > Worker Time Processing Profile.

Note:  As soon as you enable change audit, you can't delete audited time cards. But, you can delete time entries on
audited time cards.After you enable change audit, changes get tracked automatically from the specified starting point.
For example, you can set change auditing to automatically start after the first time a time card gets submitted or
approved. Or, you can automatically audit any manual changes to the time card.

244

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 44
Time Measures and Time Processing Profiles

Before Enabled Change Audit Can Work
For enabled change audit of time cards to work properly, you need to complete these tasks in the Setup and
Maintenance work area.

• Workforce Management Lookups: Support your time policies by adding change audit reasons to the

ORA_HWM_CA_REASONS lookup type. This lookup makes up the change audit reason drop-down list that
appears after people save or submit edited time cards.

• Time Layout Sets: Select the time card fields that, when combined, enable people to identify a time entry

that changed. For example, on one set of layouts, the Job and Pay Type fields together uniquely identify time
entries.

Public Holidays on Time Cards Option

When you're configuring time cards to automatically add public holiday entries, you can set the default value for the
payroll time type attribute.

For example, you created payroll elements for different countries using names like US Public Holidays, UK Public
Holidays, and Bangalore Public Holidays. For people in the US, you want to set US Public Holidays as the default value
for their public holiday entries. Use the Worker Time Processing Profile task in the Setup and Maintenance work area.
The task is part of the Workforce Deployment offering, Time and Labor functional area.

You might have profiles for people who work across multiple legislative data groups (LDGs), such as the US and Canada.
The time attribute value of the holiday entry gets set automatically only for people in the same LDG as the public
holiday element. For example, you select the US Public Holiday payroll element. The element gets used for people in
the US LDG. It doesn't get used for people in the Canada LDG. To automatically add holiday entries for everyone, you
need to create separate profiles for the two LDGs. The fastest way to do this is to duplicate the existing profile and then
update the configurations accordingly, including HCM group assignments.

Tip:  You can stop the automatic creation of public holiday entries at any time. Just clear the value from the Payroll
Element to Automatically Add Entries field on the time processing profile.

Automatic Time Card Entries
To automatically add public holiday entries to time cards, you need to complete these tasks in the Setup and
Maintenance work area.

• Create a payroll element for public holidays, for each LDG using the Elements task. These elements get used in
time card drop-down lists and to set the time attribute value when creating public holiday entries on time cards.

• Run the Generate Data Dictionary Time Attributes process after creating your public holiday payroll elements.

• Set the payroll element as one of the payroll time type attribute values to include in the drop-down list of

the multiattribute time card field. If your field definition contains attributes for multiple LDGs, you can add
another row for each public holiday payroll element you created for those LDGs. Use the Time Entry Layout
Components task.

• Make sure that you defined all observed public holidays for the appropriate geography or organization trees.

Use the Manage Calendar Events task. Be sure to set the Category to Public holiday. Also, define full-day public
holidays as 12:00a to 12:00a.

245

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 44
Time Measures and Time Processing Profiles

• Make sure that your people have one of these types of schedules defined: Work Week, Work Schedule, or

Standard Working Hours. For Work Schedule, make sure that the Public holiday event category is added as an
exception.

Related Topics

• Basic Process to Integrate Global Payroll and Time and Labor

• Create Time Card Elements for Time Entries

• How You Configure and Assign Work Schedules

• Basic Process to Create a Calendar Event Using a Geographic Tree

• Basic Process to Create a Work Schedule

On-Call Entries on Time Cards Options

You can automatically default on-call entries on enhanced time cards for worker assignments with on-call shifts
assigned. To identify the payroll element to apply to these entries, go to Setup and Maintenance > Workforce
Deployment > Time and Labor > Worker Time Processing Profile.

You can also specify a time category to use to identify the on-call payroll time types. These time types are excluded
from schedule deviation calculations and included in on-call schedule deviations. The calculation results show in the
Time Totals drawer of the enhanced time card. Here’s how total hours and schedule deviation results are calculated:

• Total Hours = All Hours - On-Call Time Category from Worker Time Processing Profile
• Schedule Deviation = Total Hours (All Hours - On-Call Time Category from Worker Time Processing Profile)

+ Equivalent Hours for Day Entries - Scheduled Hourse

246

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 45
Time Device Processing Profiles

45  Time Device Processing Profiles

How Time Device Processing Profile Components Work
Together

A time device processing profile identifies the application events and time attributes that form the time card entries for
linked individuals. It also specifies how to validate the time entries and when to automatically save and submit the time
cards.

To create these profiles, go to Setup and Maintenance > Workforce Deployment > Time and Labor > Time Device
Processing Profiles.

247

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 45
Time Device Processing Profiles

Here's how the components that make up a device processing profile work together.

Time Device Event Mapping Set
A time device event mapping set identifies the time card entries generated for the linked individuals, from time
collection device events.

A mapping set doesn't apply to Web Clock events because the application event and time attributes are part of the
button configurations. To run device and submission rules for clock events, you can create a profile that leaves this
option blank.

Time Device Rule Set
A time device rule set collects related validation rules and rule sets that support time device processing policies. For
example, automatically generate an information message if an In or Out event is outside the grace period for the

248

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 45
Time Device Processing Profiles

individual's scheduled shift. Generate warning messages if the event is inside the start early or late periods or stop early
or late periods. And, generate error messages if the event is outside the early or late periods.

Time Submission Rule Set
A time submission rule set identifies when to automatically save and submit the time card generated for the device or
clock event. For example, individuals linked to this profile badge or clock in at the start of their shifts, Monday through
Friday. And they badge or clock out at the end of their shifts. They don't badge or clock in or out for breaks and meals.
The rule in their set automatically saves their time cards after every Out application or clock event--at the end of their
workday. The same rule also submits their time cards after the fifth Out application or clock event, which is at the end of
their work week.

Time Device Export Data
A time device export data configuration sends relevant person, payroll, and schedule data to the time collection device
used by the linked individuals. The time device uses this export data to complete each time event transaction created by
the linked individuals.

Web Clock doesn't require export data because it gets person and schedule data directly from the time repository. And,
relevant payroll time data]s part of each button definition. To run device and submission rules for clock events, you can
create a profile that leaves this option blank.

HCM Group
An HCM group identifies people who share common characteristics. All group members and their managers inherit the
event mapping set, device and submission rule sets, and export data in their assigned device processing profile. Group
members who use Web Clock, and their managers, inherit the device and submission rule sets in their assigned device
processing profile. You can assign each HCM group to only one device processing profile at a time.

Related Topics

• Time Device Event Mappings

• Time Formula and Rule Types

• Overview of HCM Group Membership

• Export Data to Time Collection Devices Process

Time Attributes for In and Out Event Matching

You can select one or more time attributes to use to match In and Out device events, to create time entries.

An In event makes up the first part of a time entry. The incomplete entry becomes a complete entry when an Out event
matches to it. Time card processing matches an Out event to the nearest In event before it, accounting for any matching
time attribute option.

In Has Attribute and Out Doesn't
Here are the two most recent device events received:

•

In event with a Payroll Time Type of Regular

249

Chapter 45
Time Device Processing Profiles

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

• Out event without a payroll time type

These two events make up a time entry with the Regular payroll time type attribute.

In Doesn't Have Attribute and Out Does
Here are the two most recent device events received:

•

In event without a payroll time type

• Out event with a Payroll Time Type of Meal

These two events make up a time entry with the Meal payroll time type attribute.

In and Out Have Different Attribute Values
Here are the two most recent device events received:

•

In event with a Payroll Time Type of Regular

• Out event with a Payroll Time Type of Meal

While both events have a Payroll Time Type value, the values are different and thus the events don't match. These
events make up two incomplete time entries:

• An entry with the start time and an In event with the Regular payroll time type that's missing the stop time of

the Out event

• An entry with the stop time and an Out event with the Meal payroll time type that's missing the start time of an

In event

Someone needs to fix these incomplete entries before the time card can be submitted.

In and Out Have Same Attribute Values
Here are the two most recent device events received:

•

In event with a Payroll Time Type of Regular

• Out event with a Payroll Time Type of Regular

These two events make up a time entry with the Regular payroll time type attribute.

250

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 46
Time Profile Assignments, Priorities, and Comparison

46  Time Profile Assignments, Priorities, and
Comparison

Group Assignments on Time Profiles

You use start and end dates to assign time entry, processing, and device processing profiles to groups of individuals for
these reasons:

• You can assign more than one group to a single profile. For example, you assign the USA_Individs profile to the

FullTime_USA_Individs and PartTime_USA_Individs groups.

• You can't assign a single group to more than one profile of the same type at the same time. For example, the
FullTime_USA_Individs group can't have active assignments for both the USA_Individs and UK_Individs time
entry profiles.

You assign groups to profiles using these tasks:

• Worker Time Entry Profiles

• Worker Time Processing Profiles

• Worker Time Device Processing Profiles

Related Topics

• How Time Entry Profile Components Work Together

• How Time Processing Profile Components Work Together

• How Time Device Processing Profile Components Work Together

• Overview of HCM Group Membership

Priority of Time Profiles

You assign each time entry, processing, and device processing profile a unique priority number relative to other profiles
of the same type.

The priority decides an individual's profile if they're eligible for multiple profiles of the same type. The highest priority is
1. For example, an individual is linked to these two time entry profiles:

• US_Western, which has a priority of 5

• US_CA, which has a priority of 3

Because US_CA has a higher priority, that time entry configuration applies.

Related Topics

• How Time Profiles Get Derived

251

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 46
Time Profile Assignments, Priorities, and Comparison

How Time Profiles Get Derived

Through HCM group membership, an individual can be eligible for multiple time entry, processing, and device
processing profiles. The assignment type for each of an individual's eligible profiles decides the single profile of each
type that applies.

Priority

Assignment Type

Derivation Description

1

2

3

Individual Assignment

The profile with this assignment has the highest priority and overrides all group profile
assignments.

Make these assignments on the Troubleshoot page using the Assign Profile to Person button.

Group Assignment

The profile with the lowest priority applies when multiple group memberships qualify an
individual for multiple profiles of the same type.

Default Group Assignment

The profile with this group assignment applies to all individuals who don't have any profile
assignments. This way, they can report time and that time can get processed and transferred
to the appropriate time consumers.

Compare Time Profiles

Troubleshoot issues related to the unexpected appearance or disappearance of time card, web clock, or shift layouts
and unexpected rule results by comparing time profiles.

1. Go to My Client Groups > Time Management > Tasks panel > Worker Time Entry Profile, Worker Time

Processing Profile, or Worker Time Device Processing Profile.

2. Click Troubleshoot.

3. On the troubleshoot profile page, search for and select a person.

4. Specify the profile evaluation date.

5. To list the profiles with an effective assignment on that date, click Evaluate.

6. Select up to three of the person's profiles and view the various values for those profiles.

Related Topics

• How Time Profiles Get Derived

• Assign a Time Profile Directly to an Individual

• Delete a Direct Assignment for a Time Profile

252

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 47
Time and Labor Integration with Absence Management

47  Time and Labor Integration with Absence
Management

Basic Process to Integrate Absence Management and
Time and Labor

Let people report absences and view accrual balances on their time cards by integrating Oracle Fusion Cloud Absence
Management with Oracle Fusion Cloud Time and Labor.

You can find details about the setup tasks for Absence Management in the Implementing Absence Management guide.
The time and labor tasks are in the Setup and Maintenance work area. They're part of the Workforce Deployment
offering, Time and Labor functional area.

Absence Management Setup
Create the absence management configurations that support your absence and time management policies. Here are
key requirements when integrating with Time and Labor.

1. Make sure that a work schedule exists for each person's primary assignment.
2. Set the absence type units of measure to Hours or Days.
3. Enable the absence type for time card entry.
4. Enroll people in absence accrual plans that are associated with the absence type. Make sure that the plan

balances are up to date.

Time Entry Setup
Create the time entry configurations that support your time and absence reporting policies, as summarized here.

253

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 47
Time and Labor Integration with Absence Management

254

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 47
Time and Labor Integration with Absence Management

Also, create the time collection device configurations, as appropriate.

Time Processing Setup
Create the time processing configurations that support your time and absence processing policies, as summarized here.

255

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 47
Time and Labor Integration with Absence Management

Related Topics

• Time Entry Setup and Maintenance Tasks

• Time Processing Setup and Maintenance Tasks

• Overview of Time Collection Device and Web Clock Event Processing

• Assign the Weekly Day Office, Night Home Work Schedule

• How Absence Components Work Together

Compensatory Time and Time Cards

You can need people to work excess hours outside of their regular work schedule, such as overtime hours or hours
worked on a holiday.

256

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 47
Time and Labor Integration with Absence Management

You can convert these excess hours to earned compensatory time off, also known as time off in lieu (TOIL), instead
of monetary compensation. People can then record absences against the defined compensatory plan specific to your
policies when they take time off in the future.

Here's how people earn and use compensatory time:

1. They report earned time on the same Oracle Time and Labor Cloud time cards that they use to report

regular worked hours. This earned time transfers to Oracle Absence Management Cloud and updates the
corresponding plan balance.

2. They apply for paid time off using the corresponding compensatory absence plan.

To provide seamless integration between Time and Labor and Absence Management, you need to complete some setup
tasks. When you finish, compensatory time reported on time cards will automatically transfer to the corresponding
absence plans.

Related Topics

• How You Set Up Compensatory Time in Time and Labor

• How You Set Up Compensatory Time in Absence Management

How You Set Up Compensatory Time in Absence
Management

Here's what you need to do to implement compensatory time in Oracle Fusion Cloud Absence Management. The tasks
are in the Absence Management work area.

1. Create an absence plan with the Compensatory plan type and define the related attributes for compensatory time.

Use the Absence Plans task.

2. Create an absence type for compensatory time absence entry. Use the Absence Types task.

3. Link the absence type to the compensatory time plan. Use the Absence Types task.

What to do next

After you define the absence plan and absence type, you can enroll people in the linked compensatory plan. Use the
Absence Records task in the Person Management work area.

Related Topics

• Compensatory Time and Time Cards

• Options to Define Compensatory Plans

How You Set Up Compensatory Time in Time and Labor

To report and calculate earned compensatory time and take compensatory absences, go to Setup and Maintenance >
Workforce Deployment > Time and Labor and complete the time entry and processing configuration tasks.

257

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 47
Time and Labor Integration with Absence Management

Time Entry
Here are the configuration tasks you need to complete for time entry.

Step

Task

Description

1

2

3

4

Generate Data Dictionary Time
Attributes

Link time attributes stored in the data dictionary with any absence types enabled for time
entry. These attributes identify the time data for transfer to Absence Management for
processing.

The absence types make up the drop-down list for the Absence Management Type attribute.
You use these drop-down list values when you create time card fields and web clock buttons.
Time reporters use them when they report time worked and time off.

Time Entry Layout Components

Create a multiattribute time entry field that includes the time attributes Absence
Management Type and Compensatory Time Absence Plan.

•

•

In one row, you select the absence management type that decrements the person's
earned compensatory time--the compensatory absence.

In another row, you select the compensatory time absence plan that increments the
person's earned compensatory time.

If the individuals with time layouts that include this field have multiple compensatory
plans, we suggest you use the Assignment based List of Compensatory Time Absence
Plan for User filtered data source.

Optionally, create a dependent field to set an expiration date for earned compensatory time.

Time Layout Sets

Add the multiattribute field that includes compensatory time to the time entry, review,
view, and approval notification layouts, and the calendar entry layout. Optionally add the
dependent expiration date field to the entry-level details page of each layout.

If you use responsive time cards, then add the multiattribute field to the responsive UI
layout.

Worker Time Entry Profiles

Create profiles that link individuals and their managers to the layout set that includes the
compensatory time fields.

Time Processing
Here are the time processing tasks you need to complete.

Step

Task

Description

1

Time Rule Templates

Create rule templates to calculate earned compensatory time, as needed. Use time
categories in rule templates to identify the absence time data to use in the calculations.

You need to create rule templates for these conditions:

• You use your own formulas.

• You use multiattribute time card fields with more than one stored time attribute.

You can use delivered rule templates if the time card field or web clock button stores a
single time attribute.

258

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 47
Time and Labor Integration with Absence Management

Step

Task

Description

2

3

4

Time Rules

Create time rules using the rule templates.

• Advanced time category rules identify time events and entries using complex logic not

available in the condition components of a time category.

• Time calculation rules generate earned compensatory time, which automatically

transfers to Absence Management.

Time Rule Sets

Create collections of time calculation rules that generate earned compensatory time.

Worker Time Processing Profiles

Create profiles that link individuals and their managers to the time calculation rule set that
generates earned compensatory time.

Related Topics

• How Time Entry Profile Components Work Together

• How Time Processing Profile Components Work Together

• Overview of Linking People to Time and Labor Objects

• Overview of HCM Group Membership

How You Override the Work Location for Accurate
Absence Accrual Calculations

For people in the US to accurately accrue time off, the time entry process reads and stores the work location set in their
assignments. You can let these people override the assignment work location on their time cards.

Use these delivered time attributes: Work Location Overrides and Work Location with US Hierarchy Overrides. The
data sources for the work location override time attributes use a delivered value set of valid HR work locations. You can
create your own value set using the delivered set as a template.

You can also define time balances for people in the US using delivered time balance dimensions that include these
location attributes:

• State (area1)

• County (area2)

• City (area3)

Then, you can use the time balances and generated database items in absence accrual formula to include time card
hours in absence calculations. Here are descriptions of the supported actions for each time attribute.

Delivered Time Attribute

Actions

Work Location Override

Overrides the work location of time balances used by absence accruals

Work Location with US Hierarchy Overrides Overrides the work location of time balances used by absence accruals

Transfers the state, county, and city values to payroll for processing

259

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 47
Time and Labor Integration with Absence Management

How You Configure Work Location Override

Before you can override work locations, you need to correctly configure Oracle Fusion Cloud Global Payroll element and
work location override objects.

You also need to go to Setup and Maintenance > Workforce Deployment > Time and Labor and complete these time
entry and processing configuration tasks.

Task

Description

Generate Data Dictionary Time Attributes

Associate time attributes stored in the data dictionary with payroll elements and element input values,
 known in Global Payroll as value definitions. These associations enable Global Payroll to process the
transferred time data.

Time Entry Layout Components

Create the time card fields for work location and select the data sources. You use the fields to configure
time entry, review, view, approval, and calendar layouts. If you use responsive time cards, then you
configure the responsive UI layout.

Time Layout Sets

Time Categories

Time Balance Dimensions

Time Balance Definitions

The delivered value set of HR work locations corresponds to organizational offices. For people who
don't work in an office, such as remote workers or consultants, you can add dependent State, County,
and City fields. These dependent fields enable them to provide the appropriate location details for their
time entries.

You don't create layout components for third parties with this task. You do use layout components
created with this task to configure these layouts:

• Time card layouts that managers use to resolve device-related time exceptions

• The approval notification layout

Create different layout sets for the pages that individuals and managers use to enter, view, review,
 and approve time data, including work location overrides. Add override work location time entry
fields when you want to let individuals or managers override the work location of the individual's
assignment.

You don't create third-party device layouts with this task. You do use these layouts for these
configurations:

• Time card pages that managers use to resolve device-related time exceptions

• The approval notification layout

Create and edit categories that identify the time entries to use in time balances, rules, summaries, and
transfers based on your time and payroll policies.

View the list of delivered time balance dimensions that use the US state, county, and city summation
contexts, and the absence accrual period.

Create the time balance definitions to use in absence accrual fast formula. The time balance definition
combines one of the delivered time balance dimensions and one or more time categories.

The balance dimension sums entries based on the US state (area1), county (area2), and city (area3)
values. The created balance definition defines a database item that you can use in the absence accrual
fast formula.

260

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 47
Time and Labor Integration with Absence Management

Related Topics

• Generate Data Dictionary Time Attributes

• Overview of Layout Components for Time Entry

• Time Categories

• Time Layout Sets

• Overview of How You Configure Database Items to Summarize Time

261

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 47
Time and Labor Integration with Absence Management

262

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 48
Time and Labor Integration with Global Payroll

48  Time and Labor Integration with Global
Payroll

Basic Process to Integrate Global Payroll and Time and
Labor

You can validate, approve, and transfer reported time to payroll for payment by integrating Oracle Fusion Cloud Global
Payroll with Oracle Fusion Cloud Time and Labor.

• You can find details about the payroll costing setup tasks in the Implementing Payroll Costing guide.

• You can find details about the global payroll setup tasks in the Implementing Global Payroll guide.

• The time and labor tasks are in the Setup and Maintenance work area. They're part of the Workforce

Deployment offering, Time and Labor functional area.

Payroll Setup
Create the payroll costing and global payroll configurations that support your payroll and time management policies.
Here are key requirements when integrating with Time and Labor.

1. Configure payroll costing to let people allocate time to different cost segments. It will also let people override

default cost segments on their time cards.

2. Create elements to store payroll time types from the time card and to transfer time to payroll or a third-party

application for processing.

3. Create rate definitions to show default and payroll calculated rates on time cards and get overrides from time

card entries.

4. Create the relevant calculation value definitions to link elements and rate definitions.
5. Confirm that the Employment page has the Time Card Required option selected for each person who reports

time.

Time Entry and Collection Device Setup
Create the time entry configurations that support your time entry and payroll policies, as summarized in these
diagrams. Here are some considerations when integrating with Global Payroll.

• Make sure that dependent time card fields showing calculated rates provided by payroll populate new entries

using the Based on payroll rate function.

• You can use delivered payroll time card fields, such as Payroll Time Type and Assignment Number. If you don't

have any changes to the delivered fields and display names, you can use the delivered payroll layout set.

263

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 48
Time and Labor Integration with Global Payroll

264

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 48
Time and Labor Integration with Global Payroll

Also, create the time collection device configurations, as appropriate.

Time Processing Setup
Create the time processing configurations that support your time processing and payroll policies, as summarized in the
diagram. Here are some considerations to keep in mind when integrating with Global Payroll.

• Repeating periods for reporting and approving time can be weekly or biweekly.

• Approval periods need to match the reporting period so that the approval workflow tasks run as soon as people

submit their time cards.

• Payroll periods can be weekly, biweekly, semimonthly, or monthly.

265

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 48
Time and Labor Integration with Global Payroll

Related Topics

• Time Entry Setup and Maintenance Tasks

• Time Processing Setup and Maintenance Tasks

• Overview of Time Collection Device and Web Clock Event Processing

Create Time Card Elements for Time Entries

Time card elements support hours-based and units-based quantities. You use the units-based quantities to assign
people a flat payment amount through associated rates. For example, you pay people a meal allowance according to the
number of meals they take daily.

When you create a time card element, you also create the related payroll elements, balances, formulas, and calculation
components.

266

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 48
Time and Labor Integration with Global Payroll

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

267

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 48
Time and Labor Integration with Global Payroll

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

• Create the Units-Based Meals Taken Element for Time Entries

• Process Time Entries in Payroll

• Time Card Required Option

• Time Card Updates to Payroll

• Calculate Time Based on a User-Defined Value

Generate Time Attributes and Time Card Fields for Your
Elements

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

268

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 48
Time and Labor Integration with Global Payroll

Related Topics

• Time Attributes

• How Time Entry Profile Components Work Together

Create the Units-Based Meals Taken Element for Time
Entries

You're creating a units-based meals taken time card element with an associated flat rate from payroll.

1. Confirm that the Meal rate definition exists or create it using the Rate Definitions task in the Payroll Calculations work

area.

2. Go to Setup and Maintenance > Workforce Deployment > Elements and Formula > Elements.

3. Create the time card element.

a. On the Create Element dialog box, complete the fields, as shown here.

Field

Legislative Data Group

Primary Classification

Category

Value

FR LDG

Earnings

Time Card

b. Click Continue.

4. Configure the element.

a. On the Create Element: Basic Information page, complete the fields, as shown here.

Field

Name

Reporting Name

Value

Meals Taken

Meals Taken

Description

Units-based nonrecurring earnings element with an associated pay rate

Effective Date

January 1, 1951

b. To accept the remaining default values, click Next.
c. On the Create Element: Additional Details page, complete the fields, as shown here.

Field

Value

What is the calculation rule?

Meals Taken

269

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 48
Time and Labor Integration with Global Payroll

Field

Value

Does this element have a default rate

Yes

definition?

Rate Name

Meal Rate

If you don't specify a default rate, the element uses the rate from the salary record.

Effective Date

January 1, 1951

d. Click Next.
e. On the Create Element: Review page, review the element configuration to ensure that everything is correct.
f. Click Submit.

5. Configure the element eligibility.

a. On the Element Summary: Meals Taken page, in the Elements Overview section, select Element Eligibility.
b. On the toolbar Actions menu, select Create Element Eligibility.
c.

In the General Information section, Element Eligibility Name field, enter Meals Taken Open. Appending
Open is a standard method to easily identify that no eligibility criteria constrains the people the element
applies to. Time and labor administrators and managers typically constrain eligibility using HCM groups
and worker time entry and processing setup profiles.

d. Click Submit.
e. Click Done.

6. Configure element eligibility for each of the related elements, which share the same name as this element and have

suffixes. Suffixes include Earnings Calculator, Earnings Distributor, Earnings Results, Retro, and Retro Results.

a. On the Elements page, search for the element that you just created.
b. Click the related element name.
c. On the element summary page, complete these steps:

i.
In the Elements Overview section, select Element Eligibility.
ii. On the toolbar Actions menu, select Create Element Eligibility.
iii.

In the General Information section, Element Eligibility Name field, enter the element name and
append the term Open, for example Meals Taken Earnings Calculator Open.

iv. Click Submit.
v.
d. Click Done.

7. Generate the time attributes in the data dictionary. Use the Generate Data Dictionary task in the Setup and

Maintenance work area. The task is part of the Workforce Deployment offering, Time and Labor functional area.

a. On the Generate Data Dictionary Time Attributes page, in the Legislative Data Group field, select US LDG.
b. Click Submit.
c. On the Confirmation dialog box, click OK.

Related Topics

• Create Time Card Elements for Time Entries

270

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 49
Time and Labor Integration with Project Costing

49  Time and Labor Integration with Project
Costing

Set Up Project Costing for Use with Time and Labor

Let people working on projects report their billable hours on time cards by integrating Oracle Fusion Cloud Project
Costing and Oracle Fusion Cloud Time and Labor. Then you can automatically validate reported project time entries and
transfer validated entries to Project Costing.

These tasks are in the Setup and Maintenance work area, Project Financial Management offering.

1. Classify departments as expenditure organizations.

To let people submit time cards, the department on the person's employment record needs to be an expenditure
organization. These tasks are in the Project Organizations functional area.

a. For each department, select the Classify as project expenditure organization option. Use the Manage

Project Organization Classifications task.

b. To apply your changes, use the Submit Process to Maintain Project Organizations task.

2. Populate the Project Foundation tables because the project value sets are the data sources for these delivered time

card fields. Use the Manage Project Foundation Value Sets task in the Project Foundation functional area.

◦ Project Name for Project Team Members
◦ Project Name
◦ Project Number
◦ Task Number
◦ Project Unit
◦ Expenditure Type
◦ Expenditure Type Name
◦ Organization
◦ Expenditure Type Class (application linkage function)
◦ Billable
◦ Work Type

Option attributes:

◦ Capitalizable
◦ Contract
◦ Expenditure Organization
◦ Expenditure Type
◦ Expenditure Type Name
◦ Funding Source
◦ Project Name

271

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 49
Time and Labor Integration with Project Costing

◦ Project Name for Project Team Members
◦ Project Number
◦ Project Number for Project Team Members
◦ Task Number
◦ Task Number for Project Team Members

Related Topics

• Overview of Time Entry Configuration for Only Project Costing and Project Costing and Payroll Combined

• Overview of Time Card Processing Configuration for Only Project Costing and Project Costing and Payroll

Combined

• Overview of Grants Management Configuration

Overview of Time Entry Configuration for Only Project
Costing and Project Costing and Payroll Combined

You can let people report only project costing time on time cards or project costing, payroll, and absence time. You can
use delivered data sources, time card fields, layouts, HCM groups, and time entry profiles.

These layout configurations support time reporting for only project costing or project costing according to team
membership. There's also a layout that supports reporting time for project costing, payroll, and absences combined. Or
you can create your own configurations, as shown here.

272

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 49
Time and Labor Integration with Project Costing

If you create your own value sets and time card fields, then you need to create your own layout sets and time entry
profiles. You also need to create layout sets and profiles if you use delivered fields that the delivered layout sets don't
include. For example, you want to track funding sources and expenditure organizations for sponsored projects using
delivered fields. To do this, you need to create layout sets that include these fields and profiles that link to the new
layout sets.

To use the delivered time entry configurations with your own HCM groups, you only need to create time entry profiles.
You can link the delivered value sets, time card fields, and layout sets to your HCM groups using your profiles.

Tip:  To save time if you create your own objects, search for and duplicate the closest delivered project costing or
project costing and payroll object.

Related Topics

• Basic Process to Integrate Absence Management and Time and Labor

• Time Entry Setup and Maintenance Tasks

• Best Practices for Creating Time Entry Objects

• How Many Time Entry Layout Components, Categories, and Layout Sets to Create

• Create Value Sets to Use with Custom Time Attributes

273

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 49
Time and Labor Integration with Project Costing

Initial Assignment Info and Payroll Relationships Setup

To let new hires report project costing work on time cards, you need to set up their initial assignment information and
payroll relationships. Go to New Person > Hire an Employee.

To view and maintain assignments and payroll relationships for existing employees, go to Person Management >
Employment and Payroll Relationships.

To filter time card drop-down lists by project team membership, assign people to project teams. To enable team
membership, edit the Projects Party table, go to Project Financial Management > Manage Project Definition.

Related Topics

• Delivered Project-Specific Time Card Fields and Data Sources

• Time Layout Sets

• Overview of Linking People to Time and Labor Objects

• How Time Entry Profile Components Work Together

• Basic Time Entry Layout Component Configuration Process

Delivered Project-Specific Time Card Fields and Data
Sources

The delivered time repository includes project-specific time card fields and data sources to expedite time entry setup for
project costing and project execution management. The delivered data sources are value sets.

Primary Assignment ID
Project time entry includes the delivered Primary Assignment ID time card field. The delivered data sources use the
same private view object, List of Assignments, which contains all employees with a payroll relationship.

Single-Attribute Fields for Projects
Here are the project-specific single-attribute time card fields and the value sets that are their filtered and unfiltered data
sources. Here also are the layout sets that use each field.

Delivered Projects Fields

Delivered Value Set

Layout Set

Project Number

Filtered: PJC_PROJECTS_NUMBER_EXPEND_T_
V

Projects Layout Set

Unfiltered: PJC_PROJECTS_NUMBER_EXPEND_
A_T_V

274

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 49
Time and Labor Integration with Project Costing

Delivered Projects Fields

Delivered Value Set

Layout Set

Optional Project Number

Filtered: PJC_PROJECTS_NUMBER_EXPEND_T_
V

Projects and Payroll Layout Set

Unfiltered: PJC_PROJECTS_NUMBER_EXPEND_
A_T_V

Project Number for Project Team Members

Filtered: PJC_PROJECTS_NUMBER_
TEAMMEMBER_T_V

Projects Layout Set Filtered by Project Team
Members

Unfiltered: PJC_PROJECTS_NUMBER_EXPEND_
A_T_V

Project Unit

Filtered and unfiltered: PJC_PROJECT_UNIT_T_
V

Projects Layout Set
Projects Layout Set Filtered by Project Team
Members

Projects and Payroll Layout Set

Task Number

Filtered: PJC_TASKS_EXPEND_T_V

Projects Layout Set

Unfiltered: PJC_TASKS_EXPEND_A_T_V

Optional Task Number

Filtered: PJC_TASKS_EXPEND_T_V

Projects

Unfiltered: PJC_TASKS_EXPEND_A_T_V

Task Number for Project Team Members

Filtered: ORA_PJC_TASKS_EXPEND_
TEAMMEMBER_T_V

Projects Layout Set Filtered by Project Team
Members

Unfiltered: PJC_TASKS_EXPEND_A_T_V

Expenditure Type Name

Filtered: ORA_PJC_EXPENDITURE_TYPES_
NAME_T_V

Projects Layout Set

Unfiltered: ORA_PJC_EXPENDITURE_TYPES_
NAME_A_T_V

Projects Layout Set Filtered by Project Team
Members

Expenditure Type Class

Filtered and unfiltered: PJC_EXPEND_TYPE_
CLASS_T_V

Projects Layout Set

Projects Layout Set Filtered by Project Team
Members

Projects and Payroll Layout Set

Expenditure Type(hidden)

Filtered: PJC_EXPENDITURE_TYPES_EXPEND_
T_V

Projects Layout Set

Unfiltered: PJC_EXPENDITURE_TYPES_
EXPEND_A_T_V

Projects Layout Set Filtered by Project Team
Members

Projects and Payroll Layout Set

Contract Number

Filtered: ORA_PJC_CONTRACT_NUMBER_T_V

Available for projects layouts

275

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 49
Time and Labor Integration with Project Costing

Delivered Projects Fields

Delivered Value Set

Layout Set

Unfiltered: ORA_PJC_CONTRACT_NUMBER_A_
T_V

Funding Source

Filtered: ORA_PJC_CONTRACT_FUNDING_
SOURCE_T_V

Available for projects layouts

Unfiltered: ORA_PJC_CONTRACT_NUMBER_A_
T_V

Expenditure Organization

Filtered: ORA_PJC_EXPEND_ORGANIZATION_
T_V

Available for projects layouts

Unfiltered: ORA_PJC_EXPEND_
ORGANIZATION_A_T_V

Capitalizable

Filtered: ORA_PJC_CAPITALIZABLE_
IDENTIFIER_T_V

Available for projects layouts

Unfiltered: o ORA_PJC_CAPITALIZABLE_
IDENTIFIER_A_T_V

Project Role

Filtered: ORA_PJC_PROJECT_ROLE_T_V

Available for projects layouts

Unfiltered: ORA_PJC_PROJECT_ROLE_A_T_V

Multiple-Attribute Fields for Projects and Payroll
Here are the time attributes that provide the field definition structure for the multiattribute Time Type field. This field
has time attributes for both Project Costing and Project Execution Management, and Global Payroll. Here also are the
corresponding delivered data sources.

Delivered Time Attribute

Delivered Data Source

Data Sources Type

Expenditure Type Name

Filtered: ORA_PJC_EXPENDITURE_TYPES_
NAME_T_V

Value set

Unfiltered: ORA_PJC_EXPENDITURE_TYPES_
NAME_A_T_V

Payroll Time Type

Filtered: List of Payroll Time Types for User

Private view object

Unfiltered: List of Payroll Time Types for
Administrator

Absence Management Type

Filtered: List of Absence Types for User

Private view object

Unfiltered: List of Absence Types for
Administrator

276

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 49
Time and Labor Integration with Project Costing

Delivered Time Attribute

Delivered Data Source

Data Sources Type

Identifier

Related Topics

Filtered and unfiltered: Default format value set
for text

Value set

• Overview of Layout Components for Time Entry

• Delivered Time Card Fields

• Data Sources for Layout Components

• Delivered Time Layout Sets

• Create Value Sets to Use with Custom Time Attributes

Choice List Filters for Project Costing Time Cards

Time cards derive values for certain project-specific lists on the worker time card.

• To find the appropriate projects, the time card uses the worker's business unit. If the time card also filters by
team membership, the project names and numbers are for projects where the person is a team member.

• To find the appropriate tasks, the time card uses the selected project name or number. If the time card also

filters by team membership, the tasks are for projects where the worker is a team member.

• To find the appropriate expenditure types, the time card uses the selected project. It then uses the derived

project unit to find the appropriate expenditure types.

Overview of Time Card Processing Configuration for
Only Project Costing and Project Costing and Payroll
Combined

To process time data for only project costing or project and payroll combined, you can use delivered time processing
profiles. These profiles use delivered repeating time periods, time categories, time consumer sets, and HCM groups.

The profile configurations support project-specific time processing. Or you can create your own configurations, as
shown here.

If you create any of your own repeating time periods, time categories, and time consumer sets, then you
need to create your own processing profiles. To use the delivered time processing configurations with
your own HCM groups, then you only need to create time processing profiles. You can link the delivered

277

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 49
Time and Labor Integration with Project Costing

repeating time periods, time categories, and time consumer sets to your HCM groups using your profiles.

Related Topics

• Repeating Time Periods

• Time Consumer Sets

• How Formulas and Time Rule Components Work Together

• Overview of Linking People to Time and Labor Objects

• How Time Processing Profile Components Work Together

278

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

50  Best Practice Configurations for Time
Entry and Processing

Time Configuration When Hire Today Is on the Same Day
or a Future Day

You hire someone today with a hire date that's also today, or a future date.

Best Practice Configuration
Starting on the hire date, the active employee becomes a member of relevant HCM groups. Membership can be manual
or automatic, according to HCM group inclusion and exclusion conditions. Group membership automatically associates
the employee with time entry and processing profiles that include those HCM groups.

Functional Tasks Supported by This Configuration
Before the hire date, no person or scheduled process can create, process, approve, or transfer time data for the person.
Here's what happens after the hire date:

• Everyone with the appropriate privileges can create, edit, delete, and submit time cards for the person.

• Approval, rejection, and informational notifications get sent automatically to recipients when the person's time

cards get submitted. Task configurations for time card approval workflows identify the recipients.

• Administrators for applicable time consumers, such as payroll, transfer the approved time data. The person's
the configurations for the time consumer set and the time card approval workflow decide time data approval.

Example
Here's a visual example in context of a sample time line where the hire date is after today.

279

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

280

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

Time Configuration When Terminate Today Is on the
Same Day or a Future Day

You terminate someone's employment today with an employment termination date that's also today, or a future date.

Best Practice Configuration
The group membership configuration has the person continue as a member of relevant HCM groups even after the
employment termination date. The group membership keeps the person automatically associated with active time entry
and processing profiles that include those HCM groups.

Functional Tasks Supported by This Configuration
Here's what happens before and after the employment termination date:

• Everyone with the appropriate privileges, and scheduled processes, can create, edit, delete, and submit time
cards for the person. This protects the sensitive period so that the person can't detect a future employment
termination entered in Global HR.

• Approval, rejection, and informational notifications get sent automatically to recipients when the person's time

cards get submitted. Task configurations for the time card approval workflows identify the recipients.

Before the employment termination date, administrators for applicable time consumers, such as payroll, transfer the
approved time data. The configurations for the person's time consumer set and the time card approval workflows
decide time data approval.

After the employment termination date, administrators for applicable time consumers, such as payroll, can't transfer the
approved time data.

Example
Here's a visual example in context of a sample time line where the employment termination date is after today.

281

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

282

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

Time Configuration When Terminate Today Is on an
Earlier Date

You terminate someone's employment today with an employment termination date that's earlier than today.

Best Practice Configuration
Starting on the employment termination date, the active employee becomes an inactive employee and changes HCM
group memberships. The membership change can be manual or automatic, according to HCM group inclusion and
exclusion conditions. The change in group membership automatically changes the time entry and processing profiles
that the now inactive employee is associated with.

Functional Tasks Supported by This Configuration
Before and after the employment termination date, the person can't create, edit, delete, or submit time entries. Here's
what happens before the employment termination date:

• Managers with the appropriate privileges have full access to time data for the active employee before the

employment termination date and can make any required changes. Scheduled processes can also adjust time
data for the active employee.

• Approval, rejection, and informational notifications get sent automatically to recipients when the active
employee's adjusted time cards get submitted. Task configurations for the time card approval workflows
identify the recipients.

• Administrators for applicable time consumers, such as payroll, transfer the approved time data. The active

employee's configurations for the time consumer set and the time card approval workflows decide time data
approval.

After the employment termination date, no person or scheduled process can create, process, approve, or transfer time
data for the inactive employee.

Special Case
When the employment termination date is before today and the person is still on site, we recommend that you set the
HR employment termination date to today. Then, follow the scenario in the topic Time Configuration When Hire Today Is
on the Same Day or a Future Day.

Example
Here's a visual example in context of a sample time line where the employment termination date is before today.

283

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

284

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

Related Topics

• Time Configuration When Hire Today Is on the Same Day or a Future Day

Time Configuration When Terminate Today Is on the
Same Day or a Future Day, and Rehire Is a Future Day

Today you terminate someone's employment and rehire them with an employment termination date of today, or a
future day. The rehire date is a future day.

Best Practice Configuration
The group membership configuration has the person continue as a member of relevant HCM groups even after the
employment termination date. The group membership keeps the person automatically associated with active time
entry and processing profiles that include those HCM groups. Starting on the rehire date, the active employee changes
HCM group memberships because of the new job. The membership change can be manual or automatic, according to
group inclusion and exclusion conditions. The change in group membership automatically changes the time entry and
processing profiles that the active employee is associated with.

Functional Tasks Supported by This Configuration
Here's what happens before and after the employment termination date, and before the rehire date:

• Everyone with the appropriate privileges, and scheduled processes, can create, edit, delete, and submit time
cards for the person. This protects the sensitive period so that the person can't detect a future employment
termination entered in Global HR. Between the employment termination and rehire dates, managers with the
appropriate privileges can adjust and resubmit.

• Approval, rejection, and informational notifications get sent automatically to recipients when the person's time

cards get submitted. Task configurations for the time card approval workflows identify the recipients.

Before the employment termination date, administrators for applicable time consumers, such as payroll, transfer the
approved time data. The person's configurations for the time consumer set and the time card approval workflows
decide time data approval. After the employment termination date and before the rehire date, they can't transfer the
approved time data.

Here's what happens after the rehire date:

• Everyone with the appropriate privileges, and scheduled processes, can create, edit, delete, and submit time

cards for the person in the new job.

• Approval, rejection, and informational notifications get sent automatically to recipients when the person's time

cards get submitted. Task configurations for the time card approval workflows identify the recipients.

• Administrators for applicable time consumers, such as payroll, transfer the approved time data. The person's

new time consumer set configuration and the time card approval workflow task configurations decide time data
approval.

285

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

Example
Here's a visual example in context of a sample time line where the employment termination and rehire dates are future
days.

286

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

287

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

Time Configuration 1: When Today Is After Termination
and Before Rehire

Today is after the person left, the employment termination date, and before the rehire date. You must make adjustments
and payment before the rehire date.

Best Practice Configuration
Starting on the employment termination date, the active employee becomes an inactive employee and changes HCM
group memberships. Starting on the rehire date, the person is an active employee again and changes HCM group
memberships because of the new job. The membership changes can be manual or automatic, according to group
inclusion and exclusion conditions and whether the employee is active or inactive. The change in group membership
automatically changes the time entry and processing profiles that the active and inactive employee is associated with.

Functional Tasks Supported by This Configuration
Here's what happens before the employment termination date:

• The person and line manager can't create, edit, delete, or submit time entries.

• Time and labor managers with the appropriate privileges, and scheduled processes, can adjust and submit time

card data for the person.

• Approval, rejection, and informational notifications get sent automatically to recipients when the person's
adjusted time data gets submitted. Task configurations for the time card approval workflows identify the
recipients.

Between the employment termination and rehire dates, no person or scheduled process can create, process, approve, or
transfer time data for the person. Because the person is gone, this period isn't sensitive or protected from the person's
awareness.

Here's what happens after the rehire date:

• Everyone with the appropriate privileges, and scheduled processes, can create, edit, delete, and submit time

cards for the person in the new job.

• Approval, rejection, and informational notifications get sent automatically to recipients when the person's time

cards get submitted. Task configurations for the time card approval workflows identify the recipients.

• Administrators for applicable time consumers, such as payroll, transfer the approved time data. The person's

new time consumer set configuration and the time card approval workflow task configurations decide time data
approval.

Example
Here's a visual example in context of a sample time line. The employment termination dates before today and the rehire
date is after.

288

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

289

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

Time Configuration 2: When Today Is After Termination
and Before Rehire

Today is after the person left, the employment termination date, and before the rehire date. You must make adjustments
and payment before the rehire date.

Best Practice Configuration
Starting on the employment termination date, the active employee becomes an inactive employee and changes HCM
group memberships. Starting on the rehire date, the person is an active employee again and changes HCM group
memberships because of the new job. The membership changes can be manual or automatic, according to group
inclusion and exclusion conditions and whether the employee is active or inactive. The change in group membership
automatically changes the time entry and processing profiles that the active and inactive employee is associated with.

Functional Tasks Supported by This Configuration
Here's what happens before the employment termination date and after the rehire date:

• Everyone with the appropriate privileges, and scheduled processes, can create, edit, delete, and submit time

cards for the person.

• Approval, rejection, and informational notifications get sent automatically to recipients when the person's
adjusted time data gets submitted. Task configurations for the time card approval workflows identify the
recipients.

• Administrators for applicable time consumers, such as payroll, transfer the approved time data. The person's
configurations for the time consumer set and the time card approval workflows decide time data approval.

Between the employment termination and rehire dates, no person or scheduled process can create, process, approve, or
transfer time data for the person. Because the person is gone, this period isn't sensitive or protected from the person's
awareness.

Example
Here's a visual example in context of a sample time line where today is after the employment termination and rehire
dates.

290

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

291

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

Time Configuration for Time Data Cleanup

Here's a high-level best practice time entry and processing configuration for cleaning up time data according to
employment termination and rehire scenarios.

Today: Terminating Employment or Rehiring
Scenario 1: Today, you're terminating someone's employment on an earlier day. Time data for the period after the
employment termination date must get cleaned up, both for Time and Labor and Payroll.

Scenario 2: Today, you're rehiring someone on a future day. Time data for the period between the employment
termination and rehire dates must get cleaned up, both for Time and Labor and Payroll.

Best Practice Configuration for Both Scenarios
Starting on the employment termination date, the active employee becomes an inactive employee and changes HCM
group memberships. Starting on the rehire date, the person is an active employee again and changes HCM group
memberships because of the new job. The membership changes can be manual or automatic, according to group
inclusion and exclusion conditions and whether the employee is active or inactive. The change in group membership
automatically changes the time entry and processing profiles that the active and inactive employee is associated with.

Functional Tasks Supported by This Configuration
Here's what happens before the employment termination date and after the rehire date:

• Everyone with the appropriate privileges, and scheduled processes, can create, edit, delete, and submit time

cards for the person in each job.

• Approval, rejection, and informational notifications get sent automatically to recipients when the person's time

cards get submitted. Time card approval work flow task configurations identify the recipients.

• Administrators for applicable time consumers, such as payroll, transfer the approved time data. The person's
time consumer set configuration for each job and the time card approval workflow task configurations decide
time data approval.

Here's what happens between the employment termination and rehire dates:

• The person and line manager can't create, edit, delete, or submit time entries. Because the person is gone, this

period isn't sensitive or protected from the person's awareness.

• Time and labor managers with the appropriate privileges, and scheduled processes, can adjust and submit time

card data for the person.

• Approval, rejection, and informational notifications get sent automatically to recipients when the person's

adjusted time data gets submitted. Task configurations for time card approval workflows identify the recipients.

• Administrators for applicable time consumers, such as payroll, transfer the approved time data. The inactive
employee's time consumer set configuration and the time card approval workflow task configurations decide
time data approval.

292

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

Example
Here's a visual example in context of a sample time line. The employment termination date is before today and the
rehire date is after.

293

Oracle Fusion Cloud Human Resources
Implementing Time and Labor

Chapter 50
Best Practice Configurations for Time Entry and Processing

294

