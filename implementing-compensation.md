Oracle Fusion
Cloud Human
Resources

Implementing Compensation

Oracle Fusion Cloud Human Resources
Implementing Compensation

G34711-05

Copyright © 2011, 2025, Oracle and/or its affiliates.

Author: Srinivas Vellikad

Oracle Fusion Cloud Human Resources
Implementing Compensation

Contents

Get  Help  ................................................................................................................................    i

1 Overview of Compensation

1

Overview of Compensation Setup ..............................................................................................................................................   1

How Eligibility Works With Other Objects ................................................................................................................................   2

Eligibility Profiles ............................................................................................................................................................................   4

2 Setup and Maintenance Tasks

9

Base Pay Setup and Maintenance Tasks ..................................................................................................................................   9

Individual Compensation Setup and Maintenance Tasks .....................................................................................................  11

Grade Step Progression Setup and Maintenance Tasks .......................................................................................................  12

Workforce Compensation Setup and Maintenance Tasks ...................................................................................................   13

Total Compensation Statements Setup and Maintenance Tasks .......................................................................................  15

3 Profile Options for Compensation Pages, Actions, and Approval

Notifications

17

CMP_COMPENSATION_RESPONSIVE_ENABLED Profile Option ........................................................................................  17

BIP_ONLINE_NOTIFICATION_HCM_COMPENSATION Profile Option ...............................................................................   17

BIP_ONLINE_DISCLOSE_HISTORY_HCM_COMPENSATION Profile Options ...................................................................   17

BIP_ONLINE_HIDE_EDIT_HCM_COMPENSATION Profile Options .....................................................................................  18

ORA_PER_EMPL_ENABLE_WRK_ASG_REST_LOV Profile Option ......................................................................................  18

4 Profile Options for Salary Actions

21

HR_DISABLE_PENDING_APPROVALS_CHECK_IN _HCM_DATA_LOADER Profile Option .............................................   21

ORA_CMP_LGT_WHEN_MISSING_SALARY_DATASECURITY Profile Option ...................................................................   21

ORA_CMP_NO_SALARY_CHANGE_WHEN_INACTIVE_CHG_ASGN Profile Option ........................................................  22

ORA_CMP_SAL_REUSE_ASGN_ACTION_OCCURRENCE Profile Option ..........................................................................   22

ORA_CMP_SALARY_CHECKS_BEHAVIOR_IN_CHANGE_START_DATE Profile Option ..................................................  23

ORA_PER_CLE_COPY_FUT_ASG Profile Option ....................................................................................................................   23

ORA_PER_EMP_RETAIN_CHANGES Profile Option ..............................................................................................................   24

ORA_PER_EMPL_DEFAULT_EFFECTIVE_DATE Profile Option ...........................................................................................   24

Oracle Fusion Cloud Human Resources
Implementing Compensation

5 Profile Options for Individual Compensation Pages and Actions

25

CMP_DISABLE_PENDING_APPROVALS_CHECK_IN_MANAGE_CONTRIBUTION Profile Option ................................   25

CMP_IC_DATACHECK_IN_NONCMP_FLOWS Profile Option ...............................................................................................  25

Prevent Submissions Without Changes Profile Options ......................................................................................................  25

ORA_CMP_BIP_IC_SHOW_INPUT_VALUES Profile Option ..................................................................................................  26

ORA_CMP_LGT_WHEN_MISSING_IC_DATASECURITY Profile Option ..............................................................................   27

6 Responsive User Experience Setup

29

Search Logic Profile Options for Client List of Values .........................................................................................................  29

Use Transaction Design Studio to Configure Field Displays ..............................................................................................   29

Displayed and Hidden Responsive Compensation Management Fields .........................................................................   30

Displayed and Hidden Responsive Team Compensation Fields ........................................................................................  36

7 Approvals Overview

41

How Default Approval Tasks for Salary and Individual Compensation Work ..................................................................   41

How You Configure Different Approval Flows for Individual Compensation Allocations and Personal Contributions

...........................................................................................................................................................................................................     42

How You Can Validate Salary and Responsive Individual Compensation Approval Rule Changes ............................   43

8 Example Approval Configurations

45

Autoapprove a Salary Change If the Requester Is an HR Specialist .................................................................................   45

Grade Determines the Levels of Approval for a Salary Change ........................................................................................   45

Route Approval for a Salary Change According to Country and Amount .......................................................................   47

Route Approval for Recurring Individual Allocation When the Amount Changes by a Percentage ...........................   49

Autoapprove Personal Contributions .......................................................................................................................................  53

Route Approval for Individual Compensation or Personal Contribution Allocation by Action ....................................  54

9 Market Data

57

Overview of Market Data ...........................................................................................................................................................   57

How You Use Market Data Surveys to Create Composites .................................................................................................  58

Compensation Types for Market Data ....................................................................................................................................   59

Overview of Supplier Structures ...............................................................................................................................................  59

How You Match a Survey Job or Position to Your Internal Data .......................................................................................  60

Difference Between Global HR Benchmark Jobs and Survey Benchmark Jobs .............................................................   61

Import Survey for Market Data .................................................................................................................................................   61

Oracle Fusion Cloud Human Resources
Implementing Compensation

Market Segments .........................................................................................................................................................................   62

Import Composites for Market Data ........................................................................................................................................  63

Options to View Market Composites in Compensation ......................................................................................................   64

How You Configure Market Composites Display ..................................................................................................................   65

10 Payroll Elements and Compensation

67

How Compensation Uses Payroll Elements ...........................................................................................................................   67

Before You Can Use Payroll Elements in Compensation ....................................................................................................   67

Define Elements, Balances, and Formulas .............................................................................................................................  68

Create a Payroll Element to Use with Salary Bases ...............................................................................................................  71

Create a Payroll Element to Use with Individual Compensation Plans .............................................................................  73

Create a Payroll Element to Use with Workforce Compensation Plans ............................................................................  77

Conversion Rule Options for Configuring Additional Details of Payroll Elements .........................................................   81

11 Base Pay Overview

83

Overview of Base Pay Configuration .......................................................................................................................................   83

How Salary Basis Options Work with Salary Amounts and Calculations .........................................................................  84

How You Store the Salary Amount and Pass It to Payroll for Processing ........................................................................  84

How Many Salary Bases to Create ...........................................................................................................................................  86

How You Can Audit Salary Data ...............................................................................................................................................   87

Document Records for Salary ...................................................................................................................................................   87

Let Proposers Include Document Records in Salary Proposals .........................................................................................  88

12 Salary Basis Introduction

89

Salary Basis Options for Determining Salary Amount ........................................................................................................   89

Salary Amount Is Determined by User ...................................................................................................................................   89

Salary Amount Is Determined by Incremental Components .............................................................................................   89

Salary Amount Is Determined by Simple Components ......................................................................................................   90

Salary Amount Is Determined by Rates ..................................................................................................................................  92

Rounding Rules, Salary Amounts, and Decimal Places to Display ....................................................................................  94

13 Simple and Incremental Component Itemization of Salary

97

Considerations for Using Salary Bases with Incremental Components versus Simple Components .........................  97

Simple Component Types ..........................................................................................................................................................  99

Optional Simple Components in Salary Bases ....................................................................................................................   100

Example Simple Component Configurations with People Entering Values and Fixed Percentages ..........................  101

Oracle Fusion Cloud Human Resources
Implementing Compensation

Example  Simple  Component  Configurations  with  Grade  Progression  Rate,  User  Entered  Values,  and  Fixed

Percentages  ..................................................................................................................................................................................    102

How You Migrate Salary Bases with Simple Components ................................................................................................   103

How You Enable Salary Itemization Using Incremental Components ............................................................................   103

14 Examples of How Simple Components Work

105

A New Hire Action with Simple Components ......................................................................................................................   105

A Change Salary Action and Simple Components .............................................................................................................   106

The First Allocation and Next-Year Changes with Simple Components ........................................................................  108

Working Hours Change and Simple Components ...............................................................................................................  110

Salary Frequency Change and Simple Components ...........................................................................................................   112

Component Type Changes and Simple Components .........................................................................................................   114

15 Rates-Based Component Itemization of Salary

117

Comparison of Rate Component Categories for Salary Bases ..........................................................................................  117

Element Rate Components in a Salary Basis ........................................................................................................................  118

Derived Rate Components in a Salary Basis .........................................................................................................................  119

Grade Rate Rate Components in a Salary Basis ...................................................................................................................  119

Value by Criteria Rate Components in a Salary Basis .........................................................................................................  119

Database Items That Can Detect Proposed Info in Salary Value by Criteria Rate Definitions ....................................  120

Important Value by Criteria Settings for Rate Components in Salary Bases .................................................................   122

Run Salary Processes .................................................................................................................................................................   122

Considerations for Using Salary Bases with Simple Components versus Rate Components ....................................   124

16 Rate Component Attributes for Salary Bases

127

Base Rate Attribute for Salary Basis Rate Components .....................................................................................................  127

Overall Salary Attribute for Salary Basis Rate Components ..............................................................................................  127

Periodicity Attribute for Salary Basis Rate Components ....................................................................................................  127

Default Value Attribute for Salary Basis Rate Components ..............................................................................................   128

FTE Attribute for Salary Basis Rate Components ................................................................................................................  128

Factor Attribute for Salary Basis Rate Components ...........................................................................................................   128

Periodicity Conversion Formula Attribute for Salary Basis Rate Components ..............................................................  128

17 Example Rate Definition Configurations for a Salary Basis

129

Overview of Example Rate Definitions for a Salary Basis ..................................................................................................  129

Create a Base Salary Rate Definition .....................................................................................................................................   129

Oracle Fusion Cloud Human Resources
Implementing Compensation

Create an Allowance Rate Definition for a Salary Basis .....................................................................................................  130

Create a Short-Term Incentive Plan Rate Definition for a Salary Basis ...........................................................................   131

Create a Grade-Based Value by Criteria Definition for a Salary Basis Rate Definition .................................................   132

Create a Grade-Based Performance Award Rate Definition for a Salary Basis .............................................................   135

Create an Overall Salary Rate Definition for a Salary Basis ...............................................................................................  135

Create a Rates-Based Salary Basis .........................................................................................................................................   137

18 Rates-Based Salaries

139

Dos and Don’ts for Assigning and Changing Rates-Based Salary ..................................................................................   139

Considerations When Using Rates-Based Salary ................................................................................................................   139

19 Salary Basis FAQs

141

Can I change or delete a salary basis that's in use? ...........................................................................................................   141

Can I add effective-dated changes to the salary basis? .....................................................................................................  141

Where does the annualization factor for a salary basis that uses payroll period frequency come from? ................   141

Can I use the same payroll element for multiple salary bases? ........................................................................................  141

Can I update an element mapped to a salary basis that's in use? ...................................................................................  141

Can managers change the salary basis of a salary record? ..............................................................................................  142

20 Salary Ranges and Metrics

143

How You Validate Salary Changes with the Grade Range .................................................................................................  143

Salary Range Violation Behavior for Proposed Salaries ....................................................................................................   143

How Salary Metrics Are Calculated ........................................................................................................................................   144

21 Salary Range Differentials

145

Overview of Salary Range Differentials .................................................................................................................................  145

Configure Salary Range Differentials .....................................................................................................................................  146

Basic Process to Configure and Apply Zone-Based Salary Range Differentials ...........................................................   147

Zone-Based Salary Range Differential Processing .............................................................................................................   148

Factor Type Salary Range Differentials That Include Lower Limits ..................................................................................  151

Configure Compensation Zone Types and Zones ...............................................................................................................   151

Compensation Zone-Based Differential: Options for When Work from Home Is Yes, But Evaluation Should Use Work

Locations  .......................................................................................................................................................................................    153

Generate Compensation Zone and Address Mapping .......................................................................................................  154

Enable Geography Validation for Compensation Zones ....................................................................................................  156

Load Compensation Zone Geographies Using CSV File Export and Import .................................................................  156

Oracle Fusion Cloud Human Resources
Implementing Compensation

22 Base Pay Lookups and Troubleshooting

159

Incremental Salary Component Lookups ..............................................................................................................................  159

Simple Salary Component Lookups .......................................................................................................................................   159

Troubleshoot Salary-Related Issues .......................................................................................................................................   160

23 Default Salary from Grade Ladder Rates

163

Basic Process to Default Salary Amounts from Grade Ladder Rates ..............................................................................   163

24 Grade Step Progression Configuration

165

Manage Grade Step Progression ............................................................................................................................................   165

Examples of Adding Progression Rules ................................................................................................................................   165

25 Transaction Dates and On Eligibility in Grade Step Progression

Processing

167

Date Codes and Eligibility Options for Grade Step Progression ......................................................................................   167

26 Global Settings for Grade Step Progression Processing

169

Batch Settings for Grade Step Progression Processing .....................................................................................................   169

27 Grade Step Progression Processing

171

Overview of Grade Step Progression Processing .................................................................................................................   171

28 Examples of Grade Step Progression Processing

173

Examples of Grade Step Progression Processing ................................................................................................................  173

29 Proposed Grade Step Progression and Salary Updates

175

Overview of Proposed Progression and Salary Updates ...................................................................................................   175

30 Adjustments to Salary Amounts in Proposed Progression and Salary

Updates

177

Overview of Parameters That Affect Salary Amounts for Proposed Progression and Salary Updates ....................   177

31 Individual Compensation Plans Overview

179

Overview of Individual Compensation ...................................................................................................................................  179

Oracle Fusion Cloud Human Resources
Implementing Compensation

Options in an Individual Compensation Plan Configuration ............................................................................................   179

Document Type Settings for Individual Compensation .....................................................................................................  180

Payment Dates in an Individual Compensation Plan Configuration ...............................................................................  180

How Changing the Hire Date Affects Individual Compensation Allocations .................................................................   181

Eligibility in an Individual Compensation Plan Configuration ...........................................................................................  181

How Individual Compensation Plan Eligibility Works with Assignment Creation Flows .............................................   182

How Individual Compensation Plan Eligibility Works with Assignment Correction and Update Flows ....................  182

Plan Access Restrictions in an Individual Compensation Plan Configuration ...............................................................  182

Plan Info in an Individual Compensation Plan Configuration ..........................................................................................   182

Validate Individual Compensation Plans ...............................................................................................................................   183

Journey Checklist Tasks and Individual Compensation Plan Allocations ......................................................................   183

How You Let People Submit Personal Contributions When Earlier Contributions Are Pending Approval ..............   184

32 Payment Dates in Individual Compensation Plans

187

Sync Individual Compensation Plan Dates with the Projected Hire Date in an Offer ..................................................   187

Examples of How Payment Start Dates in an Offer Sync with the Projected Hire Date ..............................................   187

Sync Individual Compensation Plan Dates with the Start Date in a Pending Worker Action .....................................   188

Examples of How Payment Start Dates in a Pending Worker Action Sync with the Start Date .................................  189

Payment End Date Considerations for Individual Compensation Plans ........................................................................   190

How the Projected Hire, Start, or Submission Date Works in HR Actions .....................................................................   190

33 Access and Action Options, and Option Visibility in Individual

Compensation Plans

191

Plan Access Restrictions ............................................................................................................................................................  191

The Difference Between Plan Access Restriction and Access Security ..........................................................................   192

Copy Individual Compensation Allocations During Local and Global Transfer .............................................................  192

Individual Compensation Plan and Option Visibility ..........................................................................................................   193

34 Example Individual Compensation Plan Configurations

195

Spot Bonus and Stock Grant Plan Configuration ................................................................................................................   195

Car Allowance Plan Configuration ..........................................................................................................................................  195

Charity or Savings Contribution Plan Configuration ..........................................................................................................  196

35 Compensation History

197

Compensation History Categories ..........................................................................................................................................  197

How You Set Up the Other Compensation and Recurring Payments Summary Data for Compensation History ...   198

Oracle Fusion Cloud Human Resources
Implementing Compensation

36 Stock Grants

199

Manage Stock Grants in the Integrated Workbook ............................................................................................................   199

FAQ  ...............................................................................................................................................................................................     200

37 External Data

201

External Compensation Data ...................................................................................................................................................  201

Record Type Lookups for External Compensation Data ...................................................................................................   202

Import External Compensation Data in the Integrated Workbook .................................................................................   202

How can I add external compensation data for multiple assignments? ........................................................................  203

Delete External Data in Compensation .................................................................................................................................  203

38 Workforce Compensation Overview, Lookups, and Security

205

Overview of Workforce Compensation .................................................................................................................................   205

Deep Links in Workforce Compensation ..............................................................................................................................  205

Reason Lookups .........................................................................................................................................................................  205

Nonmonetary Unit of Measure Lookups .............................................................................................................................   206

User-Defined Column Lookups ..............................................................................................................................................  206

Workforce Compensation Security ........................................................................................................................................   207

Considerations for Securing Access to Workforce Compensation Plans and Task Worksheets ...............................   208

39 Workforce Compensation Plans Overview

209

Overview of Workforce Compensation Plan Configuration .............................................................................................   209

Performance Considerations for Workforce Compensation Plans .................................................................................   209

40 Foundation: Plan Details in Workforce Compensation

211

Employment Records to Use in the Compensation Cycle ..................................................................................................  211

Active and Inactive Workforce Compensation Plans ..........................................................................................................   212

Actions and Reasons in Workforce Compensation .............................................................................................................   212

41 Foundation: Plan Eligibility and Cycles in Workforce Compensation

215

Workforce Compensation Plan Eligibility ..............................................................................................................................   215

How Required and Optional Profiles Determine Compensation Eligibility ....................................................................   215

Option to Track People Ineligible for a Workforce Compensation Plan ..........................................................................  216

How the Options to Track and Hide Ineligible People Affect Plan Worksheets ............................................................   216

Eligibility Profile Testing for a Workforce Compensation Plan .........................................................................................   217

Oracle Fusion Cloud Human Resources
Implementing Compensation

Workforce Compensation Plan Cycle Dates ..........................................................................................................................  217

42 Foundation: Hierarchies in Workforce Compensation Plans

219

Workforce Compensation Plan Hierarchies ..........................................................................................................................   219

Options to Configure Workforce Compensation Plan Hierarchies ..................................................................................  220

Formula Type Is Compensation Hierarchy Determination .................................................................................................  221

Formula Type Is Compensation Default Access Level .......................................................................................................   223

43 Foundation: Plan Currency, Access, Feedback Survey, and Info in

Workforce Compensation

227

Workforce Compensation Plan Currency ..............................................................................................................................  227

Workforce Compensation Plan Access ..................................................................................................................................  227

Delivered User Roles and Duty Roles ....................................................................................................................................   228

How Plan Access, Eligibility, and Default Access Level for Plan Hierarchies Work Together .....................................   229

Workforce Compensation Plan Feedback Survey ...............................................................................................................  229

Workforce Compensation Plan Information ........................................................................................................................   230

44 Budgets: Budget Display in Workforce Compensation Plans

231

Overview of Budget Display in Workforce Compensation Plans ......................................................................................  231

Overview Configuration in Budget Display ...........................................................................................................................   231

Summary Configuration in Budget Display ..........................................................................................................................   231

Detail Table Configuration in Budget Display ......................................................................................................................   232

Worker List Configuration in Budget Display .......................................................................................................................  233

Actions Configuration in Budget Display .............................................................................................................................   234

Information Configuration in Budget Display ......................................................................................................................  235

45 Budgets Budget Pools in Workforce Compensation Plans

237

Overview of Budget Pools in Workforce Compensation Plans ........................................................................................   237

Budgeting Methods in Workforce Compensation Plan Budget Pools ............................................................................   237

Budget Storage Methods in Workforce Compensation Plan Budget Pools ..................................................................   238

Automatically Publish Budgets in a Workforce Compensation Plan ..............................................................................   239

Budget Is in Nonmonetary Units for a Workforce Compensation Plan .........................................................................  240

Reset Amounts When Budgets Are Unpublished in a Workforce Compensation Plan ...............................................   241

Budget Enforcement Options for Workforce Compensation Plan Budget Pools .........................................................   242

Prevent Allocations When Budgets Are Null .......................................................................................................................   243

Budget Group Options for Workforce Compensation Plan Budget Pools .....................................................................  244

Oracle Fusion Cloud Human Resources
Implementing Compensation

46 Worksheets: Overview and Basic Configuration Processes for Key

Columns and Actions

245

Overview of Task Worksheets in Workforce Compensation Plans ..................................................................................  245

Include Alerts in Task Worksheets .........................................................................................................................................  246

Include a Budget Group in a Compensation Task Worksheet Summary .......................................................................  247

Include Compensation Change Statements in Task Worksheets ....................................................................................  248

Include Compensation Component Columns in Task Worksheets .................................................................................  248

Include Filters in Task Worksheets and Plan Reports ........................................................................................................  249

Include Models in Task Worksheets ......................................................................................................................................   249

Include Performance Rating Columns in Task Worksheets ..............................................................................................  250

Notify People of Eligibility Changes, Reassignments, and Delegation Changes in a Workforce Compensation Plan

.........................................................................................................................................................................................................     250

47 Worksheets: Compensation Component

253

Compensation Components in Workforce Compensation Plan Worksheets ................................................................  253

Compensation Component Number and Name, and Detail Table of Worksheet Display ..........................................   253

How the Compensation Component Display Order Affects Task Worksheets and Administrator Reports ............   255

Local Currency Determination for Compensation Components .....................................................................................   257

Nonmonetary Units for Compensation Components ........................................................................................................  258

Budget Pools and Compensation Components ..................................................................................................................  258

How You Let Managers Track Off-Cycle and On-Cycle Compensation Against a Budget .........................................  259

Configure Assignment Segments Options of a Compensation Component ................................................................   259

Eligibility Profiles of Compensation Components .............................................................................................................   260

Eligibility Profile Testing for a Compensation Component ..............................................................................................   260

Formula Type Is Compensation Currency Selection ...........................................................................................................  261

48 Worksheets: Performance Ratings

263

Overview of Performance Ratings in Workforce Compensation Plan Worksheets ......................................................  263

Performance Management Ratings in Workforce Compensation Plan Worksheets ...................................................   263

Reasons to Set Performance Document Properties ..........................................................................................................   264

How the Performance Template Selection Affects Other Document Properties .........................................................   264

Compensation Performance Ratings in Workforce Compensation Plan Worksheets .................................................  265

Calibrated Performance Ratings in a Workforce Compensation Plan ............................................................................  266

49 Worksheets: Approvals and Notifications

267

Configure Approvals for Workforce Compensation Plan Worksheets ............................................................................  267

Oracle Fusion Cloud Human Resources
Implementing Compensation

Approval Modes in Worksheet Approvals Configuration ..................................................................................................  267

Submit Modes in Worksheet Approval Configuration .......................................................................................................  268

Withdraw Modes in Worksheet Approvals Configuration .................................................................................................  268

Alternate Approver Table in Worksheet Approval Configuration ....................................................................................   269

Configure Notifications for Workforce Compensation Plan Worksheets .......................................................................  269

Can I configure workflow in workforce compensation to route plan changes for approval? ....................................   270

50 Worksheets: Examples of Alternate Approver Configurations

271

Alternate Approver for Workforce Compensation Plan Changes Is the Final Approver ..............................................   271

Alternate Approver for Workforce Compensation Plan Changes Precedes the Final Approver ................................   272

Alternate Approver for Workforce Compensation Plan Changes Is in the Middle of the Primary Plan Hierarchy ...   274

51 Worksheets: Compensation Change Statements

277

Overview of Compensation Change Statements in Workforce Compensation Plan Worksheets .............................  277

Statement Groups, Templates, and Worker Statement Action for Compensation Change Statements ..................   277

How You Create a Change Statement Template .................................................................................................................  278

Download Attribute List to Add to Template .......................................................................................................................  279

How You Can Display Different Currencies In Your Statement Template ......................................................................   279

Ways to Configure Statement Text ........................................................................................................................................   279

Statement Generation Timing and Output Format for Compensation Change Statements ......................................  281

How You Generate Statements for Multiple Workers .........................................................................................................   281

Delivery Options for Compensation Change Statements ..................................................................................................  281

How Managers Can Print and Deliver Compensation Change Statements ...................................................................  281

How Managers Can Centrally Manage and Store Compensation Change Statements ..............................................   282

How You Format a Date Variable to Display Dates in a Specific Format .......................................................................   283

How You Format Numeric Separators and Decimal Precision for Numeric Data .........................................................  283

How You Find Errors in Statement Template ......................................................................................................................   283

How You Format the Same Data Differently Based on a Worker’s Location .................................................................  283

What's the difference between workforce compensation change statements and total compensation statements?

.........................................................................................................................................................................................................    284

52 Worksheets: Worksheet Display Configurations

285

Overview of Worksheet Display in Workforce Compensation Plans ...............................................................................  285

Configure the Summary Display for Compensation Task Worksheets ..........................................................................   286

Configure the Summary Displays for Communication, Performance, and Promotion Task Worksheets ................  287

Detail Table Configuration for Compensation, Detail Table Only, Performance, and Promotion Worksheets ......   289

Oracle Fusion Cloud Human Resources
Implementing Compensation

Approval Subtabs, Columns, and Worker Details Columns Configuration for Approvals Task Worksheets ...........   290

Actions  Configuration  for  Communication,  Compensation,  Detail  Table  Only,  Performance,  and  Promotion

Worksheets  ..................................................................................................................................................................................     292

Information Configuration in All Task Worksheet Displays ..............................................................................................   293

53 Worksheets: Column Properties

295

General Properties of Worksheet Columns ..........................................................................................................................  295

Visibility and Access Properties of Worksheet Columns ..................................................................................................   296

Default Value Properties of Worksheet Columns ...............................................................................................................   297

Cross-Reference Column Properties .....................................................................................................................................   298

Formula Type Is Compensation Default and Override ......................................................................................................  300

Sample Compensation Default and Override Formulas ...................................................................................................   302

Salary and Element Mapping Properties of Compensation Amount Columns ............................................................  303

Post Incremental Itemized Salary Adjustments in a Workforce Compensation Plan to HR .......................................  303

Post Salary Compensation Amounts to Simple Components in a Workforce Compensation Plan to HR ..............   304

Rate Application Result Options for Salary Adjustments to Simple Components .......................................................  305

Considerations for Posting Salary Adjustments to Simple Components ......................................................................   305

How to Post Back Salary Changes for People Whose FTE is Less Than 1 ....................................................................   306

Rounding Rule Behavior When You Post Back Salary Changes for People Whose FTE is Less Than 1 ...................   306

Rounding Rule Behavior for Base Salary – Current Column ............................................................................................   307

54 Worksheets: Dynamic Columns in Worksheet Display Configurations

309

Overview of Dynamic Columns in Workforce Compensation Plan Worksheets ..........................................................   309

Evaluation Order, Sequence, and the Default Condition of Dynamic Worksheet Columns .......................................  309

Triggering Events for Conditions of Dynamic Columns and Alerts ................................................................................   310

Descriptions for Dynamic Worksheet Column Conditions .................................................................................................   311

Basic and Advanced Tabs When Building a Condition for a Dynamic Column or an Alert .........................................   311

Configure the Compensation Amount Dynamic Column of the Bonus Component to Reward High Performers ...   312

When to Use a Fast Formula or Dynamic Column to Display Information in a Worksheet Column .........................   314

Copy Dynamic Column Configurations .................................................................................................................................   315

55 Worksheets: Configuration Guidance for Salary and Budget Component

Columns, and Promotion Effective Date

317

Guidelines to Configure the Eligible Salary Component Columns ...................................................................................  317

Guidelines to Configure the Budget Amount - Worker Component Columns ..............................................................   317

Guidelines to Allocate Compensation as Percentage of Budget ......................................................................................  318

Oracle Fusion Cloud Human Resources
Implementing Compensation

Guidelines to Configure Default Values for the Promotion Effective Date Column .....................................................   319

Update Grade Step as Part of a Workforce Compensation Cycle ....................................................................................   319

Proposed Grade Column When You Update the Grade Step ...........................................................................................  320

Worksheet Effects When You Update the Grade Step .......................................................................................................  320

Base Salary - New Column When You Update the Grade Step ........................................................................................   321

Downloaded Workbook When You Update the Grade Step ..............................................................................................   321

56 Worksheets: Miscellaneous Rate Component Columns, User-Defined

Columns, and External Data in Task Worksheets

323

Miscellaneous Rate Component Columns and User-Defined Columns .........................................................................  323

Configure User-Defined Columns of a Workforce Compensation Plan Worksheet to Show External Data ............   323

57 Worksheets: Default Worksheet Display and Individual Worker Display

325

Default Display Settings for Workforce Compensation Plan Worksheets ......................................................................  325

Overview of Individual Worker Display in Workforce Compensation Plan Worksheets ..............................................   325

Individual Worker Page Content in Workforce Compensation Plan Worksheets .........................................................   326

58 Worksheets: Alerts

329

Overview of Alerts in Workforce Compensation Plan Worksheets .................................................................................   329

Predefined Alerts for Workforce Compensation Plan Worksheets .................................................................................   329

Alert Types for Workforce Compensation ............................................................................................................................   330

Example Alert to Warn Managers That Their Allocated Compensation Amounts Changed .....................................  330

Example Alert to Prevent Managers from Allocating More Than the Targeted Compensation ................................  330

Example Alert to Notify Managers When the New Base Salary Is Greater Than the Range Maximum ....................  331

59 Worksheets: Assignment Segments

333

Overview of Assignment Segments in Workforce Compensation Plan Worksheets ...................................................   333

Basic Process to Configure Worksheet Assignment Segments .......................................................................................   333

Data for Worksheet Assignment Segments .........................................................................................................................   335

Visibility, Ability to Update, and Restrictions for Worksheet Assignment Segments ..................................................   336

Eligibility of Worksheet Assignment Segments ..................................................................................................................   336

The Start Workforce Compensation Cycle Process and Assignment Segments ..........................................................   337

The Refresh Workforce Compensation Data Process and Assignment Segments ......................................................  338

60 Modeling, Reports, Filters, and Plan Analytics

339

Overview of Modeling in Workforce Compensation Plan Worksheets ...........................................................................  339

Oracle Fusion Cloud Human Resources
Implementing Compensation

Overview of Reports in Workforce Compensation Plans ..................................................................................................   339

Administrator and Line Manager Access to OTBI and OBIEE Reports Used in Workforce Compensation Plans ...   340

How You Add Dashboard OTBI Reports to the Workforce Compensation Landing Page ..........................................  340

Dimensions and Range Increments in Worksheet Models and Plan Reports ...............................................................   341

Overview of Filters in Workforce Compensation Plan Worksheets and Reports ..........................................................  342

Overview of Landing Page Analytics in Workforce Compensation Plans ......................................................................  342

61 Validation and Processing

345

Overview of Plan Validation and Starting the Workforce Compensation Cycle ...........................................................   345

62 Global Compensation Settings

347

General and Watchlist Global Settings for Workforce Compensation Plans .................................................................   347

Global Setting Options for Workforce Compensation Plan Notifications ......................................................................   347

How Workforce Compensation Plan Notifications Work ..................................................................................................   348

Header and Message Text for All Workforce Compensation Plan Notifications ..........................................................  350

How can I configure the content that appears in the workforce compensation submit for approval notification? ..   351

63 Workforce Compensation Administration Overview

353

Prepare to Start a Workforce Compensation Cycle ............................................................................................................   353

Administer Individuals and Plans During a Workforce Compensation Cycle ...............................................................   354

Close a Workforce Compensation Cycle ...............................................................................................................................   356

64 Workforce Compensation Batch Processes to Start a Compensation Cycle

and Refresh Data

357

Start Workforce Compensation Cycle and Synchronize Hierarchy Processes ..............................................................   357

Plan Not in the Choice List of the Start Workforce Compensation Cycle Process .......................................................  358

Refresh Workforce Compensation Data Process ................................................................................................................   358

Refresh Options for the Refresh Workforce Compensation Data Process ....................................................................   359

Formula Type Is Compensation Person Selection ...............................................................................................................  361

65 Workforce Compensation Batch Process to Transfer Workforce

Compensation Data

365

Transfer Workforce Compensation Data to HR Process ....................................................................................................  365

Element and Salary Details of Transfer Workforce Compensation Data to HR Process .............................................   366

Stock Details of Transfer Workforce Compensation Data to HR Process ......................................................................   366

Promotion Details of Transfer Workforce Compensation Data to HR Process .............................................................   367

Oracle Fusion Cloud Human Resources
Implementing Compensation

Other Details of Transfer Workforce Compensation Data to HR Process ......................................................................  367

66 Workforce Compensation Batch Processes to Back Out and Purge Data,

Notify Managers, and Process Change Statement

369

Back Out and Purge Workforce Compensation Data Processes .....................................................................................   369

Notify Managers About Workforce Compensation Plan Due Dates and Cycle Status Change Processes ..............   369

Process Workforce Compensation Change Statements Process ....................................................................................   370

People Can't See Their Workforce Compensation Change Statements ........................................................................   370

67 View Compensation Administration Reports

371

Compensation and Budget Analysis Reports for Workforce Compensation .................................................................   371

Promotions and Performance Reports for Workforce Compensation ............................................................................   371

Status and Monitoring Reports for Workforce Compensation .........................................................................................  372

Data Processed Reports for Workforce Compensation .....................................................................................................   373

Consolidated Posting Summary Report Data ......................................................................................................................   373

Exports for Workforce Compensation ...................................................................................................................................  374

Batch Process Monitoring for Workforce Compensation ..................................................................................................  374

Discrimination Detection Report ............................................................................................................................................   375

68 Active Workforce Compensation Plans and Manual Currency Conversion

Rates

377

Active Workforce Compensation Plans .................................................................................................................................   377

Add and Change Currency Conversion Rates for a Workforce Compensation Plan Cycle .........................................   377

69 Administer Workforce Compensation for Workers

379

Administer Individuals During Workforce Compensation Cycles ....................................................................................  379

Reprocess an Individual or Add Them to a Workforce Compensation Plan and Cycle ...............................................  379

Administer an Individual's Hierarchies and Access for a Workforce Compensation Plan Cycle ...............................   380

Administer  an  Individual's  Manager  and  Processing  Statuses,  and  Due  Date  for  a  Workforce  Compensation  Plan

Cycle  ...............................................................................................................................................................................................    381

Administer an Individual's Eligibility for a Specific Workforce Compensation Plan Cycle ..........................................   381

Adjust Manager-Level Budgets Stored as Percentages ....................................................................................................   382

70 Examples of When to Reprocess an Individual after Starting a Workforce

Compensation Plan Cycle

383

Someone Transfers into an Organization After the Workforce Compensation Cycle Starts ......................................  383

Oracle Fusion Cloud Human Resources
Implementing Compensation

Someone's Data Is Corrected in HR After the Workforce Compensation Cycle Starts ...............................................   383

Someone Leaves an Organization After the Workforce Compensation Cycle Starts ..................................................  383

A Contingent Worker Becomes a Regular Worker After the Workforce Compensation Cycle Starts .......................   384

71 Total Compensation Statement Overview

385

Guidelines to Create Total Compensation Statement Definitions ...................................................................................  385

Overview of Creating a Total Compensation Statement ..................................................................................................   386

Display Options in Statements ...............................................................................................................................................   388

72 Total Compensation Statement Components

393

Compensation Items and Sources .........................................................................................................................................   393

Formula Type for Total Compensation Item ........................................................................................................................  395

Compensation Category Types ..............................................................................................................................................   399

Compensation Categories and Subcategories ...................................................................................................................   400

Options to Display Category Details in a Compensation Statement ..............................................................................   401

Best Practices for Planning Statement Definitions ............................................................................................................  402

Total Compensation Statement Options ..............................................................................................................................  403

Options to Include Descriptive Text in Compensation Statements ...............................................................................   404

Options to Configure Statement Periods, Welcome Message, and Feedback .............................................................   405

Options to Configure Statement Eligibility and Summary Page ....................................................................................   406

Printable Statement Templates ..............................................................................................................................................   407

FAQs  .............................................................................................................................................................................................     408

73 Total Compensation Examples

411

Create a Bonus Category ..........................................................................................................................................................   411

Create a Salary Category ..........................................................................................................................................................   413

Create a Benefits Category ......................................................................................................................................................   415

Create a User-Defined Category for Commissions .............................................................................................................  419

Create a Stock History Category .............................................................................................................................................   421

Create a Total Compensation Statement ..............................................................................................................................  423

Oracle Fusion Cloud Human Resources
Implementing Compensation

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
Implementing Compensation

Get Help

ii

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 1
Overview of Compensation

1  Overview of Compensation

Overview of Compensation Setup

You can plan and allocate salary and compensation for individuals and your workforce. You can also communicate
compensation information to individuals.

To get started implementing compensation, you need to have the Application Implementation Consultant role. With
that role, you can opt into the Compensation Management offering in the Setup and Maintenance work area. You can
also enable the relevant functional areas for your business.

Functional Area

Description

Base Pay

Grade Step Progression

Individual Compensation

Collect and store salary information and pass it to payroll for processing. Also set up salary ranges
and metrics to help managers and HR specialists follow organizational policies when proposing and
approving salary changes. For example, a manager reviewing salary information for a promotion sees
that the salary is just below the midpoint of the person's grade rate. The person is a high performer, so
the manager decides to increase the salary change to be above the midpoint.

Automate people's progression through grade ladders according to eligibility criteria and rules that
reflect your progression policies. Also propose a new salary amount for the progression, or even
automatically update the salary amount. For example, automatically promote someone to the next
step of a progression grade ladder after 1 year when their performance rates 4 or higher.

Design compensation plans that let managers and HR specialists allocate off-cycle compensation
to individuals, such as bonuses, tuition reimbursement, or allowances. Also design plans that let
individuals contribute to charities or savings plans. And, identify the compensation awards that
individuals can see in their compensation history.

Workforce Compensation

Create compensation plans and cycles used for compensating a group of workers. Configure the type
of compensation allocated, the information displayed to managers, and whether to use budgeting.
Also configure eligibility criteria for the plan or component, and the approval hierarchy.

1

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 1
Overview of Compensation

Functional Area

Description

Total Compensation Statements

Design and deliver statements for individuals that can include traditional forms of pay, such as salary
and individual compensation awards. You can also include nontraditional forms of pay, such as fringe
benefits, cost of benefits, and paid time off.

Market Data

Analyze compensation survey data, survey jobs, survey job structures, and other survey attributes.
Survey data can include key metrics, such as percentiles and deciles.

Related Topics

• Plan Your Implementation

How Eligibility Works With Other Objects

You add eligibility criteria to an eligibility profile, and then associate the profile with an object that restricts eligibility.

The following figure shows the relationships between eligibility components.

Eligibility Criteria
You can add different types of eligibility criteria to an eligibility profile. For many common criteria, such as gender or
employment status, you can select from a list of predefined criteria values. However, you must create user-defined
criteria and derived factors before you can add them to an eligibility profile.

2

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 1
Overview of Compensation

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

No

Yes

Yes

Yes

Yes

Yes

Yes

Related Topics

• Eligibility Profiles

• User-Defined Criteria

• Derived Factors

3

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 1
Overview of Compensation

Eligibility Profiles

Create eligibility profiles to define criteria that determine whether a person qualifies for objects that you associate the
profile with. You can associate eligibility profiles with objects in various business processes.

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

Setting

Profile Type

Description

Use only dependent profiles for Benefits plans or plan types when determining eligibility of
participants' spouses, family members, or other individuals who qualify as dependents.

All other profiles are participant profiles.

4

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 1
Overview of Compensation

Setting

Usage

Description

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

Employment

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

• Assignment Status

• Hourly or Salaried

• Assignment Category

5

Oracle Fusion Cloud Human Resources
Implementing Compensation

Category

Description

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

• Covered by Another Plan in Program

• Covered by Another Plan Type in Program

• Covered by Another Program

Chapter 1
Overview of Compensation

6

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 1
Overview of Compensation

Category

Description

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

Viewing the Criteria Hierarchy
Select the View Hierarchy tab to see a list of all criteria that you've saved for this profile. The list is arranged by criteria
type.

7

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 1
Overview of Compensation

Related Topics

• Create a Participant Eligibility Profile

• Examples of Eligibility Profiles

• Derived Factors

• User-Defined Criteria

• Single or Multiple Eligibility Profiles

8

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 2
Setup and Maintenance Tasks

2  Setup and Maintenance Tasks

Base Pay Setup and Maintenance Tasks

You can calculate, adjust, and maintain salary and hourly earnings for your people by completing these setup tasks in
the sequence listed.

Task Name

Elements

Grades

Grade Rates

Progression Grade Ladder

Compensation Zones

Salary Range Differentials

Description

Recommended Help

Create legislative data group (LDG) payroll
elements to use when you configure salary
bases. For example, create recurring standard
earnings to handle annual salaries and hourly
earnings.

Create grades that record people's level of
compensation. And define one or more grades
that apply for jobs and positions. You use
the grade rates for grades to validate salary
proposals.

Create grade rates to hold the pay values
related to each grade. Grade rates linked to
salary bases typically serve as guidelines to
validate that proposed salary is appropriate for
that grade.

• Create a Payroll Element to Use with

Salary Bases

• Troubleshoot Salary-Related Issues

• Grades

• How Grades, Grade Rates, and Sets Work

with Legislative Data Groups

• Grade Rates

• How Grades, Grade Rates, and Sets Work

with Legislative Data Groups

Optionally create progression grade ladders
to automatically move people from one grade,
 or grade and step, to the next level in a grade
ladder. For example, you want to automatically
move new hires to the next step after their first
6 months on the job.

• Grade Step Progression Setup and

Maintenance Tasks

• How You Validate Salary Changes with the

Grade Range

• Troubleshoot Salary-Related Issues

Optionally create compensation zone and
zone types to use in salary range differentials
that adjust base ranges by compensation or
wage regions. For example, you want to pay
everyone working on the East Coast of the US
at 1.1 times the standard grade rate. You want
to pay everyone working on the West Coast at
1.2 times. You pay Central people the standard
grade rate and everyone in the South at 0.8
times.

Optionally create salary range differentials to
adjust base salary ranges from the grade rate
associated with the salary basis. Differentials
vary, for example, to reflect the cost of living in
different locations or the relative ease of hiring.
You use these differentials when configuring
salary bases.

• Overview of Salary Range Differentials

• Configure Compensation Zone Types and

Zones

• Overview of Salary Range Differentials

• Configure Salary Range Differentials

• How You Validate Salary Changes with the

Grade Range

Configure Actions

Optionally add actions to identify the cause
when creating or changing salary. For example,

Action Framework

9

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 2
Setup and Maintenance Tasks

Task Name

Description

Recommended Help

Action Reasons

Manage Common Lookups

Salary Basis

Manage Task Configurations for Human Capital
Management

Manage Profile Options

Sandboxes

 track that salary changed as part of a
promotion or transfer.

Optionally add reasons to associate with
actions, mostly for reporting and analysis. For
example, when a manager changes someone's
salary as part of a transfer, have them indicate
whether it's because of cost of living.

Optionally change or add components to the
CMP_SALARY_COMPONENTS and ORA_
CMP_SIMPLE_SALARY_COMPS lookup types
to better support your reporting policies for
salary allocations. You use the incremental or
simple salary components when configuring
salary bases that let HR specialists and
managers itemize new or adjusted salary. The
itemizations reflect the different reasons for
their allocations.

Create salary bases that get used when creating
salary and help with processing. For example,
 salary basis settings get used to decide salary
amounts, currency, frequency, and metrics. And
the payroll element linked to the salary basis
holds the salary amount, which gets passed to
payroll for processing.

Optionally change default approval workflows
to support your salary change policies. For
example, automatically approve salary changes
proposed by HR specialists. Route approvals
based on country and amount. And specify the
levels of approval using grades.

Enable the applicable salary actions controlled
by profile options. For example, let people use
HCM Data Loader to load salary changes when
related salary is pending approval. Prevent
people who don't have access to the source
assignment salary from proposing salary
during global transfers. And copy future salary
changes during local and global transfers.
Also, if you're going to use autocomplete rules
with salary objects, you need to expose the
Autocomplete Rules feature.

Enable a sandbox to access the HCM
Experience Design Studio and Autocomplete
Rules for the Salary object. You can either
manually create and enable a sandbox or
automatically create it.

Action Framework

•

Incremental Salary Component Lookups

• Simple Salary Component Lookups

• Overview of Base Pay Configuration

• How Many Salary Bases to Create

• Salary Basis Options for Determining

Salary Amount

• Considerations for Using Salary Bases with
Incremental Components versus Simple
Components

• How Default Approval Tasks for Salary and

Individual Compensation Work

• Troubleshoot Salary-Related Issues

• CMP_COMPENSATION_RESPONSIVE_ENABLED

Profile Option

• ORA_CMP_LGT_WHEN_MISSING_SALARY_DATASECURITY

Profile Option

• BIP_ONLINE_NOTIFICATION_HCM_COMPENSATION

Profile Option

• Get Started with Autocomplete Rules

• Overview of Profile Options

• Create and Edit Profile Options

• How You Enable Access to Autocomplete

Rules

• Overview of Salary

• Delivered Rules for Salary

• General Considerations for Salary

• Prepare to Move Salary Rules to

Production Environments

10

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 2
Setup and Maintenance Tasks

Security Reference
The tasks that people can do and the data that they can see depend on their roles, duties, and privileges. For
information about these factors, see these two guides:

• Securing HCM

• Security Reference for HCM

Individual Compensation Setup and Maintenance Tasks

You can let people award compensation outside of the regular compensation cycle and manage personal contributions.
To do this, complete these setup tasks in the sequence listed.

Task Name

Elements

Configure Actions

Eligibility Profiles

Document Types

Individual Compensation Plans

Description

Recommended Help

• Create a Payroll Element to Use with

Individual Compensation Plans

Create legislative data group (LDG) payroll
elements to use when you configure individual
compensation plans. For example, create
recurring standard earnings to handle vehicle
or gym allowances. Create information
elements to handle stock grants and to store
nonmonetary information, such as durations or
points. Create recurring voluntary deductions
to handle savings plans and charitable
contributions. And create nonrecurring
voluntary deductions to handle onetime
charitable contributions.

Optionally add HR actions that specify access
to individual compensation plans. For example,
 you can add the Transfer action to a moving
allowance plan to make the plan available when
people transfer someone using that action.

• Action Framework

• Plan Access Restrictions in an Individual

Compensation Plan Configuration

• Plan Access Restrictions

Optionally create eligibility profiles to define
criteria that decide whether a person qualifies
for the linked individual compensation plan
option. For example, identify appropriate
vehicle allowance options based on people's job
title and proximity to a specific office.

Optionally create document types to link
with options for individual compensation
plans. You can then request or require people
proposing allocations for the options attach
supporting documents. Approvers can use the
documents when deciding to approve or reject
the proposals. For example, set up a vehicle
allowance option to require a vehicle details
document.

Create the individual compensation plans
that let managers and HR specialists award
compensation outside of the regular
compensation cycle. For example, let managers
give spot bonuses or grant stock shares.

• How Eligibility Works With Other Objects

• Eligibility Profiles

• Document Type Settings for Individual

Compensation

• Options in an Individual Compensation

Plan Configuration

• Overview of Individual Compensation

• Plan Access Restrictions

11

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 2
Setup and Maintenance Tasks

Task Name

Description

Recommended Help

• Spot Bonus and Stock Grant Plan

Configuration

• Car Allowance Plan Configuration

• Charity or Savings Contribution Plan

Configuration

Manage Task Configurations for Human Capital
Management

Optionally change default approval workflows
to support your individual compensation
allocation policies. For example, automatically
approve personal contributions. And route
individual compensation and administer
compensation allocations for approval.

• How Default Approval Tasks for Salary and

Individual Compensation Work

• How You Configure Different Approval
Flows for Individual Compensation
Allocations and Personal Contributions

Manage Profile Options

Enable the applicable individual compensation
actions controlled by profile options. For
example, allow people to submit more personal
contributions while other contributions are
still pending approval. Enable only people
with relevant security privileges maintain
individual compensation in HR actions that
have the section. And prevent people from
submitting a Personal Contribution, an
Individual Compensation, or an Administer
Compensation action without making changes.

• BIP_ONLINE_NOTIFICATION_HCM_COMPENSATION

Profile Option

• CMP_DISABLE_PENDING_APPROVALS_CHECK_IN_MANAGE_CONTRIBUTION

Profile Option

• ORA_CMP_BIP_IC_SHOW_INPUT_VALUES

Profile Option

• Overview of Profile Options

• Create and Edit Profile Options

Map Third-Party Plans

Create maps between plans and plan
components to transition third-party plans to
individual compensation plans.

• None

Security Reference
The tasks that people can do and the data that they can see depend on their roles, duties, and privileges. For
information about these factors, see these two guides:

• Securing HCM

• Security Reference for HCM

Grade Step Progression Setup and Maintenance Tasks

You can move people automatically from one grade, or grade and step, to the next level in a grade ladder using grade
step progression. To do this, complete these setup tasks in the sequence listed.

Task Name

Description

Recommended Help

Manage Common Lookups

Optionally, create groups for progression grade
ladders using the ORA_CMP_GSP_GRADE_
LADDER_GRP lookup. You can associate
progression grade ladders with a group. Then
you can use the group of ladders instead of
a single ladder when processing grade step
progressions.

• Overview of Lookups

• Manage Grade Step Progression

12

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 2
Setup and Maintenance Tasks

Task Name

Description

Recommended Help

Progression Grade Ladder

Create progression grade ladders with the
grades, or grades and steps, that people should
progress through, and the rules for progression.
For example, you create a grade ladder for
manufacturing workers with the Job Assembly
II grade. The grade has three steps. Progression
rules move people with that grade from 1 step
to the next, every 6 months.

• Manage Grade Step Progression

• Create a Progression Grade Ladder for

Batch Processing

• Overview of HCM Data Loader

• Guidelines for Using HCM Spreadsheet

Data Loader

Configure Global Settings (if the Redwood
experience isn’t enabled)

Grade Step Progression Settings (if the
Redwood experience is enabled)

Review the default online and batch settings
for grade step progression, and change as
appropriate.

• Guidelines for Loading Progression Grade

Ladders

• Guidelines for Loading Progression Grade

Rates

• Global Compensation Settings for

Defaulting Salary from Grade Ladder Rates

• Batch Settings for Grade Step Progression

Processing

• Batch Error Conditions for Assignment

Date in Grade Step Progression Processing

• Batch Error Conditions for Salary Date in

Grade Step Progression Processing

Run Grade Step Progression

Synchronize Grade Step Rate

Schedule the Run Grade Step Progression
process to identify the assignments eligible to
progress to a new grade or step.

• Overview of Grade Step Progression

Processing

• Run Grade Step Progression Process

Run the Synchronize Grade Step Rate process
according to your policies, to change people's
salaries after the underlying rates for the
grades or steps change.

• Overview of Grade Step Progression

Processing

• Synchronize Grade Step Rate Process

Security Reference
The tasks that people can do and the data that they can see depend on their roles, duties, and privileges. For
information about these factors, see these two guides:

• Securing HCM

• Security Reference for HCM

Workforce Compensation Setup and Maintenance Tasks

Complete these setup tasks to enable managers to award compensation within the regular compensation cycle.

13

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 2
Setup and Maintenance Tasks

Workforce Compensation Setup and Maintenance Tasks

Task Name

Description

Recommended Help

Manage Workforce Compensation Lookups

Review and maintain lookup values for budget
audit history, such as initial budget and budget
distributed by manager.

• Reason Lookups

• Nonmonetary Unit of Measure Lookups

• User-Defined Column Lookups

Workforce Compensation Plans

Create and maintain compensation plans and
associated budget details.

• Overview of Workforce Compensation Plan

Configuration

Configure Compensation History

Specify the payroll elements and input values
that make up a worker's compensation history.

Configure Global Compensation Settings

Configure properties, such as stock price and
watchlist availability, that apply to all group
compensation plans.

Configure Compensation Batch Processes

Configure processing parameters, such as the
maximum number of errors allowed, for each
batch process.

• Compensation History Categories

• How You Set Up the Other Compensation
and Recurring Payments Summary Data
for Compensation History

• General and Watchlist Global Settings for

Workforce Compensation Plans

• Global Setting Options for Workforce
Compensation Plan Notifications

• Start Workforce Compensation Cycle and

Synchronize Hierarchy Processes

• Refresh Workforce Compensation Data

Process

• Transfer Workforce Compensation Data to

HR Process

• Back Out and Purge Workforce
Compensation Data Processes

• Process Workforce Compensation Change

Statements Process

• Define Elements, Balances, and Formulas

Elements

Fast Formulas

Derived Factors

Manage Action Reasons

Profile Rating Models

Review predefined earnings and deduction
elements and create new ones, using a
questionnaire that automatically generates
the related balances, formulas, and other
components.

Review predefined formulas and create new
ones to validate or calculate data for benefits,
 human resources, absences, or payroll.

• Define Elements, Balances, and Formulas

• Overview of Using Formulas

Create and update application-calculated
eligibility criteria that can change over time,
such as participant age or length of service.

• Derived Factors

Review predefined action reasons that track
changes to data, and create new ones.

• Action Framework

Create and update models for rating the
performance, potential, and proficiency level of
workers.

• Rating Models

14

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 2
Setup and Maintenance Tasks

Security Reference
The tasks that people can do and the data that they can see depend on their roles, duties, and privileges. For
information about these factors, see these two guides:

• Securing HCM

• Security Reference for HCM

Related Topics

• Overview of Workforce Compensation

Total Compensation Statements Setup and Maintenance
Tasks

Complete these setup tasks to enable people to define and generate a total compensation statement.

Total Compensation Statements Setup and Maintenance Tasks

Task List

Task Name

Description

Recommended Help

Define Total Compensation
Statements

Compensation Items

Compensation Categories

Statement Definitions

Configure Global Settings

Configure the design, content,
 and delivery of a compensation
statement that includes
nontraditional forms of pay. For
example, you can include fringe
benefits, cost of benefits, and paid
time off, as well as base pay and
variable compensation.

Create the lowest level of detail
displayed in total compensation
statements originating from
sources such as payroll balances or
element entries.

• Overview of Creating a Total
Compensation Statement

• Compensation Items and

Sources

Create and configure categories
to display similar types of
compensation information in
tabular format in compensation
statements.

• Compensation Category

Types

• Compensation Categories and

Subcategories

Create and configure statement
definitions that determine the
structure and period of the
statement, the compensation
displayed, and the graphs and
information text that appear on the
statement.

Configure options, such as stock
price and watchlist availability, that
apply to all generated statements.

• Guidelines to Create Total
Compensation Statement
Definitions

• Best Practices for Planning
Statement Definitions

• Overview of Creating a Total
Compensation Statement

15

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 2
Setup and Maintenance Tasks

Task List

Task Name

Description

Recommended Help

Manage Payroll Objects

Manage External Compensation
Data Lookups

Configure Compensation Batch
Parameters

Balance Definitions

Fast Formulas

Manage lookup type used to
identify and categorize data from
a third-party application that you
import for use in a compensation
business process.

Configure processing parameters,
 such as the maximum number
of errors allowed, for each batch
process.

Create and configure payroll
elements, such as earnings and
deductions, as well as payroll
balances and formulas used to
manage compensation.

Review the predefined balance
definitions and create ones as
needed, including specifying
assigned dimensions and feeds.

Review predefined formulas and
create new ones to validate or
calculate data for benefits, human
resources, absences, or payroll.

• External Compensation Data

• Record Type Lookups for

External Compensation Data

• Overview of Creating a Total
Compensation Statement

• Compensation Items and

Sources

• Define Elements, Balances,

and Formulas

• Define Elements, Balances,

and Formulas

Security Reference
The tasks that people can do and the data that they can see depend on their roles, duties, and privileges. For
information about these factors, see these two guides:

• Securing HCM

• Security Reference for HCM

16

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 3
Profile Options for Compensation Pages, Actions, and
Approval Notifications

3  Profile Options for Compensation Pages,
Actions, and Approval Notifications

CMP_COMPENSATION_RESPONSIVE_ENABLED Profile
Option

To let everyone use the responsive compensation pages that adjust to the screen size of their devices, use this
option. It's enabled by default. For the enabled profile option to work, you also need to create and enable the
HCM_RESPONSIVE_PAGES_ENABLED profile option.

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

BIP_ONLINE_NOTIFICATION_HCM_COMPENSATION
Profile Option

To generate BI approval notifications for all compensation actions, such as Change Salary and Individual Compensation,
create and enable this option. For the enabled profile option to work, you also need to create and enable the
BIP_ONLINE_NOTIFICATION_HCM profile option.

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

BIP_ONLINE_DISCLOSE_HISTORY_HCM_COMPENSATION
Profile Options

To have the approval notification Approvers section include a Show Details link instead of listing submission and
approval details, create and enable these options. You reduce the initial notification content while still letting people see
the details when appropriate.

• BIP_ONLINE_DISCLOSE_HISTORY_HCM_COMPENSATION_CHANGESALARYAPPROVALTASK applies to

notifications for the Change Salary and Administer Salary tasks.

17

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 3
Profile Options for Compensation Pages, Actions, and
Approval Notifications

• BIP_ONLINE_DISCLOSE_HISTORY_HCM_COMPENSATION_VARIABLEALLOCATIONTASK applies to

notifications for the Manage Personal Contributions, Individual Compensation, and Administer Individual
Compensation tasks.

For the preceding profiles to work after you enable them, you also need to create and enable these profile options:

• BIP_ONLINE_DISCLOSE_HISTORY_HCM

• BIP_ONLINE_DISCLOSE_HISTORY_HCM_COMPENSATION

When you enable or disable these profile options, you affect all notifications generated after that change.

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

BIP_ONLINE_HIDE_EDIT_HCM_COMPENSATION Profile
Options

To hide the Edit button on approval compensation notifications, create and enable these options.

• BIP_ONLINE_HIDE_EDIT_HCM_COMPENSATION_CHANGESALARYAPPROVALTASK applies to notifications for

the Change Salary and Administer Salary tasks.

• BIP_ONLINE_HIDE_EDIT_HCM_COMPENSATION_VARIABLEALLOCATIONTASK applies to notifications for the
Manage Personal Contributions, Individual Compensation, and Administer Individual Compensation tasks.

For the preceding profiles to work after you enable them, you also need to create and enable these profile options:

• BIP_ONLINE_HIDE_EDIT_HCM

• BIP_ONLINE_HIDE_EDIT_HCM_COMPENSATION

When you enable or disable these profile options, you affect all notifications generated after that change.

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

ORA_PER_EMPL_ENABLE_WRK_ASG_REST_LOV Profile
Option

Identify the appropriate assignment in compensation responsive pages by configuring other assignment attributes to
display in the Business Title switcher. To do this, use the REST LOV in the Business Title LOV by setting the profile value
to Y.

18

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 3
Profile Options for Compensation Pages, Actions, and
Approval Notifications

Here's the general behavior of the REST Business Title LOV:

•

•

•

•

It appears on the My Compensation, Compensation Info page only when the selected person has more than
one assignment.

It lists assignments that are in any of these HR Statuses: Active, Suspended, Inactive.

It lists all assignment types except the Offer assignment.

It supports assignment-level security and lists only those assignments for the selected person that the signed
in person has access to.

The ORA_PER_EMPL_ENABLE_WRK_ASG_REST_LOV profile option setting isn't specific to the My Compensation and
Compensation Info pages. It applies to all HCM products that use the new Business Title LOV.

Related Topics

• Employment Profile Options

19

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 3
Profile Options for Compensation Pages, Actions, and
Approval Notifications

20

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 4
Profile Options for Salary Actions

4  Profile Options for Salary Actions

HR_DISABLE_PENDING_APPROVALS_CHECK_IN
_HCM_DATA_LOADER Profile Option

To load salary changes with HCM Data Loader when related salary is pending approval, enable this option.

The actions pending approvals can be from a standalone salary action, such as Change Salary. Or they can be when
salary is part of HR actions that include salary changes, such as Promote or Transfer.

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

ORA_CMP_LGT_WHEN_MISSING_SALARY_DATASECURITY
Profile Option

To prevent salary proposals during Global Transfer actions, when the proposers don’t have permission to access the
source assignment salary, enable this option. Or you can prevent copying salary from the source assignment, but still let
people propose it.

In either case, the option applies only when source and destination legal employer have the same legislative data group.

Profile Value

Outcome

Copy and allow entry (default)

Copy the salary from the source assignment and let people make changes.

Don’t copy but allow entry

Don't copy the salary from the source assignment, but let people propose a new salary.

Don’t copy nor allow entry

Don't copy the salary from the source assignment and don't let people propose a new salary.

When the global transfer can't copy salary from the source assignment to the destination assignment, people can
propose salary regardless of the profile configuration. When people have data security access on the source assignment
salary, the global transfer copies future salary for certain salary basis types. But when they don’t have access, the global
transfer doesn't copy future salary, even when people can propose the salary.

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

21

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 4
Profile Options for Salary Actions

ORA_CMP_NO_SALARY_CHANGE_WHEN_INACTIVE_CHG_ASGN
Profile Option

To let people change salary in the Change Assignment action for an inactive assignment or an assignment that will
become inactive, disable this profile option. By default, this enabled profile option prevents people from changing salary
in these instances.

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

ORA_CMP_SAL_REUSE_ASGN_ACTION_OCCURRENCE
Profile Option

To make salary reuse the action occurrence identifier of the assignment whenever a matching action and reason exists
for the salary start date, enable this option.

We recommend that you enable this profile option only if you’re using responsive pages and the enhanced Employment
Info page released in 22C. Enabling the profile option can affect the action occurrence identifier of the previous salary.
For example, you've salary on 2010, 2016, and 2021.

• When an HR specialist creates a salary for 2022, the processing tries to reuse the action occurrence identifier

for the 2022 salary and 2021 salary.

• When they change the 2021 salary, processing tries to reuse the action occurrence identifier for the 2021 salary.

• When they delete the 2021 salary, processing tries to reuse the action occurrence identifier for the 2016 salary.

Whenever someone creates or deletes a salary, processing accesses the previous salary to correct the end date. Thus
processing also tries to reuse the action occurrence identifier for that salary. Reuse of action occurrence happens
whenever people create or correct salary independently using tools, actions and pages, and processes:

• Tools examples:

◦ HCM Data Loader or HCM Spreadsheet Data Loader and Salary object
◦ Salaries REST API
◦ Download Salaries

• Responsive action and page examples:

◦ Change Salary (Line Manager)
◦ Change Salary (Compensation Manager)
◦ Edit Salary from Compensation Info
◦ Salary History

22

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 4
Profile Options for Salary Actions

◦ Local and Global Transfer
◦ Combined Correction and Deletion Employment Details (introduced in 22C update)

• Process examples:

◦ Run Salary Processes
◦ Run Grade Step Progression
◦ Synchronize Grade Step Rates
◦ Workforce Compensation Transfer (only when posting salary, without assignment changes)
◦ Mass Legal Employer Change

• Classic action and page example:

◦ Change Salary

When assignment has multiple changes on the same day with the same action and reason, we link the salary to the
most recent action occurrence. The action occurrence won't get reused while posting assignment and salary changes
from Workforce Compensation, because it posts salary changes before assignment changes.

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

ORA_CMP_SALARY_CHECKS_BEHAVIOR_IN_CHANGE_START_DATE
Profile Option

To specify how to handle salary validation failures when someone's hire date changes, use this option. The
application checks for salary-related issues and displays an error or warning message depending on the profile option
configuration.

When a validation fails and the profile option is set to Error, people can't submit their transaction. But, if the profile
option is set to Warning, they get a warning message and can submit their transaction if they ignore the warning.

These are the checks affected by this profile option:

•

Is a salary change proposal pending approval?

• Does more than one salary exist for the assignment?

•

Is the salary basis no longer active?

• Does the salary amount violate the salary range on the proposed hire date?

ORA_PER_CLE_COPY_FUT_ASG Profile Option

To copy future salary changes as part of the Local and Global Transfer flow, enable this option. For the copy to happen,
the source and destination employers need to have the same legislative data group.

23

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 4
Profile Options for Salary Actions

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

ORA_PER_EMP_RETAIN_CHANGES Profile Option

To keep salary changes made during various actions when the proposer returns to the when section and changes the
start date, enable this option.

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

ORA_PER_EMPL_DEFAULT_EFFECTIVE_DATE Profile
Option

Use this option to not default the when date in the responsive Change Salary flow. When you want to make sure that the
proposer enters a date, set the profile value for this option to N.

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

24

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 5
Profile Options for Individual Compensation Pages and
Actions

5  Profile Options for Individual Compensation
Pages and Actions

CMP_DISABLE_PENDING_APPROVALS_CHECK_IN_MANAGE_CONTRIBUTION
Profile Option

To let individuals submit more personal contributions while other contributions are pending approval, enable this
option. Also configure access details for the individual compensation plan so that people can't update or stop
contributions using the Manage Personal Contributions action.

This profile option affects only individuals submitting personal contributions. Even when it's enabled, people using
these actions to submit new allocations still have to wait for pending approvals to be resolved:

•

Individual Compensation

• Administer Compensation

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

CMP_IC_DATACHECK_IN_NONCMP_FLOWS Profile
Option

To ensure that only people with relevant data security privileges maintain individual compensation in HR actions that
have the section, enable this option. People without the necessary privileges who try to add individual compensation
get an error about insufficient privileges.

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

Prevent Submissions Without Changes Profile Options

To prevent people from submitting a Personal Contribution, an Individual Compensation, or an Administer
Compensation action without making changes, you need to enable these options. Or you can warn them instead that
they haven’t made changes.

25

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 5
Profile Options for Individual Compensation Pages and
Actions

Profile

Description

ORA_CMP_PERSONAL_CONTRIBUTION_
BLANKSUBMIT

ORA_CMP_INDIVIDUAL_COMPENSATION_
BLANKSUBMIT

ORA_CMP_ADMINISTER_
COMPENSATION_BLANKSUBMIT

Let individuals submit personal contributions without any changes.

Let people submit allocations without any changes when they use the Individual Compensation task.

Let people submit allocations without any changes when they use the Administer Compensation task.

You can set the individual profile to one of these options:

• Error: Raise an error when an individual tries to submit without any changes.

• Warning: Raise a warning when an individual tries to submit without any changes.

• Allow: Let the individual submit without any changes.

Processing tracks changes made in the Individual Compensation section to show the warning or error. Approvers can
still edit and submit allocations without making changes, even when you enable any of these options.

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

ORA_CMP_BIP_IC_SHOW_INPUT_VALUES Profile Option

To include input values in the approval notifications for the Manage Personal Contribution, Individual Compensation,
and Administer Individual Compensation actions, enable this option. Then approvers can view all the proposed input
values and not just the primary input value.

The notification includes the lookup code meanings instead of codes, and the values stored in the input values
columns. It doesn't include the meaning or descriptions when the values use validations, such as Value Set and
Validation Source.

When you enable or disable this profile option, you affect all notifications generated after that change.

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

26

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 5
Profile Options for Individual Compensation Pages and
Actions

ORA_CMP_LGT_WHEN_MISSING_IC_DATASECURITY
Profile Option

To prevent individual compensation proposals during Global Transfer actions when the proposers don’t have
permission to access the source assignment allocations, enable this option. Or prevent copying individual
compensation allocations from the source assignment, but still let people propose it.

In either case, the option applies only when source and destination legal employer have the same legislative data group.

Profile Value

Outcome

Copy and allow entry (default)

Copy the individual compensation allocations from the source assignment and let people make
changes.

Don’t copy but allow entry

Don’t copy nor allow entry

Don't copy the individual compensation allocations from the source assignment, but let people
propose a new salary.

Don't copy the individual compensation allocations from the source assignment and don't let people
propose a new salary.

When the global transfer can't copy individual compensation allocations to the destination assignment, people can
propose allocations regardless of the profile configuration.

Related Topics

• Overview of Profile Options

• Create and Edit Profile Options

27

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 5
Profile Options for Individual Compensation Pages and
Actions

28

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 6
Responsive User Experience Setup

6  Responsive User Experience Setup

Search Logic Profile Options for Client List of Values

You can use the logic <codeph>CONTAINS</codeph> to create the client list of values. This returns results containing
the characters you enter.

Optionally, for individual list of values, you could change this logic to <codeph>STARTS WITH</codeph>, to return
results that start with the search characters you enter.

For example, when you search for a person with the name John Smith while using the logic CONTAINS, you can search by
'jo' or 'sm' or 'th'. When you use the logic STARTS WITH, your search must start with 'j'.

Use the logic STARTS WITH when your list contains thousands of values (more than 15,000 records) to improve the search
performance. Or, if you don't partition your data by set ID.

Note:  If you change the search logic for a client list of values, the logic changes in all pages where the list of values is
used.

Related Topics

• Search Logic Profile Options for Client List of Values in Global Human Resources

Use Transaction Design Studio to Configure Field
Displays

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

29

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 6
Responsive User Experience Setup

Related Topics

• Overview of Page Modification

Displayed and Hidden Responsive Compensation
Management Fields

You can configure compensation management fields using Transaction Design Studio.

My Compensation
You can configure these attributes, which make up the My Compensation page.

Attribute

Current Salary

Additional Compensation

Personal Contribution

Prior Salary

Total Compensation Statements

Workforce Compensation

Shares

Recurring and One-Time Payments

Salary

Adjustment

Action

Action Reason

Start Date

Effective Period

End Date

Annual Salary

Annualized Full-Time Salary

Grade ladder

Grade Name

Grade Step

Salary Range

Displayed

Comments

Yes

Yes

Yes

Yes

Yes

Yes

Yes

Yes

Yes

Yes

No

No

Yes

No

No

Yes

No

Yes

No

No

No

Section

Section

Section

Section

Section

Section

Section

Section

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

30

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 6
Responsive User Experience Setup

Attribute

Displayed

Comments

Salary Range Midpoint

Range Position

Compa-Ratio

Quartile

Quintile

Next Salary Review Date

Adjustment Amount

Adjustment Percentage

Percentage

Amount

Annual Amount

Annualized Full-Time Amount

Salary Amount

Estimated Stock Price

Estimated Value of Vested Shares

Estimated Value of Unvested Shares

Business Title

No

Yes

No

No

No

No

Yes

Yes

Yes

Yes

Yes

No

Yes

No

No

No

No

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute, displayed with the
salary basis type of components type

Salary section attribute, displayed with the
salary basis type of components type

Salary section attribute, displayed with the
salary basis type of components type

Salary section attribute, displayed with the
salary basis type of components type

Salary section attribute, displayed with the
salary basis type of components type

Salary section attribute, displayed with the
salary basis type of components type

Salary drill-down attribute

Stock

Stock

Stock

Compensation Info
You can configure these attributes on the Compensation page.

Attribute

Current Salary

Show Future and Prior Salary.

Additional Compensation

Shares

Recurring and One-Time Payments

Salary

Displayed

Comments

Yes

Yes

Yes

Yes

Yes

Yes

Section

Section

Section

Section

Section

Salary section attribute

31

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 6
Responsive User Experience Setup

Attribute

Adjustment

Start Date

Effective Period

Action

Action Reason

Salary Basis

End Date

Annual Salary

Annualized Full-Time Salary

Grade ladder

Grade Name

Grade Step

Salary Range

Salary Range Midpoint

Range Position

Compa-Ratio

Quartile

Quintile

Next Salary Review Date

Adjustment Amount

Adjustment Percentage

Percentage

Amount

Annual Amount

Annualized Full-Time Amount

Currency

Estimated Stock Price

Estimated Value of Vested Shares

Displayed

Comments

Yes

Yes

No

Yes

Yes

Yes

No

Yes

No

Yes

No

No

No

No

Yes

No

No

No

No

Yes

Yes

Yes

Yes

Yes

No

Yes

No

No

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute

Salary section attribute, displayed with the
salary basis type of components type

Salary section attribute, displayed with the
salary basis type of components type

Salary section attribute, displayed with the
salary basis type of components type

Salary section attribute, displayed with the
salary basis type of components type

Salary section attribute, displayed with the
salary basis type of components type

Salary section attribute, displayed with the
salary basis type of components type

None

Stock

Stock

32

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 6
Responsive User Experience Setup

Attribute

Displayed

Comments

Estimated Value of Unvested Shares

Currency

Business Title

No

No

No

Stock

None

None

Salary Attributes
You can configure these salary attributes, which make up the salary sections on various compensation pages. They're
also part of various Offer and HR flows, such as Offer, Hire, Promote, and Transfer.

Attribute

Start Date

Action

Action Reason

End Date

Salary Basis

Salary Amount

Adjustment Amount

Adjustment Percentage

Annual Salary

Annualized Full-Time Salary

Next Salary Review Date

Grade Name

Salary Range

Salary Range Mid Point

Compa-Ratio

Range Position

Quartile

Quintile

Displayed

Comments

Yes

Yes

Yes

No

Yes

Yes

Yes

Yes

Yes

No

No

Yes

No

No

Yes

No

No

No

None

None

None

None

None

None

For salary components, the value appears in the
table.

This attribute doesn't appear in the new Offers
and New Hire flows delivered in 18C.

For salary components, the value appears in the
table.

This attribute doesn't appear in the new Offers
and New Hire flows delivered in 18C.

None

None

None

None

Analytic displays salary range when available.

None

None

None

None

None

33

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 6
Responsive User Experience Setup

Attribute

Currency

Displayed

No

Comments

None

Shares Section
You can configure these stock shares attributes on the My Compensation and Compensation Info pages.

Attribute

Displayed

Comments

Total Shares

Vested Shares

Unvested shares

Granted

Original Grant Price

Estimated Stock Price

Estimated Value of Vested Shares

Estimated Value of Unvested Shares

Unvested Value

Yes

Yes

Yes

Yes

Yes

No

No

No

Yes

None

None

None

None

None

Hidden by default

Hidden by default

Hidden by default

None

Salary History
You can configure the attributes in the two regions on the Salary History pages.

Salary History section

Attribute

Start Date

Action

Action Reason

End Date

Salary Basis

Salary Amount

Adjustment Amount

Adjustment Percentage

Annual Salary

Next Salary Review Date

Displayed

Comments

Yes

Yes

Yes

No

Yes

Yes

Yes

Yes

Yes

Yes

None

None

None

None

None

None

None

None

None

None

34

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 6
Responsive User Experience Setup

Attribute

Displayed

Comments

Placement in Salary Range

Quartile

Quintile

Compa-Ratio

Range Position

Salary Range

Salary Range Midpoint

Created By

Created On

Updated By

Updated On

Grade Ladder

Grade name

Grade Step

Comments and Attachments

Currency to Use

Salary Details section

Attribute

Start Date

Action

Action Reason

End Date

Salary Basis

Salary Amount

Adjustment Amount

Adjustment Percentage

Annual Salary

Annualized Full-Time Salary

Next Salary Review Date

Yes

Yes

No

Yes

No

No

No

No

No

No

No

Yes

Yes

Yes

Yes

No

None

None

None

None

None

None

None

None

None

None

None

Appears when on grade ladder

None

Appears when on grade ladder, step

Controls the display of the Comments and
Attachment section

None

Displayed

Comments

Yes

Yes

Yes

No

Yes

Yes

Yes

Yes

Yes

Yes

Yes

None

None

None

None

None

None

None

None

None

None

None

35

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 6
Responsive User Experience Setup

Attribute

Compa-Ratio

Quartile

Quintile

Range Position

Reason

Salary Range

Salary Range Midpoint

Compensation Zone

Compensation Zone Type

Working at Home

Grade Ladder

Grade name

Grade Step

Currency to Use

Prior Salary

Related Topics

Displayed

Comments

Yes

Yes

Yes

Yes

Yes

Yes

Yes

Yes

Yes

Yes

Yes

Yes

Yes

No

Yes

None

None

None

None

None

None

None

Appears while using compensation zone based
differential profile

Appears while using compensation zone based
differential profile

Appears while using compensation zone based
differential profile

Appears when on grade ladder

None

Appears when on grade ladder, step

None

None

• Use Transaction Design Studio to Configure Field Displays

Displayed and Hidden Responsive Team Compensation
Fields

You can configure team compensation fields using Transaction Design Studio.

Assignment
You can configure these assignment attributes, which make up the Overview, Compensation, and Talent tabs of the My
Team pages.

Attribute

Image

Displayed

Yes

Comments

None

36

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 6
Responsive User Experience Setup

Attribute

Displayed

Person Display Name

Business Title

Number of direct reports and total number of
reports

Text for non-primary assignments

Text for suspended assignments

Icon and text for dotted line/matrix
relationships

Text for worker type

Person List Name

Yes

Yes

Yes

Yes

Yes

Yes

Yes

No

Preferred Name (or Known As) and Last Name

No

Person Number

Assignment Number

Job Name

Job Code

Job Name and Job Code

Position Name

Position Code

Position Name and Position Code

Location Name

Location Code

Location Name and Location Code

Country Name

Country Code

Location Name and Country Code

Local Time and Location Name

Work E-mail Address

Work Phone Number

Assignment Type

Legal Employer

Legislation

No

No

No

No

No

No

No

No

No

No

No

No

No

No

No

No

No

No

No

No

Comments

None

Formerly known as Assignment Name. For
incumbents, this field isn't displayed by default.

None

None

None

Includes text for relationship type. Line
manager relationships don't display this field.

Not displayed for individuals.

None

None

None

None

None

None

None

None

None

None

None

None

None

None

None

None

None

None

None

None

None

None

37

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 6
Responsive User Experience Setup

Attribute

Displayed

Comments

Legislation Code

Cost Center

Department Name

Grade Name

Grade Code

Service Years

Business Unit

Current Salary, Currency and Basis

Salary Range, Currency and Basis

Compa-Ratio

Development Goals

Performance Goals

Performance

Potential

Risk of Loss

Impact of Loss

Talent Score

No

No

No

No

No

No

No

No

No

No

No

No

No

No

No

No

No

Team Compensation
You can configure this team compensation attribute.

Attribute

Current to Use

Displayed

Yes

None

None

None

None

None

None

None

None

None

None

None

None

None

None

None

None

None

Position
You can configure these position attributes, which make up the Overview, Compensation, and Talent tabs of the My
Team pages.

Attribute

Position Name

Position Code

Displayed

Comments

Yes

Yes

None

None

38

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 6
Responsive User Experience Setup

Attribute

Business Unit

Number of direct reports and total number of
reports

Headcount and FTE of incumbents

Headcount and FTE of open positions

Department Name

Location Name

Job Name

Entry Grade

Valid Grades

Grade Ladder

Position Headcount and FTE

Hiring Status

Type

Displayed

Comments

Yes

Yes

Yes

Yes

No

No

No

No

No

No

No

No

No

This field isn't displayed by default on mobile
devices.

None

None

None

None

None

None

None

None

None

None

None

None

Requisition
You can configure these requisition attributes on the Overview tab of the My Team pages.

Attribute

Displayed

Requisition Title

Requisition Number

Requisition Status

Recruiter

Number of Candidates

Days Since Opened

Location

Department

Work Location

Job Name

Job Family

Job Function

Yes

Yes

Yes

Yes

No

No

No

No

No

No

No

No

39

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 6
Responsive User Experience Setup

Attribute

Job Grade

Requisition Template

Internal Title

Number to Hire

Unlimited Hire

Displayed

No

No

No

No

No

Vacancy
You can configure these vacancy attributes on the Overview tab of the My Team pages.

Attribute

Vacancy Job

Department

Location

Openings

Requisition Number

Position Name

Remaining Openings

Related Topics

Displayed

Yes

Yes

Yes

Yes

No

No

No

• Use Transaction Design Studio to Configure Field Displays

40

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 7
Approvals Overview

7  Approvals Overview

How Default Approval Tasks for Salary and Individual
Compensation Work

You can route salary changes, individual compensation allocations, and workforce compensation allocations to the
appropriate approvers using approval workflow tasks.

You can configure the approval rules to support your compensation policies using these tasks in the Define Approval
Management for Human Capital Management task list:

• Manage Task Configurations for Human Capital Management

• Manage Approval Groups

To find the task list, click Search on the Setup and Maintenance work area, Tasks panel tab.

Manage Task Configurations for Human Capital Management
Approval tasks are event-driven configurations containing rules that identify the approval routing and approvers for
business objects, such as salary changes and compensation allocations.

• On the task Configuration tab of the workflows, the Once per stage task aggregation ensures that the approval

process sends only one notification per approver.

• The Assignees tab provides a technical view of each task and is where you go to the task rules.

Here's what the default compensation approval tasks do:

Task Name

Description

ChangeSalaryApprovalTask

Runs when someone submits a salary change from the Salary section of compensation page, or using
the Change Salary task or quick action. This approval task doesn't run for changes identified by the
Run Grade Step Progression or Synchronize Grade Step Rates processes.

Sends actionable notifications to the manager of the person who's salary is changing, to approve or
reject the salary changes.

•

•

If the manager rejects the change, the task is complete.

If the manager approves the change, the task sends an actionable notification to their manager
to approve or reject the change. Regardless of the second manager's action, the task stops at this
level of the supervisor hierarchy.

SalaryHistsoryApprovalTask

Runs when someone submits a salary change from the Salary History action, quick action, or task.

Sends actionable notifications to the approver, to approve or reject the salary changes.

VariableAllocationTask

Runs when someone submits an individual compensation or personal contribution allocation.

Sends actionable notifications to the manager of the person getting the individual compensation
allocation or making the personal contribution, to approve or reject the allocation.

41

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 7
Approvals Overview

Task Name

Description

•

•

If the manager rejects the allocation, the task is complete.

If the manager approves the allocation, the task sends an actionable notification to their manager
to approve or reject the allocation. Regardless of the second manager's action, the task stops at
this level of the supervisor hierarchy.

None of these approval workflow tasks include threshold rules by default. You can configure thresholds according to
salary change percentage, salary change amount, current and new compa-ratio, grade, job, and so on. For example, you
can create a rule using this IF statement that routes salary approvals when the salary change exceeds 10 percent:

Task.payload.getSalaryApprovalValuesResponse.result/value.newChangePercent more than 10.00.

Manage Approval Groups
By default, the delivered actionable approval workflow tasks route time cards using the dynamically decided supervisor
hierarchy. You can identify specific approvers to route to instead using the Manage Approval Groups task.

ApprovalTimeRecordGroup attribute values vary by implementation. To figure out your value mapping, create your own
data model report in the Reports and Analytics work area using this query:

select * from FUSION.cmp_col_attr_map where LOCATION like 'Approval' and ENTERPRISE_ID = <ent_id>;

Tip:  You can define rules on the primary input value using the Worker's Other Compensation.Details.Amount
attribute.

Related Topics

• How You Define Approvals for Human Capital Management

• The Manager Hierarchy: How It's Maintained

• Guidelines for Managing Approval Rules

• Approver Types

• HCM Approval Rules

How You Configure Different Approval Flows for
Individual Compensation Allocations and Personal
Contributions

To configure different approval flows for individual compensation allocations and personal contributions, include the
module identifier for the action in your rules.

Action

Module Identifier

Individual Compensation

(Task.payload.transactionApprovalRequest.moduleIdentifier == "Change Variable
Allocation")

42

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 7
Approvals Overview

Action

Module Identifier

Manage Personal Contribution

Administer Individual Compensation

(Task.payload.transactionApprovalRequest.moduleIdentifier == "Make Personal
Contribution")

(Task.payload.transactionApprovalRequest.moduleIdentifier == "Administer
Variable Allocation")

Related Topics

• How Default Approval Tasks for Salary and Individual Compensation Work

• Route Approval for Individual Compensation or Personal Contribution Allocation by Action

How You Can Validate Salary and Responsive Individual
Compensation Approval Rule Changes

Test approval rule changes for responsive salary and individual compensation processes and actions without creating
and submitting any new transactions. This way, you can debug and incrementally build conditional logic for approval
rules, then instantaneously see the effects.

Use the HCM Approval Rules page and Transaction Console for these responsive processes and actions:

Salary Processes and Actions

Individual Compensation Processes and Actions

• Administer Individual Compensation

• Administer Individual Compensation

• Manage Individual Compensation

• Manage Individual Compensation

• Manage Personal Contributions

• Manage Personal Contributions

This validation doesn't apply to classic individual compensation workflows because you can see the approval chain on
the transaction Review page.

You need to first commit any changes you make to the approval rules before you simulate the rules. You can search for
transactions by name, who created them, and created during a date range. To further refine your results, use the Status
field. The available statuses are Draft, In Progress, and Failed. Select from the list of filtered transactions and use those
values to simulate the approval rule results.

Tip:  To test the approval flow configuration for new transactions, you need to disable bypass approvals. But you can
test the approval flow configuration for pending, draft, and failed transactions when bypass approvals is enabled.

Note:

For more information, see these Oracle HCM Cloud Common Features Release 13 Transaction Console documents (ID
2430452.1) on My Oracle Support.

• The Basics of Approval Rules

43

Oracle Fusion Cloud Human Resources
Implementing Compensation

• The Basics of Transaction Console

Chapter 7
Approvals Overview

44

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 8
Example Approval Configurations

8  Example Approval Configurations

Autoapprove a Salary Change If the Requester Is an HR
Specialist

You control salary approvals with the ChangeSalaryApprovalTask workflow. Here's how you can configure the default
workflow to automatically approve salary changes if the requester has the HR Specialist role.

Scenario
Edit approval workflows using the Manage Task Configurations for Human Capital Management task in the Setup and
Maintenance work area. Complete this configuration of the THEN fields on the Assignees tab.

THEN Field

List Builder

Response Type

Value

Supervisory

Required

This response type makes the notification actionable, instead of just informational.

Number of levels

1

Starting Participant

Top Participant

Auto Action Enabled

Auto Action

Rule Name

Related Topics

HierarchyBuilder.getManager("supervisory",Task.payload.transactionApprovalRequest.Requestor,-1,null,null)

HierarchyBuilder.getManager("supervisory",Task.payload.transactionApprovalRequest.Requestor,-1,null,null)

True

"APPROVE"

AutoapproveHRSpecialist

• How Default Approval Tasks for Salary and Individual Compensation Work

Grade Determines the Levels of Approval for a Salary
Change

You control salary approvals with the ChangeSalaryApprovalTask workflow.

45

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 8
Example Approval Configurations

Here's an idea of how you can configure the default workflow to set different levels of required approval. In this
example, the required levels depend on the grade. If the requester's grade is X, then require only one level of approval. If
the requester's grade is Y, then require two levels of approval.

Edit approval workflows using the Manage Task Configurations for Human Capital Management task in the Setup and
Maintenance work area. Complete these steps on the Assignees tab.

1. Create the rule where the requester's grade is X.

2. Create the rule where the requester's grade is Y.

a. Create this IF expression:

Task.payload.Requestor's Assignment.result.grade.toUpperCase() is "Y"

b. Complete the THEN fields, as shown here.

Then Field

List Builder

Response Type

Value

Supervisory

Required

This response type makes the notification actionable, instead of just informational.

Number of levels

2

Starting Participant

Top Participant

Auto Action Enabled

Auto Action

Rule Name

HierarchyBuilder.getManager("supervisory",Task.payload.transactionApprovalRequest.Requestor,-1,null,null)

HierarchyBuilder.getManagerOfHierarchyPrincipal("supervisory",HierarchyBuilder.getManager
 ("supervisory",Task.payload.transactionApprovalRequest.Requestor,-1,null,null))

False

null

2LevelsforGradeY

3. Create the rule where the requester's grade is X.

a. Create this IF expression:

Task.payload.Requestor's Assignment.result.grade.toUpperCase() is "Y"

b. Complete the THEN fields, as shown here.

Then Field

List Builder

Response Type

Value

Supervisory

Required

This response type makes the notification actionable, instead of just informational.

46

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 8
Example Approval Configurations

Then Field

Number of levels

Starting Participant

Top Participant

Auto Action Enabled

Auto Action

Rule Name

Value

1

HierarchyBuilder.getManager("supervisory",Task.payload.transactionApprovalRequest.Requestor,-1,null,null)

HierarchyBuilder.getManager("supervisory",Task.payload.transactionApprovalRequest.Requestor,-1,null,null)

False

null

1LevelforGradeX

Related Topics

• How Default Approval Tasks for Salary and Individual Compensation Work

Route Approval for a Salary Change According to
Country and Amount

You control salary approvals with the ChangeSalaryApprovalTask workflow.

Here's an idea of how you can configure the default workflow to route the approval depending on the country and
amount. In this example, the country is the US. If the amount is more than 10,000, the approval routes to X and Y and
then the area of responsibility. If the amount is less than 10,000, it routes to only the area of responsibility.

Edit approval workflows using the Manage Task Configurations for Human Capital Management task in the Setup and
Maintenance work area. Complete these steps on the Assignees tab.

1. Create the rule where the country is US and the amount is more than 10,000.

a. Create this IF expression:

Task.payload.Requestor's Assignment.result.legislationCode.toUpperCase() is "US"
 andSalaryApproval.newChangeAmount.doubleValue() more than 10000

b. Complete the THEN fields for users X, as shown here.

THEN Field

List Builder

Value

Resource

Response Type

Required

This response type makes the notification actionable, instead of just informational.

47

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 8
Example Approval Configurations

THEN Field

Value

Users

Groups

Application Role

Rule Name

X

null

null

USover1000usersX

c. Complete the THEN fields for users Y, as shown here.

THEN Field

List Builder

Value

Resource

Response Type

Required

This response type makes the notification actionable, instead of just informational.

Users

Groups

Application Role

Rule Name

Y

null

null

USover1000usersY

d. Complete the THEN fields for users according to their area of responsibility, as shown here.

THEN Field

List Builder

Response Type

Users

Value

Resource

Required

This response type makes the notification actionable, instead of just informational.

GetRepresentative("HR_REP",Task.payload.Worker's Current
 Representative.result)

48

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 8
Example Approval Configurations

THEN Field

Groups

Application Role

Rule Name

Value

null

null

USover1000usersAOR

2. Create the rule where the country is US and the amount is less than 10,000.

a. Create this IF expression:

Task.payload.Requestor's Assignment.result.legislationCode.toUpperCase() is "US"
 andSalaryApproval.newChangeAmount.doubleValue() less than 10000

b. Complete the THEN fields, as shown here.

THEN Field

List Builder

Response Type

Users

Groups

Application Role

Rule Name

Value

Resource

Required

This response type makes the notification actionable, instead of just informational.

GetRepresentative("HR_REP",Task.payload.Worker's Current
 Representative.result)

null

null

USunder1000usersAOR

Related Topics

• How Default Approval Tasks for Salary and Individual Compensation Work

Route Approval for Recurring Individual Allocation When
the Amount Changes by a Percentage

You control individual compensation approvals with the VariableAllocationTask workflow.

Here's how you can configure the default workflow to handle approvals for percentage changes to recurring awards
made using responsive compensation pages. You use an approval configuration like this because the responsive pages
split updates at submission. In this example, you configure these variable allocation rules to account for both recurring
and nonrecurring elements associated with the awards and contributions.

49

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 8
Example Approval Configurations

Rule Name

Purpose

RecurUnder10%

OnetimeUnder10%

Onetime10%plus

Recur10%plus

Route recurring awards and contributions with changes that are less than 10%.

Route onetime awards and contributions with changes that are less than 10%.

Route onetime awards and contributions with changes that are 10% or more.

Route recurring awards and contributions with changes that are 10% or more.

CAUTION:  To make sure that any simultaneous updates happen correctly, confirm that the elements associated with
the individual compensation plans have Multiple entries not allowed selected.

Edit approval workflows using the Manage Task Configurations for Human Capital Management task in the Setup and
Maintenance work area. Complete these steps on the Assignees tab.

1. Enable advanced mode.

a. Expand the VariableAllocatiRules rule.
b. Click the Show Advanced Settings icon, which is between the Expand icon and the rule name.
c. Select Advanced Mode.

2. Create the RecurUnder10% rule.

a. Create this IF expression:

Task is a Task
and
Lists is a Lists
and
Each {
 ICD is a Worker's Other Compensation Details and
 FirstAmouont = ICD.Amount.doubleValue() and
 Frequency = ICD.Other Compensation Award Frequency and
 FirstPlanId = ICD.planId and
 FirstOptionId = ICD.Other Compensation Option Id and
 Mflag = ICD.multipleEntriesAllowedFlag.toUpperCase()
and
 ICD2 is a Worker's Other Compensation Details and
 SecondAmount = ICD2.Amount.doubleValue()
 ChangePercent = ((SecondAmount-FirstAmount/FirstAmount)*100
 SecondPlanId = ICD1.planId
 SecondOptionId = ICD2.Other Compensation Option Id
 (Frequency is "R" and
 Mflag is "Y" and
 SecondPlanId is FirstPlanId and
 SecondOptionId is FirstOptionId and
 ChangePercent less than 10.00 and
 ChangePercent more than 0)
}

b. Complete the THEN fields, as shown here.

THEN Field

List Builder

Response Time

Value

Resource

Required

50

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 8
Example Approval Configurations

THEN Field

Value

This response type makes the notification actionable, instead of just informational.

Users

Groups

Application Role

Rule Name

Dimension Id

X

null

null

"RecurUnder10%"

null

3. Create the OnetimeUnder10% rule.

a. Create this IF expression:

Task is a Task
and
Lists is a Lists
and
Each {
 ICD is a Worker's Other Compensation Details and
 ICD.Other Compensation Change in Value Percentage less than 10.00
}

b. Complete the THEN fields, as shown here.

THEN Field

List Builder

Response Time

Users

Groups

Application Role

Rule Name

Dimension Id

Value

Resource

Required

X

null

null

"OnetimeUnder10%"

null

4. Create the Onetime10%plus rule.

a. Create this IF expression:

Tasks is a Task
and
Lists is a Lists
and
Each {
 ICD is a Worker's Other Compensation Details and
 ICD.Other Compensation Change in Value Percentage.doubleValue() same or more than 10.00
}

51

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 8
Example Approval Configurations

b. Complete the THEN fields, as shown here.

THEN Field

List Builder

Response Time

Users

Groups

Application Role

Rule Name

Dimension Id

Value

Resource

Required

This response type makes the notification actionable, instead of just informational.

X

null

null

"Onetime10%plus"

null

5. Create the Recur10%plus rule.

a. Create this IF expression:

Task is a Task
and
Lists is a Lists
and
Each {
 ICD is a Worker's Other Compensation Details and
 FirstAmount = ICD.Amount.doubleValue() and
 Frequency = ICD.Other Compensation Award Frequency and
 FirstPlanId = ICD.planId and
 FirstOptionId = ICD.Other Compensation Option Id and
 Mflag = ICD.multipleEntriesAllowedFlag.toUpperCase()
and
 ICD2 is a Worker's Other Compensation Details and
 SecondAmount = ICD2.Amount.doubleValue()
 ChangePercent = ((SecondAmount-FirstAmount)/FirstAmount)*100
 SecondPlanId = ICD2.planId
 SecondOptionId = ICD2.Other Compensation Option Id
 (ChangePercent same or more than 10.00 and
 Frequency is "R" and
 Mflag is "Y" and
 SecondPlanId is FirstPlanId and
 SecondOptionId is FirstOptionId and
 ChangePercent more than 0)
}

b. Complete the THEN fields, as shown here.

THEN Field

List Builder

Response Time

Value

Resource

Required

52

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 8
Example Approval Configurations

THEN Field

Value

Users

Groups

Application Role

Rule Name

Dimension Id

X

null

null

"Recur10%plus"

null

Related Topics

• How Default Approval Tasks for Salary and Individual Compensation Work

Autoapprove Personal Contributions

You control salary approvals with the VariableAllocationTask workflow. Here's how you can configure the default
workflow to automatically approve personal contributions.

Edit approval workflows using the Manage Task Configurations for Human Capital Management task in the Setup and
Maintenance work area. Complete these steps on the Assignees tab.

1. Create this IF expression:

(Task.payload.transactionApprovalRequest.moduleIdentifier == "Make Personal Contribution")

2. Complete the THEN fields, as shown here.

THEN Field

List Builder

Response Type

Value

Supervisory

Required
This response type makes the notification actionable, instead of just informational.

Number of levels

1

Starting Participant

Top Participant

HierarchyBuilder.getPrincipal(Task.payload.transactionApprovalRequest.Requestor,-1,null,null)

HierarchyBuilder.getPrincipal(Task.payload.transactionApprovalRequest.Requestor,-1,null,null)

Auto Action Enabled

True

Auto Action

Rule Name

"APPROVE"

AutoapprovePersonalContribution

53

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 8
Example Approval Configurations

Related Topics

• How Default Approval Tasks for Salary and Individual Compensation Work

Route Approval for Individual Compensation or Personal
Contribution Allocation by Action

You can route individual compensation and personal contribution allocations to different approvers depending on
the action used to make the allocation. To make these changes to individual compensation and personal contribution
approval rules, go to Navigator > Tools > Transaction Console.

1. On the Transaction Manager: Transactions page, click the Approval Rules tab.
2. On the Transaction Manager: Rules page, search for and click any process you want to change:

◦ Administer Individual Compensation
◦ Manage Individual Compensation
◦ Manage Personal Contributions

3.

If the process configuration bypasses approvals, click the Bypass Approvals icon to turn off the bypass.

4. Add a rule.

a. Click the corresponding Configure Rules icon.
b. On the Approval Rules page, click the Add New Rule icon.
c. On the graphic, click the rule oval that just appeared, for example, Rule1.

5. Configure the rule to route by the module identifier.

a.

In the Rule: Add Details section, enter a rule name, such as Administer Action, Manage Action, or
Contribution Action.

b. Click Configure Rule Conditions.
c. On the Condition Details dialog box, click the box with the existing expression 1 == 1.
d. Click Edit Selection.
e. On the Approval Rules: Edit Condition Expression dialog box, change Enter a number to Select from

attribute.
In the Select Attribute list, select transactionApprovalRequest > moduleIdentifier.

f.
g. Change Select Operator to ==.
h. Change Select value type to Enter a string.
i.

In the field that appears, enter the appropriate module identifier:

Action

Module Identifier

Make Personal Contribution

Make Personal Contribution

Individual Compensation

Change Variable Allocation

54

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 8
Example Approval Configurations

Action

Module Identifier

Administer Individual Compensation

Administer Variable Allocation

j. Click OK.
k. On the Condition Details dialog box, review the expression. It should look something like this expression for

the Administer Individual Compensation module identifier:

(transactionApprovalRequest.moduleIdentifier == "Administer Variable Allocation")

l. Click OK.

6. Add the approver.

a. On the Approval Rules page graphic, in the path of your new rule, click the THEN object to highlight it.
b.

In the Approvers pane, click the Add Approver Participant icon next to the appropriate approver, such as
Representative.

c. Click Submit.

Related Topics

• How You Configure Different Approval Flows for Individual Compensation Allocations and Personal

Contributions

55

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 8
Example Approval Configurations

56

Oracle Fusion Cloud Human Resources
Implementing Compensation

9  Market Data

Overview of Market Data

Chapter 9
Market Data

Various job evaluation methods exist as a way to price jobs according to their worth. Market data are a method to price
jobs that are externally focused, so you attract and retain workers based on the labor market.

The foundation for any job evaluation method, including market data, is to start with good job descriptions.

You might want to compare your salaries, salary ranges, and other compensation such as bonus or stock to prepared
industry-wide data to make sure your compensation is in line with your company’s goals. For example, you might want
to make sure you award your people at the 50th percentile of the industry average by job and location. Or you might
want to award base pay at a lower percentile but award stock at a higher level.

With market data you map external survey jobs and locations with internal jobs and locations. Then, you import the
surveys and use the market data subject area in OTBI to consolidate the data. After you create composites of your
survey data, you import these composites. Finally you can display the composites in the worksheet or administer
workers in Workforce Compensation.

You can find the market data tasks in the Compensation work area under Market Data.

Here's a diagram that shows you the market data task flow:

57

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 9
Market Data

How You Use Market Data Surveys to Create Composites

Surveys are market data from an individual supplier. Composites are aggregated survey data.

Here are the steps that you take to import and use survey data and convert them to composites.

1. Decide which surveys to buy and participate in.
2. Receive surveys from suppliers.
3. Use OTBI to help you complete surveys.
4. Return surveys to the suppliers.
5. Receive survey results from each supplier.
6.
7. Use OTBI to analyze your people’s data versus the surveys’ data.
8. Take any actions based on your analysis, such as, updating salary ranges or aligning salaries with the market.
9. Use OTBI to aggregate surveys into composites.

Import the surveys using the Import Survey task.

58

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 9
Market Data

Import composites using the Import Composites task.

10.
11. Display composites in Workforce Compensation.
12. Line managers and administrators make compensation allocation decisions based on the composites.

Note:  If you already have composites, you can start from step 10. However, in that case, the survey data won’t be in
the subject area.

Related Topics

• Overview of Market Data

•

•

Import Survey for Market Data

Import Composites for Market Data

Compensation Types for Market Data

Your first task is to define the compensation types that you want to display in market data. Compensation types let you
identify different kinds of pay, such as base salary and bonus, and import survey data for each type.

You can find the Compensation Types page in the Compensation work area under Market Data.

The Compensation Types page is where you identify the market target. For example, if you target the 50th percentile of
the market for Base Salary then you can select that option. If you target the 40th percentile for base salary and the 60th
percentile for bonus, then this is where you identify that mix of pay. The target appears in market composites wherever
they occur in the application.

We deliver several common compensation types, but you can add your own. For example, you might want to offer
supplemental life insurance to executives and review that across competitors in the survey data. Create a compensation
type with the name Executive Benefit Supplemental Life Insurance. Select the Compensation Group of Benefits and a
Data Type of Other.

If you need to set market targets separately for different countries, create and load survey data in that manner. For
example, if the India salary market target is 60% and United States is 50%, create separate compensation types for
them. Load the India salary with one compensation type and the US salary with another.

Related Topics

• Overview of Market Data

Overview of Supplier Structures

The Supplier Structures page in the compensation work area is where you match your internal jobs and locations to
survey jobs and locations.

You start by adding your suppliers and their surveys. You can have multiple suppliers and each supplier can have
multiple surveys. On the Manage Job List page, you load or manually add survey jobs and match them to your internal
jobs or positions. On the Manage Location List page, you can load or manually add survey locations and match them to
internal locations. You can match several internal locations to a survey location.

59

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 9
Market Data

Here's a list of the subtasks for the supplier structures task:

Page

Description

Manage Surveys

Manage Job Structures

Manage Job List

You add your suppliers and their surveys on this page. You can have multiple suppliers and each
supplier can have multiple surveys. You add details for each supplier. For example, you can add a
supplier like Hay. And then you can add surveys from Hay like Hay Professional Survey and Hay
Executive Survey.

You can associate job function, job family and other structures to survey jobs. These are entirely
optional. If you do use these values you need to configure them before you add jobs. Then, you can
select the attributes from job structures when you’re in the Manage Job List page. Job structures
are Job Family, Job Function, Career Stream or Band, or Career Level. You can use the Manage Jobs
Structures task, for example, to contain info about the survey jobs. This associates these Job Structures
to survey jobs only. It's not tied to internal jobs.

You can load or manually add survey jobs or positions and match them to your internal jobs or
positions. At the top of the page there’s info about the number of survey jobs and what you’ve
matched. To use any of the Job Structures (Job Function, Job Family, Career Stream or Band, Career
Level or Other Level) associated with Survey Jobs, be sure to add them first or they won't be available
to select. These are optional.

You use the Job Match Notes section to record notes about why job matches change over time. For
example, last year you might have recorded internal Accountant 1 as a match to survey Accountant.
But this year changes in the internal job description for Accountant 1 no longer matches the survey
description for Accountant. Because you might need to explain this to the survey auditor at a later
time, it’s a good idea to make a note about your decision when it occurred.

Manage Location List

On the Manage Location List page, you can load or manually add survey locations and match them to
internal locations. You can match many internal locations to a survey location.

You can map on a many to 1 basis here. This is helpful especially if the survey location is broader than
your internal locations. For example, if the survey location is Northern California, then you can include
all your Northern California locations, such as San Ramon and Oakland in the mapping.

This helps your downstream analysis by associating the survey data with all the employees in those
internal locations. Another example is if the survey data is by country, and you have a few locations in
that country.

Related Topics

• Overview of Market Data

How You Match a Survey Job or Position to Your Internal
Data

In the Match Internal Job or Position section, you match the survey job to your job or position.

Search for the internal job or position code that matches the survey job. If you’ve identified parent benchmark jobs in
Global HR, the child jobs appear below the match.

60

Oracle Fusion Cloud Human Resources
Implementing Compensation

Related Topics

• Overview of Supplier Structures

Chapter 9
Market Data

Difference Between Global HR Benchmark Jobs and
Survey Benchmark Jobs

The Parent Job or Global HR Benchmark indicator refers to a setting in Jobs in Global HR.

Here's the difference between Global HR Benchmark jobs and Survey Benchmark jobs.

• Survey benchmark jobs are matched to internal jobs or positions in Supplier Structures. Any of your internal

jobs that you match to survey jobs, are survey benchmark jobs.

• Parent Job or Global HR benchmark jobs are indicated that way in the job table, and have child jobs associated

with them.

Related Topics

• Overview of Supplier Structures

Import Survey for Market Data

Surveys are market data from an individual supplier.

You can use the Create Import Template button on the Import Market Data page to invoke the HSDL.You can only load
surveys and not manually add them. However, after you load them, you can modify editable columns like dates, and
percentiles. You can use the HCM Data Loader to create survey records when you implement Market Data for the first
time or provide regular updates.

Before you start

Here’s some things to consider before you begin.

• You need to have a supplier and a survey, with survey jobs and locations, before you import surveys. You can

use existing compensation types.

• The Batch Name, Supplier Code, Survey Code, Survey Location Code, Survey Job Code, Compensation

Type Code, and Industry fields are required.

• The industry column can’t be blank. It can be All, ALL, #NULL, or anything else.

Here's what to do

1. Create the market data workbook in the Compensation work area.

a. On the Tasks panel tab under Market Data click Import Survey.
b. On the Import Survey page, click Create Import Template to create the workbook.

61

Oracle Fusion Cloud Human Resources
Implementing Compensation

2. Enter survey data.

Chapter 9
Market Data

Add enough rows to accommodate your supplier's data. Copy the market data and paste them into cells with a white
background. The workbook adds a symbol in the Changed field to mark the rows that you added. Reordering or
removing columns in the import file causes the upload process to fail.

3. When you're done, click Upload. The application uploads only those rows that are marked as Changed. It ignores

any changes in cells without a white background.

CAUTION:  Don't select the Upload and then immediately download option when prompted during an upload.
The data that you uploaded immediately downloads back into the workbook, hiding any errors that occurred
during the upload.

4. Validate changes.

On the Import Survey page, search for and select the start date and record type, or other search criteria.

5. Resolve errors.

The upload process automatically updates the Status cell in each workbook row. If there are errors that require
review, the process:

a. Rolls back the change in the application.
b. Sets the workbook row status to Upload Failed
c. Continues to the next workbook row

To view and resolve an error:

a. Double-click Update Failed in the Status field.
b. Fix any data issues in the workbook.
c. Upload the latest changes.

New uploads to existing data make date-effective changes to the data.

Use the Data Exchange work area under My Client Groups to see the upload. You see if the process completed
successfully and learn about any error messages.

Related Topics

• Overview of Market Data

• Guidelines for Loading Market Data Objects

Market Segments

Market segments are groups of locations.

After you review your survey and internal locations you can select segments or locations based on geographic labor
market pay differences. You can find the Market Segments task in the Compensation work area under Market Data.

You can decide, for example, that some of your market data should use internal locations for market comparisons, while
other portions of your organization need segmentation. You might want to consolidate internal locations into market
segments if your composites in some locations are all the same. Let’s say you have 3 offices in the San Francisco Bay
Area, and the market data for those is the same.

62

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 9
Market Data

Rather than loading the same data 3 times into 3 locations, you can create a market segment that includes your 3
locations and load the composites once. You might decide that the administrative jobs data differs enough locally in
the Bay Area that you want to use internal locations for those jobs. However, the manager jobs don’t have such local
differentiations. Load the administrative jobs using internal locations, and load the managerial jobs using segments.

Related Topics

• Overview of Market Data

Import Composites for Market Data

Composites are aggregated survey data. They're summaries of all survey data.

Composites are mapped to your internal jobs or positions, and internal locations or segments.

Note:  If you use only 1 survey, the survey tables hold the raw survey data from the supplier, while the composite table
holds your vetted data that you prepared for line manager consumption.

You can use the Create Import Template button on the Import Market Composite page to invoke the HDSL You can
also use the HCM Data Loader to upload the consolidated surveys from the suppliers.

Before you start

Here’s some things to consider before you begin.

• Make sure to load only segment or location within a row, and not both. If you use location, you need to make

sure the segment column has a #NULL in it.

• Similarly, make sure to load only job or position within a row, and not both. If you use position, you need to

make sure the job column has #NULL in it.

• The industry column can’t be blank. It can be All, ALL, #NULL, or anything else.

• Use internal codes for jobs, positions or locations, and not the survey codes you use to load composites.

• Remember: composites are no longer raw survey data, but aggregations of all the surveys, so any individual

survey codes no longer apply.

To use the imported data, you need to complete one or both of these tasks, either before or after the import:

• To view in workforce compensation you need to enter a market composite effective date for the plan cycle.

• To see the individual worker view you need to create a market composite tile in the individual worker view task.

Here's what to do

1. Create the market data workbook in the Compensation work area.

a. On the Tasks panel tab under Market Data click Import Composites.
b. On the Import Composites page, click Create Import Template and select either Load by Segment or

Load by Location to create the workbook.

63

Oracle Fusion Cloud Human Resources
Implementing Compensation

2. Enter composite data.

Chapter 9
Market Data

Add enough rows to accommodate your composite data. Copy the composites and paste them into cells with a white
background. The workbook adds a symbol in the Changed field to mark the rows that you added. Reordering or
removing columns in the import file causes the upload process to fail.

3. When you're done, click Upload. The application uploads only those rows that are marked as Changed. It ignores

any changes in cells without a white background.

CAUTION:  Don't select the Upload and then immediately download option when prompted during an upload.
The data that you uploaded immediately downloads back into the workbook, hiding any errors that occurred
during the upload.

4. Validate changes.

a. On the Import Composites page, search for and select the start date and record type, or other search

criteria.

5. Resolve errors.

The upload process automatically updates the Status cell in each workbook row. If there are errors that require
review, the process:

a. Rolls back the change in the application.
b. Sets the workbook row status to Upload Failed
c. Continues to the next workbook row

To view and resolve an error:

a. Double-click Update Failed in the Status field.
b. Fix any data issues in the workbook.
c. Upload the latest changes.

New uploads to existing data make date-effective changes to the data.

Use the Data Exchange work area under My Client Groups to see the upload. You see if the process completed
successfully and learn about any error messages.

Related Topics

• Overview of Market Data

• Guidelines for Loading Market Data Objects

Options to View Market Composites in Compensation

You can view market composites in workforce compensation and in market data.

Market Composite Views
To view in workforce compensation you need to do the following in the Workforce Compensation Plans setup task:

• Enter a market composite effective date on the Configure Plan Cycles page.

• Enable market composites column on the Configure Worksheet Page Layout page, Detail Table tab, Additional

Information section.

64

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 9
Market Data

• Enable Individual Worker View and create a market composite tile on the Individual Worker View page.

Line managers and administrators can view market composites in multiple ways.

Role

Line Manager

Location

Market Composites Region in the Compensation Info page, This is accessible via the Compensation
Info quick action in the My Team tab.

Line Manager or Compensation Manager Market Composites dialog box on the Workforce Compensation Worksheet

Individual Worker View page on the Workforce Compensation Worksheet

Compensation Manager

Administer Workers page, Compensation tab in the Compensation work area

Compensation Analyst

View Market Composites page in the Compensation work area

Related Topics

• Overview of Market Data

• How You Configure Market Composites Display

How You Configure Market Composites Display

You can select and label market composites for display in the downstream application using the Configure Market
Composites Display task.

You can populate all the columns in the composites table, so professional users have access to complete data, while
controlling the downstream consumption of specific columns. You select and label market composites for display in the
downstream application using the Configure Market Composites Display task.

On the Configure Market Composites Display page, first use the tabs to select the downstream application page. Next,
use the add action to include the compensation types and then use the list of values to select the compensation types
you want to display. Enter a compensation types display name if you want it to appear with a friendly label. Additionally,
enable the Market Target as desired. You can also enter a market target display name if you want it to appear with a
different label. You define the market targets within the compensation types task.

After you save, you can click the compensation types name link to go to the Configure Composite Columns subtask
where you enable the percentiles that you want to appear. You can also enable the chart and select various other
columns.

Related Topics

• Options to View Market Composites in Compensation

• Compensation Types for Market Data

65

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 9
Market Data

66

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

10  Payroll Elements and Compensation

How Compensation Uses Payroll Elements

Oracle Fusion Global Human Resources, Oracle Fusion Cloud Compensation, and Oracle Fusion Cloud Total
Compensation Statement record compensation. They then transfer the compensation to payroll providers, and store
custom data at the worker level using payroll elements.

People then link these elements to salary bases, individual and workforce compensation plans, and total compensation
statements.

Compensation Object

Element Use

Salary basis

Create element entries that pass salary amounts to payroll.

Individual compensation plan option

Record allocation amounts using the element input values. The element can also decide costing.

Create element entries that pass stock grant dates and numbers of shares granted. You can also
post stock awards directly to the compensation stock table. Use the Stock Grants task, the integrated
workbook, HCM Data Loader, or HCM Spreadsheet Data Loader.

Nonsalary workforce compensation
component

Create element entries that the Transfer Workforce Compensation Data to HR process uses to pass the
component amount, including lump sums. The process also uses them to pass stock grant dates and
numbers of shares granted.

You can also post stock awards directly to the compensation stock table. Use the Stock Grants task, the
integrated workbook, HCM Data Loader, or HCM Spreadsheet Data Loader.

Total compensation statement

A source of the actual compensation shown for the mapped compensation items.

To hold worker-level data referenced or used in a calculation during a workforce compensation cycle, you can create an
information element with multiple input values. Then people configuring workforce compensation plans can use a fast
formula to display the element entry values in appropriate worksheet columns.

Before You Can Use Payroll Elements in Compensation

Whether you've Oracle Fusion Cloud Global Payroll Interface or Oracle Fusion Cloud Global Payroll, you must define
payroll statutory units to use in Oracle Fusion Cloud Compensation. You must also associate a legislative data group
with each unit.

Do this using the Manage Legal Entities and Manage Legal Entity HCM Information tasks. It ensures that when
you hire people, payroll relationships get created automatically. People need these payroll relationships to get their
compensation element entries created.

67

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

Payroll Definitions
The payroll definition supplies each person's pay period frequency and end dates. Even if you use a third-party payroll
provider, you need to define a payroll if any of these conditions apply:

• You want to use nonrecurring elements.

Note:  We recommend that you assign payrolls to everyone, even when using only recurring elements.

• You want to create a salary basis that uses a frequency of Payroll period.

• You're implementing total compensation statements and these conditions apply:

◦ You use recurring elements and want total compensation statements to prorate salary element

entries when someone gets hired during a payroll period. You also want the proration to happen when
someone's employment is terminated during a payroll period.

◦ You want to let individuals view their total compensation statement details to see payroll period amounts.

• You license Oracle Global Payroll Interface.

You don’t need to define payroll definitions when both of these conditions apply:

• You use only recurring elements defined at the assignment level.

• You store salary at the assignment level of a legal employer.

But if you use compensation history, all compensation awards appear in the recurring payment sections as end-of-year
amounts.

Consolidation Groups
If you create payroll definitions, you need to also define consolidation groups. Each legislative data group that you
define elements for needs to have at least one consolidation group.

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

68

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

• Payroll Definitions, which is usually required to support elements

• Consolidation Groups, which is required for creating payroll definitions

If you use predefined Payroll Interface extracts to transfer data to a third-party payroll provider, you might need to
create element subclassifications, balances, organization payment methods, and object groups. See the Global Payroll
Interface documentation for more information.

Before You Begin
Before you start the Define Elements, Balances, and Formulas task list, complete the tasks these offerings contain.

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

69

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

Source Application

Element Purpose

◦ Employee contributions and employer distributions for medical options
◦ Flex credits for flex benefits
• Earnings elements to disburse unused credits as cash.

Time and Labor

Time card details such as salary, overtime hours, and shift unit payments.

Absence Management

Absence details such as number of hours, days absent, or accrual absence balance details.

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

70

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

Task

Requirements

• Validating user entries into element input values

• Configuring compensation, benefit, and accrual plan rules

• Calculating periodic values for gross earnings and defining element skip rules for the Calculate

Gross Earnings process (provided with Global Payroll Interface)

Balance Definitions

If you're using Global Payroll Interface, creating earnings elements creates balances automatically. You
can edit these generated balance definitions.
If you're using the Calculate Gross Earnings process, you might want to create other balances for
extracts or reporting.

Object Groups

You can create object groups to specify subsets of elements or payroll relationships to include in a
report or process, such as the Calculate Gross Earnings process.

Related Topics

• Overview of Using Formulas

• Payroll Definitions

• Payroll Balance Definitions

• How Payroll Elements Hold Information for Multiple Features

Create a Payroll Element to Use with Salary Bases

Configure the payroll element for use in recurring base pay, such as annual salaries and hourly earnings. This guidance
applies to US legislative data groups (LDG).

You can use the same payroll element with multiple salary bases if they've the same currency. You can’t use the same
element for salary bases, individual compensation plans, and workforce compensation plans, or a combination.

1. Go to My Client Groups > Compensation > Elements.

2. Create an element.

3. On the Create Element dialog box, complete these steps:

a. Select a US LDG.
b. Select the primary classification, such as Standard Earnings. The listed classifications depend on the LDG

that you selected.

c. Optionally select the secondary classification, such as Regular. When the selections don't really match your

purpose, you can skip this step.

d. Select the appropriate category, if required, such as Standard.
e. Click Continue.

4. On the Create Element: Basic Information page, complete these steps:

a. Enter a descriptive name that lets you and others easily figure out the use or purpose of the element.
Make sure that the name starts with a letter and contains only letters, numbers, spaces, hyphens, or a
combination of these. It can't contain any special characters.

You can include a prefix, such as SB that lets people easily identify that the element is for a salary basis. You
don't want people using the same element in different compensation objects because it can lead to payroll

71

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

conflicts. It can also lead to unexpected deletions of salary or individual compensation. Two example
names are SB US Annual Salary and SB California Hourly Wages.

b. Complete these basic information fields.

Field

Value Guidance

Reporting Name

Enter the name that you want to show in compensation history, on reports, and on payslips

for this earnings payroll element.

Reporting names need to be unique for elements that you add to compensation history.

Effective Date

Enter 1/1/1951.

Enter an early date so that the element is available for use immediately in your salary bases,

 and individual and workforce compensation plans.

Currency

Select US Dollar.

Decides each individual’s local salary currency.

What is the earliest entry date for this

Select First Standard Earning Date.

element?

What is the latest entry date for this

This date decides how element entries process after someone's job is terminated or they're

element?

transferred to another payroll. Select the value that fits your business process.

At which employment level should

Select Assignment.

this element be attached?

Term-level elements aren’t supported.

c. Specify that this element recurs each payroll period.
d. Specify whether a person can have more than one entry for this element in a payroll period. To let people

link the same salary element to multiple salary bases, select Yes.

e. To accept the remaining default values, click Next.

5.

If your implementation includes it, on the Create Element: Additional Details page, complete these steps:

a. Select the calculation rule, such as Flat amount.
b. Select the default periodicity, which is the frequency that the salary basis stores the amount in. The value

should be the same as the salary basis frequency, such as Hourly, Weekly, or Monthly.

c. Select the conversion rule for the element. For the calculation used by each conversion rule, see Conversion

Rule Options for Configuring Additional Details of Payroll Elements.

d. To accept the default values for the remaining rules, click Next.

If you use Global Payroll or Global Payroll Interface, configure more details for base pay elements, such as
proration and retroactive changes.

72

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

6. On the Create Element: Review page, complete these steps:

a. Review all your rules and options to ensure that every value is correct.
b. To create the element, click Submit.

7. On the Element Summary page, complete these steps:

a. Review the generated input values. To link the element to a salary basis, the element needs to have a

monetary input value and the Periodicity input value.

- If your implementation includes Global Payroll, you can use the automatically created Amount input
value as is with no extra configuration. If Amount wasn’t automatically created, you need to create a
monetary input value so that people can link the element to a salary basis.

- If the primary classification is Standard Earnings, the Periodicity input value was automatically

created. If the primary classification is Information, you need to create it.

b. Make the element eligible for everyone to use. The element will apply only to people assigned the salary

basis linked to this payroll element.

In the Elements Overview section, select Element Eligibility.

i.
ii. Click Actions > Create Element Eligibility.
iii.

In the General Information section, Element Eligibility Name field, enter the element name with the
suffix Open. For example, for the SB US Annual Salary payroll element, the element eligibility name
would be SB US Annual Salary Open.

iv. Enter the same effective date for element eligibility that you did for the element effective date, such

as 1/1/1951.

v. To prevent the creation of duplicate element entries when creating or loading salary, make sure that

the Automatic entry option is clear.

c. Click Submit.
d. Click Done.

Related Topics

• How Element Classification Components Work Together

• Payroll Element Eligibility

• Options to Determine an Element's Latest Entry Date

• Periodicity Conversion

• How Payroll Elements Hold Information for Multiple Features

Create a Payroll Element to Use with Individual
Compensation Plans

Configure the payroll element for use in recurring or nonrecurring individual compensation allocations, voluntary
contributions, and nonmonetary information. For example, use it for allowances, spot bonuses, stock grants, retirement
savings plans, charitable donations, and storage of duration or points information.

You can use a payroll element in only one option of one individual compensation plan. And you need to use different
elements for salary bases and individual compensation plans.

This guidance applies to US legislative data groups (LDG).

73

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

1. Go to My Client Groups > Compensation > Elements.

2. Create an element.
3. On the Create Element dialog box, complete these steps:

a. Select a US LDG.
b. Select the primary classification. The listed classifications depend on the LDG that you selected.

Element Use

Suggested Primary Classification

Recurring plan payments

Standard Earnings

Nonrecurring plan payments for

Supplemental Earnings

bonus or lump sum elements

Recurring and nonrecurring voluntary

Voluntary Deductions or Pretax Deductions

deductions for individuals’ savings

contributions and charitable

deductions

Stock grants and awards

Information

Storing nonmonetary information

c. Optionally select the secondary classification. When the selections don't really match your purpose, you

can skip this step.

Element Use

Suggested Secondary Classification

Recurring plan payments

Regular Not Worked

Nonrecurring plan payments

Awards and Prizes, Bonus, another relevant option, or leave it blank.

Recurring and nonrecurring voluntary

Select the relevant option. Otherwise, leave it blank.

deductions

Stock grants

Leave it blank.

Storing nonmonetary information

d. Select the appropriate category, if required, such as Standard.
e. Click Continue.

4. On the Create Element: Basic Information page, complete these steps:

a. Enter a descriptive name that lets you and others easily figure out the use or purpose of the element.
Make sure that the name starts with a letter and contains only letters, numbers, spaces, hyphens, or a
combination of these. It can't contain any special characters.

You can include a prefix, such as IC that lets people easily identify that the element is for an individual
compensation plan. You don't want people using the same element in different compensation objects
because it can lead to payroll conflicts. It can also lead to unexpected deletions of salary or individual

74

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

compensation. Example names are IC Gym Allowance, IC Car Allowance, IC Quarterly US Sales Award, IC
New Hire Stock Grant, and IC Red Cross Contribution.

b. Complete these basic information fields.

Field

Value Guidance

Reporting Name

Enter the name that you want to show in compensation history, on reports, and on payslips

for this earnings payroll element.

Reporting names need to be unique for elements that you add to compensation history.

Effective Date

Enter 1/1/1951.

Enter an early date so that the element is available for use immediately in your salary bases,

 and individual and workforce compensation plans.

Currency

Select US Dollar.

Identifies the currency of the entered and displayed allocation, deduction, or contribution

amount.

What is the earliest entry date for this

Select First Standard Earning Date.

element?

What is the latest entry date for this

This date decides how element entries process after someone's job is terminated or they're

element?

transferred to another payroll. Select the value that fits your business process.

At which employment level should

Select Assignment.

this element be attached?

Relationship-level and term-level elements aren’t supported.

c. Specify whether this element recurs each payroll period or requires an explicit (nonrecurring) entry, such as

a bonus, stock grant, or onetime charitable donation.

d. Specify whether a person can have more than one entry for this element in a payroll period. To let people

link the same element to multiple individual compensation plans, select Yes.

e. To accept the remaining default values, click Next.

For Information elements, skip to the Double-Check Your Selections and Submit the Element section by
clicking Next again.

75

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

5.

If your implementation includes it, on the Create Element: Additional Details page, complete these steps:

a. Select the calculation rule. For recurring and nonrecurring plan payments and nonrecurring voluntary

deductions, select Flat amount. For recurring voluntary deductions, select Flat amount or Percentage of
Earnings.

b. Select the default periodicity, which is the frequency that the plan stores the amount in.

Element Use

Value Guidance

Recurring plan payments

The typical value is Monthly.

Nonrecurring plan payments

Quarterly, Annually, or Periodically

Nonrecurring voluntary deductions

Recurring voluntary deductions

Typically the same periodicity as base pay, such as Annually or Monthly

c. Select the conversion rule for the element. For the calculation used by each conversion rule, see Conversion

Rule Options for Configuring Additional Details of Payroll Elements.

d. To accept the default values for the remaining rules, click Next.

6. On the Create Element: Review page, complete these steps:

a. Review all your rules and options to ensure that every value is correct.
b. To create the element, click Submit.

7. On the Element Summary page, complete these steps:

a. Review the generated input values.

- For the input value that you link to the plan option, make sure that Special Purpose is Primary

input value. Typically, this is the Amount input value. If the value wasn’t automatically created, you
can manually add and configure it here. On individual compensation pages and in notifications,
the primary input value appears in the Value column. Detail pages show other input values. And
notifications can show other input values if the ORA_CMP_BIP_IC_SHOW_INPUT_VALUES profile
option is enabled.

- For each input value that doesn't apply to the plan, deselect the Displayed and Allow User Entry

options, if they aren’t already clear.

- For stock grant information elements, make sure that an input value with the Number unit of

measure has Special Purpose set to Primary Input Value. The element date feeds the Grant Date
column of the stock history table and the primary input value feeds the Shares Granted column. The
Shares section of people's Compensation page uses these values. Depending on configurations,
people's total compensation statements can also use them.

- For storage of nonmonetary information, make sure that Primary Input Value doesn't have Money as

the unit of measure.

b. To validate input values entered on individual compensation pages, add the relevant validation fast

formula. For example, add a validation formula to enforce length of service requirements. A recipient's
service must be more than 10 years to get a proposed award of 1,000 USD or more. The proposed
allocation for anyone with shorter service must be less.

76

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

c. Optionally complete the steps to set up minimum and maximum values when you use these elements with

individual compensation plans:

- Standard earnings elements with a Regular Not Worked secondary classification
- Supplemental earnings elements

Setup steps:

In the Element Overview, Input Values section, select Amount.
In the Input Values section, on the Edit menu, select Correct.
In the Default Entry Values and Validation section, enter a minimum or maximum value, or both.

i.
ii.
iii.
iv. Select Warning or Error, as appropriate.

◦ Warning: Show a message when the manager or HR specialist enters an amount that's below
the minimum value or above the maximum value, if set. This usage enables them to still
continue with their submissions.

◦ Error: Show a message when someone enters an amount that's below the minimum value or

above the maximum value, if set. This usage prevents them from continuing until they enter an
amount that's within the specified limits.

d. Make the element eligible for everyone to use. The element will apply only to people assigned the salary

basis linked to this payroll element.

In the Elements Overview section, select Element Eligibility.

i.
ii. Click Actions > Create Element Eligibility.
iii.

In the General Information section, Element Eligibility Name field, enter the element name with the
suffix Open. For example, for the IC Gym Allowance payroll element, the element eligibility name
would be IC Gym Allowance Open.

e. Click Submit.
f. Click Done.

Related Topics

• How Element Classification Components Work Together

• Payroll Element Eligibility

• Options to Determine an Element's Latest Entry Date

• Periodicity Conversion

• How Payroll Elements Hold Information for Multiple Features

Create a Payroll Element to Use with Workforce
Compensation Plans

Configure the payroll element for use in recurring or nonrecurring workforce compensation allocations and
nonmonetary information. For example, use it for allowances, spot bonuses, and stock grants. Also use it to store
duration or points information and custom worker data.

This guidance applies to US legislative data groups (LDG).

77

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

You can use the same payroll element with multiple workforce compensation plans if they have the same currency. You
can’t use the same element for different components in a workforce compensation plan. You also can’t use the same
element for salary bases, individual compensation plans, and workforce compensation plans, or a combination.

1. Go to My Client Groups > Compensation > Elements.
2. Create an element.

3. On the Create Element dialog box, complete these steps:

a. Select a US LDG.
b. Select the primary classification. The listed classifications depend on the LDG that you selected.

Element Use

Suggested Primary Classification

Recurring plan payments

Standard Earnings

Nonrecurring plan payments for

Supplemental Earnings

bonus or lump sum elements

Stock grants and awards

Information

Storing nonmonetary information

c. Optionally select the secondary classification. When the selections don't really match your purpose, you

can skip this step.

Element Use

Suggested Secondary Classification

Recurring plan payments

Regular Not Worked

Nonrecurring plan payments

Awards and Prizes, Bonus, another relevant option, or leave it blank.

Stock grants

Leave it blank.

Storing nonmonetary information

d. Select the appropriate category, if required, such as Standard.
e. Click Continue.

4. On the Create Element: Basic Information page, complete these steps:

a. Enter a descriptive name that lets you and others easily figure out the use or purpose of the element.
Make sure that the name starts with a letter and contains only letters, numbers, spaces, hyphens, or a
combination of these. It can't contain any special characters.

You can include a prefix, such as WFC that lets people easily identify that the element is for a workforce
compensation plan. You don't want people using the same element in different compensation objects

78

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

because it can lead to payroll conflicts. It can also lead to unexpected deletions of salary or compensation.
Example names are WFC Gym Allowance, WFCC Car Allowance, and WFC Quarterly US Sales Award.

b. Complete these basic information fields.

Field

Value Guidance

Reporting Name

Enter the name that you want to show in compensation history, on reports, and on payslips

for this earnings payroll element.

Reporting names need to be unique for elements that you add to compensation history.

Effective Date

Enter 1/1/1951.

Enter an early date so that the element is available for use immediately in your salary bases,

 and individual and workforce compensation plans.

Currency

Select US Dollar.

Workforce compensation components with a local currency determination code of Salary

Basis Currency use the currency of the element linked to the individual’s salary basis.

What is the earliest entry date for this

Select First Standard Earning Date.

element?

What is the latest entry date for this

This date determines how element entries process after someone's job is terminated or

element?

they're transferred to another payroll. Select the value that fits your business process.

At which employment level should

Select Assignment or Term.

this element be attached?

c. Specify whether this element recurs each payroll period or requires an explicit (nonrecurring) entry, such as

a bonus or stock grant.

d. Specify whether a person can have more than one entry for this element in a payroll period. To let people

link the same element to multiple workforce compensation plans, select Yes.

e. To accept the remaining default values, click Next.

For Information elements, skip to the Double-Check Your Selections and Submit the Element section by
clicking Next again.

5.

If your implementation includes it, on the Create Element: Additional Details page, complete these steps:

a. For the calculation rule, select Flat amount.
b. Select the default periodicity, which is the frequency that the plan stores the amount in.

Element Use

Value Guidance

Recurring plan payments

The typical value is Monthly.

79

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

Element Use

Value Guidance

Nonrecurring plan payments

Quarterly, Annually, or Periodically

c. Select the conversion rule for the element. For the calculation used by each conversion rule, see Conversion

Rule Options for Configuring Additional Details of Payroll Elements.

d. To accept the default values for the remaining rules, click Next.

6. On the Create Element: Review page, complete these steps:

a. Review all your rules and options to ensure that every value is correct.
b. To create the element, click Submit.

7. On the Element Summary page, complete these steps:
a. Review the generated input values.

- For the input value that you link to the compensation component, make sure that Special Purpose
is Primary input value. Typically, this is the Amount input value. If the value wasn’t automatically
created, you can manually add and configure it here.

- For each input value that doesn't apply to the plan, deselect the Displayed and Allow User Entry

options, if they aren’t already clear.

- For stock grant information elements, make sure that an input value with the Number unit of

measure has Special Purpose set to Primary Input Value. The element date feeds the Grant Date
column of the stock history table and the primary input value feeds the Shares Granted column. The
Shares section of people's Compensation page uses these values. Depending on configurations,
people's total compensation statements can also use them.

- For storage of nonmonetary information, make sure that Primary Input Value doesn't have Money as

the unit of measure.

b. Make the element eligible for everyone to use. The element will apply only to people assigned the salary

basis linked to this payroll element.

In the Elements Overview section, select Element Eligibility.

i.
ii. Click Actions > Create Element Eligibility.
iii.

In the General Information section, Element Eligibility Name field, enter the element name with the
suffix Open. For example, for the WFC Gym Allowance payroll element, the element eligibility name
would be WFC Gym Allowance Open.

c. Click Submit.
d. Click Done.

Related Topics

• How Element Classification Components Work Together

• Payroll Element Eligibility

• Options to Determine an Element's Latest Entry Date

• Periodicity Conversion

• How Payroll Elements Hold Information for Multiple Features

80

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

Conversion Rule Options for Configuring Additional
Details of Payroll Elements

Use this information to help you select the correct conversion rule when you're configuring the additional details for
payroll elements linked to compensation objects.

Conversion Rule

Calculation

Example

Standard Rate Annualized

1. Convert the source amount and

NA

periodicity to an annual value using
default values of 2080 hours, 260 working
days.

2. Convert the amount to the required

periodicity and rate.

Standard Rate Daily

1. Calculate a daily rate using default value

NA

Standard Working Hours Rate
Annualized

260 working days.

2. Convert the amount to the required

output periodicity and rate.

1. Convert the source amount and working

hours to an annual value. Use the person's
standard working hours.

2. Calculate the rate.

Scenario: The person works 40 hours a week with a monthly
salary of 1000 US dollars.

Calculation: ((1000*12) / (40.00*52) = 5.77 an hour

Assignment Working Hours Rate
Annualized

1. Convert the source amount and working

hours to an annual value. Use the person's
working hours.
2. Calculate the rate.

Scenario: The person works 40 hours a week, with a 37.5
standard working hours a week, and a monthly salary of 1000
US dollars.

Calculation: ((1000*12) / (37.50*52) = 6.15 an hour

Periodic Work Schedule Rate
Annualized

1. Convert the monetary value and work

Scenario for a person assigned a monthly payroll:

schedule to an annual value. Use the
person's work schedule for the payroll
period for daily and hourly conversions.

2. Calculate the rate.

• The person has a monthly salary of 1000 US dollars.

• The formula checks the work schedule details for the

month.

Daily conversion calculation: 1000 a month / 20 days in the
month = 50

For a person not assigned a payroll: The calculation uses the
weekly rate and converts the result to an annual amount. The
calculation then divides the annual amount by the number of
days or hours in that week, according to the work schedule.

81

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 10
Payroll Elements and Compensation

82

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 11
Base Pay Overview

11  Base Pay Overview

Overview of Base Pay Configuration

Base pay is a person's salary amount. Managers and HR specialists view and adjust this amount or any component
amounts or percentages over the time someone works in their organization. Each salary record they manage has an
associated salary basis.

Here's how the salary basis configuration works with salary records and payroll processing.

• Calculations use the frequency and annualization factor of the salary basis to decide the annualized salary that

appears on the salary record. Calculations also use these salary basis settings and the full-time equivalent value
from the employment record to decide the annualized full-time salary.

• The salary record uses any salary components configured on the salary basis to itemize salary adjustments for

reports, such as merit and location.

• The payroll element associated with the salary basis holds the salary amount entered on the salary record. The

basis passes that amount to payroll for processing.

• The grade rate and differential profile associated with the salary basis decide the salary metrics and validation

messages people see on the salary record. Associating them with the salary basis is optional, so they aren't part
of every salary basis configuration.

You configure grades, grade rates, progression grade ladders, rate definitions, and payroll elements using the Base Pay
task list in the Compensation work area. You can also manage lookups, actions, and action reasons.

Related Topics

• How You Enable Salary Itemization Using Incremental Components

• How You Store the Salary Amount and Pass It to Payroll for Processing

• How Salary Metrics Are Calculated

83

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 11
Base Pay Overview

How Salary Basis Options Work with Salary Amounts and
Calculations

The interval used to quote and store salary, such as hourly or annually, is the frequency of the salary basis associated
with the salary record.

The annualization factor is the numeric multiplier for the frequency. Calculations use the factor and the salary amount
to decide the annual salary amount, as these examples show.

Frequency

Annualization Factor

Salary (USD)

Annual Salary (USD)

Annually

Monthly

Hourly

1

12

2080

50,000

10,000

100

50,000

120,000

208,000

Related Topics

• Overview of Base Pay Configuration

• Examples of Annual Salary and Annualized Full-Time Salary Calculations

• How You Change a Salary to Account for a Changed FTE

How You Store the Salary Amount and Pass It to Payroll
for Processing

The salary basis holds the overall salary amount from the salary record. It passes the amount to the element entry for
payroll processing each pay period.

Legislative Data Group (LDG)
You configure each salary basis for a specified LDG. If your organization has multiple LDGs, you need to create a
uniquely named salary basis for each unique set of characteristics applicable to each LDG. The LDG limits the payroll
elements that you can associate with the salary basis.

Payroll Element
You attach a single payroll element to each salary basis to hold the overall salary amount. The elements that you can
select from meet these criteria:

• They're valid for the selected LDG.

• They recur.

84

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 11
Base Pay Overview

• They're either Earning or Information elements.

• They include eligibility definitions.

The required element eligibility definition can include eligibility criteria. We recommend that you leave the
eligibility open on the payroll element.

Make sure that individual compensation doesn't also use the element you select. Using the same element across
compensation objects can lead to payroll conflicts. It can also lead to unexpected deletions of salary or individual
compensation.

Restrictions
You can link recurring elements to multiple salary bases only if they meet these conditions:

• Headquarters-based grades have a base pay of X.

• Grades for all other locations have a base pay of X - 2%.

Input Value
An element can have multiple input values. The element input value that you select in the salary basis, such as Amount,
is the value that stores the salary amount.

The monetary amount stored in the element entry is the salary amount in the salary information for the person's
assignment. That salary amount is in the frequency of the person's salary basis, such as annually or hourly.

If you don't use Oracle Fusion Global Payroll, you can store the salary amount using information payroll elements.

•

•

If the element includes the Periodicity input value, the element entry stores the annual salary amount.

If the element doesn't include the Periodicity input value, the element entry stores the salary amount in the
same frequency as the salary basis.

Here's how the payroll formula processes the input values of element entries received in the frequency of the salary
basis:

Salary Basis Frequency

Amount Passed to Payroll

Payroll Processing

Annually

Hourly

Annual amount

Hourly rate

Converts the annual amount to the appropriate
payroll period amount.

Multiplies the hourly rate by the number of
hours reported for the payroll period.

The resulting base pay earnings appear on the payslip for the payroll element associated with the salary basis.

Currency
The element currency automatically decides the salary basis currency used to pay the person.

Reference
The Configuring Payroll Elements for Use in Oracle Fusion Compensation document (ID 1589502.1) explains how
compensation uses payroll elements. It also explains how to configure the elements for specific uses.

85

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 11
Base Pay Overview

Related Topics

• Overview of Base Pay Configuration

• Create a Payroll Element to Use with Salary Bases

How Many Salary Bases to Create

You need to create a separate salary basis, for each unique combination of the following characteristics associated with
a worker's base pay.

A good practice if you require many salary bases in your organization is to use descriptive names. Examples are CA
Hourly Wages, UK Annual Salary with Components, and Adjunct Pay 3 Credit Courses.

Legislative Data Group (LDG)
How many LDGs are in your enterprise? You can create salary bases within a particular LDG. You can't share salary bases
across LDGs. Each salary basis name and each salary basis code must be unique within a legislative data group (LDG).

Frequency and Annualization Factor
How many different frequencies for quoting base pay are in use? People with multiple assignments on different payroll
frequencies need to have a different salary basis associated with each assignment.

Do any of the frequencies have multiple annualization factors for base pay? Your number of salary bases increases by
one for each extra annualization factor in each separate LDG.

Payroll Element and Currency
Do you want to use the same payroll element for different salary bases? You can do this if the element has these
configurations:

•

•

It's a recurring earnings element.

It allows multiple entries in the same period.

How many currencies do you pay people in, within a single LDG? You need one payroll element for each currency within
an LDG. You also need a separate salary basis for each payroll element.

Components
Do you want to itemize salary? You need one extra salary basis for each unique collection of components.

Grade Rates and Differential Profiles
How many grade rates are you using? The number of salary bases increases by one for each grade rate in use. You can
reduce the number of grade rates by using a differential profile. Profiles with the compensation zone or compensation
zone and business unit criteria can have grade rates configured instead of multipliers. The number of salary bases
increases by one for each differential profile in use.

86

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 11
Base Pay Overview

Rounding Rules and Decimal Precision
How many different rounding rules do you use for salary amount? The number of salary bases increases by one for
each rounding rule in use.

How many different decimal places do you display? The number of salary bases increases by one for each decimal
precision in use.

Related Topics
•

Incremental Salary Component Lookups

• How Salary Basis Options Work with Salary Amounts and Calculations

• Create a Payroll Element to Use with Salary Bases

• Grade Rates

How You Can Audit Salary Data

You need to enable audit for salary data using the Manage Audit Policies task.

Document Records for Salary

Proposers can attach document records while submitting salary proposals using responsive Change Salary and Salary
History actions. Approvers can view the attachments while deciding to approve or reject the proposal.

After approval, the attachments are available in the individual's document records. People can also see the attached
document records on the My Compensation and Compensation Info salary details pages.

Proposers can include document records of both Person and Assignment types. And actions tag document records with
the action occurrence identifier. Here's what happens to salary and the document record during certain scenarios, and
depending on your setup:

Scenario

What Happens

During global transfer that copies salary

• The Global Transfer action copies salary to the destination legal employer.

• The action moves the assignment-level document record. But it doesn’t link the document to the

copied salary.

When someone uses Change Salary to
correct a salary created with HR actions,
 such as Hire, Promote, and Local and
Global Transfer

When someone uses Change Salary to
correct a salary created with compensation
actions, such as Change Salary or Salary
History

• The action creates an action occurrence.

• The document of record created with the original transaction isn’t visible.

• The process doesn’t create an action occurrence.

• The document of record created with the original transaction is visible.

87

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 11
Base Pay Overview

Scenario

What Happens

When you've Reuse Action Occurrence
Identifier enabled

• Actions reuse the action occurrence when the effective date, action, and reason match that of the
assignment. The document of record created with the original transaction is visible and people
can’t delete it.

• Actions create an action occurrence when the effective date, action, and reason are different. The

document of record created with the original transaction isn’t visible.

When you've Combined Correction and
Deletion for Assignment, Salary, and
Document Records on View Employment
Details Page enabled

• Actions overwrite the action occurrence with the value selected by the proposer in the action. If

the proposer’s selection is different from that of the salary, then the document of record attached
to the salary isn’t visible.

Let Proposers Include Document Records in Salary
Proposals

Make the Document Records section visible so that proposers can include documents in their salary proposals. And
optionally filter the types of documents that they can include by action.

1. Make the Document Records section visible in these Transaction Design Studio rules:

◦ Change Salary
◦ Salary History
◦ My Compensation
◦ Compensation Info

2. Optionally, filter the document types by action. If you don’t do this filtering, proposers can add all document types
allowed by their document type security profiles. This filtering applies only when proposers add new document
records.
a.

In the Setup and Maintenance work area, search for and click the Manage Enterprise HCM Information
task.

b. Search for HCM Flow and Document Type Mapping.
c. Select the document types for these HCM flows:

- Change Salary for Line Manager
- Change Salary for Compensation Manager
- Salary History

88

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 12
Salary Basis Introduction

12  Salary Basis Introduction

Salary Basis Options for Determining Salary Amount

When you configure a salary basis, you need to specify whether it determines the salary amount by user, by incremental
components, by simple components, or by rate components.

Related Topics

• Salary Amount Is Determined by User

• Salary Amount Is Determined by Incremental Components

• Salary Amount Is Determined by Simple Components

• Salary Amount Is Determined by Rates

• FTE Adjustments When Salary Amount Is Determined by Simple Components

Salary Amount Is Determined by User

With this type of salary basis, HR specialists or managers enter salary amounts, adjustment amounts, or adjustment
percentages when changing salary. You can use this type to identify salary amounts using grade step progression.

Related Topics

• Basic Process to Default Salary Amounts from Grade Ladder Rates

Salary Amount Is Determined by Incremental
Components

With this type of salary basis, HCM specialists or managers itemize the salary adjustment using incremental
components provided by the basis. Or they select the components when changing salary. Which method they use
depends on the salary basis configuration.

CAUTION:  To identify salary amounts using grade step progression, don't select this type of salary basis.

Only the first salary record itemizes the entire salary amount. All later salary records itemize only the adjustment
amount, using percentages or amounts.

Example
On the first salary record, the HR specialist defines a 28,000 USD salary, as shown here.

89

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 12
Salary Basis Introduction

Component

Base

Merit

Location

Amount

20,000

5,000

3,000

The next year, the manager adjusts that person's salary to 32,000 USD, as shown here.

Component

Adjustment Amount

Adjustment Percentage

Base

Merit

Location

5,000

0

-1,000

Related Topics
•

Incremental Salary Component Lookups

18

0

-0.04

Salary Amount Is Determined by Simple Components

With this type of salary basis, HCM specialists or managers itemize salary changes using simple components. For
example, this $100 salary is made up of four itemizations.

90

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 12
Salary Basis Introduction

Each component has its own characteristic and change history, and affects salary in a different way. For example,
a component can be a fixed or user-enterable amount. Or it can be a fixed or user-enterable percentage of another
component. And you can add the component to the overall salary, subtract it from the overall salary, or make it
independent of the overall salary.

Tip:  You should use the simple components on responsive pages with salary information. Don't use classic pages to
create, change, or delete salary that uses simple components. You can use classic pages to view simple component
information.

Example
Here's a person's initial salary determined by three simple components and how their manager uses theses
components to adjust their salary a year later. On their first salary record, the HCM specialist defines their 25,000 USD
salary, as shown here.

Component

Base

Merit

Location

Amount

20,000

5,000

3,000

91

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 12
Salary Basis Introduction

The next year, their manager adjusts their salary to 32,000 USD, as shown here.

Component

Amount

Adjustment Amount

Adjustment Percentage

Prior Value

Base

Merit

Location

25,000

5,000

2,000

5,000

0

-1,000

25

0

-33.33

20,000

5,000

3,000

Related Topics

• Simple Salary Component Lookups

• Example Simple Component Configurations with People Entering Values and Fixed Percentages

• Example Simple Component Configurations with Grade Progression Rate, User Entered Values, and Fixed

Percentages

Salary Amount Is Determined by Rates

With this type of salary basis, HCM specialists or managers itemize the salary adjustment using Oracle Fusion Cloud
Global Payroll rate definitions. The overall salary is calculated by summing and subtracting other rates included in the
salary basis.

Rates can be entered by users or calculated by multiplying a factor against another rate value. They can also be derived
using value by criteria or the progression grade ladder. The rates included in the salary basis can have default values.
They can also have frequencies and currencies that are different from those for the overall salary.

CAUTION:  Don't include formula-based rate definitions and rate contributors in a salary basis. Also don't use
formulas for validation or to default values. Fast formula database items can't access data proposed in flows and not
yet saved to the database.

You create salary basis rate components using the payroll Rate Definitions quick action for My Client Groups. Be sure to
link a rate definition to only one salary basis to avoid issues when moving a worker to another basis.

Examples
Here, a person's overall salary is calculated by summing three other rate components. Two of the components have the
same frequency as the overall salary component, and one component has a different frequency.

Salary Component

Frequency

Component Value Source

Annual Base

Allowance 1

Annual

Annual

User entered

User entered

Incentive

Monthly

Defaulted from an element entry

Example

40,000

20,000

1,000

92

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 12
Salary Basis Introduction

Salary Component

Frequency

Component Value Source

Overall Salary

Annual

Calculated with this expression: Annual Base + Allowance 1 + (Incentive
x 12)

Example

72,000

40,000 + 20,000 + (1,000 x 12)

40,000 + 20,000 + 12,000

Here, a person's overall salary is calculated by summing two other rate components. Both components have the same
frequency as the overall salary component.

Salary Component

Frequency

Component Value Source

Annual Base

Annual

User entered

Housing Allowance

Annual

Calculated with workers at headquarters getting 50 percent of their annual base
and all others getting 40 percent

Example

40,000

20,000

Overall Salary

Annual

Calculated using this expression: Annual Base + Housing Allowance

60,000

40,000 + (40,000 x .50)

40,000 + 20,000

Here, a person's overall salary is calculated by summing four other rate components. One of the components has the
same frequency as the overall salary component, and the other three components have a different frequency.

Salary Component

Frequency

Component Value Source

Annual Base

Annual

User entered

Housing Allowance

Monthly

Calculated as 50 percent of monthly base

(Annual Base / 12) x .50

(48,000 / 12) x .50

4,000 x .50

Special Allowance

Monthly

Defaulted from an element entry

Variable Incentive

Monthly

Specified factor to apply to the Annual Base component, the calculated value is
loaded into an element entry

Example

48,000

2,000

1,000

1%

Overall Salary

Annual

Calculated with this expression: Annual Base + (Housing Allowance x 12)
+ (Special Allowance x 12) + (Variable Allowance x 12)

84,480

48,000 + (2,000 x 12) + (1,000 x 12) + (80,000 x .01)

48,000 + 24,000 + 12,000 + 480

93

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 12
Salary Basis Introduction

Rounding Rules, Salary Amounts, and Decimal Places to
Display

You can specify separate rounding rules for the salary amount, annualized values, and salary ranges on a salary basis.
You can also specify the decimal places to show for all numeric salary values that you see on the salary record.

Use the Salary Basis task in the Compensation Management work area.

Rounding Rules and Usages
Here's how amounts and ranges use each rounding rule.

Rounding Rule

Usage

Salary amount

Used by calculations that include the salary amount, for example:

• To increase a salary using a percentage, such as 3.5%

• To convert the salary to a different frequency, such as from monthly to annually

• To prorate the salary based on a specific full-time equivalent, such as from 1 FTE to 0.5 FTE

It’s also used when calculating simple component amounts from percentages or adjustment
percentages. The rounding rule doesn’t apply to the overall salary amount because it’s a sum of the
component amounts.

Annualized values

Specifies how the annual salary and annualized full-time salary amounts appear.

Salary range

Specifies how salary ranges appear and when calculating revised salary ranges, for example:

• To convert the salary range from one frequency to another

• To apply salary differentials

The rounding rules always affect amounts and values from when you set them and onward. They don't affect previously
calculated amounts and values. Here's how you can ensure consistency across historical and current salary amounts:

1. Create another salary basis with new rules instead of editing an existing salary basis.
2. Update the salary records with this new salary basis from a specific date.

You can use loading tools, such as HCM Data Loader and HCM Spreadsheet Data Loader to make this transition
seamless. Be sure to set the old salary basis to Inactive. This way it's no longer available for people to add it as part of
their salary proposals.

Rounding Rule Place and Decimal Place to Display
We recommend that you match the decimal place of your salary amount rounding rule with the decimal place to display.
Here's what happens when the decimal and rounding rule places don't match.

94

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 12
Salary Basis Introduction

Mismatch Issue

Example Scenario

Example Results

If the decimal place to display is longer than
your rounding rule place, salary amounts have
extra zeroes at the end.

Salary amount: 15.7923234

Decimal place to display: 4

Rounding rule: Nearest .01

Calculations round the amount to 15.79 and
salary pages display the amount as 15.7900.

If the decimal place to display is shorter than
your rounding rule place, salary amounts get
truncated.

Salary amount: 15.7923234

Decimal place to display: 2

Calculations round the amount to 15.7923 and
salary pages display the amount as 15.79.

Rounding rule: Nearest .0001

Payroll element entries ignore the decimal place to display from the salary basis because the elements always use the
decimal place of the currency definition. For example, US currency is defined to 2 decimal places. Even if you set your
salary amount display to 4 places, the element entries round the amount to 2 places.

Related Topics

• Overview of Base Pay Configuration

• Can HCM Data Loader round salary amounts when it loads salary information?

95

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 12
Salary Basis Introduction

96

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 13
Simple and Incremental Component Itemization of Salary

13  Simple and Incremental Component
Itemization of Salary

Considerations for Using Salary Bases with Incremental
Components versus Simple Components

When you configure salary bases, you can use incremental or simple components to itemize salary adjustments. The
incremental and simple components that you can configure come from lookups and their values can be either an
amount or a percentage.

Consider these key differences when selecting the salary basis type.

Criteria

Incremental Components

Simple Components

Source of component names

CMP_SALARY_COMPONENTS lookup

ORA_CMP_SIMPLE_SALARY_COMPS lookup

Component types

None

Input type

A Person can enter an amount or a percentage
against the incremental component.

Default value

None

User entered amount

User entered percentage

Fixed amount

Fixed percentage

Overall salary

Progression grade ladder rate

When allowed, a person can enter an amount
or a percentage. The percentage applies
to the amount of another, specified simple
component. A person can also enter the
adjustment amount or percentage to apply to
the previous simple component value.

You can configure the simple components to
use static default values or values provided by
progression grade ladder rates.

You can even configure the components to
use default values calculated by applying
percentages to other specific simple
components. For example, you can calculate a
car or housing allowance as a percentage of a
base salary.

Amount or percentage

Adjustment history

The adjustment applies to only the current
salary record.

Adjustments apply to the current and future
salary records.

Can be either

97

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 13
Simple and Incremental Component Itemization of Salary

Criteria

Incremental Components

Simple Components

Example scenario: In 2001 the worker gets a merit component of $100. In 2002, they get a $10
increase and in 2003, they get a $15 increase.

Results: Their salary history shows the
incremental merit component amount of $100
in 2001. It shows the adjustment amounts of
$10 in 2002 and $15 in 2003.

Their history doesn't show the calculated
amount of $110 in 2002 or $125 in 2003.

Results: Their salary history for the simple merit
component shows the amount of $100 in 2001,
 $110 in 2002, and $125 in 2003.

The history of a simple component is preserved
when the salary basis changes and both
bases use simple components of the same
component type.

Visibility of previous amount

None. People proposing or reviewing proposed
salary changes can’t see the previous amounts
or percentages.

People proposing and reviewing proposed
salary changes can see previous amounts or
percentages.

Effect of full-time equivalent (FTE)

None

Each value gets adjusted for FTE.

Effect on overall salary

The individual values are added to the previous
salary amount to decide the new overall salary.

You can specify whether the individual values
add to or subtract from the overall salary
amount. You can also configure individual
values to be independent of the overall salary.

Required or optional

You can configure a fixed set of incremental
components that always show when people
propose salary changes. Or, you can let them
select the incremental components they want
to use in their salary proposal, if any.

You specify whether they're optional. People
need to provide values for any required
simple components when they propose salary
changes. And, they can select the optional
components they want to include, if any.

Grade Step Progression
Consider these key differences when selecting the salary basis type of a salary basis used in grade step progression:

Criteria

Incremental Components

Simple Components

Populate salary from progression grade ladder

No

Yes when the simple component type is
Progression grade ladder rate

Grade step progression batch processes

Not available

Available

Integration
Consider these key integration differences when selecting the salary basis type:

Criteria

Incremental Components

Simple Components

Workforce Compensation

Total Compensation Statements

Oracle Transactional Business Intelligence
(OTBI) reports

Can include

Available

98

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 13
Simple and Incremental Component Itemization of Salary

Criteria

Incremental Components

Simple Components

Global Payroll

Supported flows

Approval payload

Available

HR actions, Offers, Change Salary, Salary History

Attributes available

Notifications shows component break up

GHR actions, Offers, Change Salary, Salary
History

Change Salary, Salary History

Also available in GHR data models

HCM Data Loader Salary Basis and Salary
Allocation objects

Supported

HCM Extracts

Global transfer

REST services

Download salaries

Database view

Audit

Autocomplete

User entities and database item groups available

Supported when you can let HCM specialists
and managers select the incremental
components to use in their salary proposal, if
any

Supported

Supported

Supported

Not supported

CMP_ASG_SALARY_COMPONENTS_V

CMP_ASG_SALARY_SIMPLE_CMPTS_V

Available

There's no new object available to set defaults for either incremental or simple component
values. You can default only the salary basis, not other attributes, such as component amounts or
percentages.

Related Topics

• Salary Amount Is Determined by Incremental Components

• Salary Amount Is Determined by Simple Components

Simple Component Types

You can include up to six different types of simple components in a salary basis configuration.

Type of Simple Component

Description

User entered amount

The person proposing salary can enter the amount.

User entered percentage

The person proposing salary can enter the percentage, which is then applied to the specified
component.

Fixed amount

The amount comes from the salary basis configuration and the person proposing salary can't override
it.

99

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 13
Simple and Incremental Component Itemization of Salary

Type of Simple Component

Description

Fixed percentage

Overall salary

The percentage comes from the salary basis configuration and the person proposing salary can't
override it. The percentage applies to the other, specified component.

The amount is calculated from the other component amounts that are configured to add to or subtract
from the overall salary. The person proposing salary can't override the amount.

Progression grade ladder rate

The amount comes from the progression grade ladder configuration. it can be either the grade rate
value or grade step rate value. The person proposing salary can overwrite the value.

Related Topics

• Create a Progression Grade Ladder to Default Salary Amounts

• Create a Progression Grade Ladder for Batch Processing

Optional Simple Components in Salary Bases

People proposing salary add or remove optional simple components in responsive flows using the Choose Components
menu. They’re included at the end of the salary details table instead of the position specified by the sequence set on the
salary basis.

The optional components do appear in the specified sequence when people view salary history.

HCM specialists and line managers all see the same optional components for the salary basis. If you need only HCM
specialists to add them, consider adding guidance on pages with salary information that discourages line managers
from adding them.

Tip:  You can't include simple components when you use classic Change Salary pages or Salary sections.

You've three options for the Optional attribute:

Option

No

Yes, don't carry forward

Yes, carry forward

Effect on the Simple Component

It's required and appears in all salary changes.

It’s optional and won't ever appear automatically when proposing or creating salary through scheduled
processes, HCM Data Loader, and HCM Spreadsheet Data Loader. The person proposing a salary
change needs to select the component to include it in their proposal. They need to do this for each
salary proposal, even if the current salary includes the optional component.

It’s optional and won’t automatically appear as a part of the first salary proposal. The person proposing
a salary change needs to select the component to include it in their proposal. After they include, it
continues to appear in future salary changes.

For example, the salary basis has car allowance set as an optional component to carry forward. A line
manager adds the car allowance to their worker’s salary change. All future salary proposals for that
worker continue to include the car allowance component until it’s explicitly removed.

100

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 13
Simple and Incremental Component Itemization of Salary

Example Simple Component Configurations with People
Entering Values and Fixed Percentages

Here are two examples of how you can configure simple components for people to enter amounts and percentages to
add to the overall salary. You can also include simple components that are fixed percentages and independent of the
overall salary.

Example 1
The first example has three simple components that add to an overall salary component. It also has two fixed
percentage components that are independent of the overall salary.

Component

Type

Component
Percentage Applies
To

Effect on Overall
Salary

Default Value

Example

Basic salary

User entered amount

NA

Housing

User entered
percentage

NA

Flexible benefit plan

User entered amount

NA

Annual gross pay

Overall salary

NA

Provident fund

Fixed percentage

Basic salary

Gratuity

Fixed percentage

Basic salary

Add

Add

Add

NA

None

None

NA

50%

NA

NA

12%

4.81%

100,000

50,000

60,000

210,000

12,000

4,810

Example 2
The second example also has three simple components that add to an overall salary component. And, it has three fixed
percentage components that are independent of the overall salary.

Component

Type

Component
Percentage Applies
To

Effect on Overall
Salary

Default Value

Example

Basic salary

User entered amount

NA

Housing

User entered
percentage

NA

Special allowance

User entered amount

NA

Annual gross pay

Overall salary

NA

Provident fund

Fixed percentage

Basic salary

Add

Add

Add

NA

None

NA

40%

NA

NA

12%

100,000

40,000

60,000

200,000

12,000

101

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 13
Simple and Incremental Component Itemization of Salary

Component

Type

Component
Percentage Applies
To

Effect on Overall
Salary

Default Value

Example

Gratuity

Fixed percentage

Basic salary

Variable pay

Fixed percentage

Overall salary

None

None

4.81%

20%

4,810

40,000

Related Topics

• Salary Amount Is Determined by Simple Components

Example Simple Component Configurations with Grade
Progression Rate, User Entered Values, and Fixed
Percentages

Here are two examples of how you can configure simple components that provide salary from rates in progression
grade ladders.

You can include simple components for people to enter amounts and percentages that also add to the overall salary.
And, you can include simple components that are fixed percentages that add to the overall salary or are independent of
it.

Example 1
The first example has five simple components that add to an overall salary component.

Component

Type

Component
Percentage Applies
To

Effect on Overall
Salary

Default Value

Example

Basic salary

Grade progression rate NA

Housing

Fixed percentage

NA

Flexible benefit plan

User entered amount

NA

Provident fund

Fixed percentage

Basic salary

Gratuity

User entered
percentage

Basic salary

Total cash

Overall salary

NA

Add

Add

Add

Add

Add

NA

NA

50%

NA

12%

5%

NA

100,000

50,000

60,000

7,200

5,000

222,200

Example 2
The second example also has five simple components that add to an overall salary component. And, it has a fixed
percentage component that's independent of the overall salary.

102

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 13
Simple and Incremental Component Itemization of Salary

Component

Type

Component
Percentage Applies
To

Effect on Overall
Salary

Default Value

Example

Basic salary

Grade progression rate NA

Housing

Fixed percentage

NA

Flexible benefit plan

User entered amount

NA

Provident fund

Fixed percentage

Basic salary

Gratuity

User entered
percentage

Basic salary

Total cash

Overall salary

NA

Variable pay

Fixed percentage

Basic salary

Add

Add

Add

Add

Add

NA

None

NA

50%

NA

12%

5%

NA

20%

100,000

50,000

60,000

7,200

5,000

222,200

44,440

Related Topics

• Salary Amount Is Determined by Simple Components

How You Migrate Salary Bases with Simple Components

You can use the standard import and export methods and the .csv or .xml files.

How You Enable Salary Itemization Using Incremental
Components

You can enable itemization that lets HR specialists and managers reflect the different reasons for salary changes, such
as merit or location. Use the Salary Basis task in the Compensation work area.

Incremental Component Configuration
Here are the key settings for the salary basis that let you include salary components for itemization.

Field

Value

Salary Basis Type

Salary adjustment amount is determined by incremental components.

Components to Display When Adjusting
Salary

Either of these:

• Select specific incremental components to display during allocation.

• Enable incremental component selection during allocation.

103

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 13
Simple and Incremental Component Itemization of Salary

You add incremental salary components or can change the available components by editing the
CMP_SALARY_COMPONENTS lookup type. Use the Manage Common Lookups task in the Compensation work area.

Incremental Component Processing
When values change for incremental salary components, the payroll element associated with the salary basis holds the
new salary amount calculated from the component adjustments. Payroll doesn't receive individual component values
for processing.

Example
The person's current salary is 50,000 USD. Their manager enters incremental component adjustment percentages and
salary calculations decide the monetary amounts, as shown here. The calculations then sum the monetary amounts and
the original salary amount to decide the new salary amount of 60,000 USD. Here's the equation:

(5,000 + 3,000 + 2,000 + 50,000)

Salary Component

Adjustment Percentage

Calculated USD

Merit

Promotion

Adjustment

10

6

4

Related Topics
•

Incremental Salary Component Lookups

5,000

3,000

2,000

104

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 14
Examples of How Simple Components Work

14  Examples of How Simple Components
Work

A New Hire Action with Simple Components

Here's an example of what happens in the salary section of a New Hire action when the selected salary basis type is
simple components.

1. You select the Simple Components Salary Basis (all required) salary basis and the required components appear

in the table.

2. The Basic salary component lets you enter an amount, such as 40,000.
3. The Housing allowance component lets you enter a percentage, such as 60%. Then it applies the percentage to

the Basic salary component amount to calculate the allowance amount, such as 24,000.

4. The Transport allowance component is a fixed amount, such as 1,800, that you can't remove or change.
5. The Special allowance component is a fixed percentage, such as 40% that you can’t remove or change. The

component applies the percentage to the Basic salary component to calculate the allowance amount.

105

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 14
Examples of How Simple Components Work

6. The Overall salary component adds all the other component amounts together to get the overall salary amount,

such as 81,800.

Related Topics

• Salary Amount Is Determined by Simple Components

A Change Salary Action and Simple Components

Here's an example of what happens in the salary section of a Change Salary action when the selected salary basis type
is simple components.

1. For the Basic salary component, you can enter an adjustment amount, such as 2,000, or a percentage, such as
5%. Then it calculates the adjustment percentage or amount and the proposed component amount, such as
42,000. Or you can directly enter the proposed amount and the component calculates the adjustment amount
and percentage.

106

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 14
Examples of How Simple Components Work

2. For the Housing allowance component, you can enter an adjustment amount, such as 1,620, or percentage,

such as 6.75%. Then it calculates the adjustment percentage or amount and the proposed component amount,
such as 25,620. Or you can directly enter the proposed amount and the component calculates the adjustment
amount and percentage.

3. The Transport allowance component is a fixed amount, such as 1,800, and you can't remove or change it.
4. For the Special allowance component, the adjusted percentage, such as 5%, is fixed and you can't change it.

The component calculates the adjustment amount, such as 800, and the proposed component amount, such
as 16,800.

5. The Overall salary component adds all the other component amounts together to get the overall salary amount,

such as 86,220.

Related Topics

• Salary Amount Is Determined by Simple Components

107

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 14
Examples of How Simple Components Work

The First Allocation and Next-Year Changes with Simple
Components

Here’s an example where you enter the salary information for a new hire and then change their salary a year later. This
salary information includes a salary basis with required simple components.

New Hire Action
While working through the New Hire action, in the Salary section, you select the Salary Required Components salary
basis, which includes required simple components. In the table that appears, you see all the required components and
any default values. You also see that you can enter a basic salary amount and adjust the default housing allowance
percentage. The travel and city allowance value are fixed, so you can’t remove or edit them.

The name of the other component appears below the percentage component name. For example, Housing allowance is
calculated as 50% of Basic salary component value. So below Housing allowance you Basic salary as a tip that housing
allowance is based on it.

Component Name

Percentage

Amount

Annual Amount

Annualized Full-Time
Amount

Basic salary

Housing allowance

(Basic salary)

Travel allowance

City allowance

(Basic salary)

Overall salary

NA

50

NA

10

NA

0

0

19,600

0

0

0

19,600

0

0

0

19,600

0

19,600

19,600

19,600

When you enter the basic salary amount of 50,000, the salary calculations automatically decide the other component
values.

Component Name

Percentage

Amount

Annual Amount

Annualized Full-Time
Amount

Basic salary

Housing allowance

(Basic salary)

NA

50

50,000

25,000

50,000

25,000

50,000

25,000

Travel allowance

NA

19,600

19,600

19,600

108

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 14
Examples of How Simple Components Work

Component Name

Percentage

Amount

Annual Amount

Annualized Full-Time
Amount

City allowance

10

5,000

5,000

5,000

(Basic salary)

Overall salary

NA

99,600

99,600

99,600

Change Salary Action
It's a year later and you want to change the person's salary. The Change Salary page shows the current salary details. In
the prior amount column, you see the current component amounts adjusted for frequency and FTE, if any.

Component Name Prior Amount

Adjustment
Amount

Adjustment
Percentage

Percentage

Amount

Annual Amount

Basic salary

50,000

Housing allowance

25,000

(Basic salary)

Travel allowance

19,600

City allowance

5,000

(Basic salary)

Overall salary

99,600

0

0

0

0

0

0

0

0

0

0

NA

0

NA

10

NA

50,000

25,000

19,600

5,000

50,000

25,000

19,600

5,000

99,600

99,600

You can use either the adjustment amount or adjustment percentage to calculate the new component amount. Or you
can directly enter the new component amount. Whichever way you make your changes, as you enter the values, other
values for that component get recalculated. And the other effected components with a higher process order also get
recalculated.

Component Name Prior Amount

Adjustment
Amount

Adjustment
Percentage

Percentage

Amount

Annual Amount

Basic salary

50,000

Housing allowance

25,000

(Basic salary)

Travel allowance

19,600

City allowance

5,000

(Basic salary)

5,000

5,250

400

500

10

21

2.04

10

NA

55

NA

10

55,000

30,250

20,000

5,500

55,000

20,250

20,000

5,500

109

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 14
Examples of How Simple Components Work

Component Name Prior Amount

Adjustment
Amount

Adjustment
Percentage

Percentage

Amount

Annual Amount

Overall salary

99,600

11,150

11.19

NA

110,750

110,750

Working Hours Change and Simple Components

When you change a person’s FTE (full-time equivalent) value, for example from 1 to .9, the prior component amounts
automatically adjust for the proposed FTE. This way you can do a direct comparison between current and proposed
amounts.

110

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 14
Examples of How Simple Components Work

111

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 14
Examples of How Simple Components Work

Salary Frequency Change and Simple Components

When you change from a salary basis with a monthly frequency to a salary basis with an annual frequency, the prior
component amounts adjust automatically.

The current monthly amounts get converted to prior annual amounts. And these annual amounts become the default
proposed amounts and annual amounts. This way values set for simple components of a salary basis configuration
carry forward to the simple components of another salary basis.

112

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 14
Examples of How Simple Components Work

113

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 14
Examples of How Simple Components Work

Component Type Changes and Simple Components

When you change from a salary basis with simple components to a salary basis that includes components of the same
name and type, the component values carry across the salaries. If the type changes, you don’t see a prior amount.

The salary bases in this example both have five simple components.

• Both bases include the Basic salary, Travel allowance, and Overall salary components and the components have

the same type.

• Both bases include the Housing allowance component. But the first basis has the user entering a percentage

while the second basis has the user entering an amount.

• Only the first basis includes a City allowance component.

• Only the second basis has a Variable allowance component.

• The first salary basis has an annual frequency and all five components are required.

• The second salary basis has a monthly frequency and three components are required while two components

are optional.

Annual Salary Basis with Five Required Components

Component

Type

Component
Percentage Applies
To

Affect on Overall
Salary

Optional

Default Value

Basic salary

User enters amount

NA

Housing allowance

User enters
percentage

Basic salary

Travel allowance

Fixed amount

NA

City allowance

Fixed percentage

Basic salary

Add

Add

Add

Add

Overall salary

Overall salary

NA

No effect

No

No

No

No

No

0

50

19,200

10

NA

Monthly Salary Basis with Three Required Components and Two Optional
Components

Component

Type

Component
Percentage Applies
To

Affect on Overall
Salary

Optional

Default Value

Basic salary

User enters amount

Housing allowance

User enters amount

Travel allowance

Fixed amount

NA

NA

NA

Add

Add

Add

No

No

Yes, don’t carry
forward

None

None

1,600

114

Oracle Fusion Cloud Human Resources
Implementing Compensation

Component

Type

Chapter 14
Examples of How Simple Components Work

Component
Percentage Applies
To

Affect on Overall
Salary

Optional

Default Value

Overall salary

Overall salary

Variable allowance

User enters amount

NA

NA

No effect

No effect

No

Yes, don’t carry
forward

NA

0

You start proposing a salary change and select the second salary basis. You can see that only the prior Basic salary
amount adjusted for the new frequency, from 50,000 to 4,166.67. Even though the Housing allowance exists in the
second salary basis, you don't see a prior amount because the component types are different.

Next, you include the optional components, which appear in the last rows of the table, below the Overall salary
component. You can see that the prior Travel allowance amount automatically adjusted from 19,200 to 1,600 because of
the new frequency.

115

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 14
Examples of How Simple Components Work

116

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 15
Rates-Based Component Itemization of Salary

15  Rates-Based Component Itemization of
Salary

Comparison of Rate Component Categories for Salary
Bases

When you determine the salary amount using rates, you can use Element, Derived, Grade Rate, and Value by Criteria
rate definitions. These definitions are the multiple components of pay that make up the salary amount.

We don't recommend using other rate categories, such as Formula, because of possible performance issues and data
access constraints.

As shown here, Element rates use payroll element input values of either amount or factor. Value by Criteria rate
definitions use Value by Criteria definitions. And Derived rates can use Element, Grade Rate, and Value by Criteria rates
as rate contributors.

117

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 15
Rates-Based Component Itemization of Salary

This table identifies key properties and whether they're allowed or required (Y) or not allowed or required (N).

Property

Element Rate
Definitions

Derived Rate
Definitions

Overall Salary Rate
Definitions

Grade Rate Rate
Definitions

Value by Criteria Rate
Definitions

Y

Y

Y

Y

Need to associate a
payroll element

User can enter or
override the value

Store the rate value in
an element entry

After final salary
approval, calculate
salary component
values and store them
in the CMP_SALARY_
PAY_COMPONENTS
table

Rate provides a default
value

Y

Rate can be a base rate Y

Rate can be an overall
salary

Y

N

N

N

Y

N

Y

Y

Y

N

N

Y

N

Y

NAW

N

N

N

Y

Y

Y

N

N

N

N

Y

N

N

N

Element Rate Components in a Salary Basis

Use Element rate definitions in a salary basis to get a default value from element entries. Or use them to let the person
allocating salary enter a flat amount or factor as an input value for a payroll element.

For example, you create a rate definition that uses the Incentive element. If the incentive is stored as a monetary value,
select Amount. If the incentive is a factor of another value, such as another rate definition, select Factor.

You need to create the payroll element with a calculation type of Flat amount or Factor before you can use it in an
Element rate definition. Choosing Amount in the rate definition automatically defines the contributor. You must define
the contributor when choosing Factor. The factor is used to calculate the rate amount, which can be included in the
overall salary amount. For both rate definitions, you need to select the corresponding calculation rule. For element rates
of Amount, select Flat amount. For element rates of Factor, select Factor.

CAUTION:  Link a payroll element to only one rate. Linking the element to multiple rates can cause issues, such
as when a worker moves to another salary basis. Also be sure to select the Override Allowed option for the rate
definition. This way people allocating salary can enter an amount or a factor.

To create rate definitions, go to My Client Groups > Compensation > Rate Definitions. Be sure to link a rate definition
to only one salary basis to avoid issues when moving a worker to another basis.

118

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 15
Rates-Based Component Itemization of Salary

Derived Rate Components in a Salary Basis

Use Derived rate definitions in a salary basis to get a calculated rate by adding or subtracting one or more rates, or rate
contributors.

Derived rate definitions can get values from one or more other rate definitions, including rates that get element entry
values. For example, you can add regular salary, car allowance, and incentive pay rate contributors together to create
an overall salary rate definition. When creating a derived rate definition, you add the relevant contributors and specify
whether to add or subtract each contributor when calculating the derived rate value.

To create rate definitions, go to My Client Groups > Compensation > Rate Definitions. Be sure to link a rate definition
to only one salary basis to avoid issues when moving a worker to another basis.

Grade Rate Rate Components in a Salary Basis

Use Grade Rate rate definitions in a salary basis to get the rate value for the grade or grade and step value of the
person's work assignment.

The grade or grade and step can come directly from the assignment progression ladder or from the retained pay
extensible flexfield (EFF) associated with the assignment. For example, you've the Consultants grade ladder with these
grades, steps, and rate values:

Grade

G1

G1

G2

Step

S1

S2

S1

Rate Value

11

12

21

One worker's salary basis has the rate contributor as a grade ladder, and their work assignment has the grade G1 and
step S1, so their rate is 11. Another worker's salary basis has the rate contributor as a retained pay EFF. And the retained
pay EFF for their work assignment has the grade G2 and step S1, so their rate is 21.

To create rate definitions, go to My Client Groups > Compensation > Rate Definitions. Be sure to link a rate definition
to only one salary basis to avoid issues when moving a worker to another basis.

Value by Criteria Rate Components in a Salary Basis

Use Value by Criteria rate definitions in a salary basis to get a value from an Oracle Fusion Cloud Global Payroll value by
criteria definition.

119

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 15
Rates-Based Component Itemization of Salary

You decide the criteria to enter and the resulting tree structure. In each branch of the tree, you can have multiple
evaluation conditions and the value to return. You can also define a default value, for criteria that doesn't meet the
conditions, or to define minimum and maximum thresholds.

For example, you can calculate allowance for workers based on their job.

•

•

•

If the worker is a Consultant, pay them 45,000 USD.

If the worker is a Senior Consultant, pay them 55,000 USD.

If the worker is a Principal Consultant, pay them 65,000 USD.

• Otherwise, pay them 35,000 USD

Or you create a value by criteria definition that returns a flat amount based on the worker's location. You use that
definition in a Value by Criteria rate, and include that rate as a contributor to a derived rate definition.

To create rate definitions, go to My Client Groups > Compensation > Rate Definitions. Be sure to link a rate definition
to only one salary basis to avoid issues when moving a worker to another basis.

Related Topics

• Overview of Values Defined by Criteria

• Calculate Values Defined by Criteria

• Calculate a Rate Using Multiple Values Defined by Criteria

• Rates Based on Values Defined by Criteria

• Allowance Setup Using Rate Definition and Value By Criteria for Qatar

Database Items That Can Detect Proposed Info in Salary
Value by Criteria Rate Definitions

You can detect proposed information and calculate rate values in various flows, such as Hire an Employee, and Local
and Global Transfer, when using these special database items in Value by Criteria rate definitions.

Other database items won’t detect the proposed information and will thus calculate rate values based on information in
the database tables.

Attribute Name

Database Item Name

Comments

Business Unit

Location

Legal Employer

Department

PER_ASG_BUSINESS_UNIT_ID

PER_ASG_LOCATION_NAME

PER_ASG_ORG_LEGAL_EMPLOYER_NAME

PER_ASG_ORG_DEPARTMENT_NAME

Worker Category

PER_ASG_EMPLOYEE_CATEGORY_MEANING

Period of Service (seniority)

PER_ASG_REL_LENGTH_OF_SERVICE

PER_ASG_EMPLOYMENT_CATEGORY_
MEANING

120

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 15
Rates-Based Component Itemization of Salary

Attribute Name

Database Item Name

Comments

Legal Employer Level Seniority Date

PER_ASG_REL_ADJUSTED_SVC_DATE.

Returns seniority date in a legal employer
(relationship seniority date).

Enterprise Seniority Date

PAYROLL_INTERFACE_ORIGINAL_DATE_OF_
HIRE

Returns first original date of hire regardless of
legal employer.

Legal Employer Level Hire Date

PER_ASG_REL_ORIGINAL_DATE_OF_HIRE

Returns relationship original date of hire.

Enterprise Hire Date

PER_PERSON_ENTERPRISE_HIRE_DATE

Returns earliest relationship start date, which is
the first hire date regardless of legal employer.

Number of Child Dependents

PER_PER_CONTACT_DEPEN_CHILD_COUNT

PER_PER_CONTACT_DEPEN_CHILD_COUNT_
LOC

Assignment Number

PER_ASG_ASSIGNMENT_NUMBER

Assignment ID

PER_ASG_ASSIGNMENT_ID

Assignment Start Date

PER_ASG_EFFECTIVE_START_DATE

Job

Job Code

Job Family

Business Unit

Location

Department

Legal Entity

Normal Hours

PER_ASG_JOB_ID

PER_ASG_JOB_NAME

PER_ASG_JOB_CODE

PER_JOB_FAMILY_ID

PER_JOB_FAMILY_NAME

PER_ASG_BUSINESS_UNIT_NAME

PER_ASG_LOCATION_ID

PER_ASG_DEPARTMENT_ID

PER_ASG_LEGAL_ENTITY_ID

PER_ASG_NORMAL_HOURS

Assignment Category

PER_ASG_EMPLOYEE_CATEGORY

Legal Employer

Assignment Flex

Grade Flex

Grade Code

Grade

Grade Ladder

Grade Step

Location Flex

PER_ASG_EMPLOYMENT_CATEGORY

PER_ASG_ORG_LEGAL_EMPLOYER_NAME

PER_ASG_DF

PER_GRADES_DF

PER_ASG_GRADE_CODE

PER_ASG_GRADE_ID

PER_ASG_GRADE_LADDER_PGM_ID

PER_GRADE_STEP_NAME

Descriptive flexfield.

Descriptive flexfield.

PER_LOCATIONS_DF

Descriptive flexfield.

121

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 15
Rates-Based Component Itemization of Salary

Attribute Name

Database Item Name

Comments

Grade

Salary Basis

Action

Reason

PER_ASG_GRADE_NAME

CMP_ASSIGNMENT_SALARY_BASIS_NAME

PER_ASG_ACTION_CODE

PER_ASG_ACTION_REASON_CODE

Works in only flows that have both employment
and salary sections included. Won’t work in the
standalone Change Salary flow

Important Value by Criteria Settings for Rate
Components in Salary Bases

Here are some important naming conventions and selections to follow when creating value by criteria definitions to use
in salary bases with rate components.

• A value definition is required to create a Value by Criteria definition, but rates-based salaries ignore the value

definition. You can select any existing value definition or create your own.

• The Criteria and Value names need to be unique for the selected legislative data group.

• To return an amount, in the Unit of Measure field, select Money. Also select the relevant Periodicity and

Currency values.

• To return a factor, in the Unit of Measure field, select Number.

Related Topics

• Overview of Values Defined by Criteria

Run Salary Processes

Salaries can change because of changes to the salary structure or worker attributes. Use the Run Salary Processes and
Review Proposed Salary Changes and Rate Values tasks to handle these changes.

Tip:  The Run Salary Processes process doesn’t affect candidates and pending worker salaries.

When you submit the Run Salary Processes process, you specify whether to create salaries or correct salary records, by
recalculating rate values. You use population filters to identify the workers and salary assignments the process should
check. Use the run type to specify whether to commit the new or corrected salaries to the CMP salary, CMP rate values,
and PAY EE tables. Or you can specify to wait for review.

When it runs, the process calculates what the rate values will be on the effective date and compares the results with
CMP table values to identify salary changes. It creates salary proposals and details. For example, the process identifies
whether the proposal is for a new salary or a correction and includes the salary amount, rate values, action, and reason.
If you specified to wait for review, you review the Run Rates-based Process results using the Review Proposed Salary
Changes and Rate Values task.

122

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 15
Rates-Based Component Itemization of Salary

For example, the salary for a group of workers has two components. One component is a user-entered annual base
amount, the other is a derived rate that's 50% of the annual base for people working at headquarters. Changes
to compensation policy for this group require changes to the relevant salary basis rate component. Workers at
headquarters need to get a derived rate that's 60% of the annual base. Here's how you'd configure the processed
depending on whether you want to change or correct salary.

Parameter

Change

Correct

Process Mode

Create another salary by recalculating rate

Correct salary by recalculating rate values

values

Effective Date

Run Type

January 1 of next year

Start date of the salary basis

Calculate salary values and wait for review

Calculate salary values and wait for review

Population Filter

Select the relevant salary basis

Select the relevant salary basis

Here's a flow diagram of Run Salary Processes.

The Run Salary Processes and Review Proposed Salary Changes and Rate Values tasks are available on the My Client
Groups > Compensation page.

Improve Performance
By default, the Run Salary Processes process has 3 threads with chunk sizes of 20. You can increase the total threads
and check performance until you reach the best total for your volume.

1. Go to My Client Groups > Compensation > Configure Compensation Batch Parameters.
2. Change the Run Salary Processes total threads count.

123

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 15
Rates-Based Component Itemization of Salary

3. Save your changes and close the page.
4. Test performance.
5. Repeat until you reach the best performance for your volume.

Note:  Changes to the total threads for this parameter also affect the Generate Compensation Zone and Address
Mapping process.

Considerations for Using Salary Bases with Simple
Components versus Rate Components

When you configure salary bases, you can use simple or rate components to itemize salary adjustments.

The simple components that you can configure come from lookups and their values can be either an amount or a
percentage. The rate components come from rate definitions and can be element, derived, grade rate, or value by
criteria rates.

Consider these key differences when selecting the salary basis type.

Criteria

Simple Components

Level of configuration effort

Simple

Simple to medium

Supported requirement
complexity

Component creation

Rate Components

Medium to complex

Medium to complex

ORA_CMP_SIMPLE_SALARY_COMPS lookup type that shows
on salary bases in component drop-down lists

Rate definitions that show on salary bases in
component drop-down lists

Component types

User entered amount

User entered percentage

Fixed amount

Fixed percentage

Progression grade ladder based

Overall salary

Element amount rate

Element factor rate

Value defined by criteria rate

Derived rate

Grade rate

Retained pay

Element entry creation for salary Element created for the overall salary component, with the

Element created for the overall salary rate

provided value

Correct or update existing
salaries when component
calculation logic changes

Post salary change proposals
automatically

No

No

Value isn't stored for the element created for
the overall salary

Yes, use the Run Salary Processes process

Yes, use the Run Salary Processes process

124

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 15
Rates-Based Component Itemization of Salary

Criteria

Simple Components

Rate Components

Wait for salary change proposal
reviews before posting

Enter or fix components

Values can be amount or
percentage

Calculated value can be
overridden

Default component

No

Yes

Yes

No

No

Default component using logic

No, you can default only a fixed value

Calculate component value
based on other attributes, such
as grade or location

No

Include components that don't
affect overall salary

Yes

Component calculations can
include other component values

Limited

Define valid component value
ranges

No

Components can be optional

Yes, you can carry forward an optional component for all later
changes or applicable for just the single proposal

Accept overall salary and
distribute that into other
components

No

(India basket of allowance sort of
requirements)

FTE won't affect the component
value

No

Define rounding rules per
component

Define decimal display per
component

No, only at the salary-basis level

No, only at the salary-basis level

Vary currency or frequency per
component

No

Where frequency is configured

Salary basis

Can make date-effective
changes to components

No

Can add or remove components
for a salary basis that's in use

Not recommended

Yes, use the Run Salary Processes process

Yes

Yes

No

No

Yes, using value by criteria or another rate
definition

Yes, see Database Items That Can Detect
Proposed Info in Salary Value by Criteria Rate
Definitions

Yes, you still need to add these rates to the
overall salary rate definition and deduct them

Yes

Yes

No

Yes

Configurable

Yes

Yes

Yes

Overall salary rate definition using a custom
periodicity fast formula

Yes, but not recommended

Not recommended

125

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 15
Rates-Based Component Itemization of Salary

Criteria

Simple Components

Rate Components

Can use in offers and workforce
compensation

Grade step progression
processes can change salary

Database items for use in
other HCM products, including
Global Payroll and Workforce
Compensation. You can also
use them in HCM extracts for
external interfaces

Yes

Yes

Yes

No

Yes, ORA_CMP_ASSIGNMENT_SALARY_SIMPLE_
COMPONENT_UE and ORA_CMP_ASSIGNMENT_SALARY_
SIMPLE_COMPONENT_RGE_UE

Yes, ORA_CMP_ASSIGNMENT_SALARY_
RATES_UE and ORA_CMP_ASSIGNMENT_
SALARY_RATES_RGE_UE

Database view

CMP_ASG_SALARY_SIMPLE_CMPTS_V

CMP_ASG_SALARY_RATE_COMPTS_V

Supports REST, HCM Data
Loader, and HCM Spreadsheet
Data Loader

Yes

Limitations

Lookup tags aren't considered; all components configured for
the salary basis show when proposing salary

Can use the Salary History
action

Yes

Yes

See the limitations section, for example, a
rates-based salary needs to have all future
salary bases also be rates-based

No

126

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 16
Rate Component Attributes for Salary Bases

16  Rate Component Attributes for Salary
Bases

Base Rate Attribute for Salary Basis Rate Components

Select the Base Rate rate component attribute if other rates in the salary basis base their calculations on this rate.

For example, your day shift and night shift workers have different base pay rates. You provide each set of workers
different allowances, which are a percentage of the base rate.

1. You create two salary bases, one for night shift and one for day shift, and add the appropriate base rates to

each salary basis.

2. You add the same allowance rate to each salary basis. The allowance rate will use the base rate in it's salary

basis to calculate the allowance amount.

You can add a base rate contributor without needing to explicitly identify the contributing rate. This flexibility lets
you define multiple base rates for different worker groups and a subset of other rates that use the base rate in their
calculations.

Overall Salary Attribute for Salary Basis Rate
Components

Select the Overall Salary rate component attribute if the rate represents an overall salary rate to use in the salary basis.
The overall salary is calculated by summing and subtracting other rates included in the salary basis.

Rates-based salary bases need to have an overall salary rate to get certain salary basis attributes. For example, the
periodicity of the overall salary rate sets the salary basis frequency. The overall salary rate also calculates the overall
salary amount used in the Change Salary task.

Periodicity Attribute for Salary Basis Rate Components

You need to specify a periodicity, such as Hourly or Weekly, for the returned rate and each rate contributor used in
salary basis rate components. The overall salary rate definition periodicity is the rate component frequency for the
salary basis.

Derived rate calculations use the periodicity of the rate contributors to appropriately convert contributor values and
derive the rate value when not all periodicities are the same. Typically, the derived rate and associated rate contributors
all have the same periodicity--and frequency.

127

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 16
Rate Component Attributes for Salary Bases

Default Value Attribute for Salary Basis Rate Components

You can default values for element rates by specifying a specific value or selecting a value by criteria definition. When
you select a value by criteria definition, the definition needs to return a number.

FTE Attribute for Salary Basis Rate Components

You can have a rate definition consider the full-time equivalent when calculating the value by selecting the FTE option.

We recommend that you don't select this option because salary ranges, compa-ratio, and other salary metrics are
already adjusted for FTE. Adjusting individual rates for FTE might result in inaccurate salary values.

Factor Attribute for Salary Basis Rate Components

You can set a factor in the rate definition. When you use a factor, the rate amount is calculated by multiplying the rate
contributor or the rate value by the factor.

For example, one rate definition for a salary basis is a monthly Variable Incentive that's 1% of the Annual Base rate
definition. So the factor of the incentive rate definition is .01.

Periodicity Conversion Formula Attribute for Salary Basis
Rate Components

You can control the annualization factor by specifying a periodicity conversion fast formula.

Here's what to do if you need an annualization factor not available in the delivered formula:

1. Create a formula by copying the text from a delivered conversion formula.

2.

In the copy, make the input and output parameter names the same.

3. Save, compile, and use the copy fast formula in the rate definition.

Note:  The Hourly rate periodicity differs from the Work Hour compensation annualization factor. The Hourly
periodicity is 2920 while the Work Hour annualization factor is 2080.

128

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 17
Example Rate Definition Configurations for a Salary Basis

17  Example Rate Definition Configurations for
a Salary Basis

Overview of Example Rate Definitions for a Salary Basis

The topics in this chapter show you examples of how to set up five different types of rate definitions for a salary basis.

The definitions will be for a base salary, an allowance, a short-term incentive plan, a grade-based performance award,
and an overall salary. Users will enter values for the base salary and short-term incentive plan rate components. The
values for the other three rate components are calculated and can't be overridden.

Create a Base Salary Rate Definition

Users enter the base salary rate value while allocating salary. The rate contributes to the overall salary rate (also known
as total target compensation) and is used to calculate the short-term incentive plan amount.

1. Create the payroll element, US Base Salary in this example, using the Standard Earnings template, the Flat amount
calculation rule, and an Annually periodicity. We recommend that you configure the element eligibility as open. For
more details about creating compensation payroll elements, see Create a Payroll Element to Use with Salary Bases.

2. Go to My Client Groups > Compensation > Rates Definition.

3. Create a rate definition.

4. On the Create Rate Definition dialog box, complete the required fields, as shown by these example values:

Field

Category

Effective Start Date

Legislative Data Group field

Storage Type

Value

Element

1/1/00

US LDG

Amount

The calculation rate contributor is automatically defined for this storage type.

Element

US Base Salary

 such as when a worker moves to another salary basis.

◦ Link a payroll element to only one rate. Linking the element to multiple rates can cause issues,
◦ The element name becomes the default rate definition name and short name, which you can

overwrite as appropriate.

5. Click OK.

6. On the Create Rate Definition page, in the Basic Details section, select the Base Rate checkbox.

7.

In the Returned Rate Details section, confirm that the Periodicity value is Annually.

129

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 17
Example Rate Definition Configurations for a Salary Basis

8. Click the Override and Defaulting Rules tab.

9. Select the Override Allowed checkbox so that people allocating salary can enter an amount.
10. Click Submit.

Related Topics

• Element Rate Components in a Salary Basis

Create an Allowance Rate Definition for a Salary Basis

Users enter the allowance rate value while allocating salary. The rate contributes to the overall salary rate (also know as
total target compensation).

1. Create the payroll element, US Allowance in this example, using the Standard Earnings template, the Flat amount

calculation rule, and a Calendar Month periodicity. We recommend that you configure the element eligibility as open.
For more details about creating compensation payroll elements, see Create a Payroll Element to Use with Salary
Bases.

2. Go to My Client Groups > Compensation > Rates Definition.

3. Create a rate definition.

4. On the Create Rate Definition dialog box, complete the fields, as shown by these example values:

Field

Category

Effective Start Date

Legislative Data Group field

Storage Type

Value

Element

1/1/00

US LDG

Amount

The calculation rate contributor is automatically defined for this storage type.

Element

US Allowance

 such as when a worker moves to another salary basis.

◦ Link a payroll element to only one rate. Linking the element to multiple rates can cause issues,
◦ The element name becomes the default rate definition name and short name, which you can

overwrite as appropriate.

5. Click OK.

6. On the Create Rate Definition page, in the Returned Rate Details section, confirm that the Periodicity value is

Calendar Month.

7. Click the Override and Defaulting Rules tab.

8. Select the Override Allowed check box so that people allocating salary can enter an amount.
9. Click Submit.

130

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 17
Example Rate Definition Configurations for a Salary Basis

Create a Short-Term Incentive Plan Rate Definition for a
Salary Basis

Users enter the short-term incentive plan rate percentage value while allocating salary. It's stored in an element entry
and the corresponding amount is calculated immediately. The plan rate contributes to the overall salary rate, also known
as total target compensation.

1. Create the US STIP payroll element using the Standard Earnings template, the Factor calculation rule, and an

Annually periodicity. We recommend that you configure the element eligibility as open. For more details about
creating compensation payroll elements, see Create a Payroll Element to Use with Salary Bases.

2. Go to My Client Groups > Compensation > Rates Definition.

3. Create a rate definition.

4. On the Create Rate Definition dialog box, complete the required fields as shown here:

Field

Category

Effective Start Date

Legislative Data Group field

Storage Type

Value

Element

1/1/00

US LDG

Factor

You'll need to define the calculation rate contributor for this storage type.

Element

US Short-Term Incentive Plan

 such as when a worker moves to another salary basis.

◦ Link a payroll element to only one rate. Linking the element to multiple rates can cause issues,
◦ The element name becomes the default rate definition name and short name, which you can

overwrite as appropriate.

5. Click OK.

6. On the Create Rate Definition page, in the Returned Rate Details section, confirm that the Periodicity value is

Annually.

7.

In the Calculation Details section, click the Add icon.

8. On the Create Rate Contributor dialog box, select Base Rate.

9. On the Create Rate Contributor page, in the Periodicity field, select Annually.

10. Click Save and Continue.

11. Click the Override and Defaulting Rules tab.

12. Select the Override Allowed checkbox so that people allocating salary can enter an amount.

13. Click Submit.

131

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 17
Example Rate Definition Configurations for a Salary Basis

Create a Grade-Based Value by Criteria Definition for a
Salary Basis Rate Definition

The grade-based performance award rate value identifies hourly workers with a grade of M1, M2, or M3 using value by
criteria conditions.

1. Go to My Client Groups > Compensation > Values Defined by Criteria.

2. Create the Hourly Staff Performance Award value definition.

a. On the Criteria and Values toolbar, click the Create icon.
b. On the Create Values Defined by Criteria dialog box, complete the fields, as shown by these example values.

Field

Name

Value

Grade-Based Performance Award

Effective Start Date

Legislative Data Group

1/1/00

US LDG

Use existing range group

Select

Value Definition Group

Any value, such as Workers Compensation

c. Click OK.

3. On the Create Values Defined by Criteria: Grade-Based Performance Award page, configure the value definition

criteria.

a. Select the Grade-Based Performance Award row.
b. On the toolbar, click the New icon.
c. On the Create Calculation Value Definition dialog box, select Criteria.
d. Click OK.
e. On the Create Criteria dialog box, complete the fields, as shown by these example values.

Field

Value

Calculation Value Definition Name

Pay Frequency

Value Definition Group

Any value, such as Performance Award

Retrieval Date

Effective Date

Sequence

1

Database Item Name

PER_ASG_HOURLY_SALARIED_CODE

Display Name

Pay Frequency

132

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 17
Example Rate Definition Configurations for a Salary Basis

Field

Operand

Literal Value

f. Click OK.

Value

=

H

4. On the Create Values Defined by Criteria: Grade-Based Performance Award page, create the M1, M2, and M3 criteria

In the Criteria and Values table, expand the Grade-Based Performance Award row.

definitions.
a.
b. Select the Pay Frequency = H row.
c. On the toolbar, click the New icon.
d. On the Create Calculation Value Definition dialog box, select Criteria.
e. Click OK.
f. On the Create Criteria dialog box, complete the fields, as shown by these example values.

Field

M1

M2

M3

Calculation Value Definition

Grade = M1

Grade = M2

Grade = M3

Name

Value Definition Group

Any value, such as

Performance Award

Any value, such as

Performance Award

Any value, such as

Performance Award

Retrieval Date

Effective Date

Effective Date

Effective Date

Sequence

1

2

3

Database Item Name

PER_ASG_GRADE_NAME

PER_ASG_GRADE_NAME

PER_ASG_GRADE_NAME

Display Name

Grade

Operand

Literal Value

=

M1

Grade

=

M1

Grade

=

M1

g. Click OK. Repeat these steps twice, to add the M2 and M3 calculation value criteria.

133

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 17
Example Rate Definition Configurations for a Salary Basis

5. On the Create Values Defined by Criteria: Grade-Based Performance Award page, create the M1, M2, and M3 value

In the Criteria and Values table, expand the Grade-Based Performance Award row.

definitions.
a.
b. Select the Grade = M1, M2, or M3 row.
c. On the toolbar, click the New icon.
d. On the Create Calculation Value Definition dialog box, select Value.
e. Click OK.
f. On the Create Value dialog box, complete the fields, as shown by these example values.

Field

Value

Calculation Value Definition

M1

Name

M2

M2

M3

M3

Value Definition Group

Any value, such as Workers

Any value, such as Workers

Any value, such as Workers

Compensation

Compensation

Compensation

Retrieval Date

Effective Date

Effective Date

Effective Date

Calculation Type

Flat Amount

Flat Amount

Flat Amount

Periodicity

Annually

Unit of Measure

Money

Currency

Flat Amount

USD

700

Annually

Money

USD

750

Annually

Money

USD

800

g. Click OK. Repeat these steps twice, to add the M2 and M3 calculation value definitions.

6. On the Create Values Defined by Criteria: Grade-Based Performance Award page, create the default criteria.

a. Select the Grade-Based Performance Award row.
b. On the toolbar, click the New icon.
c. On the Create Calculation Value Definition dialog box, select Criteria.
d. Click OK.
e. On the Create Criteria dialog box, complete the fields, as shown by these example values.

Field

Value

Calculation Value Definition Name

Default Condition

Value Definition Group

Any value, such as Workers Compensation

Retrieval Date

Effective Date

Default Criteria

Select

f. Click OK.

7. On the Create Values Defined by Criteria: Grade-Based Performance Award page, review your value definition.

8. When you're ready, click Submit.

134

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 17
Example Rate Definition Configurations for a Salary Basis

9. Click Done.

Create a Grade-Based Performance Award Rate
Definition for a Salary Basis

The grade-based performance award rate value identifies hourly workers with the M1, M2, or M3 grades using value by
criteria conditions.

1. Create the values defined by criteria definition, Grade-Based Performance Award in this example.

2. Go to My Client Groups > Compensation > Rates Definition.

3. On the Rate Definitions page, click the Create icon.

4. On the Create Rate Definition dialog box, complete the required fields, as shown by these example values:

Field

Category

Effective Start Date

Legislative Data Group field

5. Click OK.

Value

Value by Criteria

1/1/00

US LDG

6. On the Create Rate Definition page, enter a short name, such as Grade Perf Award Hrly.

7.

In the Value by Criteria Name field, search for and select the value definition, such as Grade-Based Performance
Award.

8. Select the Reporting Required option, if it's not already selected.

9. Click Submit.

Create an Overall Salary Rate Definition for a Salary Basis

The overall salary rate definition is derived from other rate definitions. In this example, the overall salary is derived from
the base salary, allowance, short-term incentive, and performance award rate definitions.

1. Create the payroll element, US Overall Salary in this example, using the Standard Earnings template, the Flat amount

calculation rule, and an Annually periodicity.

On the Element Summary: US Overall Salary page, in the Standard Rates section, make sure that the Process in
payroll run option isn't selected. Or, you can make sure that Process in payroll run isn't selected for the elements
of any rate contributors, and is selected for the overall salary element. We also recommend that you configure the
element eligibility as open.

135

Chapter 17
Example Rate Definition Configurations for a Salary Basis

Oracle Fusion Cloud Human Resources
Implementing Compensation

2. Create these rate definitions:
◦ Base salary
◦ Allowance
◦ Short-term incentive
◦ Performance award

3. Go to My Client Groups > Compensation > Rates Definition.

4. On the Rate Definitions page, click the Create icon.

5. On the Create Rate Definition dialog box, complete the required fields, as shown by these example values:

Field

Category

Effective Start Date

Legislative Data Group field

6. Click OK.

Value

Derived Rate

1/1/00

US LDG

7. On the Create Rate Definition page, complete the basic fields, as shown by these example values:

Field

Name

Short Name

Element Name

Value

Overall Salary

OVERALL SALARY

US Overall Salary

You need to associate a payroll element with this rate to store the amount in an element entry.

Overall Salary

Select

This amount appears on pages and in work flows containing salary information, and it's used to
calculate salary metrics, such as compa-ratio.

Reporting Required

Select

8. In the Rate Contributors section, added the base salary rate definition.

a. On the toolbar, click the Create icon.
b. On the Create Rate Contributor dialog box, in the Contributor Type field, select Base Rate.
c. On the Create Rate Contributor page, in the Employment Level field, select Payroll Assignment.
d. Click Save and Continue.

136

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 17
Example Rate Definition Configurations for a Salary Basis

9.

In the Rate Contributors section, add the allowance, short-term incentive, and performance award rate definitions.

a. On the toolbar, click the Create icon.
b. On the Create Rate Contributor dialog box, in the Contributor Type field, select Rate Definition.
c. On the Create Rate Contributor page, in the Rate Name field, select the appropriate rate definition.
d. Confirm that the periodicity is correct.
e. Click Save and Continue.
f. Repeat these steps until you've added all the rate definitions contributing to the overall salary.

Create a Rates-Based Salary Basis

Create a salary basis with base salary, allowance, short-term incentive plan, grade-based performance award, and
overall salary rate components. Users will enter values for the base salary and short-term components. The other
component values are calculated and can't be overridden.

1. Go to My Client Groups > Compensation > Salary Basis.

2. On the Salary Basis page, click the Create icon.

3. On the Create Salary Basis page, enter a name, such as US Rates-Based Salary.
4. In the Salary Basis Type field, select Salary amount is determined by rates.

5.

In the Rates section, add the rate definitions, as shown by these example values:

Rate Definition Name

Category

US Base Salary

US Allowance

US Short-Term Incentive Plan

Element

Element

Element

Grade-Based Performance Award

Value by Criteria

Overall Salary

Derived Rate

6. Click Validate.

7. Fix any validation issues and validate again until validation completes successfully.

8. Click Save and Close.

137

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 17
Example Rate Definition Configurations for a Salary Basis

138

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 18
Rates-Based Salaries

18  Rates-Based Salaries

Dos and Don’ts for Assigning and Changing Rates-Based
Salary

After you assign workers a rates-based salary basis, you shouldn’t make intrusive changes to the rate definitions
or component configurations. Instead, create other definitions or salary bases with the new rate component
configurations.

Examples of intrusive changes:

• Adding or removing rates from the salary basis

• End dating rate definitions

• Adding, removing, or changing contributing rates

Here’s the best practice method for handling changes to rates-based worker salaries:

1. Create other rate definitions or another salary basis with the new rate components configuration.
2. Assign the new salary basis to workers effective as of the change date.
3.

Inactivate the old salary basis, so that it’s no longer used.

Considerations When Using Rates-Based Salary

Consider dates used in salary calculations, inserting retroactive salaries, handling employment terminations, and
changing the salary basis type. Also consider salary copy during mass change of legal employer and what corrections
and updates you can make using HCM Data Loader.

Consideration

Comments

Date used in salary calculations for offer
and pending worker flows

The calculations use the assignment effective start date, which changes depending on if the proposed
start date is in the future or the past.

• Future: The assignment effective start date is the same as the offer creation date.

• Past: The assignment effective start date is the same as the proposed start date.

Inserting retroactive salary

Use the Change Salary task in the compensation app to insert the retroactive rates-based salary
between existing rates-based salary.

You can’t use HCM Data Loader.

Handling employment termination

Terminating a worker’s employment end dates the corresponding element entries based on their
termination rule. Their salary doesn’t get end dated, but rate values no longer get calculated. So, you
need to manually end date the salary.

Changing to another salary basis type

Delete all the rates-based salaries for the assignment. Then you can create another salary for the
worker that’s user determined, uses incremental components, or uses standard components.

139

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 18
Rates-Based Salaries

Consideration

Comments

CAUTION:  These kinds of deletions can create cascading effects on payroll or other downstream
processing, so be careful making these kinds of changes.

It’s a best practice to use rates-based salary for all employees in the legislative data group or legal
employer. This way migrating from rates-based salary to another type is no longer necessary.

Copying salary during mass change legal
employer

Rates-based salary can include element rates, which the salary process can copy to the destination
employer. The payroll process also copies element entries. This dual copy can lead to errors when
creating the destination salary.

To prevent errors, you can define an element group to exclude rate elements when submitting the
mass change process. This ensures that the salary copy process copies the element entries, but not the
payroll process.

Salary corrections and updates using HCM
Data Loader

After a worker has a rates-based salary basis, you can’t correct their salary with another salary basis.
You need to delete the rates-based salary and create another salary using the new salary basis.

Note:  You can delete only the most recent salary.

When you update salary with another rates-based salary basis, the element entries belonging to the
primary rates of the old salary basis aren’t end dated. You need to use HCM Data Loader and the
Element Entry object to update the end date of the affected element entries.

New work relationship created as part of
a global transfer for a source assignment
that uses a rates-based salary type

The rates-based salary of the source assignment gets end dated 1 day before the effective date of
the new relationship. If you cancel the new relationship, the end date for the source assignment isn't
automatically removed. You need to remove it manually.

Sharing rate definitions among salary
bases

There can be issues with worker salaries when they're shifted between salary bases that share rate
definitions.

Element rate value behavior for FTE
Changes

Salary amounts are adjusted for changes in full-time equivalent (FTE) when using flows such as
Change Working Hours. However, this adjustment doesn’t occur for an element rate.

140

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 19
Salary Basis FAQs

19  Salary Basis FAQs

Can I change or delete a salary basis that's in use?

You can't delete or change any characteristic after you associate the salary basis with anyone.

Can I add effective-dated changes to the salary basis?

You can't because the salary basis isn't an effective-dated object.

Where does the annualization factor for a salary basis
that uses payroll period frequency come from?

The period type on the payroll linked to a person's assignment decides the number of payroll periods in a year. These
payroll periods are the annualization factor.

Can I use the same payroll element for multiple salary
bases?

Yes, if it's a recurring element that you classify as an earnings element and configure to enable multiple entries in the
same period.

Related Topics

Can I update an element mapped to a salary basis that's
in use?

Yes, but only the next salary change recognizes the updated element or input value. At that time, salary processing end
dates the element entry associated with the prior salary.

When you update the element mapping, no changes apply to the person's data.

141

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 19
Salary Basis FAQs

Can managers change the salary basis of a salary
record?

Yes. You can hide or show the edit capability for managers using personalization on the pages where managers enter
salary allocations.

142

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 20
Salary Ranges and Metrics

20  Salary Ranges and Metrics

How You Validate Salary Changes with the Grade Range

You can verify that salary changes fall within the appropriate range for each person using grade range validation.

This validation generates a warning message when someone enters a new or adjusted salary that's outside the person's
assignment grade range. The person can ignore the message or revise the salary to fall within the valid range.

The assignment grade in the grade rate attached to the salary basis defines the minimum and maximum grade range
values. You can adjust the base ranges by linking a differential profile to the salary basis. Differentials apply according to
one of these criteria:

• Location

• Business unit

• Location and business unit

• Compensation zone

• Compensation zone and business unit

You can also associate grade rate differentials that override the grade rate, and thus the grades and grade ranges,
associated with the salary basis. The grade rate from the differential profile needs to have corresponding grades for all
the grades of the grade rate linked to the salary basis.

Related Topics

• Overview of Salary Range Differentials

• Grade Rates

Salary Range Violation Behavior for Proposed Salaries

Specify how to handle salary range violation for various compensation actions, such as Change Salary and Salary
History. This handling also applies to Offer and HR actions that include the Salary section, such as Offer, Hire, Promote,
and Transfer.

You configure violation behavior using the Salary Range Violation Behavior field of the salary basis. You can let people
propose salaries that violate the salary range with or without a warning. Or, you can prevent people from proposing any
salaries that violate the salary range. For example, you warn people when their proposed salaries are below or over the
specified salary range. Or, you don't let anyone propose salaries that are below or over the specified salary range.

The default value for the Salary Range Violation Behavior field of all existing salary bases is Warn. We don't recommend
that you change it to Error for existing salary bases because you can get errors with historic data. For example, you've
an existing salary basis with a salary range of 100 to 200 USD. The salary basis is associated with a 2010 salary record
where the salary amount was 95 USD. It's also associated with a 2015 salary record where the salary amount was 105
USD. When you change the violation behavior to Error and try to load salary for 2020, you can get the violation error for
2010. The error occurs even though that's not the record you're correcting. To set the violation behavior to Error, then

143

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 20
Salary Ranges and Metrics

we recommend that you create another salary basis to use with new salaries. This way, you can avoid issues with historic
data.

When you set the violation behavior to Warn, you don't see the warning message when you load salaries using
these tools: REST API, HCM Data Loader, and HCM Spreadsheet Data Loader. These tools show you only errors. The
Download Salaries task and grate step progression processes ignore this violation behavior.

Related Topics

• Overview of Base Pay Configuration

• How You Validate Salary Changes with the Grade Range

• Overview of Salary Range Differentials

• How Salary Metrics Change According to the Grade Rate and Salary Range Differentials

How Salary Metrics Are Calculated

Salary amount has a date while full-time equivalent (FTE), grade, grade rate, and differential profile have effective dates.
Thus, a salary record can apply logic for multiple combinations of FTE, grade, grade rate, and differential to different
time periods.

So, how are salary metrics, such as compa-ratio, range minimum, and range maximum, calculated? The metric
calculations use a reference date. Here's how we decide that date:

•

•

•

If the salary record has an end date that's earlier than the current date, then use the salary end date.

If the start date of the salary record is in future, then use the salary start date.

If the salary record started in the past and doesn't have an end date, then use the current device date.

Related Topics

• How Salary Metrics Change According to the Grade Rate and Salary Range Differentials

144

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 21
Salary Range Differentials

21  Salary Range Differentials

Overview of Salary Range Differentials

You can configure salary range differentials to adjust base salary ranges from the grade rate associated with the salary
basis. Differentials vary, for example, to reflect the cost of living in different locations or the relative ease of hiring.

For example, salaries for workers in the Central US are in the base range of the grade rate. Salaries for workers in the
South are in a discounted range with a 0.9 factor, and for workers on the East and West Coasts, they’re in a premium
range with a 1.1 factor. Salaries in New York City, Los Angeles, and San Francisco are in a super premium range with a
factor of 1.2.

Select the level of granularity that best supports your salary policies and processes:

• Location

• Business unit

• Location and business unit

• Compensation zone

• Compensation zone and business unit

145

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 21
Salary Range Differentials

When using a Grade Rate type differential profile, you can configure an overriding grade rate to use instead of the salary
basis grade rate. The adjusted salary range is the range of the overriding grade rate.

When using a Factor type differential profile, you can configure the differentials to enforce relevant statutory limits
around minimum salaries by setting lower limits.

You can also configure compensation zone, and compensation zone and business unit differentials to account for
nonoffice workers. Do this by specifying which address types to use, and in what order, to identify the applicable
differential. For example, you're going to associate the differentials with people who work at client sites and from home.
And, you want to use their remote addresses, rather than their work addresses to identify their compensation zones and
differential factors. You want to identify the client site address first and the home address only if there isn’t a client site
address.

Related Topics

• How Salary Metrics Are Calculated

• How Salary Metrics Change According to the Grade Rate and Salary Range Differentials

Configure Salary Range Differentials

You can adjust base salary ranges from the grade rate associated with the salary basis using salary range differentials.

1. Go to My Client Groups > Compensation > Salary Range Differentials.

2. On the Salary Range Differentials page, click the Create icon.

3. On the Create Salary Range Differential page, in the Properties section, complete the required fields.

4. Select the criteria, such as Location or Compensation Zone.

5. Select the type.

6. In the Differentials section, configure the differentials. When your criteria is compensation zone based, you can

select the Factor or Grade Rate type.

◦ To configure the differential to apply factors to the existing grade rates, select Factor.
◦ To configure the differential to apply alternate grade rates in place of the grade grate associated with the

salary basis, select Grade Rate.

7. Optionally, for differentials that use compensation zone criteria, enable checking for the remote worker address

type. Specify up to three address types to check in the order that differential processing should consider them. The
process stops checking as soon as it finds an address, whether that address is in the first address type or the last.

8. Save and close the differential.

Related Topics

• Overview of Salary Range Differentials

• Configure Compensation Zone Types and Zones

• How Salary Metrics Change According to the Grade Rate and Salary Range Differentials

146

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 21
Salary Range Differentials

Basic Process to Configure and Apply Zone-Based Salary
Range Differentials

You need to complete these tasks to set up and use compensation zones in salary range differentials. These types of
differential profiles work with only responsive salary pages and flows. Classic pages and flows ignore them.

1. Create compensation zone types by going to Setup and Maintenance > Compensation > Base Pay >

Compensation Zones.

You use compensation zone types, such as compensation or wage regions, to categorize zones and group them
together. You need to create your zone types before you define one or more zones for a geographical boundary.
You can create a zone type that contains geographical boundaries from anywhere in the world, or that contains only
geographies in a specified country. When you create a zone type for a country, you can define which geography
types or geographies you can select when you create the zones.

2. Create compensation zones by going to Compensation Zones.

Compensation zones are geographical boundaries for a zone type, for example, the San Jose compensation zone.
Zones are based on the geography hierarchy data of the master reference. You create zones in a zone type and
you can associate geographies to define the zone. For example, you've the Compensation Regions zone type. You
create a West Coast zone that has the state of California as one of its geographies. In a geography, you can specify a
postal range. So for the state of California, for example, you can specify that the zone spans the postal codes 90001
through 90011.

Compensation zones are intelligent enough to apply salary range differentials based on the worker’s assignment or
nonassignment location. For example, they can apply the differential to the work location or a remote location, such
as a client location or home address. The salary range differential identifies the compensation zone that the address
is part of, and applies the factor or overriding grade rate defined for that zone.

Optionally load compensation zone geographies using only the Export to CSV File and Import from CSV File actions
for the Compensation Zones task.

3. Create zone-based salary range differentials by going to My Client Groups > Compensation > Salary Range

Differentials. You can also create them using HCM Data Loader or HCM Spreadsheet Data Loader. You configure
salary range differential details at the level of granularity that best supports your salary policies and processes. For
example, you can maintain differential factors at the location level, or at the State or District level. Add compensation
zone criteria and define the differentials for each zone type and zone.

Optionally set minimum limits when you've statutory minimum salary limits that you need to enforce. You can also
enable work from home processing for people working remotely, such as at client sites or from home.

4. Create salary bases by going to My Client Groups > Compensation > Salary Basis. On the Salary Ranges tab, add a

grade rate to the salary basis. Then add the appropriate zone-based differential profile.

Related Topics

• Configure Compensation Zone Types and Zones

• Overview of Base Pay Configuration

• Configure Salary Range Differentials

147

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 21
Salary Range Differentials

Zone-Based Salary Range Differential Processing

Differential processing identifies the minimum, midpoint, and maximum points of the salary range using the
assignment grade and the grade rate of the salary basis. When the worker is working from home, it then decides if the
differential profile has work from home processing enabled.

•

•

If not enabled, it finds the work location to process. If there’s no work location or a location isn’t included in the
differential profile, the salary basis grade rate is used in payroll processing. No differential is applied.

If enabled, it finds the person addresses to process.

Next differential processing finds the compensation zone type and zone for the identified address of work location or
person. And it applies the differential factor or overriding grade rate for the corresponding compensation zone type and
zone. It uses the differential factor or overriding grade rate to recalculate the minimum, midpoint, and maximum points
of the salary range.

148

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 21
Salary Range Differentials

149

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 21
Salary Range Differentials

Work Location Example
Here’s an example of this differential processing based on the work location for two workers in California. They both
have the same assignment grade and salary basis. Their locations put them in different compensation zones, so their
salary ranges and related salary metrics are thus different.

Assignment Info

Grade

Work Location

Salary Info

Salary Basis

Grade Name

Salary Range

Worker 1

ZMCP IC1

Worker 2

ZMCP IC1

Bakersfield Branch Office

Redwood Shores HQ

Individual Contributor

Individual Contributor

ZMCP IC1

ZMCP IC1

50,000 – 100,000 USD annually

150,000 – 300,000 USD annually

Compensation Zone Type

Individual Contributor CA

Individual Contributor CA

Compensation Zone

Bakersfield

Headquarters

Salary

61,000 USD annually

161,000 USD annually

Remote Work Example
Here’s how differential processing would change the salary range for Worker 2 if they were a remote worker. They live in
Modesto, CA, which is in the same compensation zone as Bakersfield.

Assignment Info

Worker 2

Work Location

Home Address

Grade

Working at Home?

Salary Info

Salary Basis

Grade Name

Salary Range

Redwood Shores, CA

Modesto, CA

ZMCP IC1

Yes

Individual Contributor

ZMCP IC1

50,000 – 100,000 USD annually

Compensation Zone Type

Individual Contributor CA

Compensation Zone

Bakersfield

Salary

161,000 USD annually

150

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 21
Salary Range Differentials

Factor Type Salary Range Differentials That Include
Lower Limits

You might have statutory limits for salaries that you need to enforce, such as salary minimums. You can enforce lower
limits in factor type salary range differentials associated with salary bases.

These differential processing flows compare the processing behavior when the differential has lower limits versus when
it doesn't. In this example differential profile, the Redwood Shores HQ zone has a lower limit of 160,000.

Compensation Zone

Differential Factor

Lower Limit

Frequency of Minimum Amount

Annualization Factor for Minimum
Amount

Redwood Shores HQ

Bakersfield Branch Office

1.5

0.5

160,000

80,000

Annually

Annually

1

1

The base range of the salary basis that includes this differential profile is 100,000 to 200,000. Normally, the adjusted
ranges for the Redwood Shores HQ zone would be 150,000 to 300,000 after applying the 1.5 differential. But, this
differential has a lower limit of 160,000 and that minimum overrides the 150,000 minimum. So the effective salary
range becomes 160,000 to 300,000. If the differential profile didn’t have any lower limit, the adjusted base range would
remain 150,000 to 300,000.

Configure Compensation Zone Types and Zones

Here's how you configure the compensation zone types used to group zones together and the zones that make up a
zone type. Go to Setup and Maintenance > Compensation Management > Base Pay > Compensation Zones.

Create the Compensation Zone Type
We recommend limiting the number of compensation zone types, preferably to 1, such as by postal code. Here's how
you create a zone type:

1. On the Manage Zone Types page, click the Create icon.
2. Enter a name for the zone type.
3. Specify the boundary of the zone type.
4. Select the geography.
5. At the appropriate geographic level, such as Postal Code, select Zone Creation Allowed.

CAUTION:  You need to make sure that geography validation is enabled for the No Styles Format address style of the
selected geography level. Otherwise you won't see the adjusted salary ranges for individuals in this compensation
zone. Use the Manage Geographies task and the Manage Geography Validation action.

151

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 21
Salary Range Differentials

Create a Zone
Configure your zones so that an address is part of only one zone. If an address is part of multiple zones, the salary
changes that include zone-based differentials can't figure out which zone applies. Thus, they can't apply any differential.
Also, configure the zones for a zone type at the same level to minimize or prevent zone overlaps. For example, if Zone 1
is at the State level, then define the other zones at the State level also.

Here's how you create a zone:

1. On the Manage Zone Types page, search for and select your new zone type. If you click the zone type, you open

a read-only page with details of the zone type configuration. You can't add zones from that page.

2. Click Next.
3. On the Manage Zones for Zone Type page, click the Add icon.
4. On the Create Zone page, enter the general information.
5. Associate geographies with your new zone.

a. Click the Add icon.
b. On the Add Geography dialog box, search for and select the geography that you want to add.
c. Click Save and Close.
d. Review the start dates of the associated geographies. When you associated the geography, it

automatically set the start date to the system date at that time. You can edit the date, as needed.
e. When you finish associating geographies, on the Create Zone page, save and close your new zone.

6. When you finish adding zones to your zone type, on the Manage Zones for Zone Type page, save and close

your zone type.

Best Practices When Using Postal Codes
If you've fewer than 5 postal codes, add the codes directly in the zone definition instead of using postal ranges. For
example, add the 90009 postal code directly to the zone instead of adding it as the range, from 90009 to 90009.

Avoid defining overlapping geographies or postal code ranges across compensation zones. For example, you defined
these postal code ranges:

• Compensation Zone 1 for CA with the range from 91000 to 91999

• Compensation Zone 2 for CA with the range from 91111 to 91729

In this case, the differential profile logic identifies both compensation zones for the 91112 postal code and thus won't
apply any differentials for 91112.

Tip:  The postal code data type is CHAR, so the zone ranges get calculated as character ranges, not numeric. For
example, a zone with the postal range from 10 to 100 includes these postal codes: 11, 12, 13, and 14. It doesn't include
these postal codes: 20, 21, 30, 31, 40, 90, 99.

Related Topics

• Overview of Salary Range Differentials

• Configure Salary Range Differentials

• How Salary Metrics Change According to the Grade Rate and Salary Range Differentials

152

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 21
Salary Range Differentials

Compensation Zone-Based Differential: Options for
When Work from Home Is Yes, But Evaluation Should
Use Work Locations

You can configure compensation zone-based salary range differentials to evaluate remote worker addresses and
calculate salary ranges. And you can specify the processing order for up to three address types.

You can configure compensation zone-based salary range differentials to evaluate remote worker addresses and
calculate salary ranges. And you can specify the processing order for up to three address types.

When using this kind of differential, can you use work locations to identify the applicable differential for certain remote
workers? For example, in some US states, remote workers have the option to go into an office. Or they need to go in 1 or
2 days a week. So for some states, even when Work from Home is Yes, you want the differential to use the work location.

Here are three configuration options that let you use people’s work locations to identify the applicable differentials, even
when Work from Home is Yes.

Separate Differentials and Salary Bases
In this approach, you can create two different differential profiles for the remote workers.

• One differential doesn’t process remote workers, thus evaluating only people’s work locations.

• Another differential does process remote workers and specifies to use home addresses.

Each set of remote workers needs to have a different salary basis, such as, US Remote by Work and US Remote by
Home.

Different Field to Record Actual Work from Home Status
In this approach, you can use a different assignment field or a descriptive flexfield to record the actual work from
home status. The value of this other field could typically be the same as the value of the delivered Work from Home
assignment field. But you can vary the value for people in the states where differential processing should use the work
location instead of remote addresses.

• Where differential processing should use remote workers’ home addresses, make sure that the Work from

Home assignment field is Yes.

• Where differential processing should use remote workers’ work locations, make sure that the Work from Home

assignment field is No.

Then you can create a differential that processes remote workers. Processing will evaluate the addresses as specified.

Person Addresses with Work Locations
In this approach, you extend the address type lookup to let you set up a work address as another person address. Next,
for the remote workers where differential processing should use their work location, you create the appropriate work
person addresses. Then you create a differential with remote worker processing enabled. Processing will evaluate the
specified address types in the specified order.

153

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 21
Salary Range Differentials

For example, a remote worker has a home-type address in Jacksonville, FL, a work-type address in Orlando, FL. And
their Work from Home is Yes. Their differential has the Work address type as sequence 1 and Home address type as
sequence 2, so differential processing uses their Orlando, FL address.

This approach means that every applicable remote worker will also have their work address maintained as one of their
person addresses. Whenever the work location changes, someone also needs to manually change the corresponding
person address.

Generate Compensation Zone and Address Mapping

For salary range differentials with compensation zone criteria, differential processing finds the zone and zone type each
time someone views and adjusts the salary amount.

The differential process does this by evaluating the person's maintained addresses against the defined compensation
zones. Depending on the number of zones, zone types, and address details, this evaluation can be time consuming.
To see the correct salary ranges in Oracle Fusion Cloud Workforce Compensation and Oracle Transactional Business
Intelligence reports, run the Generate Compensation Zone and Address Mapping process. Also run it to optimize
differential processing because it finds the compensation zone and zone type for each address, and stores them for
immediate reference.

You can run the generate process in two modes.

Run Mode

Descriptions

Create incremental mappings

Creates mappings between zones and zone types that match the specified parameters and person or
work location addresses when something changed or is new

Purge and recreate mappings

Purges all existing mappings

Creates the maps again between the zones and zone types that match the specified parameters and all
person or work location addresses

Here's how we recommend that you schedule the process.

Schedule Mode

Descriptions

One-time

Recurring

Run the mapping process to create all zone mappings for both work location and person addresses.
You might use this mode to create a baseline. You might also use it to update work location addresses
because they change infrequently.

Schedule the mapping process to run regularly to create incremental zone mappings. You might use
this mode to update person addresses for remote workers because they can change more often. For
example, client work locations change as the person moves changes projects.

The generated mappings improve the performance of responsive pages with salary information. The differential
process knows the person's compensation zone and can apply the relevant differential to salary range calculations.
Here's the high-level process flow.

154

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 21
Salary Range Differentials

When the mapping isn't available, differential processing finds the zone and zone type for the person or work address. It
then applies the relevant differential.

Improve Performance
By default, the Generate Compensation Zone and Address Mapping process has 3 threads with chunk sizes of 20. You
can increase the total threads and check performance until you reach the best total for your volume.

1. Go to My Client Groups > Compensation > Configure Compensation Batch Parameters.
2. Change the Run Salary Processes total threads count.
3. Save your changes and close the page.
4. Test performance.
5. Repeat until you reach the best performance for your volume.

Note:  Changes to the total threads for this parameter also affect the Run Salary Processes process.

Related Topics

• Overview of Salary Range Differentials

• Configure Compensation Zone Types and Zones

155

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 21
Salary Range Differentials

Enable Geography Validation for Compensation Zones

You need to make sure that geography validation is enabled for the No Styles Format address style of the selected
geography level.

1. Go to Setup and Maintenance > Tasks panel Search > Manage Geographies.

2. Search for a country. For example, you can search by entering the country name United States or the two letter ISO

code US.

3.

In the Search Results area, select the country, such as United States.

4. Click Actions > Manage Geography Validation.

5. On the Manage Geography Validation page, you see the geography types that are available for the country in the

Geography Mapping and Validation section.

6. Make sure that the No Styles Format address style is selected. You define validation for this address style so that

the validations are run for all addresses in the country.

7. For the geography types to include in the geography validation, such as Postal Code, select Geography Validation.

Load Compensation Zone Geographies Using CSV File
Export and Import

After you create you compensation zone types and zones, you can load the corresponding zone geographies from a .csv
file.

1. Go to Setup and Maintenance > Compensation > Base Pay.

2.

3.

In the Show field, select All Tasks.

If you don’t see the Actions column, on the toolbar select View > Columns > Actions.

4. Generate a CSV export package for the Compensation Zones task by selecting Actions > Create New > Export to

CSV File.

a. On the Export Setup Data to CSV File page, enter a descriptive process name.
b. Click Submit.

5. Track the export process by selecting Actions > View All > Export to CSV File.

6. Download the export file from the Export Setup Data to CSV File History: Compensation Zones page, after the export

process completes. Select Actions > CSV File Package > Download.

7. Extract the contents from the .zip file to an appropriate folder.

8. Open the ORA_HZ_GEO_RELATIONSHIP.csv file.

156

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 21
Salary Range Differentials

9. Using the existing geography rows as reference, add the new geographies. For each new geography, you need to add
2 rows to the file. To avoid damaging the data, use a text editor, such as Notepad++, and not Microsoft Excel. Save
the file as you go and when you're done.

Also, the ORA_HZ_GEO_RELATIONSHIP.csv file has three start date columns. Here's the date you need to enter in
each column:

◦ StartDate: Enter the start date of the zone.
◦ SubjStartDate:

- If the 'SubjGeographyName' column is zone, enter the zone start date.
- If the 'SubjGeographyName' column is postal code, enter the postal code start date.

◦ ObjStartDate:

- If the 'ObjGeographyName' column is zone, enter the zone start date.
- If the 'ObjGeographyName' column is postal code, enter the postal code start date.

You can source the start and end dates by running these two queries:

SELECT
 geography_name,
 to_char(start_date, 'YYYY/MM/DD') start_date,
 to_char(end_date, 'YYYY/MM/DD') end_date,
FROM
 fusion.hz_geogrpahies
WHERE
 geography_name in ('_ZONE_NAME')

SELECT
 geography_name,
 country_code,
 geography_element2,
 geography_element3,
 geography_element4,
 to_char(start_date, 'YYYY/MM/
DD') start_date,
 to_char(end_date, 'YYYY/MM/DD')
 end_date,
FROM
 fusion.hz_geogrpahies
WHERE
 geography_name in ('999999')
 AND country_code = 'US'
 AND geography_type = 'POSTAL_
CODE'
 AND geography_use = 'MASTER_
REF'
ORDER BY
 Geography_element2,
 Geography_element3,
 Geography_element4,
 Geography_name

10. Create a .zip file with all the extracted files and the updated ORA_HZ_GEO_RELATIONSHIP.csv file.

11. Import the .zip file for the Compensation Zones task by selecting Actions > Create New > Import from CSV File.
12. On the Import Setup Data from CSV File page, search for and select the new .zip file.

13. Click Submit.

14.Track the import process by selecting Actions > View All > Import from CSV File.

15. After the process completes, you’re ready to verify the loaded geography data.

157

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 21
Salary Range Differentials

158

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 22
Base Pay Lookups and Troubleshooting

22  Base Pay Lookups and Troubleshooting

Incremental Salary Component Lookups

HR specialists and line managers can use incremental salary components to itemize new or adjusted salary, to reflect
the different reasons for their allocations. Here are the incremental components bundled in the implementation:

• Adjustment: Regular and automatic adjustment

• Cost of Living

• Equity: Adjustment to correct salary compression or inversion

• Location

• Market: Adjustment due to salary being out of line with the market

• Merit

• Promotion

• Progression: Regular and automatic adjustment

• Structured: Adjustment dictated by union or employment contract, such as an increase after 3 months

You can change or add components to the CMP_SALARY_COMPONENTS lookup type to better support your reporting
policies for salary allocations. Use the Manage Common Lookups task in the Setup and Maintenance work area.

Itemization
The salary record stores the incremental component itemizations and uses them to calculate new salary. When
component values change, the payroll element holds the new salary amount calculated from the component
adjustments. But it doesn't receive individual component amounts for processing. The incremental values entered in
the salary record apply only to that record and don't apply to any future salary records.

Related Topics

• How You Enable Salary Itemization Using Incremental Components

• Overview of Lookups

Simple Salary Component Lookups

HR specialists and line managers can use simple salary components to itemize new or adjusted salary, to reflect the
different reasons for their allocations. Here are the simple components bundled in the implementation:

• Basic salary

• Housing allowance

• Special allowance

• City allowance

159

Oracle Fusion Cloud Human Resources
Implementing Compensation

• Transport allowance

• Travel allowance

• Wage progression rate

• Variable allowance

• Overall salary

Chapter 22
Base Pay Lookups and Troubleshooting

You can change or add components to the ORA_CMP_SIMPLE_SALARY_COMPS lookup type to better support your
reporting policies for salary allocations. Use the Manage Common Lookups task in the Setup and Maintenance work
area.

Itemization
Simple component itemizations let you maintain the values for the components and you typically configure them to
calculate new salary. When simple component values change, the salary record calculates the new salary amount. The
payroll element holds this new salary amount, but it doesn't receive individual component amounts for processing.

Related Topics

• Salary Amount Is Determined by Simple Components

• Overview of Lookups

Troubleshoot Salary-Related Issues

Here are some salary-related issues that might occur and solutions to help you fix them.

Issue

Solution

The salary element entry didn't get
created.

The salary basis element doesn't get created if inconsistencies exist between the element eligibility and
the payroll data of the person's assignment.

Using the Element Entries task in the Person Management work area, set the Effective Date to same
date as the salary start date. Then search for the salary basis element in the Element Name column.
If you don't see the element listed, the person isn't eligible for the element. You need to verify the
eligibility and effective dates configured for the element.

The salary ranges are incorrect for an
hourly person.

Check the annualization factor of the grade rate associated with the salary basis. The annualization
factors for the salary basis and grade rate might differ, even if the frequency for both is Hourly. Salary
range calculations use the frequencies and factors of the salary basis and the grade rate. If they don't
match, the calculations convert grade rate values to those of the salary basis.

Salary changes are stuck in the approval
flow.

An individual's salary page has a message
that's something like this: Changes to
this data are pending approval. HR
specialists and compensation managers
or administrators don't have a Withdraw
option for the transaction in their worklist.
And sometimes, the person record gets
locked after changing the salary.

Ask the person who submitted the salary change to use their worklist to withdraw the change. They
can also see who the current approver is, so they can ask the approver to approve or reject the
proposed changes.

If you still see the pending approval notification in the Change Salary flow, your approvals
administrator can use the transaction console to cancel the change. If you still see the pending
approval, have your help desk log a bug with Oracle Support. The bug should be for the Salary
component of Oracle Fusion Workforce Compensation.

160

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 22
Base Pay Lookups and Troubleshooting

Issue

Solution

Salary notifications are blank.

The person might have a custom role. Add the Approve Salary Updates privilege to their application
role. Or, add these three resources to a custom entitlement and add the entitlement to their application
role.

• HcmDetectCompletedTransaction.xml

• ChangeSalaryApprovalTask_TaskFlow.xml

• ChangePayNtfsFlow.xml

The salary details in notifications are
blank.

The person probably doesn't have a compensation role. Depending on whether they should have read-
only or read and write accesses to the salary details, add one of these job roles:

People need to see salary information, but
not make any changes.

• View Salaries

• Manage Salaries

For detailed solution steps, see Approval Notifications - You Don’t Have Permission to Access this
Information (document ID 2212593.1).

People need to see salary information, but
must not be able to make any changes.

Grant them access to the Compensation Info task, which they can review salary information. Reserve
the Change Salary role for the people who need to manage the salary data.

161

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 22
Base Pay Lookups and Troubleshooting

162

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 23
Default Salary from Grade Ladder Rates

23  Default Salary from Grade Ladder Rates

Basic Process to Default Salary Amounts from Grade
Ladder Rates

For details about defaulting salary, see the How do I default salary from grade ladder rates? playbook.

163

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 23
Default Salary from Grade Ladder Rates

164

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 24
Grade Step Progression Configuration

24  Grade Step Progression Configuration

Manage Grade Step Progression

For information about setting up grade step progression, see the How do I set up a grade ladder for grade step
progression? playbook.

Examples of Adding Progression Rules

For details, see Example Progression Rules Applied at Each Level in the How do I create progression rules? playbook.

165

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 24
Grade Step Progression Configuration

166

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 25
Transaction Dates and On Eligibility in Grade Step
Progression Processing

25  Transaction Dates and On Eligibility in
Grade Step Progression Processing

Date Codes and Eligibility Options for Grade Step
Progression

For information about setting up grade step progression, see the How do I set up a grade ladder for grade step
progression? playbook.

167

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 25
Transaction Dates and On Eligibility in Grade Step
Progression Processing

168

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 26
Global Settings for Grade Step Progression Processing

26  Global Settings for Grade Step Progression
Processing

Batch Settings for Grade Step Progression Processing

For information about batch settings, see the Global Settings for Grade Step Progression Processing chapter in the How
do I manage grade step progression processes? playbook.

169

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 26
Global Settings for Grade Step Progression Processing

170

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 27
Grade Step Progression Processing

27  Grade Step Progression Processing

Overview of Grade Step Progression Processing

For information about processing, see the Grade Step Progression Processing chapter in the How do I manage grade
step progression processes? playbook.

171

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 27
Grade Step Progression Processing

172

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 28
Examples of Grade Step Progression Processing

28  Examples of Grade Step Progression
Processing

Examples of Grade Step Progression Processing

For examples about processing, see the Examples of Grade Step Progression Processing chapter in the How do I manage
grade step progression processes? playbook.

173

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 28
Examples of Grade Step Progression Processing

174

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 29
Proposed Grade Step Progression and Salary Updates

29  Proposed Grade Step Progression and
Salary Updates

Overview of Proposed Progression and Salary Updates

For information about proposals, see the How do review and understand results from grade step progression processes?
playbook

175

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 29
Proposed Grade Step Progression and Salary Updates

176

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 30
Adjustments to Salary Amounts in Proposed Progression
and Salary Updates

30  Adjustments to Salary Amounts in
Proposed Progression and Salary Updates

Overview of Parameters That Affect Salary Amounts for
Proposed Progression and Salary Updates

For information about the parameters, see the How do review and understand results from grade step progression
processes? playbook

177

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 30
Adjustments to Salary Amounts in Proposed Progression
and Salary Updates

178

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 31
Individual Compensation Plans Overview

31  Individual Compensation Plans Overview

Overview of Individual Compensation

You can let managers and specialists award compensation outside of the regular compensation cycle. For example,
a line manager can give someone a spot bonus or grant stock shares. And a compensation manager can give people
education reimbursements.

You can also let people make and change their own contributions to charitable or savings plans. These off-cycle
allocations and contributions require appropriate payroll elements and individual compensation plans.

• The payroll element communicates the payment or distribution details to payroll for processing. For example, a
company car plan has options with different compensation amounts for various mileage ranges. A spots bonus
plan has options with different fixed monetary amounts.

• The plan includes at least one option that links the payroll element to the plan. It also decides when payments

start and end, the people eligible for the plan, and when people can access the plan. For example, a car
allowance plan has multiple options for monthly payments starting January 1 and ending December 31
according to mileage ranges. People in field sales and service jobs are eligible for the plan, and managers can
award compensation when they hire, transfer, and promote people.

You can also let people view nonmonetary awards by adding the relevant plans to compensation history. To let them
view their payment and contribution history, add the payroll elements linked to the plans that have recurring payments
or contributions.

Options in an Individual Compensation Plan
Configuration

Each individual compensation plan needs at least one option. You can set up a nonmonetary option, such as grant
stock shares, or a monetary option. Link a payroll element, and optionally select a budget pool and request or require
attachments.

When you create the option, you need to select the appropriate payroll element. You can select one element per
legislative data group. So you can link an option to multiple elements only when the element legislative data groups
are different. Proposers see the input values configured for the element when they select the option while allocating
compensation or contribution. The monetary amounts that they propose are in the currency of the element. On pages
that include the currency switcher, people viewing the proposed amounts can see them in their preferred currency.

CAUTION:  Make sure that salary bases don't use the element selected for the option. Using the same element across
compensation objects can lead to payroll conflicts. It can also lead to unexpected deletions of salary or individual
compensation.

You can optionally select a budget pool to let managers track off-cycle and on-cycle awards.

179

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 31
Individual Compensation Plans Overview

You can also request or require that proposers attach a specific document type to help approvers decide whether to
approve or reject proposed plan allocations. For example, set up a vehicle allowance option to require a vehicle details
document. The documents get retained in people's document records for future reference.

The document settings affect all flows except Offer flows. Currently people can't add attachments in the Offer flows, so
the flows ignore any option document settings configured for the individual compensation plan.

Related Topics

• Document Type Settings for Individual Compensation

• Create a Payroll Element to Use with Individual Compensation Plans

• How You Let Managers Track Off-Cycle and On-Cycle Compensation Against a Budget

Document Type Settings for Individual Compensation

Make sure that document types you use with compensation objects, such as options for individual compensation plans,
have these configurations. Manage document type configurations using the Document Type task.

Field

Value

Document Type Level

Assignment

Category

Compensation

Minimum Attachments

0

Document Name Applicable

Relevant and Required

All other attributes

Not required

Allow Occurrences

Yes

Payment Dates in an Individual Compensation Plan
Configuration

You specify when plan payments start and end using standard date rules. For example, the person proposing the award
can set the payment date. You only need to set end dates for recurring payments, such as car allowances.

If you select the Start or submission date option, the award or contribution uses the start date when people can set it
during actions. Otherwise, the award or contribution uses the date when they submit the action.

180

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 31
Individual Compensation Plans Overview

Related Topics

• Sync Individual Compensation Plan Dates with the Start Date in a Pending Worker Action

• Sync Individual Compensation Plan Dates with the Projected Hire Date in an Offer

• Payment End Date Considerations for Individual Compensation Plans

• How the Projected Hire, Start, or Submission Date Works in HR Actions

How Changing the Hire Date Affects Individual
Compensation Allocations

Here's what happens when you change the hire date using the Change Start Date or Edit Work Relationship page:

Date Change

Affect on Recurring and Nonrecurring Allocations

New date is before the allocation start date None

New date is between the allocation start
and end dates

Allocation start date changes to match the new hire date

New date is after the allocation end date

Allocation will be deleted

Eligibility in an Individual Compensation Plan
Configuration

You decide who can participate in the compensation plans or options with eligibility profiles. You can attach eligibility
profiles to the plan, an option, or both.

For example, to the company car plan, you attach an eligibility profile that includes only the Sales and Field Service
departments. To the options, you attach other profiles that restrict payment amounts by mileage ranges.

Compensation eligibility evaluations also use criteria defined at the element eligibility level to decide if someone is
eligible for a compensation plan. The best practice for controlling eligibility is to either use eligibility profiles or element
eligibility, but not both.

If you add multiple profiles, you need to mark at least one profile as required.

Related Topics

• Eligibility Profiles

181

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 31
Individual Compensation Plans Overview

How Individual Compensation Plan Eligibility Works with
Assignment Creation Flows

Payroll element eligibility and plan-level or option-level eligibility profiles don't apply because the assignment
information hasn't been submitted yet.

How Individual Compensation Plan Eligibility Works with
Assignment Correction and Update Flows

Payroll element eligibility and plan-level or option-level eligibility profiles apply to the existing assignment information.
But they don't apply to the corrected or updated information because it hasn't been submitted yet.

Plan Access Restrictions in an Individual Compensation
Plan Configuration

Control who can start, update, or stop individual compensation allocations, and for what circumstances by restricting
plan access. For example, set up a plan so that only people using the Manager Personal Contributions action can start,
update, or stop contributions.

Related Topics

• Plan Access Restrictions

• The Difference Between Plan Access Restriction and Access Security

• Copy Individual Compensation Allocations During Local and Global Transfer

•

Individual Compensation Plan and Option Visibility

Plan Info in an Individual Compensation Plan
Configuration

To help managers awarding the plan or individuals contributing to the plan, you can optionally provide background
information or instructions. Also include links to relevant documents and websites.

You can also specify whether people viewing the plan see this information when they select the plan, or after they click
Show plan info.

182

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 31
Individual Compensation Plans Overview

Validate Individual Compensation Plans

You can validate the integrity of the individual compensation plan that you're editing. Or you can validate all of the plans
on the Individual Compensation Plans page.

You can detect and report on references to all deleted payroll elements still retained in the configured individual
compensation plan options. When someone deletes a payroll element before removing it from the plan option, it creates
orphan data in the individual compensation plan setup table. The orphan data can cause issues in allocations. To
prevent these issues, you can run the Purge Orphaned Payroll Element Setup Data from Individual Compensation Plans
process.

Before purging the orphaned payroll element data, you can run the process in Preview mode and generate a log with
the data the process will likely purge. When you run the process to purge the orphan rows, it cleans up the individual
compensation setup tables.

Journey Checklist Tasks and Individual Compensation
Plan Allocations

You can send people checklist tasks as part of their journeys when they get new individual compensation allocations.
For example, an individual subscribes to a voluntary deduction.

The corresponding journey includes checklist tasks that require an HR specialist to manually generate a membership ID,
enable portal access, and issue a welcome kit.

Assign Checklists
You can assign checklist tasks only when people add new individual compensation allocations using actions, such as
these:

•

Individual Compensation

• Manage Personal Contribution

• Administer Individual Compensation

You can also assign tasks with Recruiting and Global Human Resource actions that add individual compensation
allocations. The checklist assigns the tasks after the new individual compensation allocation passes final
approval and the element entries get created. The checklist listens to the new element entries for the
individual compensation allocation using events. For the events to work, make sure that the profile option
HRC_DISABLE_HCM_EVENTS_PROCESSING is N.

Create the Checklist Template
You create a checklist template following the standard procedure and using these individual compensation settings:

• On the General tab, select a category.

• On the Tasks tab, configure the tasks.

183

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 31
Individual Compensation Plans Overview

• On the Actions and Events tab, configure the event that causes the journey to assign the checklist. For new

individual compensation allocations, the creation of the entry for the specified element causes the checklist to
assign the task.

a. Add an event. Then in the Name field, select Individual Compensation.
b. Edit the condition and create a group. The attribute defaults to Element Type and the condition defaults

c.

to the Equals operator and Constant operand type.
In the Operand Value field, click search. Use the Search and Select dialog box to select the appropriate
payroll element for the individual compensation option.

You can use only the OR group connector when you define group conditions for individual compensation. The
conditions don't support the AND connector.

Control When the Checklist Triggers
To control when the checklist triggers, you use the allocation criteria.

• The default Checklist manually allocated or record created or approved option triggers when the individual

compensation allocation gets approved and element entries get created. The trigger ignores the payment start
date.

• The When the action record becomes effective option triggers the checklist on the payment start date.

Related Topics

• Predefined Journey Templates

• Journey Template Definition

• Considerations for Configuring Actions in Journeys

• How You Configure Events in Journeys

• Journey Display Properties

• Deep Links in Journeys

How You Let People Submit Personal Contributions
When Earlier Contributions Are Pending Approval

To let people submit personal contributions when earlier contributions are pending approval, you need to enable the
CMP_DISABLE_PENDING_APPROVALS_CHECK_IN_MANAGE_CONTRIBUTION profile option at the Site level.

You also need to configure the access details of the relevant individual compensation plans. For the Manage Personal
Contribution task, never allow update allocations and never allow the discontinuation of allocations. This access
detail configuration ensures that individuals can't change or delete existing contributions, preventing conflicts for
contributions that are pending approval.

With this option enabled, approvers can't edit submitted contributions as part of their approval. Also, they can't see the
submitted values if they edit the submitted contribution. Line managers, compensation managers and administrators,
and HR specialists can still make updates or deletions using the Manage Individual Compensation or Administer
Individual Compensation tasks. This visibility assumes you configured the plan access to include the corresponding
actions for these tasks.

184

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 31
Individual Compensation Plans Overview

Related Topics

• Plan Access Restrictions

185

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 31
Individual Compensation Plans Overview

186

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 32
Payment Dates in Individual Compensation Plans

32  Payment Dates in Individual Compensation
Plans

Sync Individual Compensation Plan Dates with the
Projected Hire Date in an Offer

You can sync the payment start and end dates of individual compensation plans included in an offer, with the projected
hire date.

Do this by setting the payment start and end dates of the individual compensation plans to Projected Hire, Start, or
Submission Date. Then whenever you change the projected hire date in an offer and go to the individual compensation
section, the plan payment dates adjust automatically.

For example, you've an offer with a projected hire date of January 1, 2022. The offer includes an individual
compensation plan with payments that start the same day. Later you revise the projected hire date to February 1, 2022.
When you get to the individual compensation section, the existing payment start date automatically adjusts to February
1, 2022, to align with the new projected hire date.

Delay Payment
You can optionally delay the payment date by a specific number of days, months, years, or combination. The offer
calculates the payment start and end dates using the projected hire date and the specified delay. For example, your
offer includes paying a sign-on bonus 1 month after the projected hire date. Because your current projected hire date is
February 1, 2022, the payment start date of the bonus allocation is March 1, 2022.

Override the Payment Date
You can let recruiters override the calculated payment start date, end date, or both when they include the plan in their
offers. When they do override the payment dates, the projected hire date and the payment dates can't automatically
sync anymore. The recruiters need to delete the individual compensation plan and add it again every time they change
the projected hire date. They can't correct the existing payment dates.

Offer flows indicated overridden plan dates with (Set manually).

Examples of How Payment Start Dates in an Offer Sync
with the Projected Hire Date

You have an offer with three individual compensation plans that have slightly different configurations for the payment
start date of Projected Hire, Start, or Submission Date.

Here's how the configurations affect the payment start dates for the three plans when the projected hire date for the
offer changes.

187

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 32
Payment Dates in Individual Compensation Plans

Payment Start Date
Configuration

Original Projected Hire
Date

Original Payment Start
Date

Revised Projected Hire
Date

Adjusted Payment Start
Date

Plan 1, the start date is the
projected hire date

Plan 2, the start date is 1
month after the projected
hire date

Plan 3, the start date is the
projected hire date, but
recruiters can override the
date

Jan 1, 2022

Jan 1, 2022

Mar 1, 2022

Mar 1, 2022

Jan 1, 2022

Feb 1, 2022

Mar 1, 2022

Apr 1, 2022

Jan 1, 2022

Initially set to Jan 1, 2022

Mar 1, 2022

Apr 1, 2022

Recruiter overrides to Apr 1,
 2022

Overridden dates remain
unadjusted

The payment start date for Plan 3 doesn't change because the recruiter overrode the original date. The recruiter needs
to delete this individual compensation plan and add it again with the revised payment start date.

After the external candidate accepts the offer with the projected hire date of March 1, 2021, the individual compensation
plans show up on the pending worker page. The plan payment dates for the pending worker are the same dates shown
in the Adjusted Payment Start Date column.

Sync Individual Compensation Plan Dates with the Start
Date in a Pending Worker Action

You can sync the payment start and end dates of individual compensation plans included in a pending worker action,
with the start date.

Do this by setting the payment start and end dates of the individual compensation plans to Projected Hire, Start, or
Submission Date. The plan payment dates adjust automatically whenever people change the start date in the Edit
Pending Worker action and go to the individual compensation section.

For example, you've a pending worker with a start date of January 1, 2022. The details include an individual
compensation plan with payments that start the same day. Later you revise the start date to February 1, 2022. When you
get to the individual compensation section, the existing payment start date automatically adjusts to February 1, 2022, to
align with the new start date.

The plan payment dates won't adjust if people change the start date and don't visit the individual compensation
section. They won't automatically adjust in these situations either:

• When people change the start date in other flows, such as Employment details, Change Employment Start

Dates, and Change Work Relationship Start Date

• On any other pages where people can change the start date of the pending worker.

• When people use HCM Data Loader or REST services

People need to manually delete and re-add the individual compensation plans in all such scenarios.

When someone end dates the individual compensation row in the pending worker flow, the flow carries the end date
forward to the conversion stage.

188

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 32
Payment Dates in Individual Compensation Plans

Delay Payment
You can optionally delay the payment dates by a specific number of days, months, years, or combination. The pending
worker flow calculates the payment start and end dates using the start date and the specified delay. For example, your
details include paying a sign-on bonus 1 month after the start date. Because your current start date is February 1, 2022,
the payment start date of the bonus allocation is March 1, 2022.

Override the Payment Date
You can let people override the calculated payment start date, end date, or both when they include the plan in the
individual compensation section. When they do override the payment dates, the start date and the payment dates can't
automatically sync anymore. They need to delete the individual compensation plan and add it again every time they
change the start date. They can't correct the existing payment dates.

Pending worker flows identify overridden plan dates with (Set manually).

Examples of How Payment Start Dates in a Pending
Worker Action Sync with the Start Date

You've a pending worker action with three individual compensation plans that have slightly different configurations for
the payment start date of Projected Hire, Start, or Submission Date.

Here's how the configurations affect the payment start dates for the three plans when the start date for the pending
worker changes.

Payment Start Date
Configuration

Original Projected Hire
Date

Original Payment Start
Date

Revised Projected Hire
Date

Adjusted Payment Start
Date

Plan 1, the start date is the
pending worker start date

Plan 2, the start date is 1
month after the pending
worker start date

Plan 3, the start date is the
pending worker start date,
 but people can override the
date

Jan 1, 2022

Jan 1, 2022

Mar 1, 2022

Mar 1, 2022

Jan 1, 2022

Feb 1, 2022

Mar 1, 2022

Apr 1, 2022

Jan 1, 2022

Initially set to Feb 1, 2022

Mar 1, 2022

Apr 1, 2022

Overridden to Apr 1, 2022

Overridden dates remain
unadjusted

The payment start date for Plan 3 doesn't change because you overrode the original date. When you need to revise the
dates, you need to delete this individual compensation plan and add it again with the revised payment start date.

189

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 32
Payment Dates in Individual Compensation Plans

Payment End Date Considerations for Individual
Compensation Plans

If the individual compensation plan configuration has a nonrecurring payroll element, the payment end date depends
on the person's payroll relationship. Here are situations that ignore the payment end date configured for the plan:

• When payroll isn't available in the payroll relationship, the payment end date is the same as the payment start

date.

• When payroll is available in the payroll relationship, the payment end date is the period end date for the payroll

process.

The Offer and Pending Worker flow end dates carry forward to the next stage when the end date for the plan payment is
Projected Hire, Start, or Submission Date.

How the Projected Hire, Start, or Submission Date Works
in HR Actions

Here's how the Projected Hire, Start, or Submission Date payment date works with HR actions started from the Manage
Job Offers page or elsewhere.

Started from Manage Job Offers
You can sync the initial payment start and end dates of individual compensation plans included with the projected
hire date of the internal offer. Do this by setting the payment start and end dates of the individual compensation plans
to Projected Hire, Start, or Submission Date. When the proposer starts the HR action, the when date defaults to the
projected hire date of the offer. If the proposer changes the when date and goes to the individual compensation section,
the plan payment dates adjust automatically. If the proposer changes the when date later on, they need to delete and
add the individual compensation plans again, with the correct payment dates.

For example, you've an internal candidate offer with the projected hire date of January 1, 2022. You then start
processing the global transfer with a when date of January 1, 2022. The transfer includes an individual compensation
plan with payments that start the same day. When you get to the individual compensation section, you see that the plan
has a payment start date of January 1, 2022. Before you submit the transfer, you revise the when date to February 1,
2022. When you get to the individual compensation section this time, the existing payment start date remains January
1, 2022. You need to delete the plan and add it again with the correct payment dates.

Started from a Page Other Than Manage Job Offers
The Projected Hire, Start, or Submission Date option works the same as the Start or Submission Date option. When the
proposer sets the when date and goes to the individual compensation section, the section sets the payment dates to
the when date. After that, if the proposer changes the when date, they need to delete the plan and add it again with the
correct payment dates.

190

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 33
Access and Action Options, and Option Visibility in
Individual Compensation Plans

33  Access and Action Options, and Option
Visibility in Individual Compensation Plans

Plan Access Restrictions

You control the situations when a manager can create, update, or discontinue individual compensation awards using
plan restrictions. These same restrictions let you control similar actions for people contributing to savings and donation
plans.

You configure these restrictions when you create the individual compensation plan using the Individual Compensation
Plans task in the Compensation work area.

Whether to Restrict Access
The first decision you make on the Plan Access tab is whether to restrict access to the plan.

•

•

If you select No, the plan becomes available to everyone on all pages where people hire individuals, or manage
individual compensation or personal contributions. It's very rare that you'd select this option. For example,
if you don't restrict access to a bonus plan, then people could manage the bonus plan for themselves. That's
because the plan would appear in the Manage Personal Contributions action.

If you select Yes, you need to add at least one action where the plan should be available. Make sure that you
select all related actions. For example, you set up the plan so that it's visible in the Pending Worker action.
You also want to make it visible in the Hire action. Otherwise, when someone converts to an employee, their
manager can't see the allocation. And, when the manager submits their changes, the employee's allocation gets
removed. You can optionally configure the corresponding access details about when people can start, update,
or stop allocations or contributions.

All Action
The default action All is similar to setting Restrict Plan Access to No, except that you can configure access details. This
action opens plan access to all actions available in the list, including the Manage Contributions action. Basically, anyone
who meets the eligibility criteria for the plan can see the plan. If you added this action to a bonus plan, for example,
anyone eligible for the plan could award themselves a bonus.

To add other access actions, you need to change the All action to something else, such as Hire. Then, the Add icon is
available and you can add any other access actions that are appropriate for the plan.

HR Actions
To make the plan available to people as part of an HR action, add one or more HR actions. For example, add the Transfer
action to a moving allowance plan to make the plan available when people transfer someone using that action.

To make the plan available to recruiters creating or editing job offers, you need to add the same action that they select
in the offer. For example, the recruiter selects the Add Pending Worker or Add Assignment action while creating the
offer. The individual compensation plan access needs to include the same action for the plan to appear in the Other
Compensation section of the job offer.

191

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 33
Access and Action Options, and Option Visibility in
Individual Compensation Plans

Manage Individual Compensation Action
To make the plan available to people when they want to award off-cycle compensation to someone, add the Manage
Individual Compensation action. You can add only this action or also add HR actions. For example:

• You want managers to use the Bonus plan to reward performance. So, you restrict plan access to the Manage

Individual Compensation actions.

• You want managers to use the Bonus plan to award hiring bonuses or to reward performance. So, you restrict

plan access to the Hire and Manage Individual Compensation actions.

Administer Individual Compensation Action
To make the plan available to only HR specialists, compensation specialists, and compensation managers, add
the Administer Individual Compensation action. These people can see plans with this plan access action using the
Administer Individual Compensation task.

Manage Contributions Action
To make the plan available for people to contribute to, such as for retirement savings or charities, add the Manage
Contributions action. Don't add any other actions for contribution plans.

The Difference Between Plan Access Restriction and
Access Security

Access security identifies which roles grant access to actions, such as Individual Compensation, Manage Personal
Contribution, and Administer Individual Compensation.

Plan access restriction identifies which actions, such as Personal Contribution or Individual Compensation, show the
plan. It also lets you control if people can add, edit, or delete contributions or allocations.

Copy Individual Compensation Allocations During Local
and Global Transfer

You can ensure that local and global transfers automatically copy individual compensation allocations and personal
contributions to the new assignment. Do this when you configure plan access for individual compensation plans.

Either set Restrict Plan Access to No. Or set it to Yes and add the Global Transfer action.

Tip:  When the plan element uses the Last Standard Process Date or Last Standard Earning Date date, the plan isn't
end dated for the source assignment.

192

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 33
Access and Action Options, and Option Visibility in
Individual Compensation Plans

When Allocations and Contributions Aren't Copied
The automatic copy doesn't happen for these situations:

•

•

•

If the legal employers for the source and destination assignments have different legislative data groups

If the local and global transfer action doesn't include the Individual Compensation section, or the person
proposing the transfer don't visit the section

If Restrict Plan Access is Yes and the Global Transfer action isn't added

Individual Compensation Plan and Option Visibility

Your plan configuration decides whether people can see the plan or option when they use the Administer Individual
Compensation, Individual Compensation, and Manage Personal Contribution tasks.

The person getting the compensation allocation or making the personal contribution needs to meet these conditions:

• Be eligible for the element you associated with the option.

• Meet the criteria of the eligibility profile you associated with the plan, option, or both.

Also, the plan status needs to be Active and plan access should have the appropriate actions added. For example, to be
visible for the Manage Personal Contributions task, plan access needs to have the Manage Contribution action.

Related Topics

• Plan Access Restrictions

193

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 33
Access and Action Options, and Option Visibility in
Individual Compensation Plans

194

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 34
Example Individual Compensation Plan Configurations

34  Example Individual Compensation Plan
Configurations

Spot Bonus and Stock Grant Plan Configuration

Here's how you create a plan to make a onetime spot bonus payment or stock grant.

1. Create a payroll element that makes a onetime payment. Configure the element to process once per payroll period

and let managers enter the payment amount or grant quantity.

Go to My Client Groups > Compensation > Elements.

2. Create the plan.

a. Go to My Client Groups > Compensation > Individual Compensation Plans.
b. Add an option with the payroll element. For stock grants, be sure to set the nonmonetary units to Shares

and select the grant type.

c. Select a payment or grant start date. If it's present, leave the end date blank to indicate this is a onetime

payment.

d. Optionally, add an eligibility profile to limit the people that the plan applies to. For example, use derived

factors to identify full-time people with a minimum service of 1 year as eligible for the spot bonus. Identify
full-time people with a minimum service of 5 years as eligible for the stock grant.

e. Restrict access to specific HR actions, such as Hire and Promote. Also add the Manage Individual

Compensation action so that managers can award bonuses or grant stock to their people using the
Individual Compensation action.

Stock grant records get the stock or trading symbol and grant type from the plan option. They get the grant date and
number of shares granted from the element entries.

Car Allowance Plan Configuration

Here's how you create an ongoing car allowance plan with two payment options. The options vary according to the
distance of regional territories from headquarters.

1. Create two payroll elements to make recurring payments once a month. For territories within a 100-mile radius of

headquarters, set the input value default to 300. For territories beyond a 100-mile radius, set the input value default
to 500.

Go to My Client Groups > Compensation > Elements.

195

Oracle Fusion Cloud Human Resources
Implementing Compensation

2. Create the plan.

Chapter 34
Example Individual Compensation Plan Configurations

a. Go to My Client Groups > Compensation > Individual Compensation Plans
b. Configure an option for each payroll element.
c. Let managers enter payment start and end dates according to agreements with their people. For example,
a manager starts payment on the first of the month or the first payroll period after a promotion. They end
payment after 1 year.

d. Attach an eligibility profile that limits plan eligibility to people with the Regional Sales Manager job.
e. Restrict access to specific HR actions, such as Hire and Transfer. Also add the Manage Individual

Compensation action so that managers can award or update the car allowance for their people using that
action.

f. Optionally, add instructions that tell managers how the payment policy varies according to the distance

from headquarters. And, include a link to the policy.

Charity or Savings Contribution Plan Configuration

Here's how you create a plan that lets people manage their personal contributions.

1. Create a payroll element to accept recurring contributions per payroll period. Configure the input value to be either a

flat amount or percentage.

Go to My Client Groups > Compensation > Elements.

2. Create the plan.

a. Go to My Client Groups > Compensation > Individual Compensation Plans.
b. Add an option for contributions of either amount or percentage.
c. Select a start date, typically January 1 of the next calendar year or after open enrollment.
d. Restrict access to the Manage Contributions action to let people manage their instances of the plan.

You can define periods when people can enroll for the first time, update existing contributions, or stop
contributions. For example, let people always create allocations. Restrict when they can make updates or
discontinuations to a specified period, such as an open enrollment period of November 15 through 30.

e. Optionally, add instructions that clarify specific plan policies.

196

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 35
Compensation History

35  Compensation History

Compensation History Categories

Compensation history has a summary table with four categories--Salary, Stock, Other Compensation, and Recurring
Payments--and links to compensation details. Summary info covers 5 years of history while details cover all years.

Salary
The Salary category has these three rows of information:

Row

Overall Salary

Comments

For the current year, it's the most recent pay rate. The rate appears in the frequency of the person's
salary basis, such as hourly, monthly, or annually.

For previous years, it's the pay rate on 31 December of that year.

Annualized rate

Calculated using the person's overall salary and the annualization factor of the salary basis frequency
as of 31 December of that year.

Percentage change

The difference in the person's overall salary from the previous year, if history exists.

In the summary table, click the base pay link to view detailed information about salary history, percentage change,
compa-ratio, and growth rate. The detail view includes links to individual base pay change records.

Stock
The Stock category shows a total for each grant type awarded in the unit granted, such as shares or options. In the
summary table, click the grant name to view more information, such as grant date, vested shares, and the estimated
value of unvested shares.

Other Compensation
The Other Compensation category shows nonrecurring monetary compensation, such as commissions, bonuses,
overtime, and reimbursable expenses. In the summary table, click the compensation name to view effective date,
amount, currency, and grand total information about all awards.

You can see elements information with only input values that are numbers, integers, and money because history was
designed for monetary and quantity compensation. For example, you can see salary, bonus, and allowance amounts
and quantities of vested, unvested, exercised, and unexercised stock shares. Also, the overall view shows various totals,
which history can't calculate for nonmonetary and nonnumeric values.

197

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 35
Compensation History

Recurring Payments
The Recurring Payments category includes the latest amount of recurring compensation, such as car allowances and
education assistance. In the summary table, click the payment name to view effective date, amount, currency, and grand
total information for an individual award or compensation amounts.

Related Topics

• How You Set Up the Other Compensation and Recurring Payments Summary Data for Compensation History

How You Set Up the Other Compensation and Recurring
Payments Summary Data for Compensation History

You set up the summary table data that shows in the Other Compensation and Recurring Payments compensation
history categories. Go to My Client Groups > Compensation > Compensation History.

The Other Compensation category groups one-time payments, such as bonuses. The Recurring Payments category
groups nonbase pay distributions, such as allowances or tuition reimbursements. To include compensation in these
history categories, on the Compensation History page, select the appropriate payroll elements and corresponding input
values. The payroll element definition automatically supplies the remaining data and identifies the history category
based on the recurrence of the payroll element.

Compensation history automatically gets the applicable Salary and Stock summary data, you don't need to do any
setup.

Related Topics

• Compensation History Categories

198

Oracle Fusion Cloud Human Resources
Implementing Compensation

36  Stock Grants

Chapter 36
Stock Grants

Manage Stock Grants in the Integrated Workbook

You can add and edit stock grant data and upload it into the application using an integrated Microsoft Excel workbook.

1.

In the Compensation work area, click Manage Stock Grants.

2. On the Manage Stock Grants page, click Prepare Import Spreadsheet.

3. Copy the stock grant data provided by your supplier. Make sure that each row contains a unique grant date, grant ID,

and grant number. The workbook adds a symbol in the Changed field to mark the rows that you added.

CAUTION:  Don't delete or reorder template columns. The upload process might fail.

4. When you're done, click Upload. The application uploads only those rows that are marked as Changed and ignores

any changes in cells that don't have a white background.

CAUTION:  Don't select the Upload and then immediately download option when prompted during an upload.
The data that you uploaded immediately downloads back into the workbook, hiding any errors that occurred
during the upload.

5. Validate the changes.

a. Open the Manage Stock Grants page and search for and view the imported stock grant data.

6. Resolve errors. The upload process automatically updates the Status field in each workbook row.

If there are errors that require review, the process:

a. Rolls back the change in the application.
b. Sets the workbook row status to Upload Failed
c. Continues to the next workbook row

To view and resolve an error:

In the Status field, double-click Update Failed.

a.
b. Fix any data issues in the workbook.
c. Upload the latest changes.

Related Topics

• How can I import stock data sent to me by my supplier?

• Set Up Desktop Integration for Excel

• Guidelines for Using Desktop Integrated Excel Workbooks

• Troubleshoot Desktop Integration for Excel

199

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 36
Stock Grants

FAQ

How can I import stock data sent to me by my supplier?

On the Manage Stock Grants page, use the Prepare Import Spreadsheet button to generate the stock table spreadsheet.
Enter your supplier's data, ensuring that each row contains a unique Grant Date, Grant ID, and Grant Number. Upload
the information into the stock table.

200

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 37
External Data

37  External Data

External Compensation Data

You can add compensation-related information from third-party and legacy applications, such as pension, annuity,
royalty, and assignment segments. You can include this external data as default values in worksheet columns for
workforce compensation plans.

You can also include it as compensation items in total compensation statements.

Person by Person or Many People at a Time
You can manually enter data for one person at a time using the External Data task in the Compensation work area. On
the same page, you can use the Prepare Import Spreadsheet button to import external data for many people at a time.

Data to Add
Here's the data you add, regardless of method:

• Record type

• Start Date

• End Date

• Sequence Number

• Currency

• Columns, such as Column 01 and Column 02

To avoid difficulties when adding other data in the future, be sure to provide all relevant data, such as end date,
sequence, and currency. For example, if you're external data includes amounts, you might need the currency to ensure
calculations handle the amounts correctly.

Person-Level Data to Assignment-Level Data
You can add external data at the person or assignment level. Adding it at the assignment level lets you use assignment-
level security. You can update personal-level external data to assignment-level using the Update Assignments process.
The process updates the data to the primary assignment as of the start date for the external data record.

Related Topics

• Record Type Lookups for External Compensation Data

•

Import External Compensation Data in the Integrated Workbook

201

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 37
External Data

Record Type Lookups for External Compensation Data

When you import data from third-party or legacy applications, you need to select the record type. The record types in
the choice list come from the CMP_EXTERNAL_DATA_RECORD_TYPE lookup type.

You can change delivered values, such as data from a third-party supplier application, at any time. And you can add new
values. For example, you add a lookup code to identify data from the third-party partner that manages your pension,
annuity, royalty, or 401k.

Use the Lookups task in the Compensation work area.

Related Topics

• Overview of Lookups

Import External Compensation Data in the Integrated
Workbook

You can enter and edit external compensation data, such as third-party or legacy data, using an integrated Microsoft
Excel workbook. Then, upload the data into the application.

Before you start

You might optionally want to create your own lookup codes if you find the two delivered codes too
broad. For example, you might want to create lookup codes for pension or sales incentive data. Add a
CMP_EXTERNAL_DATA_RECORD_TYPE lookup code using the Manage Lookups task in the compensation work area.

To use the imported data, you need to complete one or both of these tasks, either before or after the import:

• To use the external data in workforce compensation, configure one or more user-defined worksheet columns.

• To show external data in total compensation statements, create one or more compensation items with a source

type of External Data.

Here's what to do

1.

In the Compensation work area, Common Configuration section, click Manage External Data.

2. On the Manage External Data page, click Prepare Import Spreadsheet to create the workbook.

3. Enter the external data.

Add enough rows to accommodate your supplier's data. Copy the external compensation data and paste them into
cells with a white background. The workbook adds a symbol in the Changed field to mark the rows that you added.
Reordering or removing columns in the import file causes the upload process to fail.

202

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 37
External Data

4. When you finish, click Upload. The application uploads only those rows marked as Changed. It ignores any changes

in cells without a white background.

CAUTION:  Don't select the Upload and then immediately download option when prompted during an upload.
The data that you uploaded immediately download back into the workbook, hiding any errors that occurred during
the upload.

5. Validate the changes.

a. On the Manage External Data page search for and select the start date and record type, or other search

criteria.

6. Resolve the errors.

The upload process automatically updates the Status cell in each workbook row. If there are errors that require
review, the process:

a. Rolls back the change in the application.
b. Sets the workbook row status to Upload Failed
c. Continues to the next workbook row

To view and resolve an error:

In the Status field, double-click Update Failed.

a.
b. Fix any data issues in the workbook.
c. Upload the latest changes.

New uploads to existing data make date-effective changes to the data.

Related Topics

• Record Type Lookups for External Compensation Data

• Set Up Desktop Integration for Excel

• Guidelines for Using Desktop Integrated Excel Workbooks

• Troubleshoot Desktop Integration for Excel

How can I add external compensation data for multiple
assignments?

Enter a unique assignment ID for each row of data on the Manage External Data page of the Compensation work area.

Delete External Data in Compensation

On the External Data page, Actions menu select either Purge Entire Table or Delete Records Matching Criteria.

Or you can use the HCM Data Loader (HDL) to delete selected rows (My Client Groups, Data Exchange).

203

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 37
External Data

204

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 38
Workforce Compensation Overview, Lookups, and Security

38  Workforce Compensation Overview,
Lookups, and Security

Overview of Workforce Compensation

Let managers and specialists allocate compensation, such as merit increases or stock grants, to groups of people on a
focal, anniversary, or periodic basis. This includes letting them promote people and rate performances while allocating
compensation, as well as communicating compensation changes.

Also set up managers so they can automatically calculate and allocate compensation using models and analyze
proposed changes to ensure outcomes like these:

• Equity among peer groups and by manager

• Alignment with the market and with organizational compensation strategies for performance

You do all of this when you set up your workforce compensation plans. The setup involves configuring the foundation,
budgets, worksheets, models, and reports aspects of each plan. Managers and specialists use the worksheets to
propose compensation, performance ratings, and promotions. They also use them to approve proposed changes and
communicate the changes. You can also optionally extend certain lookups that people in various job roles use in the
workforce compensation cycle. And you can use a fast formula to retrieve data or run calculations on data.

Deep Links in Workforce Compensation

You can let people access workforce compensation from external sites or include workforce compensation in a
journey checklist. To use deep links in compensation, go to Navigator > Tools > Deep Links > search for workforce
compensation.

The deep link takes people to the workforce compensation landing page. People still need to navigate to the desired
plan. This prevents people from accessing plans where plan cycles are closed or are outside of the plan cycle dates.

Related Topics

• Deep Links

• Deep Links in Journeys

Reason Lookups

When you adjust a budget, you include a reason. The budget audit history shows this reason, along with the adjustment
and other budget changes. The CMP_BUDGET_AUDIT_REASONSlookup type already has the following reasons set up.

205

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 38
Workforce Compensation Overview, Lookups, and Security

The CMP_BUDGET_AUDIT_REASONS lookup type already has the following reasons set up. You can't change or delete
them, but you can add reasons that support your adjustment policies. The codes that start with CMP appear in audit
history.

• Worker eligibility change

• Eligible salary change

• Worker budget change

• Budget automatically issued

• Budget distributed by manager

• Manager budget change

• Worksheet budget change

• Worker reassignment

•

Initial budget

• Miscellaneous adjustment

• Supplemental funding

You configure lookups in the Compensation work area using the Lookups task.

Related Topics

• Overview of Lookups

Nonmonetary Unit of Measure Lookups

You use nonmonetary units of measure throughout workforce compensation, for example, to set up a compensation
worksheet for stock grants. The CMP_NONMONETARY_UOMlookup type already has these units of measure set up,
which you can change and add to, to support your compensation policies.

• Days

• Hours

•

Items

• Shares

• Units

You configure lookups in the Compensation work area using the Lookups task.

Related Topics

• Overview of Lookups

User-Defined Column Lookups

To let managers select from relevant choice lists on task worksheets, you can enable a column and configure the
associated user-defined lookup type.

206

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 38
Workforce Compensation Overview, Lookups, and Security

For example, you create a user-defined column called Up For Promotion. Then you configure the related user-defined
lookup type with these meanings: Yes and No. Managers can use the user-defined column to indicate if people are up
for promotion.

These are the bundled user-defined column lookup types.

• CMP_CWB_CUST_COL_46_LIST

• CMP_CWB_CUST_COL_47_LIST

• CMP_CWB_CUST_COL_48_LIST

• CMP_CWB_CUST_COL_49_LIST

• CMP_CWB_CUST_COL_50_LIST

While the bundled lookup code Meaning is DEFAULT, any lookup codes you add need to be only numeric. The
meanings can be characters, numbers, or a combination of both. You configure lookups in the Compensation work area
using the Lookups task.

Related Topics

• Overview of Lookups

Workforce Compensation Security

The workforce compensation tasks, plans, and task worksheets that people can use and access depend on plans, user
roles, and security profiles setup.

Person Security Profile
To determine the managers a higher-level manager or specialist can switch to on the Workforce Compensation
page, you set up security profiles. The profiles also determine individuals that people can handle changes for on the
Administer Workers page in the Compensation work area. And, the profiles determine the people included in the full
administration download. The profiles don't affect the people managers see in the task worksheets of a workforce
compensation plan.

User Roles
Bundled job roles and duty roles determine the people who can use workforce compensation tasks and work with
workforce compensation plans. You can also create your own roles to grant or remove access to specific compensation
tasks.

Plan Configuration
At a more granular level than the profiles and roles, you can specify the managers who can access the plan tasks.
You can also specify the people they can see on each task worksheet using the plan hierarchy. To further limit plan
access, you can use plan access overrides and plan status controls. For example, you can make plans available to only
compensation administrators using the plan status controls.

207

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 38
Workforce Compensation Overview, Lookups, and Security

Reference
For more information about workforce compensation security, see Security and Workforce Compensation (document ID
1556468.1) on My Oracle Support at https://support.oracle.com.

Considerations for Securing Access to Workforce
Compensation Plans and Task Worksheets

Do you want to secure access to your workforce compensation plans and if so, how? Keep these key considerations in
mind when setting up various configurations:

• Do you want to let managers and HR specialists only view plans and let only compensation administrators

make changes? You can do this when you configure plan access as part of the foundation plan setup.

• Do you want to let managers change plan access for their subordinate managers? You can do this when you

configure approvals and notifications as part of the worksheets plan setup.

• Do you want to let managers change worksheet access for their subordinate managers? You can do this when

you configure actions as part of the worksheets display plan setup.

Here are some scenarios and example access configurations.

Scenario

Example Configuration

Workforce Compensation Plan Task

Limit compensation manager access using the
Act as Proxy task according to roles.

When you configure plan access, add roles
in the Roles with the Plan Access from the
Compensation Work Area section.

Configure Plan Access

Limit when managers access their plan
worksheets.

Configure Plan Hierarchies

To start, when you configure plan hierarchies,
 set a default access level to determine who
has immediate access, such as compensation
administrators. Or you can use a fast formula.

During the workforce compensation cycle,
 when managers can access their plan
worksheets, compensation administrators
can change manager access using the plan
approvals task. Or plan administrators can
change the worksheet display configuration
to enable the approvals task to let managers
change the access of their subordinate
managers.

Related Topics

• Workforce Compensation Plan Hierarchies

• Workforce Compensation Plan Access

208

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 39
Workforce Compensation Plans Overview

39  Workforce Compensation Plans Overview

Overview of Workforce Compensation Plan
Configuration

People use workforce compensation plans to allocate budgets to managers and compensation to groups of people
during a compensation cycle. The plans are highly configurable, so you can determine the specific tasks and
information that a plan provides to administrators, managers, and specialists. The setup page displays pertinent plan
details and existing budget, component, and worksheet configurations.

To set up a plan, use the Workforce Compensation Plans task in the My Client Groups > Compensation work area to
configure these aspects:

• Configure Foundation: Set up details, such as the employment records the Start Workforce Compensation
Cycle process evaluates for the plan. Also specify if the plan is active or inactive, configure eligibility, and
identify cycle dates that determine plan access and eligibility. Set hierarchies that determine whether people
have primary responsibility for the plan, can provide suggestions, or can only review the plan. And enable
currency switching and configure currency properties, set up plan access, and configure a feedback survey and
plan information.

• Configure Budgets: Specify how to distribute budgets, set up budget groups, and identify storage methods for

budget pools. Also track on-cycle and off-cycle compensation against the budget.

• Configure Worksheets: Determine which worksheets to include in a plan as well as display properties, dynamic

calculations, alerts, and assignment segments. Managers and specialists use these worksheets to propose
compensation, performance ratings, and promotions. They also use them to approve proposed changes and
communicate the changes.

• Configure Models and Reports: Let managers and specialists build compensation models that help them

align their budgets and compensation allocations with organizational pay practices and guidelines. Let them
automatically allocate modeled amounts according to each person's country, job, grade, and quartile. And
create Oracle Transactional Business Intelligence reports to give managers and specialists relevant contextual
information so that they can make informed compensation changes. Also configure plan filters and analytics.

Performance Considerations for Workforce
Compensation Plans

Watch video

You need to consider how responsive workforce compensation plans are when determining how many plans to create.
Plans can include a few or many simple dynamic calculations and few or many complex calculations. The more dynamic
calculations and the more complex the calculations, the slower the plans respond when people change different values.

To optimize plan performance, you want to create plans tailored to specific audiences. For example, compensation
administrators want to optimize compensation budgets and allocations across their client groups. They typically

209

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 39
Workforce Compensation Plans Overview

need more information to test different allocation scenarios beyond what the modeling functionality can handle. Line
managers though want the absolute minimum information that they need to make appropriate allocations across their
teams. And they want any contextual or background information about their people in reports or a detailed worksheet
that they can look at separately, as needed.

You create separate plans for each audience. The plans for compensation administrators include the dynamic
calculations and fast formulas that can slow plan performance. The plans for line managers include cross-references to
key calculations in the administrator plans, so the managers can see critical calculation results. And manager plans can
include fewer dynamic calculations with simpler conditions, as appropriate. Or you might let managers use models to
explore allocation scenarios instead of configuring dynamic calculations for their plans.

To further optimize plan performance, you want to validate each plan. Validation lets you check that the evaluation
order for dynamic columns is correct and generates the results expected by the plan audience. It also helps you
determine the optimal number of dynamic calculations and alerts to include so the plan responds as each audience
considers acceptable.

Related Topics

• Considerations for Securing Access to Workforce Compensation Plans and Task Worksheets

210

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 40
Foundation: Plan Details in Workforce Compensation

40  Foundation: Plan Details in Workforce
Compensation

Employment Records to Use in the Compensation Cycle

You can specify the employment records used by the Start Workforce Compensation Cycle and Refresh Workforce
Compensation Data processes when you configure plan details.

Primary Assignments
The processes include people and set their eligibility status according to only their primary assignments. Anyone
who has multiple assignments and a plan that uses a manager hierarchy appears only on their primary assignment
manager's worksheet.

All Assignments
The processes include people and set their eligibility status according to all of their assignments. Anyone who has
multiple assignments might appear on their manager's worksheet more than once. And they might have different
eligibility statuses. For example, they might have an Eligible status according to the primary assignment and an
Ineligible status according to another assignment. If the manager for each assignment is different, the individual might
appear on worksheets for multiple managers.

Employment Terms
The processes include people and set their eligibility status according to the employment terms of legal employers
using the three-tier employment model. If the plan uses a manager hierarchy, people appear on the primary assignment
manager's worksheet.

The processes exclude people whose legal employers have employment terms that use the two-tier employment model.

Any Assignment or Employment Term with a Salary
The processes include people and set their eligibility status for all of their assignments and employment terms that
have a linked salary record. If the plan uses a manager hierarchy, people appear on the primary assignment manager's
worksheet. Anyone who has multiple assignments with a salary record might appear on their manager's worksheet
more than once. They could have a different base salary for each assignment. And they might have different eligibility
statuses. For example, they might have an Eligible status according to the primary assignment and an Ineligible status
according to another assignment. If the manager for each assignment is different, the individual might appear on
worksheets for multiple managers, with different salaries for each.

The processes exclude people whose assignments and employment terms don't have a linked salary record.

211

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 40
Foundation: Plan Details in Workforce Compensation

Active and Inactive Workforce Compensation Plans

When you configure plan details, you need to specify whether the plan status is Active or Inactive.

Compensation cycles include active plans. At any time during specified cycle dates, line managers can access their
active plans using the Workforce Compensation task for their team. Even after approved changes transfer to HR,
compensation managers can view plans using the Compensation task for their client groups.

Subsequent workforce compensation processes exclude inactive plans. Line and compensation managers can't view
or update the plans. Typically, you use this status to create and test plans, or for obsolete plans. You can purge only
inactive cycles.

Compensation administrators can change the status back to Active at any time.

Actions and Reasons in Workforce Compensation

To provide context, all salary and assignment changes include an action and optional action reason. You need to select
the action when you configure plan details. The bundled action that you can set in plan details is Allocate Workforce
Compensation.

If the plan includes different task worksheets for different allocation types, such as merit increases, bonuses, and stock
shares, you don't select an action reason. If the plan focuses on a single action, you can select the appropriate action
reason. For example, you create a plan where managers change compensation according to performance evaluations,
so you select the Performance action reason.

The action and reason are stored with all salary and assignment changes that transfer to HR after the compensation
cycle is complete. Changes from the performance evaluation plan would show in people's salary history as Allocate
Workforce Compensation and Performance.

Here's a comprehensive list of the bundled compensation action reasons.

• Anniversary

• Career Progression

• Cost of Living Adjustment

• Market Adjustment

• Mass Adjustment

• Merit

• Performance

• Periodic Review

• Promotion

You can extend the available actions and action reasons using the Configure Actions and Action Reasons quick actions
under My Client Groups > Workforce Structures.

212

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 40
Foundation: Plan Details in Workforce Compensation

Related Topics

• Reason Lookups

• Action Framework

213

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 40
Foundation: Plan Details in Workforce Compensation

214

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 41
Foundation: Plan Eligibility and Cycles in Workforce
Compensation

41  Foundation: Plan Eligibility and Cycles in
Workforce Compensation

Workforce Compensation Plan Eligibility

You determine the people who are eligible and ineligible for allocations from workforce compensation plans with
eligibility profiles. Here are examples of available criteria:

• Personal, such as gender and home location

• Employment, such as assignment status, hourly or salaried, grade, job, and performance rating

• Derived factors, such as age, length of service, or a combination of both

• Other, such as formula and user-defined criteria

• Labor relations, such as bargaining unit, union, and collective agreement

Add the relevant profiles when you configure plan eligibility. You can also create additional profiles to add, as needed.

Tip:  Make sure that on your eligibility profiles, you set Assignment to Use to Specific assignment.

The profile configuration determines what it means to meet criteria. The Start Workforce Compensation Cycle and
Refresh Workforce Compensation Data processes set the status of people who meet inclusion criteria to Eligible. The
processes set the status of people who don't meet inclusion criteria, or who do meet exclusion criteria, to Ineligible. For
managers determined ineligible with subordinates determined eligible, the processes set the manager eligibility status
to Limited.

Related Topics

• How Plan Access, Eligibility, and Default Access Level for Plan Hierarchies Work Together

• How Eligibility Works With Other Objects

• Eligibility Profiles

How Required and Optional Profiles Determine
Compensation Eligibility

If you add only one eligibility profile, people have to meet the profile criteria before the processes can set their eligibility
statuses. This requirement is true, even if you don't select Required. Here's what the processes require when you add
multiple eligibility profiles:

•

•

If all profiles are optional, people have to meet the criteria of at least one profile before the processes can set
their eligibility statuses.

If all profiles are required, people have to meet the criteria of all profiles before the processes can set their
eligibility statuses.

215

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 41
Foundation: Plan Eligibility and Cycles in Workforce
Compensation

•

If some profiles are required, people have to meet the criteria of all required profiles and at least one optional
profile. Then the processes can set their eligibility statuses.

Related Topics

• How Eligibility Works With Other Objects

• Eligibility Profiles

Option to Track People Ineligible for a Workforce
Compensation Plan

You can track ineligible people when you configure plan eligibility. The Start Workforce Compensation Cycle and Refresh
Workforce Compensation Data processes include these people on the plan worksheets.

These people also appear on the Compensation work area, Administer Workers page. Each person has an eligibility
status of Ineligible and none of their fields are editable. Because these people are visible, plan managers and
administrators can change statuses to Eligible, as they deem appropriate. The approving manager reviews the status
and proposed compensation changes when determining whether to approve or reject the submitted plan.

Tip:  You can include ineligible people on worksheets and let managers hide them when they want by enabling the
Hide Ineligible Workers action for plan worksheets.

When you don't track ineligible people, administrators must manually process the people to include them in the plan.

Related Topics

• Actions Configuration for Communication, Compensation, Detail Table Only, Performance, and Promotion

Worksheets

How the Options to Track and Hide Ineligible People
Affect Plan Worksheets

You determine which people the Start Workforce Compensation Cycle and Refresh Workforce Compensation Data
processes include on the plan worksheets.

Track Ineligible Workers

Hide Ineligible Workers

Worksheet Effects of Start
Process

Worksheet Effects of Refresh
Process

Selected

Selected

Selected

Cleared

Doesn't add newly evaluated
people it found ineligible to the
worksheet.

People found ineligible midcycle
drop off the worksheet.

Adds newly evaluated people it
found ineligible to the worksheet.

People found ineligible midcycle
remain on the worksheet.
This includes people whose

216

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 41
Foundation: Plan Eligibility and Cycles in Workforce
Compensation

Track Ineligible Workers

Hide Ineligible Workers

Worksheet Effects of Start
Process

Worksheet Effects of Refresh
Process

Cleared

Cleared

Selected

Cleared

Doesn't add newly evaluated
people it found ineligible to the
worksheet.

Doesn't add newly evaluated
people it found ineligible to the
worksheet.

termination date is between the
cycle evaluation start date and the
HR data extraction date.

People found ineligible midcycle
drop off the worksheet.

People found ineligible midcycle
remain on the worksheet. This
includes people who meet the
eligibility criteria and whose
termination date is between the
cycle evaluation start date and the
HR data extraction date.

Eligibility Profile Testing for a Workforce Compensation
Plan

You can test the eligibility profiles you add when configuring plan eligibility. The test lets you select a cycle, a sample
person, and an active assignment for your test.

Data security applies, so the person and assignment you can see for the cycle depend on your privileges. If profile
criteria includes fast formula, you can see if it worked correctly by reviewing the formula logs. Data security applies, so
the person and assignment you can see for the cycle depend on your privileges.

Workforce Compensation Plan Cycle Dates

You determine various aspects of workforce compensation cycles, such as plan access and eligibility, when you
configure plan cycle dates. You can reuse workforce compensation plans across multiple cycles, with a unique set of
dates for each cycle.

Here's a comprehensive list of the dates you can set.

Date

Description

Evaluation Period Start and End Dates

Period in which, such as a calendar or fiscal year, a quarter, or a month, when you can evaluate
groups of people for compensation allocations. Typically, fast formulas use these evaluation periods.
Informational only.

Plan Access Start and End Dates

Read-only period when managers can see their active plans. For example, they can review their people
and contextual information to prepare for upcoming allocations.

Worksheet Update Period Start and End
Dates

Active period when managers and administrators can make changes to their active plans.

217

Oracle Fusion Cloud Human Resources
Implementing Compensation

Date

Description

Chapter 41
Foundation: Plan Eligibility and Cycles in Workforce
Compensation

HR Data Extraction Date

When the Start Workforce Compensation Cycle process initially extracts person and assignment data
from HR employment records, and places it in the compensation tables. Also the date that the Refresh
Workforce Compensation Data process uses to update the data already in the compensation tables.

Eligibility Determination Date

When the Start Workforce Compensation Cycle and Refresh Workforce Compensation Data
processes evaluate the specified employment records to determine people's eligibility status.

Currency Conversion Date

When the Start Workforce Compensation Cycle and Refresh Workforce Compensation Data
processes obtain conversion rates from the general ledger daily rates table. Plans use the rates to
convert monetary amounts for different currencies.

Performance Rating Date

Date that identifies which workforce compensation plans share changes to compensation performance
rating. Plans with the same date share any rating changes.

Default Promotion Effective Date

To include performance rating information in compensation change statements, you need to select a
date. But, the date doesn't affect the sharing of development and performance ratings between Oracle
Fusion Performance Management Cloud Service and the workforce compensation plan.

When the Transfer Workforce Compensation Data to HR process sets everyone's job, grade,
 and position changes to take effect. Date the Start Workforce Compensation Cycle and Refresh
Workforce Compensation Data processes use to get the new salary range, compa-ratio, and salary
metrics for people whose grade changed.

To make proposed promotions available in multiple plans when managers promote people, use
the same date across the plans. Also, you can let managers override this date when you configure
worksheet column properties. Or you can set an override date when you run the Transfer Workforce
Compensation Data to HR process.

Default Due Date

When managers need to submit their plan changes.

You can configure different due dates by hierarchy level. Optionally, you can notify managers when a
date changes.

Market Composites Effective Date

When the Start Workforce Compensation Cycle process extracts market composite information.
It places the information in the compensation tables according to job or position, and location or
segment.

218

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 42
Foundation: Hierarchies in Workforce Compensation Plans

42  Foundation: Hierarchies in Workforce
Compensation Plans

Workforce Compensation Plan Hierarchies

You can give multiple managers different levels of access to people's allocation during a compensation cycle when you
configure hierarchies for workforce compensation plans.

These hierarchies determine the primary and secondary plan managers and the people they see in their worksheets.
It also determines the plan reviewers and the people they see. The primary hierarchy also determines how budgets roll
down to subordinate managers and approvals route to higher-level managers.

Examples
Here are some scenarios and examples of how you can configure hierarchies.

Scenario

Example Hierarchies

Country leaders need to manage the
budget and line managers need to allocate
compensation for their organization.

Set the source of the primary hierarchy to Other Manager Hierarchy and then select the appropriate
manager type for the country leader.

Set the source of the secondary hierarchy to Primary Manager Hierarchy.

Dotted-line managers need access to
people's compensation, for example,
if they completed projects for these
managers during the compensation cycle.

Set the source of the primary hierarchy to Primary Manager Hierarchy.

Set the source of the secondary hierarchy to Other Manager Hierarchy and select the appropriate
manager type for the dotted-line managers, such as Project Manager. Or you can use a fast formula
to determine the dotted-line relationship.

Country-specific HR specialists need
access to everyone in their country,
regardless of who people's primary plan
managers are.

Set the source of the primary hierarchy to Primary Manager Hierarchy.

Set the source of the reviewers hierarchy to a fast formula that determines the country-specific HR
specialist.

Related Topics

• How Plan Access, Eligibility, and Default Access Level for Plan Hierarchies Work Together

• Configure Approvals for Workforce Compensation Plan Worksheets

• Considerations for Securing Access to Workforce Compensation Plans and Task Worksheets

• Primary, Secondary, and Other Workforce Compensation Plans

219

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 42
Foundation: Hierarchies in Workforce Compensation Plans

Options to Configure Workforce Compensation Plan
Hierarchies

To give multiple managers different levels of access to the same people, you can configure up to three hierarchies for a
single workforce compensation plan.

Source
To build the management and optional reviewers hierarchies for each plan worksheet, you select a source. You need to
select a source for the primary hierarchy, even if you don't configure secondary or reviewers hierarchies.

Source Option

How It Determines the Management Hierarchy

Primary Manager Hierarchy

Uses the primary manager associated with each person's assignment

To use the new HCM position management structure instead of primary managers, sync the position
managers with people's assignments. Then select this source. As position managers change, you need
to sync the managers and assignments again. Then run the Refresh Workforce Compensation Data
process.

Other Manager Hierarchy

Uses the specified manager type associated with each person's assignment, such as project, resource,
 or regional manager

To use this hierarchy instead of primary managers, make sure that the manager type you select is on
people's assignments. If the managers with that manager type change during an open cycle, you need
to update the assignments. Then run the Refresh Workforce Compensation Data process.

Formula

Position Tree

Uses the specified hierarchy determination fast formula

Uses the structure of the specified position tree

For this source to determine the correct hierarchy, you need to sync position managers to people's
assignments. Then use the primary line manager hierarchy.

Department Tree

Uses the manager defined for the specified department tree

Missing Managers
You can specify how to handle people who don't have a manager. The available options vary depending on the selected
source.

Missing Relationships
You can record missing relationships in the log files for the Start Workforce Compensation Cycle and Refresh
Workforce Compensation Data processes. When you select this option, the processes include hierarchy breaks in the
log files, for example, when a plan manager doesn't have a manager. Or when an individual doesn't have a primary
manager on their assignment. You want to correct hierarchy breaks so workforce compensation plans roll up properly
and include all eligible individuals.

220

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 42
Foundation: Hierarchies in Workforce Compensation Plans

Default Access Level
You decide the update and access levels for managers by selecting a default access level or by using a formula. You
might use a formula when you want to set up different access to different sets of managers. For example, you select a
formula that lets only managers at or above Grade M4 make updates. It also specifies that all other managers in the
source hierarchy get no access.

Changing the access level doesn't change the hierarchy.

CAUTION:  If you select Refresh default access level when you run the refresh data process and access changes,
the next time the refresh process runs, it resets access to the default.

Related Topics

• Workforce Compensation Plan Hierarchies

• Formula Type Is Compensation Hierarchy Determination

• Overview of Using Formulas

• HCM Trees

• How Line Managers Are Synchronized Using Position Hierarchy

Formula Type Is Compensation Hierarchy Determination

To build your own management or reviewer hierarchy for use in a workforce compensation plan, you can create
formulas using the Compensation Hierarchy Determination formula type. You select the formula when you configure
hierarchies for the workforce compensation plan.

Here's a comprehensive list of the contexts available to this type of formula:

• DATE_EARNED

• EFFECTIVE_DATE

• HR_ASSIGNMENT_ID

• END_DATE

• START_DATE

• HR_TERM_ID

• JOB_ID

• LEGISLATIVE_DATA_GROUP_ID

• COMPENSATION_RECORD_TYPE

• ORGANIZATION_ID

• PAYROLL_ASSIGNMENT_ID

• PAYROLL_RELATIONSHIP_ID

• PAYROLL_TERM_ID

• PERSON_ID

221

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 42
Foundation: Hierarchies in Workforce Compensation Plans

The database items available for this type of formula are related to Person, Assignment, Salary, Element Entries,
Compensation Record, and From and End Dates.

These are the input variables available to this type of formula:

Input Value

Data Type

Required

Description

CMP_IV_ASSIGNMENT_ID

Number

CMP_IV_PLAN_ID

CMP_IV_PERIOD_ID

Number

Number

CMP_IV_COMPONENT_ID

Number

CMP_IV_PERSON_ID

Number

CMP_IV_PLAN_START_DATE

CMP_IV_PLAN_END_DATE

CMP_IV_PLAN_EXTRACTION_
DATE

CMP_IV_PLAN_ELIG_DATE

CMP_IV_PERFORMANCE_EFF_
DATE

Date

Date

Date

Date

Date

CMP_IV_PROMOTION_EFF_DATE

Date

CMP_IV_XCHG_RATE_DATE

Date

Y

Y

Y

Y

Y

Y

Y

Y

Y

Y

Y

Y

Assignment ID

Plan ID

Period ID

Component ID

Worker ID

Plan Start Date

Plan End Date

Plan Extraction Date

Plan Eligibility Date

Performance Effective Date

Promotion Effective Date

Currency Conversion Date

These are the return variables available to this type of formula:

Return Value

Data Type

Required

Description

L_PERSON_ID

L_ASSIGNMENT_ID

Number

Number

Y

Y

Person ID of manager

Assignment ID of manager

Or

Return Value

Data Type

Required

Description

L_PERSON_NUMBER

Number

Y

Person number of manager

The Start Workforce Compensation Cycle and Refresh Workforce Compensation Data processes show this error
when they can’t find the assignment ID:

• Formula passed in an invalid person number <15465857>. Assignment ID couldn't be obtained.

This sample formula determines the manager of a person when the assignment_id is passed.

/***********************************************************
FORMULA NAME : Compensation Hierarchy Determination Formula

222

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 42
Foundation: Hierarchies in Workforce Compensation Plans

FORMULA TYPE : Compensation Hierarchy Determination
DESCRIPTION: Hierarchy determination fast formula which is based on assignment_id
************************************************************/

/*=========== INPUT VALUES DEFAULTS BEGIN =====================*/
INPUTS ARE CMP_IV_ASSIGNMENT_ID (number), CMP_IV_PLAN_ID (number), CMP_IV_PERIOD_ID (number)/*===========
 INPUT VALUES DEFAULTS ENDS======================*/

/*================ FORMULA SECTION BEGIN =======================*/
DEFAULT FOR CMP_IV_ASSIGNMENT_ID IS 0
L_PERSON_ID = '0' L_ASSIGNMENT_ID = '0'
 if (CMP_IV_ASSIGNMENT_ID = 100000008154060 ) THEN
(
L_PERSON_ID = to_char(-999) //-999 indicates top level
//Manager.
L_ASSIGNMENT_ID = to_char(-999)
)
ELSE
(
L_PERSON_ID = to_char(100000008153756)
L_ASSIGNMENT_ID = to_char(100000008154060)
)

RETURN L_PERSON_ID , L_ASSIGNMENT_ID

/*================ FORMULA SECTION END =======================*/

Related Topics

• Options to Configure Workforce Compensation Plan Hierarchies

• Formula Compilation Errors

• Formula Execution Errors

• When do I run the Compile Formula process?

• Example of Writing a Fast Formula Using Formula Text

Formula Type Is Compensation Default Access Level

To determine the access level for the selected workforce compensation plan hierarchy, you can create formulas using
the Compensation Default Access Level formula type. You select formulas of this type on the Configure Hierarchies
page.

Here's a comprehensive list of the contexts available to this type of formula:

• DATE_EARNED

• EFFECTIVE_DATE

• END_DATE

• START_DATE

• HR_ASSIGNMENT_ID

• HR_TERM_ID

• JOB_ID

• LEGISLATIVE_DATA_GROUP_ID

• COMPENSATION_RECORD_TYPE

223

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 42
Foundation: Hierarchies in Workforce Compensation Plans

• ORGANIZATION_ID

• PAYROLL_ASSIGNMENT_ID

• PAYROLL_RELATIONSHIP_ID

• PAYROLL_TERM_ID

• PERSON_ID

The database items available for this type of formula are related to Person, Assignment, Salary, Element Entries,
Compensation Record, and From and End Dates.

These are the input variables available to this type of formula:

Input Value

Data Type

Required

Description

CMP_IV_PLAN_ID

CMP_IV_PERIOD_ID

Number

Number

CMP_IV_PLAN_EXTRACTION_
DATE

CMP_IV_HIERARCHY_TYPE

CMP_IV_PLAN_START_DATE

CMP_IV_PLAN_END_DATE

CMP_IV_PLAN_ELIG_DATE

CMP_IV_PERFORMANCE_EFF_
DATE

Date

Char

Date

Date

Date

Date

CMP_IV_PROMOTION_EFF_DATE

Date

CMP_IV_XCHG_RATE_DATE

Date

CMP_IV_ASSIGNMENT_ID

Number

CMP_IV_PERSON_ID

Number

Y

Y

Y

Y

Y

Y

Y

Y

Y

Y

Y

Y

Plan ID

Period ID

Plan Extraction Date

Hierarchy Type

Plan Start Date

Plan End Date

Plan Eligibility Date

Performance Effective Date

Promotion Effective Date

Currency Conversion Date

Assignment ID

Worker ID

These are the return variables available to this type of formula:

Return Value

Data Type

Required

Description

UPDATABLE

READONLY

NOACCESS

Char

Char

Char

Y

Y

Y

Updatable

Read-only

No Access

This sample formula determines if a person is selected for a workforce compensation plan based on their
assignment_id.

/*******************************************************************
FORMULA NAME : Compensation Default Access Level
FORMULA TYPE : Compensation Default Access Level
DESCRIPTION : Assignment_id based selection fast formula

224

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 42
Foundation: Hierarchies in Workforce Compensation Plans

*******************************************************************/

/*=========== INPUT VALUES DEFAULTS BEGIN =====================*/
INPUTS ARE CMP_IV_ASSIGNMENT_ID (number), CMP_IV_PLAN_ID (number)
/*=========== INPUT VALUES DEFAULTS ENDS======================*/

/*================ FORMULA SECTION BEGIN =======================*/

l_hr_assign_id = get_context(HR_ASSIGNMENT_ID, -1)
L_DEFAULT_VALUE='UPDATABLE'

IF l_hr_assign_id = 100000016858755
THEN
(
L_DEFAULT_VALUE = 'UPDATABLE'
)
ELSE IF l_hr_assign_id = 100000016873381
THEN
(
L_DEFAULT_VALUE = 'NOACCESS'
)
ELSE IF l_hr_assign_id = 300100009424371
THEN
(
L_DEFAULT_VALUE = 'READONLY'
)
ELSE
(
L_DEFAULT_VALUE = 'READONLY'
)

RET=ESS_LOG_WRITE('L_DEFAULT_VALUE: '|| L_DEFAULT_VALUE)
return L_DEFAULT_VALUE
/*================ FORMULA SECTION END =======================*/

Related Topics

• Formula Compilation Errors

• Formula Execution Errors

• When do I run the Compile Formula process?

• Example of Writing a Fast Formula Using Formula Text

225

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 42
Foundation: Hierarchies in Workforce Compensation Plans

226

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 43
Foundation: Plan Currency, Access, Feedback Survey, and
Info in Workforce Compensation

43  Foundation: Plan Currency, Access,
Feedback Survey, and Info in Workforce
Compensation

Workforce Compensation Plan Currency

You can let managers switch between the corporate currency, their preferred currency, and their people's local
currencies. If you don't let people switch, then everyone sees monetary amounts in the corporate currency. You can also
specify the default currency to show in plan worksheets. You can select how to display the currency in the worksheet.
Options are currency code, currency name, and currency code and name.

Optionally, you can set a rounding rule to apply for a specified currency. For example, you want to round Euro (EUR)
to nearest 10 and US dollars (USD) down to .01. These rules apply to any monetary columns that you enable in the
worksheets when you set the column Rounding Rule to Use Currency Rounding.

Typically, you configure any rounding rules before running the Start Workforce Compensation Cycle process.
For changes made during the cycle to take effect in the plan worksheets, you need to run the Refresh Workforce
Compensation Data process.

Related Topics

• Enter Daily Rates Using the Daily Rates Spreadsheet

• Update Currency Rates

Workforce Compensation Plan Access

You can specify which job roles can and can't update workforce compensation plans when you configure plan access.
When you set Restrict Access to Yes and don't do anything else, no one can see the plan, let alone update it.

To let people with the appropriate roles make plan updates, add the roles to the appropriate work area and set access to
Allow updates. For example, you add the Line Manager role to the Workforce Compensation work area. You add the
Compensation Manager role to the Compensation work area. And you allow both roles to make updates.

To let people with the appropriate roles only read the plan, add the roles to the appropriate work area. Also set access
to No updates allowed. For example, you add reviewer roles to the Workforce Compensation work area and don't allow
updates.

To let people with the appropriate roles set up plans, add the roles in the plan setup access section. Also set access to
Allow updates. For example, you add the Compensation Administrator role to plan setup access and allow the role to
make updates.

227

Oracle Fusion Cloud Human Resources
Implementing Compensation

Related Topics

Chapter 43
Foundation: Plan Currency, Access, Feedback Survey, and
Info in Workforce Compensation

• How Plan Access, Eligibility, and Default Access Level for Plan Hierarchies Work Together

• Workforce Compensation Security

• Considerations for Securing Access to Workforce Compensation Plans and Task Worksheets

Delivered User Roles and Duty Roles

The tasks listed in the Compensation work area are the ones you need to administer workforce compensation plans.
Depending on your role, you might have access to some or all of the tasks. For example, the Compensation Manager
has access to worker data only, whereas the Compensation Administrator has access to plan configuration and setup
data only.

Here are the delivered user roles you can assign to people, along with the duty roles, tasks and the entitlement that
secures each task pane entry:

Role

Duty Role

Task Pane Entry

Entitlement

Compensation Manager

Compensation Manager Workforce

Act as Proxy

Administer Workers

Compensation Management Duty

View Administration Reports

Manage Global Models

Manage Workforce Compensation
When Acting as Proxy

Administer Workers for Workforce
Compensation

View Workforce Compensation
Administration Reports

Manage Workforce Compensation
Global Models

Compensation Administrator

Workforce Compensation Setup
Duty

Run Batch Processes

Run Group Compensation Batch
Processes

Manage Plans

Manage Active Plans

Define Compensation Plan
Definition

Manage Compensation Plan
Definition

Configure Global Settings

Manage Compensation Plan Global
Options for Group Compensation

Compensation Analyst

Compensation Workforce Analysis
Duty

View Administration Reports

View Workforce Compensation
Administration Reports

Manage Global Models

Manage Workforce Compensation
Global Models

Note:  These roles inherit other privileges that aren’t directly related to Workforce Compensation plan administration.
You can refer to the security reference manual for additional details.

228

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 43
Foundation: Plan Currency, Access, Feedback Survey, and
Info in Workforce Compensation

How Plan Access, Eligibility, and Default Access Level for
Plan Hierarchies Work Together

You determine who can access workforce compensation plans when you configure plan eligibility, hierarchies, and
access as part of the foundation plan setup.

Plan Access Configuration
Your plan access configuration determines the roles that can and can't access the plan. By default, all roles can access.

Plan Eligibility Configuration
Your plan eligibility configuration has the criteria that processes use to determine the individuals who are and aren't
eligible for the plan. If the plan access configuration lets managers access the plan and the managers have subordinates
eligible for the plan, the managers can see the plan. But if they don't have any subordinates eligible for the plan, the
managers won't see the plan.

Plan Hierarchies Configuration
Your plan hierarchies configuration determines the access level that managers have to the plan. If these conditions are
met, the managers can see the plan and task worksheets:

• The plan access configuration lets managers access the plan.

• The managers have subordinates eligible for the plan.

• The default access level for the primary plan hierarchy is Updates Allowed or No Updates Allowed.

If the default access level is No access, the managers can't see the plan or task worksheets. This happens even if the
other two conditions are met.

Related Topics

• Workforce Compensation Security

• Considerations for Securing Access to Workforce Compensation Plans and Task Worksheets

Workforce Compensation Plan Feedback Survey

Let the people who use the plan to allocate workforce compensation during compensation cycles give you feedback on
their experiences with the plan.

This feedback can help you determine if you need to further refine plans to different audiences, such as compensation
administrators and line managers. It can also help you refine what task worksheets and reports to include, and what
information to include in each worksheet and report. These kinds of changes help you improve productivity and
satisfaction with the plans over time.

229

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 43
Foundation: Plan Currency, Access, Feedback Survey, and
Info in Workforce Compensation

You can let people provide ratings for their experiences and include up to five survey questions. You can view survey
responses using the View Administration Reports task.

Related Topics

• Performance Considerations for Workforce Compensation Plans

Workforce Compensation Plan Information

You can provide additional information that administrators and managers might find useful when you configure plan
information.

You can include important information, such as the manager due date and evaluation and plan access periods from
cycle setup. You can also include text, for example, about new or updated compensation policies with links to relevant
details.

This information shows up as a task in workforce compensation plans, in the area with the Models and Reports tasks.

230

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 44
Budgets: Budget Display in Workforce Compensation Plans

44  Budgets: Budget Display in Workforce
Compensation Plans

Overview of Budget Display in Workforce Compensation
Plans

You determine the information that appears on the Manage Budget page and on the budget worksheet when you
configure the budget display. You also determine the actions available on the worksheet and provide information that
applies to the entire budget pool.

For example, you communicate policy changes that affect budget allocation and include links to detail information.

Overview Configuration in Budget Display

You can enable the columns that appear as overview information in the budget row on the Manage Budgets page. You
can also override the display name for some columns.

For example, you show the budget pool name and number of people eligible for the pool. And you change the Workers
label to Eligible People.

When the budget is monetary, the Units value is the plan currency, such as USD. When the budget is nonmonetary, the
Units value is whatever you selected for the budget pool, such as Shares for a stock budget.

Summary Configuration in Budget Display

You can enable the views that appear in the summary area of the budget worksheet, such as a scoreboard, a table, or
both.

231

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 44
Budgets: Budget Display in Workforce Compensation Plans

If you enable both views, you also specify which view appears by default when managers open the worksheet. Here's an
example budget worksheet with only the table view enabled.

You can enable the columns that appear on the view and override all of the default display names. For example, you
change Budget Distribution Percentage to Budget Distribution %. And you can override the default sequence of any
column, as appropriate to best support how your managers expect their analytics. For the table view, use the Refresh
icon on the Column Preview panel to see how the reordered columns will appear in the summary area.

You can also configure properties for the columns you enable, such as setting a rounding rule and the decimal places to
display. The actual properties vary depending on the column. All columns include a Plan Info property that you can use
to communicate useful information to managers. For example, you share the expression used to calculate the column
values, or add a definition for the column, such as explaining what is compa-ratio.

Detail Table Configuration in Budget Display

You can enable columns from manager information, eligibility, budget distribution, targets, published budgets, and
workforce allocation groups in the main table of the budget worksheet. You can also configure your own numeric
columns for your enabled compensation components using the miscellaneous rate columns.

Tip:  To prevent managers from inadvertently increasing their allocated budgets, don't enable the Worker List column
for worker-level budgeting. If you do enable the column, managers can adjust the budget amounts for individuals,
thus inadvertently increasing their allocated budgets.

232

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 44
Budgets: Budget Display in Workforce Compensation Plans

Display Names and Column Sequences
You can provide meaningful column names for plan audience by changing the default display names. For example, you
change Eligible Salary - Component 1 to Eligible Salary for Merit Increase. And you can change the default sequence
of any column, as appropriate. Use the Refresh icon on the Column Preview panel to see how the reordered columns
will appear in the table.

Column Properties
You can also configure general properties for the columns you enable as well as default values. The actual properties
depend on the column.

All columns include a Plan Info property that you can use to communicate useful information to plan audiences. For
example, you share the expression used to calculate the column values, or add a definition for the column, such as
explaining what is compa-ratio. When you include plan info for a column, people viewing the worksheet see a blue icon
with an i in it on the column header. They click the icon or hover over it to see the information.

Worker List Configuration in Budget Display

You can enable the columns that appear in the main table on the worker list page that managers open from the budget
worksheet. You can override all of the default display names.

For example, you change Budget Percentage to Budget %. And you can override the default sequence of any column,
as appropriate. Use the Refresh icon on the Column Preview panel to see how the reordered columns will appear in the
table.

You can also configure properties for the columns you enable, such as setting a rounding rule or a default and override
formula. The actual properties vary depending on the column. All columns include a Plan Info property that you can
use to communicate useful information to managers. For example, you share the expression used to calculate the
column values, or add a definition for the column, such as explaining what is compa-ratio.

233

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 44
Budgets: Budget Display in Workforce Compensation Plans

Note:  If you don't enable the Worker List column on the Detail Table tab, the managers can't open the worker list
page. Thus, they won't see any columns that you configure on the Worker List tab.

Actions Configuration in Budget Display

You can specify the options available on the Actions, View, and Format menus and on the detail table toolbar when you
configure the budget display.

You can also specify the actions available on the worker list page, such as Request Eligibility Change and Reassign
Workers to Another Manager.

234

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 44
Budgets: Budget Display in Workforce Compensation Plans

Note:  If you don't enable the Worker List column on the Detail Table tab, the managers can't open the worker list
page. Thus, they won't see any options that you configure on the Actions tab.

Related Topics

• Budget Worksheet Actions

• Compensation and Promotion Worksheet Actions

• Performance Worksheet Actions

• Approval Worksheet Actions

• Communication Worksheet Actions

Information Configuration in Budget Display

You can provide managers with important budgetary information in the header of the budget worksheet when you
configure the budget display.

For example, you can explain policies that apply to the budgets for the upcoming focal compensation cycle and include
links to details. You can also show important underlying calculations used to determine the results in various columns.

235

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 44
Budgets: Budget Display in Workforce Compensation Plans

236

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 45
Budgets Budget Pools in Workforce Compensation Plans

45  Budgets Budget Pools in Workforce
Compensation Plans

Overview of Budget Pools in Workforce Compensation
Plans

You can align focal compensation for your people with organizational strategies and policies using budget pools. Add
anywhere from zero to five budget pools to your workforce compensation plan.

For example, your plan has bonus, cost of living, merit, and stock compensation components. You can create
two budget pools, one pool for the monetary allocations and one pool for the shares allocations. You can create a
separate pool for each component. Or, you can use minimum and maximum options on the worksheet compensation
components, explained in a later chapter, instead of setting up any pools.

To configure budget pools, you enable budgeting and then create the budget pools.

CAUTION:  Any changes you make to an existing budget pool affects any open cycles. If you have an open cycle,
you'll need to either update the status for all cycles to Closed in Active plans or run the Back Out Workforce
Compensation Data process. After there are no open cycles, make your budget pool changes and then run the Start
Workforce Compensation Cycle process.

Related Topics

• Budget Pools and Compensation Components

• Overview of Budget Display in Workforce Compensation Plans

Budgeting Methods in Workforce Compensation Plan
Budget Pools

You specify whether budgets are worker or manager level when you configure budget pools.

Manager-Level Budgeting
You can specify whether to store budget amounts or percentages, automatically publish budgets, and allow over
budgeting for the linked plan compensation components. Then primary plan managers can set the budget method for
the budget worksheet, either the first time they open the budget, or on the worksheet. They can pass down budgets to
only their subordinate managers who report directly to them. Or, they can pass down budgets to all of their subordinate
managers in the primary hierarchy. Their selection determines the worksheet that opens.

The summary table doesn't show any budget information when managers filter worksheets to see information for their
subordinate managers two or three levels down. The summary table does show them a message that budget details

237

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 45
Budgets Budget Pools in Workforce Compensation Plans

aren't available for this level of filtering, as appropriate. They can see summary budget information when they filter for
their direct reports or all of their people.

Worker-Level Budgeting
You can store only budget amounts and only automatically publish budgets. You can't allow over budgeting. You can
also let managers monitor worker-level budgets and control spending by configuring a budget group.

Related Topics
•

Include a Budget Group in a Compensation Task Worksheet Summary

Budget Storage Methods in Workforce Compensation
Plan Budget Pools

You can store your budgets as amounts or percentages. The storage method you select affects published budgets when
managers reassign people to other managers or change their eligibility status.

Amounts
The published amounts stay with the manager when their total eligible salary changes, such as when they reassign
people or change their eligibility status. For example, you publish a $100,000 budget to David. David publishes budgets
for himself and his direct reports, Rosa and Lee, as shown here:

Manager

Total Eligible Salary (USD)

Calculated Budget Percentage

Stored Budget Amount (USD)

David

Rosa

Lee

Total

100,000

500,000

400,000

1,000,000

10

10

10

NA

10,000

50,000

40,000

100,000

Then Lee reassigns one of his people with an eligible salary of $100,000 to Rosa. This reassignment decreases his
calculated budget percentage and increases Rosa's, as shown here. The stored budget amounts remain unchanged.

Manager

Total Eligible Salary (USD)

Calculated Budget Percentage

Stored Budget Amount (USD)

David

Rosa

Lee

Total

100,000

600,000

300,000

1,000,000

10

8.3

13.3

NA

10,000

50,000

40,000

100,000

238

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 45
Budgets Budget Pools in Workforce Compensation Plans

Percentages
The published budget amounts change when a manager's total eligible salary changes, such as when they reassign
people or change their eligibility status. For example, you publish a budget to David as 10% of total eligible salary. David
publishes budget percentages for himself and his direct reports, Rosa and Lee, as shown here:

Manager

Total Eligible Salary (USD)

Stored Budget Percentage

Calculated Budget Amount (USD)

David

Rosa

Lee

Total

100,000

500,000

400,000

1,000,000

10

10

10

NA

10,000

50,000

40,000

100,000

Then Lee reassigns one of his people with an eligible salary of $100,000 to Rosa. Now Lee's total eligible salary
decreases and Rosa's increases, affecting their calculated budget amounts, as shown here:

Manager

Total Eligible Salary (USD)

Stored Budget Percentage

Calculated Budget Amount (USD)

David

Rosa

Lee

Total

100,000

600,000

300,000

1,000,000

10

10

10

NA

10,000

60,000

30,000

100,000

Related Topics

• Budget Worksheet Actions

Automatically Publish Budgets in a Workforce
Compensation Plan

You can specify whether the Start Workforce Compensation Cycle process automatically publishes budgets for
manager-level budget pools. The process always publishes worker-level budget pools automatically.

Every time you run the Start Workforce Compensation Cycle process, it distributes the new or updated budget pools
that have automatic publishing enabled. How the process distributes the budgets depends on how you setup key
columns when you configure budget display. This setup is explained in more detail in the next chapter.

The option to automatically publish budgets also affects how managers can distribute budgets using models.

239

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 45
Budgets Budget Pools in Workforce Compensation Plans

Manager-Level Budgeting
The process distributes budgets as amounts to all managers with at least one subordinate manager when you set up
these configurations:

• On the Summary tab, Table View, under Budget distribution, you can enable either the Distributed Amount
or Distributed Percentage column, or both. The enabled columns appear in the top table of the budget
worksheet, which shows the summary information for that primary plan manager's budget.

• On the Detail Table tab, under Budget Distribution, enable either the Distributed Amount or Distributed

Percentage column, or both. The enabled columns appear in the bottom table on the budget worksheet. The
table shows the budget information for each manager reporting to the primary plan manager.

• Optionally configure the column properties of only one of these four summary and detail columns to set a

default value.

Worker-Level Budgeting
The process distributes budgets as amounts or percentages at the worker level when you set up these configurations.

• On the Worker List tab, under Budget, enable either the Budget Amount or Budget Percentage column, or

both.

• Optionally configure the column properties of only one of these columns to set a default value.

The manager-level budgets are the sum of the individual worker budgets.

Models
If you configure models for the workforce compensation plan and enable automatic budget publishing, managers
can publish budgets as part of their modeling. If you configure models but don't enable automatic budget publishing,
managers can still use models to publish budgets. They have to take the extra step of going to the budget and
publishing the model changes there.

Budget Is in Nonmonetary Units for a Workforce
Compensation Plan

You can specify the budget units when you configure a budget pool. If you don't select the Budget is in nonmonetary
units option, the units are the corporate currency set for the plan, such as USD.

If you do select the option, you can specify the units, such as Days, Hours, Items, Shares, or Units.

Related Topics

• Nonmonetary Unit of Measure Lookups

240

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 45
Budgets Budget Pools in Workforce Compensation Plans

Reset Amounts When Budgets Are Unpublished in a
Workforce Compensation Plan

You can specify to reset amounts when budgets are unpublished, when you configure budget pools for a workforce
compensation plan. When the primary plan manager unpublishes budgets, they reset summary and detail values.

Summary View Table Changes
Managers can see the summary view table in the header area of their budget worksheet. If you enable reset amounts,
the unpublish action decreases the Budget Distribution Amount and Budget Distribution Percentage values by the
original budget distribution amount.

When managers change the Budget Amount to 0, they're also decreasing these summary values by the same amount:

• Budget Distribution Amount

• Budget Distribution Percentage

And they're increasing the Available for Distribution value by that same amount.

Detail Table Changes
Managers see the detail table in the main area of the budget worksheet. The table has separate rows for each of their
subordinate managers, in a hierarchical representation. If you enable reset amounts, the unpublish action clears the
Budget Distribution Amount, Budget Distribution Percent, and Unpublished Amount values in the detail section. It
also sets the Available Budget to 0.

Examples
Here are example summary and detail tables for the Merit budget worksheet before the manager unpublishes the
budget for a specific subordinate manager. The monetary amounts are in USD.

Summary Table Columns Before Unpublish

Eligible Salary

Budget
Amount

Budget %

Budget
Distribution
Amount

Available for
Distribution

Budget
Distribution %

Unpublished
Amount

Available
Budget

3,667,253

110,018

3

110,018

0

3

30,990

110,018

Detail Table Columns Before Unpublish

Manager

Eligible Salary

Budget Distribution
Amount

Budget Distribution
%

Unpublished Amount Available Budget

Direct Reports

763,300.36

22,899.01

Rosa

1,033,012.00

30,990.37

3.00

3.00

22,899.01

30,990.37

0

241

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 45
Budgets Budget Pools in Workforce Compensation Plans

Manager

Eligible Salary

Budget Distribution
Amount

Budget Distribution
%

Unpublished Amount Available Budget

Lee

Blair

1,174,646.00

35,239.38

696,294.36

20,888.83

3.00

3.00

35,239.38

20,888.83

20,888.83

Here are those same tables after the manager unpublishes Rosa's budget amount of 30,990.37.

Summary Table Columns After Unpublish

Eligible Salary

Budget
Amount

Budget %

Budget
Distribution
Amount

Available for
Distribution

Budget
Distribution %

Unpublished
Amount

Available
Budget

3,667,253

110,018

3

79,027.63

0

0

30,990

141,008.37

Detail Table Columns After Unpublish

Manager

Eligible Salary

Budget Distribution
Amount

Budget Distribution
%

Unpublished Amount Available Budget

Direct Reports

763,300.36

22,899.01

3.00

Rosa

Lee

Blair

1,033,012.00

1,174,646.00

35,239.38

696,294.36

20,888.83

3.00

3.00

22,899.01

0

35,239.38

20,888.83

20,888.83

Budget Enforcement Options for Workforce
Compensation Plan Budget Pools

You can let managers reward performance during the compensation cycle, beyond their allotted budgets. You can
provide this controlled flexibility when you configure budget pools.

Allow Over Budget When Budgeting
You can specify the maximum percentage over their allocated budgets managers can go when publishing budgets to
their subordinate managers. Do this by enabling the Allow over budget when budgeting option.

242

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 45
Budgets Budget Pools in Workforce Compensation Plans

Allow Over Budget When Allocating Compensation
You can specify the maximum percentage over their allocated budgets managers can go when allocating compensation
for their people. Do this by enabling the Allow over budget when allocating compensation option.

Severity When Over Budget
You can specify whether to show warnings or errors when managers budget or allocate compensation between the
published amount and the maximum overage. Managers get errors when they attempt to go over the maximum allowed
overage.

When Budget is Null
You can specify whether to show warnings or errors when managers try to budget or allocate compensation when there
is no published budget.

When Under Budget
You can specify whether to show warnings or errors when managers try to budget or allocate compensation under the
published amount.

Prevent Allocations When Budgets Are Null

When you configure a budget pool, you can prevent managers from submitting allocations before they're issued a
budget when you select a rule from the When Budget is Null list.

In the When Budget is Null list, select the Error preventing Save rule when you have configured plans with the Submit
Mode of Disable submit on the Configure Approvals and Notifications page in plan setup. You can also select to use
this option and change the Submit Mode to Disable submit in Active Plans and then change it back after you've issued
budgets.

Use the Error preventing Save and Submit rule when you configure plans with the Submit Mode of Submit anytime
or Only after approving all managers.

If you enable modeling, you can use models to apply compensation amounts while budgets are null. Worksheet
managers won't be able to make and save changes in the worksheet to applied amounts. If you've selected to have
compensation amounts filled as a part of the Start process using default values or dynamic calculations, managers
won't be able to make and save changes in the worksheet until you've issued a budget to them.

After you've issued a budget, configured budget validation rules apply.

243

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 45
Budgets Budget Pools in Workforce Compensation Plans

Budget Group Options for Workforce Compensation Plan
Budget Pools

To track and monitor worker-level budgeting for specific populations, you can set up a budget group. The budget
group lets you identify, for example, everyone in the same country or grade. You set up the group when you configure a
budget pool.

Related Topics
•

Include a Budget Group in a Compensation Task Worksheet Summary

244

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 46
Worksheets: Overview and Basic Configuration Processes
for Key Columns and Actions

46  Worksheets: Overview and Basic
Configuration Processes for Key Columns and
Actions

Overview of Task Worksheets in Workforce
Compensation Plans

Compensation administrators optimize compensation budgets and allocations across their client groups using
task worksheets in workforce compensation plans. Managers and specialists also use task worksheets to propose
compensation, performance ratings, promotions; to approve proposed changes; and to communicate the changes.

You can vary the worksheets that you include in a plan to best support the plan audience in their compensation tasks.
Worksheets consist almost entirely of columns and actions. When you configure the page layout for a task, you enable
summary views and columns, detail table columns, and detail table actions.

• Configuration can be straightforward, such as enabling the Personal > Country column.

• Configuration can involve interdependencies, such as between actions and columns. For example, to let

managers rank their people, you need to enable the Performance > Ranking column in the detail table. You
also need to enable the appropriate rank worker actions. And to let managers see full details about someone's
ranking, you need to enable the Right Click Menu > View Ranking Details action.

For all worksheet columns, you can set column properties. The available properties depend on the column.

Type

General

Examples

Column shading, rounding rule, and decimal precision.

Visibility and access

Line managers can only read the column data but compensation administrators read and edit it.

Default value

A specific number or text; or values provided by a specified formula, compensation derived factor, or
from a cross-referenced column.

Salary and element mapping

Post a single payment or base pay adjustment and select the payroll element to use.

Information

The formula or dynamic column condition used to determine the column amounts or the source of the
column data.

For many columns, you can also build dynamic conditions, for example, to ensure that proposed changes don't exceed
existing compensation by a specific maximum.

To include data not already available in the provided columns, you can enable and configure miscellaneous rate and
user-defined columns. For example, you can use user-defined columns to share external data, such as market data
supplied by third parties.

245

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 46
Worksheets: Overview and Basic Configuration Processes
for Key Columns and Actions

While you can go straight to configuring worksheet columns as part of configuring worksheet displays, it's worth
completing other, related configurations first. Here are some examples of configurations with interdependent
configuration tasks:

•

Include prorated values for relevant worksheet columns by setting up assignment segment options.

• Specify how to determine local currencies for a compensation component, and if the component units should

be nonmonetary, such as Days or Shares.

• Share performance ratings and changes between Oracle Fusion Performance Management Cloud Service and

compensation plan worksheets.

• Designate review hierarchies that are separate from the primary manager hierarchy. Also override any global
notification settings, as appropriate for the specific plan. For example, you have a global setting for how
everyone publishes and withdraws budgets, but want to change the settings for a specific plan.

• Specify how to generate and store statements that managers use to communicate compensation changes to

their people.

• Build and enable the alerts that plan worksheets need to include.

You configure plan worksheets using the Workforce Compensation Plans task, Worksheets task list in the My Client
Groups > Compensation work area. The other topics in this chapter have the basic processes to fully configure alerts,
compensation change statement, compensation component, and performance rating columns. It also has basic
processes to fully configure worksheet models and filters for worksheets and reports. The following chapters have
information about each task in the Worksheets task list.

Reference
For descriptions of every worksheet column and action, see Workforce Compensation Worksheet Configuration
Definition (document ID 1450891.1) on My Oracle Support (support.oracle.com). To help you locate columns and actions,
the document tabs organize information in the same groupings as the Configure Worksheet Page Layout pages.

For columns, the document has this information:

• The navigation path for columns that map directly to a field in Oracle Fusion Global HR Cloud Service

•

•

If you can default column values using a plan cross-reference

If people can update the values in their plan budget and task worksheets

For actions, it tells you about any dependent configurations you need to complete.

Related Topics

• Overview of Worksheet Display in Workforce Compensation Plans

• Miscellaneous Rate Component Columns and User-Defined Columns

• Performance Considerations for Workforce Compensation Plans

• Overview of Workforce Compensation Plan Configuration

Include Alerts in Task Worksheets

Here's the basic process to include alerts in the task worksheets of a workforce compensation plan:

246

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 46
Worksheets: Overview and Basic Configuration Processes
for Key Columns and Actions

1. Enable predefined alerts and create and enable your own alerts using the Configure Alerts task. All the enabled
alerts for the plan appear in the enabled Alert column of every enabled worksheet when the alert conditions are
met. You can't enable different alerts for different worksheets. You can elect to not complete step 3 for various
worksheets.

2. Enable the task worksheet using the Configure Worksheet Display task.

3. Enable Alerts column in the Alerts column group of the detail table using the Configure Task Layout icon.

Related Topics

• Overview of Alerts in Workforce Compensation Plan Worksheets

• Detail Table Configuration for Compensation, Detail Table Only, Performance, and Promotion Worksheets

• Overview of Worksheet Display in Workforce Compensation Plans

Include a Budget Group in a Compensation Task
Worksheet Summary

Here's the basic process to include a budget group in the summary of a compensation task worksheet, in a workforce
compensation plan:

1. Enable a compensation task worksheet using the Configure Worksheet Display task.

2. Complete these steps using the Configure Task Layout icon.

a. On the Summary tab, enable the group view. Optionally change the Group column display name to reflect

the grouping criteria, such as Location or Grade and Country.

If you enable the analytic view, you can also enable group view for that summary information.

b. On the Detail Table tab, enable the column you want to use as a group, such as Personal > Country or

Employment > Location. To reference data not in the available columns through a fast formula or dynamic
calculation, you can enable and configure a user-defined text column. For example, to use a formula to
prevent managers from crossing budget limits or to track budgets by both Grade and Country columns.

You can't use these kinds of columns for grouping: person number, email, worker number or name, date,
updated by, performance management rating, or numeric.
c. Grouping columns show only the first 150 characters of text.

3. Create the budget pool or edit an existing pool using the Configure Budget Pools task.

a. Enable worker-level budgeting.
b. Set the applicable column as the grouping column.
c. Optionally enforce budgets by grouping column and set a maximum percentage over allocation. You can

also set the severity when people go over budget, such as Error or Warning.

Related Topics

• Detail Table Configuration in Budget Display

• Guidelines to Configure the Budget Amount - Worker Component Columns

• Miscellaneous Rate Component Columns and User-Defined Columns

• Configure the Summary Display for Compensation Task Worksheets

247

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 46
Worksheets: Overview and Basic Configuration Processes
for Key Columns and Actions

Include Compensation Change Statements in Task
Worksheets

Here's the basic process to include compensation change statements in the communication task worksheets of a
workforce compensation plan:

1. Configure what changes you want managers to communicate and how they communicate the changes using the

Configure Compensation Change Statements task.

2. Enable a communications task worksheet using the Configure Worksheet Display task.

3. Enable the applicable summary columns and the applicable actions using the Configure Task Layout icon.

Related Topics

• Overview of Compensation Change Statements in Workforce Compensation Plan Worksheets

• Actions Configuration for Communication, Compensation, Detail Table Only, Performance, and Promotion

Worksheets

• Overview of Worksheet Display in Workforce Compensation Plans

• Configure the Summary Displays for Communication, Performance, and Promotion Task Worksheets

Include Compensation Component Columns in Task
Worksheets

Here's the basic process to include compensation component columns in the worksheet summary views and detail
tables of a workforce compensation plan:

1. Configure up to five compensation components using the Configure Compensation Components task.

2. Enable a task worksheet using the Configure Worksheet Display task.

3. Complete these steps using the Configure Task Layout icon:

a. Enable the components to include in summary views, the relevant summary views, and the applicable

component columns.

b. Enable applicable columns in the component column groups of the detail table.

To post the approved plan changes as salary updates or element entries, be sure to enable the
Compensation Amount column for at least one component. You also need to set the salary and element
mapping properties for the column.

248

Oracle Fusion Cloud Human Resources
Implementing Compensation

Related Topics

Chapter 46
Worksheets: Overview and Basic Configuration Processes
for Key Columns and Actions

• Compensation Components in Workforce Compensation Plan Worksheets

• Detail Table Configuration for Compensation, Detail Table Only, Performance, and Promotion Worksheets

• Guidelines to Allocate Compensation as Percentage of Budget

• Guidelines to Configure the Budget Amount - Worker Component Columns

• Configure the Summary Display for Compensation Task Worksheets

Include Filters in Task Worksheets and Plan Reports

Here's the basic process to include filters in the task worksheets and reports of a workforce compensation plan:

1. Enable a task worksheet using the Configure Worksheet Display task.
2. Enable the corresponding detail table columns. For example, you want to let people filter by country and job. You

need to enable the Country column in the Personal group and the Job column in the Employment group.

3. Enable the Filters action using the Configure Task Layout icon.

4. Enable the appropriate filters using the Configure Filters task. All the filters that you enable for the plan appear on
the worksheet and report Filters dialog box. You can't enable different filters for different worksheets and reports in
the same plan. You can elect to not complete step 2 for various worksheets.

Related Topics

• Overview of Filters in Workforce Compensation Plan Worksheets and Reports

• Detail Table Configuration for Compensation, Detail Table Only, Performance, and Promotion Worksheets

• Actions Configuration for Communication, Compensation, Detail Table Only, Performance, and Promotion

Worksheets

• Overview of Worksheet Display in Workforce Compensation Plans

Include Models in Task Worksheets

Here's the basic process to include models in the task worksheets and reports of a workforce compensation plan:

1. Enable a task worksheet using the Configure Worksheet Display task.

2. Enable Models actions, such as Model - Create Model, Model - Open Model, and Model - Apply Model, using the

Configure Task Layout icon.

3. Enable model access, sharing restrictions, usage, and allocation methods using the Configure Models task. All the
settings that you enable appear on the worksheet and report Filters dialog box. You can't enable different filters for
different worksheets and reports in the same plan. You can elect to not complete step 2 for various worksheets.

4. Enable the modeling criteria you want to let people select from, such as Country and Job using the Configure

Report Dimensions and Modeling Criteria task. You can use delivered dimensions and define your own dimensions
using delivered job attributes, grade attributes, user-defined worksheet columns, and compensation attributes.

249

Oracle Fusion Cloud Human Resources
Implementing Compensation

Related Topics

Chapter 46
Worksheets: Overview and Basic Configuration Processes
for Key Columns and Actions

• Detail Table Configuration for Compensation, Detail Table Only, Performance, and Promotion Worksheets

• Actions Configuration for Communication, Compensation, Detail Table Only, Performance, and Promotion

Worksheets

• Overview of Modeling in Workforce Compensation Plan Worksheets

• Dimensions and Range Increments in Worksheet Models and Plan Reports

• Overview of Worksheet Display in Workforce Compensation Plans

Include Performance Rating Columns in Task Worksheets

Here's the basic process to include performance columns in task worksheets of a workforce compensation plan:

1. Optionally configure performance management ratings, compensation performance ratings, or both using the

Configure Performance Ratings task.

2. Enable a task worksheet, ideally of type Performance using the Configure Worksheet Display task.

3. Complete these steps using the Configure Task Layout icon:

a. Enable a task worksheet, ideally of type Performance. Optionally enable the Performance Rating

summary column of the performance task worksheet.

b. Enable at least one performance management rating or compensation rating column in the detail table.

These columns are in the Performance column group.

Related Topics

• Overview of Performance Ratings in Workforce Compensation Plan Worksheets

• Detail Table Configuration for Compensation, Detail Table Only, Performance, and Promotion Worksheets

• Actions Configuration for Communication, Compensation, Detail Table Only, Performance, and Promotion

Worksheets

• Configure the Summary Displays for Communication, Performance, and Promotion Task Worksheets

Notify People of Eligibility Changes, Reassignments, and
Delegation Changes in a Workforce Compensation Plan

Here's the basic process to notify plan managers and other reviewers of individuals' eligibility changes, reassignments,
and delegation changes in a workforce compensation plan. The initial, saved changes appear as alerts in the relevant
worksheets. When the changes are approved, the managers and reviewers get FYI notifications.

1.

In each of the enabled task worksheets, enable these actions using the Configure Worksheet Display task:

◦ Request eligibility change
◦ Reassign workers to another manager

250

Oracle Fusion Cloud Human Resources
Implementing Compensation

◦ Manage delegations

Chapter 46
Worksheets: Overview and Basic Configuration Processes
for Key Columns and Actions

2. Select Approval required for these notification settings using the Configure Global Setting task:

◦ Eligibility Changes
◦ Worker Reassignments
◦ Delegate Worker
◦ Remove Worker Delegation

Related Topics

• Actions Configuration for Communication, Compensation, Detail Table Only, Performance, and Promotion

Worksheets

• Global Setting Options for Workforce Compensation Plan Notifications

• How Workforce Compensation Plan Notifications Work

• Header and Message Text for All Workforce Compensation Plan Notifications

251

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 46
Worksheets: Overview and Basic Configuration Processes
for Key Columns and Actions

252

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 47
Worksheets: Compensation Component

47  Worksheets: Compensation Component

Compensation Components in Workforce Compensation
Plan Worksheets

Compensation components are the building blocks of workforce compensation plans. You can handle all types of
allocation, such as merit increases, bonus awards, and stock grants by configuring up to five separate components.

For example, you create one monetary component for merit increases, another monetary component for bonus awards,
and a nonmonetary component for stock grants.

While you can go straight to configuring component columns as part of configuring worksheet displays, it's worth
configuring the necessary compensation components first. Here's what you can do when you configure compensation
components that you can't do when you configure worksheet displays.

• Specify how to determine local currency, which is especially important if you enabled currency switching in the
plan currency configuration. For example, you want to use the currencies from input values of payroll elements
or from salary bases.

• Set nonmonetary the unit of measure for the component, such as Days, Hours, Shares, or Units.

• Link budget pools to manager allocations to align the allocations with organizational policies.

•

Include prorated values for the relevant worksheet columns by setting up assignment segment options.

Tip:  You need to configure assignment segments first, using the Configure Assignment Segments task,
before you can link them to a component.

The component columns that you enable in task worksheets inherit these compensation component settings.

Related Topics

• Compensation Component Number and Name, and Detail Table of Worksheet Display

• Detail Table Configuration for Compensation, Detail Table Only, Performance, and Promotion Worksheets

•

Include Compensation Component Columns in Task Worksheets

Compensation Component Number and Name, and
Detail Table of Worksheet Display

When you configure a compensation component, you select the component number and enter a name. The number
and name let you identify the corresponding component columns on the Detail Table tab when you configure the
worksheet display for a task.

For example, you configure these compensation components:

253

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 47
Worksheets: Compensation Component

Name

Bonus

Merit

Component Number

2

1

On the Detail Table tab, the appropriate column group name has the component name appended, such as Component
1 (Merit) and Component 2 (Bonus). And the names of the individual columns in a component group all end with
the component number. This suffix lets you know which compensation component you're configuring. The suffix is
especially important when you scroll down enough that you can't see the column group name anymore. Here are some
examples of monetary component column names:

Component 1 (Merit) Column

Component 2 (Bonus) Column

Eligible Salary - Component 1

Eligible Salary - Component 2

Percentage of Eligible Salary - Component
1

Percentage of Eligible Salary - Component 2

Compensation Amount - Component 1

Compensation Amount - Component 2

Here's an example Detail Table tab showing these same column group name and individual column names for
compensation component 1.

254

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 47
Worksheets: Compensation Component

Related Topics
•

Include Compensation Component Columns in Task Worksheets

How the Compensation Component Display Order
Affects Task Worksheets and Administrator Reports

You can specify the order that compensation components show in the summary areas of task worksheets. It also
determines their order in the Component choice list on administration reports.

Do this by setting the display order when you configure the compensation component. In summary views other than
the table view, managers can use the X of Y link and Previous and Next icons to move between components. For
example, in the score board or analytic summary view of the Reward compensation worksheet, a manager clicks the 1
of 3 link.

You set the display order when you configure the compensation component. The display order can mirror the
component number, but it can also be different. Here's an example of when they match:

255

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 47
Worksheets: Compensation Component

Name

Bonus

Salary - Merit

Stock

Component Number

Display Order

2

3

1

2

3

1

And here's an example of how they can be different:

Name

Bonus

Salary - Merit

Stock

Component Number

Display Order

3

2

1

2

1

3

Here's an example of what managers see in the summary table view of a compensation task worksheet:

Here's an example of the Component choice list on the Compensation Allocations administration report:

256

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 47
Worksheets: Compensation Component

Local Currency Determination for Compensation
Components

When you configure a compensation component, you need to specify how the component determines local currency.
Here's the local currency source for each available option:

Option

Corporate

Element Input

Legal Employer

Salary Basis

Formula

Source of the Local Currency

Usage Example

The configured plan currency

Monetary changes are all in the corporate
currency

The input currency for the payroll element
mapped to the Component Amount column
of the compensation component, such as
Compensation Amount - Component 1

Bonuses

The currency defined for the individual's legal
employer

The input currency for the payroll element
of the salary basis linked to the individual's
employment record

Salary adjustments, such as merit or cost of
living increase, when the currency of the legal
employer is different from the salary basis
currency

Salary adjustments, such as merit or cost of
living increase

The currency retrieved by the specified formula
from some other source

When none of the other options fit your
business requirements

257

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 47
Worksheets: Compensation Component

Tip:  To prevent data corruption, you can't change the Local Currency Determination selection after you run
the Start Workforce Compensation Cycle process. You have to set all plan cycles to Closed or run the Back Out
Workforce Compensation Data process. Then change the local currency determination and run the Start Workforce
Compensation Cycle process again.

Related Topics

• Workforce Compensation Plan Currency

• Salary and Element Mapping Properties of Compensation Amount Columns

• Back Out and Purge Workforce Compensation Data Processes

• Formula Type Is Compensation Currency Selection

• Overview of Using Fast Formulas

Nonmonetary Units for Compensation Components

By default, the units of measure for the amount columns of the compensation component are monetary. You can
specify that the columns use a nonmonetary unit for amounts when you configure the compensation component. For
example, you can select Days, Items, Shares, or Units.

Budget Pools and Compensation Components

To align a compensation component with organizational strategies and policies, you can select a budget pool. You can
even select the same budget pool for multiple compensation components.

For example, your plan includes the Merit, Bonus, and Market Adjustment compensation components that you can
configure with the Monetary Allocation budget pool.

For budget values to increase and decrease according to managers' allocations, you need to link the budget pool to a
compensation component. Any budget pool that you create for the plan and don't link to a compensation component
just shows static budgetary information.

Primary Component for Budgeting
When you have multiple components with the same budget pool, you need to select Primary component for
budgeting for one of the components. The salaries of the people who are eligible for the primary component determine
the total eligible salaries used for their managers' budgeting.

For example, of the three configured components, you make Merit the primary budgeting component. The total eligible
salaries for managers' budgeting include the salaries of their people who're eligible for Merit. The totals exclude their
people who are eligible for Bonus, Market Adjustment, or both, but aren't eligible for Merit.

Related Topics

• Overview of Budget Pools in Workforce Compensation Plans

258

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 47
Worksheets: Compensation Component

How You Let Managers Track Off-Cycle and On-Cycle
Compensation Against a Budget

Here's how you can enable managers to track off-cycle and on-cycle awards when they review their budget pool.

1. Create the workforce compensation plan using the Workforce Compensation Plans task in the Compensation work

area.

a. Configure the plan details.
b. Configure the budget pool.
c. Create at least one worksheet compensation component and associate the budget pool with it.
d. Run the Start Compensation Cycle process.

2. After you start the compensation cycle, associate the budget pool with an individual compensation plan option. Use
the Individual Compensation Plans task in the Compensation work area. Select the budget pool when you add or
edit the relevant plan option.

Configure Assignment Segments Options of a
Compensation Component

You can include prorated values for relevant component worksheet columns. Do this by setting up assignment segment
options for only one of the compensation components configured for the compensation cycle. Don't enable assignment
segments for a component that you're mapping to salary rates.

1. On the create or edit component dialog box for the appropriate compensation component, select Component for

assignment segments. For example, you want to prorate bonus allocations, so you enable the Bonus compensation
component for assignment segments.

2. Select an amount column for assignment segments, either the Compensation Amount column or a miscellaneous

rate column for the component. This selection lets you feed the assignment segment total to a column that
managers see in their summaries.

The amount could have additional calculations done on it before it's passed to payroll element entries. For example,
you select a miscellaneous rate column for the assignment segment. The value in that rate column could be part of
a dynamic calculation configured on the compensation amount column. The calculation could increase or decrease
the rate column value further.

CAUTION:  Don't select a column that you're configuring with a dynamic calculation or a default value. Specifying
the column as an assignment segment takes precedent over any other configurations for that column, and the
other configurations are ignored.

The selected column shows as read-only in any task worksheets with the column enabled. If you select the
compensation amount column, these columns are also read-only in any worksheet where you enable them:

◦ Percentage of Eligible Salary
◦ Percentage of Budget Pool

259

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 47
Worksheets: Compensation Component

3. Specify whether to publish the total segments amount to the selected amount column by default when you run the

Start Workforce Compensation Cycle process.

Related Topics

• Overview of Assignment Segments in Workforce Compensation Plan Worksheets

• Basic Process to Configure Worksheet Assignment Segments

Eligibility Profiles of Compensation Components

As part of the foundation configuration tasks, you configure plan eligibility to identify the people who are eligible and
ineligible for the plan.

You can also add eligibility profiles to compensation components to determine who is eligible and ineligible for
the components. The component-level eligibility considers only the people whose status the plan-level eligibility
configuration set to Eligible. It ignores everyone whose plan-level status is Ineligible or Limited.

Assignment Segments
If you enable the Component for Assignment Segments option, the component eligibility also determines segment
eligibility. Managers can update compensation values for only people who're eligible for a segment. They can only read
the segment values in these situations:

• Their people are ineligible for the segment.

• The person's assignment is processed or partially processed.

• The manager has read-only access to the worksheet.

Administrators can see all assignment segment columns, update all segment values, and update any segment eligibility
using the Administer Workers task. You can also change segment eligibility by changing the external data and then
running the Refresh Workforce Compensation Data process.

Related Topics

• Workforce Compensation Plan Eligibility

• How Required and Optional Profiles Determine Compensation Eligibility

• Configure User-Defined Columns of a Workforce Compensation Plan Worksheet to Show External Data

Eligibility Profile Testing for a Compensation Component

You can test how long it takes to evaluate the eligibility profiles in compensation component configurations and view
test results. The test lets you select a cycle, a sample person, and an active assignment for your test.

Data security applies, so the person and assignment you can see for the cycle depend on your privileges. If profile
criteria includes fast formula, you can see if it worked correctly by reviewing the formula logs.

260

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 47
Worksheets: Compensation Component

Formula Type Is Compensation Currency Selection

To determine the local currency for a workforce compensation component, you can create formulas using the
Compensation Currency Selection formula type.

Here's a comprehensive list of the contexts available to this type of formula:

• DATE_EARNED

• EFFECTIVE_DATE

• END_DATE

• START_DATE

• HR_ASSIGNMENT_ID

• HR_TERM_ID

• JOB_ID

• LEGISLATIVE_DATA_GROUP_ID

• COMPENSATION_RECORD_TYPE

• ORGANIZATION_ID

• PAYROLL_ASSIGNMENT_ID

• PAYROLL_RELATIONSHIP_ID

• PAYROLL_TERM_ID

• PERSON_ID

The database items available for this type of formula are related to Person, Assignment, Salary, Element Entries,
Compensation Record, and From and End Dates.

These are the input variables available to this type of formula:

Input Value

Data Type

Required

Description

CMP_IV_PLAN_ID

Number

CMP_IV_ASSIGNMENT_ID

Number

CMP_IV_PERIOD_ID

Number

CMP_IV_COMPONENT_ID

Number

CMP_IV_PLAN_START_DATE

CMP_IV_PLAN_END_DATE

CMP_IV_PLAN_EXTRACTION_
DATE

CMP_IV_PLAN_ELIG_DATE

CMP_IV_PERFORMANCE_EFF_
DATE

Date

Date

Date

Date

Date

Y

Y

Y

Y

Y

Y

Y

Y

Y

Plan ID

Assignment ID

Period ID

Component ID

Plan Start Date

Plan End Date

Plan Extraction Date

Plan Eligibility Date

Performance Effective Date

261

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 47
Worksheets: Compensation Component

Input Value

Data Type

Required

Description

CMP_IV_PROMOTION_EFF_DATE

Date

CMP_IV_XCHG_RATE_DATE

Date

CMP_IV_ASSIGNMENT_ID

Number

CMP_IV_PERSON_ID

Number

Y

Y

Y

Y

These are the return variables available to this type of formula:

Promotion Effective Date

Currency Conversion Date

Assignment ID

Worker ID

Return Value

Data Type

Required

Description

L_CURR_CODE

Char

N

Currency code from the formula

This sample formula determines the currency for a plan based on the component ID.

/*****************************************************************
FORMULA NAME : Compensation Currency Selection Formula
FORMULA TYPE : Compensation Currency Selection
DESCRIPTION: It returns the currency code based on component_id.
******************************************************************/

/*=========== INPUT VALUES DEFAULTS BEGIN =====================*/
INPUTS ARE CMP_IV_ASSIGNMENT_ID (number), CMP_IV_PLAN_ID (number), CMP_IV_PERIOD_ID (number),
 CMP_IV_COMPONENT_ID (number)
/*=========== INPUT VALUES DEFAULTS ENDS======================*/

/*================ FORMULA SECTION BEGIN =======================*/
DEFAULT FOR CMP_IV_COMPONENT_ID IS 0
l_curr_code = 'XXX'
IF (CMP_IV_COMPONENT_ID = 489) THEN
(
l_curr_code = 'USD'
)
ELSE IF (CMP_IV_COMPONENT_ID = 490THEN
(
l_curr_code = 'GBP'
)
RETURN l_curr_code
/*================ FORMULA SECTION END =======================*/

Related Topics

• Formula Compilation Errors

• Formula Execution Errors

• When do I run the Compile Formula process?

• Example of Writing a Fast Formula Using Formula Text

262

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 48
Worksheets: Performance Ratings

48  Worksheets: Performance Ratings

Overview of Performance Ratings in Workforce
Compensation Plan Worksheets

While you can go straight to configuring performance rating columns as part of configuring worksheet displays, it's
worth configuring performance ratings first. Here's why:

• You can include development and performance goal ratings from Oracle Fusion Performance Management

Cloud Service in your task worksheets. And these ratings get updated automatically when managers save their
rating changes in their worksheets during the workforce compensation cycle.

• You can share compensation performance ratings among plan managers and optionally specify the rating
model for them to use. For example, select a model that indicates level of interest, level of performance, or
proficiency in competencies.

You can also use both integrated Performance Management ratings and compensation performance ratings. For
example, your managers used Performance Management to rate their people several months before the compensation
cycle started. Now you want the managers to make sure that their people's current and past performance is meeting
expectations.

Related Topics

• Workforce Compensation Plan Cycle Dates

• Detail Table Configuration for Compensation, Detail Table Only, Performance, and Promotion Worksheets

• Actions Configuration for Communication, Compensation, Detail Table Only, Performance, and Promotion

Worksheets

• Configure the Summary Displays for Communication, Performance, and Promotion Task Worksheets

Performance Management Ratings in Workforce
Compensation Plan Worksheets

You can share development and performance ratings and documents from Oracle Fusion Performance Management
Cloud Service with managers in task worksheets for workforce compensation plans.

These ratings update automatically when managers save their rating changes in their plan worksheets. Managers can
even set ratings for the first time in a task worksheet as long as the performance document exists in Performance
Management.

You can enable this integration when you configure performance ratings and later, when you enable development and
performance rating columns when you configure worksheet displays.

263

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 48
Worksheets: Performance Ratings

Test Performance Document
You can test your performance document and rating data on the same configuration page. You don't have to wait until
you start a workforce compensation cycle for the plan.

Related Topics

• Workforce Compensation Plan Cycle Dates

• Detail Table Configuration for Compensation, Detail Table Only, Performance, and Promotion Worksheets

• Actions Configuration for Communication, Compensation, Detail Table Only, Performance, and Promotion

Worksheets

•

Include Performance Rating Columns in Task Worksheets

• Configure the Summary Displays for Communication, Performance, and Promotion Task Worksheets

Reasons to Set Performance Document Properties

By default, managers see the most recent manager-submitted ratings and corresponding performance documents, if
they exist, when they open the relevant task worksheet.

If your managers can have many people reporting to them, the default behavior can significantly affect their worksheet
performance. And depending on how regularly people use Performance Management, people's most recent ratings
and documents could be from years ago. Managers won't see this in the rating columns, but they can see it in the
performance document. Thus, you may want managers to consider specific ratings and performance documents when
proposing changes for the workforce compensation plan.

You can override the default behavior by setting performance document properties when you configure performance
ratings that integrate with Oracle Fusion Performance Management Cloud Service.

Related Topics

• Workforce Compensation Plan Cycle Dates

How the Performance Template Selection Affects Other
Document Properties

You can set performance document properties when you configure performance ratings that integrate with Oracle
Fusion Performance Management Cloud Service. A key property is the performance template selection.

Template and Document Type
You can show specific kinds of ratings by selecting a performance template, such as Competency Progress or Annual
360 Evaluation with Development Goals. If the template has a corresponding document type, selecting the template
also sets the performance document type. For example, you select Annual 360 Evaluation with Development Goals,
which sets the performance document type to Annual Evaluation.

264

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 48
Worksheets: Performance Ratings

Template and Timing Options
You can show only ratings and documents for a specific template and period. When you select a performance template,
you make the Timing options available, including Period Specific. Selecting Period Specific makes the Period Name
choice list available so you can select the appropriate period. These choice list values change depending on your
template selection.

If a person doesn't have any ratings or document for that period, the relevant columns in the worksheet are empty.

Timing Period Name and Review Period
The template Period Name choice list values also change if you set a review period. If you want to use a review period
and a specific template period, set the review period before you set the period name. Setting the review period after
the period name also removes the period name and you need to set the name again. This removal happens even if the
period name you selected would be the only choice list value if you set the review period first.

Related Topics

• Workforce Compensation Plan Cycle Dates

• How Performance Document Components Work Together

Compensation Performance Ratings in Workforce
Compensation Plan Worksheets

You can let managers share the performance ratings that don't transfer to Oracle Fusion Performance Management
Cloud Service or HR.

They share their ratings in task worksheets across the primary, secondary, and reviewer plan hierarchies as they allocate
workforce compensation during the current compensation cycle.

You can enable compensation ratings when you configure performance ratings. Then you specify whether managers
rate people using a choice list or stars. You determine the scale used for the choice list or stars with the rating model
that you select. You can also create a rating model, as needed.

Related Topics

• Detail Table Configuration for Compensation, Detail Table Only, Performance, and Promotion Worksheets

• Actions Configuration for Communication, Compensation, Detail Table Only, Performance, and Promotion

Worksheets

•

Include Performance Rating Columns in Task Worksheets

• Configure the Summary Displays for Communication, Performance, and Promotion Task Worksheets

• Rating Models

265

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 48
Worksheets: Performance Ratings

Calibrated Performance Ratings in a Workforce
Compensation Plan

Some organizations use a process called Performance Calibration to achieve a common agreement on a performance
evaluation rating. Managers enter worker performance ratings in the performance documents. In the compensation
plan, managers can edit ratings that override the ratings for workers in their performance documents.

In Workforce Compensation you can let managers and administrators know the calibration status of the Performance
Management Rating for a selected worker. On the Performance Management task, enable performance ratings. Then,
enable and configure the Calibration Status column in the Performance section of columns when you configure the
worksheet display.

Related Topics

• How You Prevent Changes to Section Ratings During Compensation Calibration

266

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 49
Worksheets: Approvals and Notifications

49  Worksheets: Approvals and Notifications

Configure Approvals for Workforce Compensation Plan
Worksheets

By default, managers allocating compensation with a workforce compensation plan can submit their changes to the
plan at any time. And managers higher in the primary plan hierarchy can approve their subordinate managers' plan
changes at any time.

You can change the plan approval and submission modes when you configure approvals. You can also identify an
alternate approval hierarchy to use instead of the primary plan hierarchy.

Related Topics

• Workforce Compensation Plan Hierarchies

• Options to Configure Workforce Compensation Plan Hierarchies

• Considerations for Securing Access to Workforce Compensation Plans and Task Worksheets

• How You Let Managers Track Off-Cycle and On-Cycle Compensation Against a Budget

Approval Modes in Worksheet Approvals Configuration

You specify when managers can approve their subordinate managers' plan changes with the Approval Mode option you
select when you configure approvals.

Mode

Description

You specify when managers can approve
their subordinate managers' plan changes
with the Approval Mode option you select
when you configure approvals.

Let subordinate managers complete their allocations before higher-level managers can approve
subordinate changes because their approvals make the plan unavailable to their subordinate
managers.

Approve anytime
(default selection)

Disable approvals

Higher-level managers can approve their subordinate managers' plan changes at any time during the
period the plan is available to the higher-level managers.

Approvals aren't required and higher-level managers don't have the Approve and Return for
Correction actions available to them.

You can change the approval mode after the Start Workforce Compensation Cycle process runs using the Active
Plans task.

267

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 49
Worksheets: Approvals and Notifications

Submit Modes in Worksheet Approval Configuration

You specify when managers can submit their plan changes with the Submit Mode option you select when you configure
approvals.

Mode

Description

All managers must be approved

Starting at the lowest tier of the hierarchy, managers need to review and approve plan changes
submitted by their direct reports. Then the current tier of managers can submit their own plan changes
for approval.

Submit anytime
(default selection)

Managers can submit their plan changes at any time during the period the plan is available to them.

Disable submit

Managers can only save their plan changes. The Submit action isn't available for the plan.

Withdraw Modes in Worksheet Approvals Configuration

You specify when managers can withdraw their plan changes with the Withdraw Mode option you select when you
configure approvals.

Withdraw Modes in Worksheet Approvals Configuration

Mode

Description

Withdraw anytime

Managers can withdraw their plan changes at any time during the period the plan is available to them.

(default selection)

Disable withdraw

Managers can’t withdraw their plan changes after they submit them.

Higher level managers or administrators need to use the Return for Correction option to return a worksheet to a
manager if they need to make changes to a plan.

268

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 49
Worksheets: Approvals and Notifications

Alternate Approver Table in Worksheet Approval
Configuration

By default, the approval hierarchy for a workforce compensation plan is the primary plan hierarchy. To have people other
than primary plan managers handle approvals, select an alternate approver table when you configure approvals for
worksheets.

Typically, you use alternate approver hierarchies when you transition approval control from managers to the HR
department.

You can set an alternate approver for a specified worksheet manager when you create the alternate approver table. The
worksheet manager options come from the primary plan hierarchy. The alternate approver that you select replaces
the person who would otherwise approve plan changes submitted by the specified worksheet manager. The alternate
approver doesn't replace the specified worksheet manager in the approval hierarchy. Thus the alternate doesn't approve
plan changes that the specified worksheet manager normally approves.

Each alternate approver approves plan changes according to their approval sequence. The person with the lowest
approval sequence approves first and the person with the highest sequence approves last.

Tip:  If you add or delete alternate approvers in a table, you need to run the Refresh Workforce Compensation Data
process afterward. You don't need to run the process if you only change the approval sequence of existing alternate
approvers.

Related Topics

• Workforce Compensation Plan Hierarchies

• Options to Configure Workforce Compensation Plan Hierarchies

• Alternate Approver for Workforce Compensation Plan Changes Is the Final Approver

• Alternate Approver for Workforce Compensation Plan Changes Precedes the Final Approver

• Alternate Approver for Workforce Compensation Plan Changes Is in the Middle of the Primary Plan Hierarchy

Configure Notifications for Workforce Compensation
Plan Worksheets

You can configure notification settings that apply across all workforce compensation plans, such as Notify, Disable, or
Prompt Manager, using the Configure Global Settings task.

For example, notify managers when their budgets are published or withdrawn and prompt managers when their plan
changes are returned for corrections. When at least some or even all of these global settings aren't appropriate for a
specific plan, you can override these global settings. Configure plan-specific notification settings, when you configure
approvals and notifications for task worksheets in workforce compensation plans.

269

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 49
Worksheets: Approvals and Notifications

The Notify action sends the notification immediately. The Prompt manager action lets the manager decide whether or
not to send the notification.

Related Topics

• Header and Message Text for All Workforce Compensation Plan Notifications

• How Workforce Compensation Plan Notifications Work

Can I configure workflow in workforce compensation to
route plan changes for approval?

No. Workforce compensation uses the primary plan hierarchy to route approvals to the highest-level manager. While
you can't create your own approval routes, you can create alternate approvers for individual managers using the
Configure Approvals and Notifications task.

Related Topics

270

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 50
Worksheets: Examples of Alternate Approver
Configurations

50  Worksheets: Examples of Alternate
Approver Configurations

Alternate Approver for Workforce Compensation Plan
Changes Is the Final Approver

Carlos, the CEO, is the top manager in the primary plan hierarchy. Company policy is that his plan changes go to a
designated HR manager for final review and approval. Here's how you build the alternate approver table:

Primary Worksheet Manager

Approval Sequence

Alternate Approver

Carlos

1

Maria

And here's an example of how plan change submissions are approved using the primary plan hierarchy and this
alternate approver table.

1. John, a director, submits his plan changes to Vijay, VP West, for approval.
2. Vijay reviews and approves John's changes, then makes his own plan changes and submits them to Sara, a

senior VP.

3. Sara reviews and approves Vijay's plan changes, then makes her own plan changes and submits them.
4. Carlos, the CEO, reviews and approves Sara's plan changes, then makes his own plan changes and submits

them. At this point, the plan status for Carlos is In Approvals.

5. Maria, an HR manager, reviews Carlos's plan changes. When she approves the changes, Carlos's plan status

becomes fully approved.

271

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 50
Worksheets: Examples of Alternate Approver
Configurations

Alternate Approver for Workforce Compensation Plan
Changes Precedes the Final Approver

Carlos is the CEO and top manager in the primary plan hierarchy. He doesn't participate in the approval process for
workforce compensation changes from his subordinate managers under Sara, a senior VP.

Carlos gets an informational notification when Sara submits her plan changes, but Maria, a manager in HR, has final
approval. Here's how you build the alternate approver table:

Primary Worksheet Manager

Approval Sequence

Alternate Approver

Sara

1

Maria

272

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 50
Worksheets: Examples of Alternate Approver
Configurations

And here's an example of how plan change submissions are approved using the primary plan hierarchy and this
alternate approver table.

1. John, a director, submits his plan changes to Vijay, VP West, for approval.
2. Vijay reviews and approves John's changes, then makes his own plan changes and submits them to Sara, a

senior VP.

3. Sara reviews and approves Vijay's plan changes, then makes her own plan changes and submits them.
4. Carlos, as Sara's normal approver, gets an informational notification that Sara submitted her plan changes.
Maria, an HR manager, is Sara's alternate approver. She gets the approval notification and reviews Sara's
plan changes. When Maria approves them, the plan status for Sara and all of her subordinate managers is In
Approval.

5. When Carlos checks his approvals task worksheet a few days after getting Sara's submission notification, he

sees that Maria approved Sara's plan changes. If Sara is eligible, Carlos can change her allocations.

6. After Carlos saves his plan changes, he reviews and approves all of his plan changes and the plan changes that

Maria approved. His approval makes the plan fully approved.

273

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 50
Worksheets: Examples of Alternate Approver
Configurations

Alternate Approver for Workforce Compensation Plan
Changes Is in the Middle of the Primary Plan Hierarchy

John, a director, reports to Vijay, VP West, according to the primary plan hierarchy. But, John's entire team did a special
project for Lakshmi during most of the past year.

Sara, the senior VP whom Vijay reports to, wants Lakshmi to review and approve the compensation for John's team
rather than Vijay. Here's how you build the alternate approver table:

Primary Worksheet Manager

Approval Sequence

Alternate Approver

John

1

Lakshmi

And here's an example of how plan change submissions are approved using the primary plan hierarchy and this
alternate approver table.

1. John, a director, submits his plan changes.
2. Vijay, as John's normal approver, gets an informational notification that John submitted his plan changes.

Lakshmi, VP East and the alternate approver, gets an approval notification that she uses to approve or reject
John's plan changes. She can open the Workforce Compensation work area from the notification. At the top
of the page, she can select John from the manager list and review his worksheet details for the plan. But, she
can't approve or reject John's plan changes in the work area. She approves or rejects John's plan changes using
actions in the approval notification.

3. When Vijay checks his approvals task worksheet a few days after getting John's submission notification,

he sees that Lakshmi approved John's plan changes. In the detail table, the status for John's changes is In
Approvals.

4. Vijay can now make and submit his own plan changes to progress the plan through the approval process.

Vijay, Sara, and Carlos, the CEO whom Sara reports to, can still make plan changes for John's team even after
Lakshmi approves John's changes.

274

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 50
Worksheets: Examples of Alternate Approver
Configurations

275

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 50
Worksheets: Examples of Alternate Approver
Configurations

276

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 51
Worksheets: Compensation Change Statements

51  Worksheets: Compensation Change
Statements

Overview of Compensation Change Statements in
Workforce Compensation Plan Worksheets

You can let managers and HR specialists communicate compensation and performance rating changes to people as
part of a workforce compensation cycle.

They communicate the changes with compensation change statements using the communications-type task
worksheet. They can also use the change statements to communicate promotions done as part of the cycle. The
changes that they can communicate, and how they communicate them depends on how you configure compensation
change statements.

Related Topics

• Overview of Worksheet Display in Workforce Compensation Plans

•

Include Compensation Change Statements in Task Worksheets

• Configure the Summary Displays for Communication, Performance, and Promotion Task Worksheets

Statement Groups, Templates, and Worker Statement
Action for Compensation Change Statements

Statement groups are fundamental to compensation change statements. The selected group identifies what templates
to use for whom, and what statement action individuals are responsible for. You set up all of these options on the
Manage Statement Groups page.

Name
Use a broad, descriptive name so that people understand what to expect from the statement. For example, your latest
compensation and performance statement group might be 2021 Compensation and Performance Changes. And your
latest promotions statement group might be 2021 Promotions.

Templates
When you add a template to the statement group, you can set a display name and add criteria for when to use the
template. Typically, you add a separate row for each language that you use to communicate changes. Here are some
examples for compensation and performance changes:

277

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 51
Worksheets: Compensation Change Statements

Template

Display Name

Criteria

Compensation and Performance Change
Statement.rtf

English Compensation and Performance
Change Statement

Country = US or UK or Canada

Cambios en Compensación y Rendimiento en
2021.rtf

Spanish Compensation and Performance
Change Statement

Country = Spain or Mexico or Costa Rica

Here are some examples for promotions:

•

•

If you use the same template for the entire company, you might have something similar to the first row.

If you have templates in different languages, you might have something similar to the second row.

Template

Promotion.rtf

Promotion.rtf

Display Name

Criteria

Promotion Statement

Country = US or UK or Canada

English Promotion Statement

Country = US or UK or Canada and Proposed
Grade Is not blank

To create and load other templates for selection, you can use the Manage Templates page. This page also has sample
files to help you create your own templates:

• A list of all the attributes you can include in your own templates.

• Sample compensation change and salary change analytic templates that you can download and tailor for your

change communications. Be sure to change the file name before you upload your template.

You can’t delete a template that has generated statements associated with it.

Worker Statement Action
When you want a record that individuals received their change statements, you can set a worker statement action for
the template. For example, you want individuals to acknowledge or sign electronically when they received a statement.
You can configure worker statement actions to be completed before or after people have reviewed their compensation
change statements.

How You Create a Change Statement Template

You can create the change statement template using attributes or tokens and special syntax to create conditional
statements. You need to incrementally test the statement to ensure that there are no errors.

You can add any formatting, logos, text, and data that you want to display in the statement. You need to create the file in
the .rtf format. You can't change an existing .doc file to .rtf file type.

To access the predefined template, click Manage Workforce Compensation Plans > Compensation Change Statements >
Manage Statement Groups > Manage Templates and downloading the Compensation Change Statement Template.rtf.

278

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 51
Worksheets: Compensation Change Statements

Download Attribute List to Add to Template

Attributes (or tokens) represent worker-specific data displayed in the statement. You can include all columns (excluding
iconic columns) that are available to display in the worksheet in a statement template. You add these attributes to your
template in the location and formatting you want.

Here’s how you can download the list of attributes from the compensation setup pages:

1. Click Compensation tile in My Client Groups.
2. Under Workforce Compensation, click Workforce Compensation Plans.
3. From the Workforce Compensation Plans page, create a new plan or select an existing plan.
4. Click the Compensation Change Statements task.
5.
6. Click the Manage Statement Groups button.
7.
8.
9. Optionally, you can download the sample Compensation Change Statement Template.rtf to use as a reference.

In the Manage Statement Groups page, click the Manage Templates button.
In the Sample Templates region of the window, download the All Attributes List.rtf and save it to your computer.

If the Enable Worker Statements field isn't set to Yes, change it to Yes.

How You Can Display Different Currencies In Your
Statement Template

Salary columns and component columns (such as Compensation Amount, Eligible Salary, targets, and miscellaneous
columns) appear in each worker’s local currency. The currencies in which custom numeric columns appear depending
on the values determined in those columns.

1. To display salary or component columns in a different currency, you need to create a dynamic calculation on a

custom numeric column.

2. Create one or more conditions that multiply the selected column times the currency conversion rates and use the

custom column in your statement template.

Ways to Configure Statement Text

You can format the change statement template to display text exactly how you want.

Text Format

Description

Example

Display Text Always

To include text with no conditions, you can
simply copy the variable from the All Attributes
Template.rtf for the column you want to display,
 and paste it into your template.

In this example, you are displaying the worker’s
first and last name, their worker number,
 Custom Text Column 1 which, has been
configured to display the division, and the
primary manager’s name. The Worker’s name
will be in bold in the generated statement.

279

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 51
Worksheets: Compensation Change Statements

Text Format

Description

Example

Display Text Conditionally

You can make a sentence, paragraph, or region
of the page display conditionally based on
workers meeting certain criteria.

 Name: <?FIRST_NAME?> <?LAST_NAME?>

Employee ID: <?WORKER_NUMBER?>

Job Title: <?CURRENT_JOB?>

Division: <?CUSTOM_COLUMN_1_TEXT?>
 Manager: <?PRIMARY_MANAGER?>

The Award Amount: along with the actual
monetary value will only be displayed if the
Compensation Amount column for component
1 is not equal to zero. The variable name that
represents the worksheet column is the text
between the < and >, and syntax before and
after create the condition. <?end if?> defines
the end of the conditional statement.

<?if: COMP_1_COMPENSATION_AMOUNT!=0?>
 Award Amount: <?COMP_1_COMPENSATION_
AMOUNT?> <?COMP_1_CURRENCY?>

<?end if?>

You can display text conditionally if a worksheet
column value is not null. In this example, the
sentence only appears if the Proposed Job Title
field is not null for the worker.

Important: The correct syntax is two single
quotes, not a single double quote.

<?if: New_Job !=’’ ?>You are being
 promoted to <?NEW_JOB?> as of
 January 1, 2012.

<?end if?>

You can also display or hide an entire sentence
or paragraph. The below paragraph will only
appear in the statement if the worker was
given a new job, position or grade during the
compensation cycle.

<?if:NEW_JOB!=’’ or NEW_POSITION!=’’
 or NEW_GRADE!=’’?>We recognize and
 thank you for your hard work and
 contribution towards the company’s
 success. As of <?PROMOTION_
DATE?, you are being promoted. <?
if@inlines:NEW_JOB!=’’?>Your new job
 title is <?NEW_JOB?>.<?end if?><?
if@inlines:NEW_POSITION!=’’?>Your new
 position is <?NEW_POSITION?>. <?end
 if?><?if@inlines:NEW_GRADE!=’’?>Your
 new grade is <?NEW_GRADE?>.

<?end if?>

280

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 51
Worksheets: Compensation Change Statements

Statement Generation Timing and Output Format for
Compensation Change Statements

You can specify when individuals can get their compensation change statements, according to your organizational
policies. For example, anyone can get their statement at any time. Or only people whose changes were posted to HR, or
have final approval can get their statements.

You can also specify whether to generate the statements as .pdf or .rtf files.

How You Generate Statements for Multiple Workers

You can configure the template to allow managers to generate the statement for multiple workers at the same time.

To do so, the template must begin with the following: <?for-each: PERSONINFO?>

The template must end with the following: <?split-by-page-break:?><?end for-each?>

If the template doesn't include the above 2 statements, managers will only be able to generate the statement for a single
selected worker at a time.

Delivery Options for Compensation Change Statements

You can specify how to generate and deliver worker statements when you configure compensation change statements.

Here are the delivery options that apply for primary plan managers:

• Printed and delivered by managers

• Centrally managed and stored

Administrators using the Administer Workers task can manage change statements for the plan regardless of how
they're generated or delivered.

How Managers Can Print and Deliver Compensation
Change Statements

Managers can generate the statements using the Communication task worksheet in the plan.

When configured, the statements are automatically available to managers or administrators, but not individuals. You
can let managers generate statements at the same time for specific people, all of their direct reports, or all of their
subordinates. When managers generate statements for more than one person using the Selected Workers or the
Direct Workers option the application ignores any statement criteria. The managers must select the statement they

281

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 51
Worksheets: Compensation Change Statements

want to use for the selected population.When configured, the statements are automatically available to managers or
administrators, but not individuals. You can let managers generate statements at the same time for specific people, all
of their direct reports, or all of their subordinates. When managers generate statements for more than one person using
the Selected Workers or the Direct Workers option the application ignores any statement criteria. The managers must
select the statement they want to use for the selected population.

When managers use the management hierarchy option, they can also generate statements for their people in a
specified country. The process generates the statements in a single file for the selected template. If a manager decides
to provide individual statements to people and the file contains multiple statements, they need to split the file into
separate statements. Then they can provide a copy of each statement to the appropriate individual. Their people can
see only the statements that the manager provides to them, as long as they keep the statements.

How Managers Can Centrally Manage and Store
Compensation Change Statements

Managers can generate an individual compensation change statement for each of their people and provide them a
copy.

You can also enable people to access the centrally stored statements from their compensation pages unless processing
made the statements visible to only administrators and managers. Again, depending on the process configuration,
managers can view and print the statements.

Here are the other options you can set if you centrally manage and store statements:

Option

Description

Let managers control when to release the
statements to their people

Enable the Allow staggered release of statements option. For example, your policy is to have managers
meet with their people to discuss their compensation changes before releasing the statements. If
individuals have more than one statement available to them, then their manager has to release each
statement separately.

Automatically delete the statements from
storage

Set the Days Until Expiration option. For example, your organization has a 90-day retention policy, so
you set the expiration to 90. Individuals can save their statements if they want to access them after 90
days. Administrators can override this expiration as appropriate, using the Update Expiration option
when they run the Process Workforce Compensation Change Statement process.

Show everyone the same statement name
in the plan

Set a global statement name. For example, the template display names identify the template
language, such as 2021 Compensation and Performance Changes Spanish or 2021 Compensation and
Performance Changes French. Or you want everyone to see the same statement name in the corporate
language, for example, 2021 Compensation and Performance Changes.

Compensation administrators configure and run the Process Workforce Compensation Change Statement process to
generate and store these changes statements. They run the process according to organizational policies, such as at the
end of the workforce compensation cycle, when all changes are finished and approved.

282

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 51
Worksheets: Compensation Change Statements

How You Format a Date Variable to Display Dates in a
Specific Format

You can format the date variable using the function <?format-date:DATE_VARIABLE;'YYYY-MM-DD'?>. You can modify the
String 'YYYY-MM-DD' according to your date format requirements. For example:

<?format-date:JOB_CHANGE_DATE;'YYYY-MM-DD'?>

If value of the variable JOB_CHANGE_DATE is Jan 1st 2013, the above expression will display it as “2013-01-01”.

You can also make use of form field options for this purpose.

How You Format Numeric Separators and Decimal
Precision for Numeric Data

You can use the function <?format-number:NUMERIC_VARIABLE; ’9G999D99'?> where G stands for the position of the
comma (,) and D stands for position of the decimal. For example:

<?format-number:COMP_1_COMPENSATION_AMOUNT; ’9G999D99'?>

If the value of the variable COMP_1_COMPENSATION_AMOUNT is 1234.5678, the above expression will display it as
“1,234.57” after rounding the numeric data to two decimal places.

Alternatively, you can also make use of form field options.

How You Find Errors in Statement Template

You can find errors in your template by saving the file to your computer and then open it using Notepad or another text
editing application. You can then find the error details and correct your template.

How You Format the Same Data Differently Based on a
Worker’s Location

You can use a custom text column to default the location of the worker and display data conditionally or vary data based
on value of the custom text column. You can also create multiple statement templates, one for each location. When
using multiple templates, managers may have to select the appropriate template to use for each worker based on their
location.

283

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 51
Worksheets: Compensation Change Statements

What's the difference between workforce compensation
change statements and total compensation statements?

Workforce compensation statements show recent changes to base and variable pay. They apply to a statement group,
which has RTF templates that can include criteria to identify which people get the template.

For example, people in Spanish-speaking countries get the Spanish version of the statement. The workforce
compensation plan containing the statement configuration determines the statement content. You configure
these compensation change statements for a specific plan using the Workforce Compensation Plans task in the
Compensation work area.

Total compensation statements show base and variable pay, fringe benefits, and perks for a specified period of time,
typically a year. These statements are available both online and in PDF format. You configure these statements using
the Total Compensation Statement tasks in the Compensation work area.

284

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 52
Worksheets: Worksheet Display Configurations

52  Worksheets: Worksheet Display
Configurations

Overview of Worksheet Display in Workforce
Compensation Plans

You determine the summary and detail information on compensation, performance, promotion, detail table only,
approvals, and communication task worksheets when you configure worksheet display.

The specific information managers and HR specialists see depends on the task types and the columns that you enable
and configure. Some columns are enabled by default. You can deselect any enabled columns that you don't want to
appear in a worksheet.

You also determine the actions available on a worksheet, such as letting managers reassign or delegate individuals or
request eligibility changes. And you can provide information that applies to the entire worksheet. For example, you let
people know about organizational policies that affect compensation allocations, performance ratings, or promotions,
and include links to details.

You can configure up to 10 task worksheets for a plan. For managers to access a workforce compensation plan,
you need to configure at least 1 task worksheet. To require approvals for plan changes, you also need to enable and
configure an approvals task worksheet.

You enable task worksheets using the Configure Worksheet Display task. You configure the layout of each enabled
worksheet using the Configure Task Layout icon on the Configure Worksheet Display page.

Reference
For descriptions of every worksheet column and action, see Workforce Compensation Worksheet Configuration
Definition (document ID 1450891.1) on My Oracle Support (support.oracle.com). To help you locate columns and actions,
the document tabs organize information in the same groupings as the Configure Worksheet Page Layout pages.

For columns, the document has this information:

• The navigation path for columns that map directly to a field in Oracle Fusion Global HR Cloud Service

•

•

If you can default column values using a plan cross-reference

If people can update the values in their plan budget and task worksheets

For actions, it tells you about any dependent configurations you need to complete.

Related Topics

• Performance Considerations for Workforce Compensation Plans

• Compensation Components in Workforce Compensation Plan Worksheets

• Overview of Performance Ratings in Workforce Compensation Plan Worksheets

• Overview of Compensation Change Statements in Workforce Compensation Plan Worksheets

285

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 52
Worksheets: Worksheet Display Configurations

Configure the Summary Display for Compensation Task
Worksheets

You can include key summary information for the compensation component at the top of compensation-type task
worksheets. What people see depends on the population that they're viewing in the detail table.

1. Enable the compensation components.

Select the configured compensation components that you want to show summary information for. For example,
you're configuring separate task worksheets for your Merit and Bonus compensation components. In the
worksheet display for the Merit compensation task, you select the Merit compensation component as the summary
component. For the Bonus compensation task, you select the Bonus compensation component.

2. Enable the summary views.

Enable the views that you want to show, such as the scoreboard, table, analytic, or group view, or a combination of
views. When you enable multiple views, you need to make one view the default view that people see whenever they
first open the task worksheet.

If you're using worker-level budgeting and setting a budget group, enable the group view. Optionally change the
Group column display name to reflect the grouping criteria, such as Location or Grade and Country. If you enable
the analytic view, you can also enable group view for that summary information.

3. Enable the columns to show.

Enable the columns that you want to show in the summary section. For example, in the scoreboard view, you enable
these columns for each enabled compensation component:

◦ Compensated Workers with %
◦ Currency or Units
◦ Eligible Salary
◦ Allocate with %
◦ Budget with %
◦ Remaining Budget with %

For the analytic view, you enable analytics that provide a snapshot of allocations in the current cycle. For example,
you enable the Worker Population, Allocation Statistics, Allocation Amount, and Salary Statistics analytics.

To show managers and HR specialists the same summary information regardless of any filters they apply to the
detail table, enable these three static columns. To show them summary information that changes depending on the
filters they apply to the detail table, you can enable three filtered columns.

Static

Filtered

◦ Overall Budget
◦ Overall Available Budget

◦ Budget - Filtered by Team (enabled by default)
◦ Available Budget - Filtered by Team

286

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 52
Worksheets: Worksheet Display Configurations

Static

Filtered

◦ Overall Compensation Amount

◦ Compensation Amount - Filtered by Team

For example, you enable the Overall Budget summary column and leave the Budget - Filtered by Team column
enabled. A manager changes the Team filter on the worksheet to Direct Reports. The summary section Overall
Budget column shows the budget amount for all the manager's subordinates. The Budget - Filtered by Team
column shows the budget amount for only their direct reports.

4. Optionally change display names and default sequences.

You can change the display names and default sequences, as appropriate for the audience. For the analytic view,
you can change the title. Certain titles also have subtitles that you can change. For example, you want to make your
names more human, so you change Compensated Workers with % to Compensated Individuals with %. And you
change Worker Population to Population.

5. Optionally configure column properties.

You can configure general and information column properties for the scoreboard, table, and group views. For
example, you can set a rounding rule and the decimal place to display. The actual properties vary depending on the
column.

All columns include a Plan Info property that you can use to communicate useful information to managers. For
example, you share the expression used to calculate the column values, or add a definition for the column, such as
explaining what's compa-ratio. When you include plan info for a column, people viewing the worksheet see a blue
icon with an i in it on the column header. They click the icon or hover over it to see the information.

To show column totals in the summary section, you can select Show totals for columns that include the property.
You probably don't want to show totals in a worksheet that has compensation components with different units of
measure enabled. The totals would be meaningless. For example, one component is in monetary units and another
is in shares. The Compensated Workers with % column total would combine the numeric monetary and shares
values.

6. Check the configuration.

To see the worksheet summary just the way that the plan audience will see it when the plan becomes active, use the
Preview tab. You can easily test different summary configurations to find the summary that best conveys the key
information the audience needs and wants to see.

Related Topics

• Compensation Components in Workforce Compensation Plan Worksheets

Configure the Summary Displays for Communication,
Performance, and Promotion Task Worksheets

You can include key summary information at the top of communication, performance, and promotion type worksheets.
What people see depends on the population that they're viewing in the detail table.

287

Oracle Fusion Cloud Human Resources
Implementing Compensation

1. Enable summary columns.

Chapter 52
Worksheets: Worksheet Display Configurations

For all three types of task worksheets, enable the columns that you want to show in the summary section. Here are
some examples:

◦ In the communication-type task worksheet, you enable the Compensation Amount - Component 1 and

Eligibility Status - Component 1 columns.

◦ In the performance-type task worksheet, you enable the Performance Rating, Workers with

Compensation, Actual Percentage, and Total Compensation Percentage columns.

◦ In the promotions-type task worksheet, you enable the Promotions, Percent Promoted, Deviation from

Company Target, and Filter columns.

For communication-type worksheets, you can configure the View or Print column properties to hide the print icon
for ineligible individuals.

For performance-type task worksheets, you can also hide the graph, compensation performance ratings,
performance management ratings, all, or a combination in the summary.

For promotion-type task worksheets, you can also enable subtabs that group table information. For example, you
enable these subtabs: By Team, By Country, By Years in Job, By Performance Management Rating, By Text
Column 1, and Organization Averages.

◦ You configure the specifics for By Text Column 1 on the Detail Table tab, under the User-Defined Columns
group. You can configure the column properties and manage dynamic column conditions and results. The
summary subtab aggregates the values from the detail table for all plan management levels.

◦ If you enable the Organization Averages subtab, you can also enable the specific rows that you want that
table to show. For example, you enable the Team One Level Up, Team Two Levels Up, Department, and
Enterprise rows.

2. Optionally change display names and default sequences.

You can change the display names and default sequences of summary columns, as appropriate for the audience. For
example, you want to make your names more meaningful. So, you change Compensation Amount - Component 1
to Merit Compensation Amount and Eligibility Status - Component 1 to Merit Eligibility Status.

3. Optionally configure plan info.

You can configure the Plan Info property for summary columns in the communication and performance type
worksheets. Use the property to communicate useful information to managers. For example, you share the
expression used to calculate the column values, or add a definition for the column, such as explaining what's compa-
ratio. When you include plan info for a column, people viewing the worksheet see a blue icon with an i in it on the
column header. They click the icon or hover over it to see the information.

4. Configure the summary display options for promotion worksheets.

You can also configure display options for promotion summaries. For example, you enter Company Target -
Average Percent Promoted and Minimum Team Size to See Company Target values. And you set the default
display order and graph bar color.

5. Check the configuration.

To see the worksheet summary just the way that the plan audience will see it when the plan becomes active, use the
Preview tab. You can easily test different summary configurations to find the summary that best conveys the key
information the audience needs and wants to see.

288

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 52
Worksheets: Worksheet Display Configurations

Related Topics

• Overview of Performance Ratings in Workforce Compensation Plan Worksheets

• Overview of Compensation Change Statements in Workforce Compensation Plan Worksheets

Detail Table Configuration for Compensation, Detail
Table Only, Performance, and Promotion Worksheets

You can enable columns from the personal, alerts, employment, salary, component, promotion, and performance
groups to appear in the main table of task worksheets. You can also configure your own, user-defined text, numeric,
and list columns.

You can enable additional information columns, such as notes, attachments, and histories. You do all of this when you
configure the worksheet display. The compensation, detail table only, performance, and promotion task worksheets all
have a detail table. The communication and approvals worksheets don't.

Display Names and Column Sequences
You can provide meaningful column names for the plan audience by changing the default display names. For example,
you change Eligible Salary - Component 1 to Eligible Salary for Merit Increase. And you can change the default
sequence of any column, as appropriate. Use the Refresh icon on the Column Preview panel to see how the reordered
columns will appear in the table.

Column Properties
You can configure general, visibility and access, default value, and salary and element mapping properties for the
columns you enable. The available sections and properties vary depending on the column.

All columns include a Plan Info property that you can use to communicate useful information to managers. For
example, you share the expression used to calculate the column values, or add a definition for the column, such as
explaining what is compa-ratio. When you include plan info for a column, people viewing the worksheet see a blue icon
with an i in it on the column header. They click the icon or hover over it to see the information.

Preview Tab
To quickly check your page layout configuration for the compensation, detail only, performance, and promotion task
worksheets at any time, use the Preview tab. The preview shows the entire worksheet, including the enabled summary
information, detail table columns, actions, and column-level and plan-level information.

The approvals and communication task worksheets don't have the Preview tab.

Related Topics

• Compensation Component Number and Name, and Detail Table of Worksheet Display

• Overview of Performance Ratings in Workforce Compensation Plan Worksheets

289

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 52
Worksheets: Worksheet Display Configurations

Approval Subtabs, Columns, and Worker Details Columns
Configuration for Approvals Task Worksheets

Only managers with at least one subordinate manager have the approvals task worksheet in their workforce
compensation plan. Managers use the approvals worksheet to view the status of their subordinate managers' plan
changes, approve or reject submitted changes, or request more information.

Here's how you configure the display for approvals task worksheets. For all three steps, you can optionally change the
display and default sequence.

1. Enable the worksheet tabs that managers see, such as approvals, compensation overview, salary range

analysis, and alerts.

2. Enable the columns that appear on each tab.
3. Enable the columns that appear on the Worker Details dialog box. Managers open the dialog box when they

click a link in a column that contains the number of workers or a percentage.

The column group names and the approval tab names that you see on the Configure Worksheet Page Layout page need
to match. This way you know which tab you're configuring columns and worker details columns for.

Example
On the Approvals Subtabs tab, you enable the Compensation Overview tab. On the Columns tab, in the Compensation
Overview column group, you enable these columns:

Workers

Allocated

Budget

• Eligible

•

Ineligible

• Compensated

• Percentage of Workers Compensated

• Eligible Salary

• Overall Budget Amount

• Compensation Amount

• Overall Available Budget

• Compensation Percentage

• Overall Budget Percentage

On the Worker Details Columns tab, in the Compensation Overview column group, you enable these columns:

• Allocation columns: Eligible Salary, Compensation Amount - Filtered by Team, and Compensation Percentage

• Effective Date

• Notes

On the Actions tab you can configure the task actions such as Request for Information, Change Access for Managers,
and Export to Workbook. You can also have the Approval chain appear at the top of the page to let managers see where
their plan changes are in the cycle.

When Andy Anderson opens his approvals task worksheet and clicks the Compensation Overview tab, he sees the
columns that you enabled in the table. When Andy clicks the link for his 8 eligible workers, he opens the Worker Details:
Andy Anderson Team dialog box with the worker details columns you enabled.

290

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 52
Worksheets: Worksheet Display Configurations

Approval Subtabs
Here are descriptions for the approval subtabs on the setup page and on the approvals worksheet.

Subtab

Approvals

Compensation Overview

Allocation Statistics

Salary Analysis

Target Analysis

Performance

Promotions

Alerts

Related Topics

Description

You show a hierarchy of all subordinate managers and the status of their plan changes. We recommend
that you leave this subtab enabled.

You can show how many people were awarded compensation during the cycle, the total amount
allocated, and the total available budget.

You can enable up to five buttons. The buttons show the average allocation and allocation spread. They
also show allocations by overall performance rating, by country, and by compensation performance
rating.

You can enable up to six buttons. The buttons show the compa-ratio, quartile, quintile, and salary
range analysis. They also show the total salary cost and average salary.

You can enable up to three buttons that show the target overview, target versus actual, and deviation
from target.

You can enable up to eight buttons. The performance management buttons show the overall rating,
 overall competency rating, overall goal rating, and overall development goal rating. The other buttons
show compensation performance rating, calculated rating, worker potential, and risk of loss.

You show the number of people whose job, grade, or position changed during the compensation cycle.

You show all the currently enabled alerts and the alert counts. You can also let managers view the
affected individuals.

• Configure Approvals for Workforce Compensation Plan Worksheets

291

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 52
Worksheets: Worksheet Display Configurations

Actions Configuration for Communication,
Compensation, Detail Table Only, Performance, and
Promotion Worksheets

These actions enable managers to set their own defaults using the Personalize Layout tool on their worksheets. You
enable the actions as part of the Configure Worksheet Display task. You set the initial default values using the Configure
Default Worksheet Display task.

You set the initial default values using the Configure Default Worksheet Display task. The specific actions that you can
enable depend on what type of task the worksheet is for. For example, in compensation worksheets, you can enable the
Actions, View, and Format menus and corresponding options that show on the detail table. Communication worksheets
don't have the Actions menu or corresponding options.

For these actions, you also need to enable a corresponding column in the Detail Table tab:

Enabled Action

Detail table Column to Also Enable

Any rank workers actions in the Actions >
Rank Workers group.

Ranking in the Performance group

Tip:  To let managers see full ranking
details, also enable View Ranking
Details in the Right Click Menu group.

View Compensation History in the Right
Click Menu group.

Manage Notes in the Right Click Menu
group.

Any Apply Targets actions in the Apply
Targets group and Apply Targets in the
Right Click Menu group

Compensation History in the Additional Information group

Notes in the Additional Information group

At least one target column in an enabled component group, such as Target Compensation Amount -
Component 1

Hide Ineligible Workers Action
This action applies to people with an Ineligible status after the Start Workforce Compensation Cycle and Refresh
Workforce Compensation Data processes evaluate the plan-level eligibility profiles. The action ignores anyone with an
Ineligible status according to eligibility profiles added to the compensation components.

Model Actions
You can add the models task worksheet to the plan using the Configure Models task. And managers can use that task
worksheet for all of their modeling. You can also enable the Model actions for a worksheet to let managers create and
apply models while they're in that worksheet. You don't need to enable model actions to include the model worksheet.
But if you enable any model actions, you also need to configure modeling.

292

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 52
Worksheets: Worksheet Display Configurations

Preview Tab
To quickly check your page layout configuration for the compensation, detail only, performance, and promotion task
worksheets at any time, use the Preview tab. The preview shows the entire worksheet, including the enabled summary
information, detail table columns, actions, and column-level and plan-level information.

The approvals and communication task worksheets don't have the Preview tab.

Related Topics

• Compensation and Promotion Worksheet Actions

• Performance Worksheet Actions

• Communication Worksheet Actions

• How the Ranking Score Is Calculated

Information Configuration in All Task Worksheet Displays

You can provide managers with important information in the page header of any task worksheet when you configure
the worksheet display.

For example, you can explain policies that apply to merit increases, performance evaluations, or promotions for the
upcoming focal compensation cycle. You can also include links to details.

293

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 52
Worksheets: Worksheet Display Configurations

294

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 53
Worksheets: Column Properties

53  Worksheets: Column Properties

General Properties of Worksheet Columns

You control the column appearance, position, and data storage using the options available in the General section of the
Configure Column Properties page. The available properties depend on the type of column you're configuring and the
selections you make on the page.

Here's a comprehensive list of the General section properties:

Field

Column

Description

Read-only field that identifies the column you're configuring the properties for.

Column Width in Pixels

Set the specific width, anywhere from 50 to 200 pixels.

Data Type

Read-only field that identifies whether the column values are numbers or characters.

Decimal Place to Display

Identify the number of places to show to the right of the decimal.

Default Sequence

Display Name

Default position of the column in relation to the other columns in the summary area, detail table, or
dialog box that you're configuring.

Identify the column with a name that's meaningful to the people working with the workforce
compensation plan.

Enable large amount of text

For user-defined text columns 12 -- 15, let managers enter up to 4,000 characters in the column.

Include 0 allocations in summary totals

Include the 0 allocations in the summary counts when you start Workforce Compensation plan cycle.

Include in audit trail

Include changes made to this column in the audit trail.

Monetary

Show the monetary values in the currency selected on the worksheet. The worksheet currency could
be the corporate currency, the manager's preferred currency, or the individual's local currency. When
the manager switches the currency, the worksheet converts the monetary values from the previous
currency to the current currency using the specified conversion rate.

Option to Display in Worksheet

For the country column, specify how the country information is displayed. Choices are country code,
 country name, and country code and name.

Rounding Rule

Specify whether to round numbers up or down and to what decimal place, such as Round down to .01.
Or, you can use currency rounding and make sure to populate Configure Currency Properties using
the Configure Plan Currency task.

Show numeric separators

Show separators for numbers, such as commas and periods.

Show totals

Include the total for all components in the summary section of the compensation worksheet. Available
for only numeric compensation component columns on the Summary tab.

Value Remains Unchanged

Keep the percentages stored in these columns, even when the corresponding amount changes:

• Compensation Percentage of Eligible Salary

• Compensation Percentage of Maximum

• Compensation Percentage of Minimum

295

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 53
Worksheets: Column Properties

Field

Description

• Target Percentage

• Target Percentage Maximum

• Target Percentage Minimum

• Worker Budget Percentage

• Percentage of Budget Pool

Wrap text

Adjust row height rather than column width to show all of the value.

Related Topics

• Overview of Worksheet Display in Workforce Compensation Plans

Visibility and Access Properties of Worksheet Columns

You control the visibility of and access to the column using options on the Configure Column Properties page. The type
of column you're configuring determines whether this section is available.

Main Column Settings
Determine whether to include the column in the worksheet and if people can only view data or can also update it using
main column settings. If you enable the column, you can also specify whether it should not appear until the manager
opts to show it. If you initially hide the column, you need to enable View on the Actions tab so that managers can show
it. You can also control general column access. If you set role-based overrides, the main column access setting applies to
all roles not identified as part of the override.

Role-Based Overrides
You can refine column visibility and access by roles. You select the main column setting you want to override. Next you
specify whether the override applies to either the people who have the added roles or who have none of them. And
then you add the applicable roles. Any role-based overrides take precedent over the main column visibility and access
settings.

We recommend that you configure the main column setting to apply to the majority of roles. Then, configure the
override settings for the least affected roles.

Example Configurations
You want everyone but line managers to see the current compa-ratio column.

In the column properties Visibility and Access section, set Override Setting to Not Enabled.

1. Enable the Salary Range Compa-Ratio - Current column.
2.
3. Set Condition to User has any of these roles.
4. Add the Line Manager role.

296

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 53
Worksheets: Column Properties

You want everyone to see the Individual Performance Multiplier user-defined column but only compensation
managers to update values.

In the column properties Visibility and Access section, set Override Setting to Updatable.

1. Enable a user-defined numeric column and name it Individual Performance Multiplier.
2.
3. Set Condition to User has any of these roles.
4. Add the Compensation Manager role.

You want everyone to see and update the Individual Performance Multiplier user-defined column. You don't want
alternate approvers who aren't compensation or line managers to view or update it.

1. Enable a user-defined numeric column and name it Individual Performance Multiplier.
2.
3. Set Condition to User has none of these roles.Add the Line Manager and Compensation Manager roles.

In the column properties Visibility and Access section, set Override Setting to Not enabled.

Related Topics

• Overview of Worksheet Display in Workforce Compensation Plans

• Performance Considerations for Workforce Compensation Plans

Default Value Properties of Worksheet Columns

You can set default values for the column by selecting from the options available in the Default Values section of the
Configure Column Properties page. The values populate the worksheet column when you run the Start Workforce
Compensation Cycle process.

Here are properties that you can select from to set default values. Unless otherwise specified, after you set a property,
the other properties disappear except Default value subject to refresh. You can see all properties again by clearing the
current setting.

Property

Description

Default Value

Enter a specific number of series of characters that appears by default in the column.

Default and Override Formula

Replace any existing values, including blank, with default values returned by the specified
Compensation Default and Override formula. For example, use a formula to get stored scores, rating,
 incentive plan amounts, target percentages, and special earning calculator values. Then use the
formula results to set default values for the column.

To verify that the selected formula returns the expected results, run a test using a sample person
record. Run the test by clicking the Test Condition and Column Results icon next to the formula.

•

•

•

If you get an incorrect formula, use the Fast Formulas task to correct your formula.

If you don't see an expected salary, make sure that the person's salary record exists as of the HR
data extract date.

If a person unexpectedly has an Ineligible status, check the eligibility profile for their assignment.

Compensation Derived Factor

Set default column values using a compensation derived factor. You create derived factors for
compensation using the Derived Factors task in the Compensation work area.

Cross Reference Plan

Select the workforce compensation plan with the data you want to use as default values in this column.
It can be the same plan.

297

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 53
Worksheets: Column Properties

Property

Description

After you select the plan, you need to specify which cycle and column to extract the default values
from.

External Data Record Type

Specify whether the external data you're showing in the column is from a legacy application or third
party.

After you select the record type, you need to select the external data column to get the default values
from, for example, Column 16.

Reference
For descriptions of every worksheet column, see Workforce Compensation Worksheet Configuration Definition
(document ID 1450891.1) on My Oracle Support (support.oracle.com). You can also see this information:

• The navigation path for columns that map directly to a field in Oracle Fusion Global HR Cloud Service

•

•

If you can default column values using a plan cross-reference

If people can update the values in their plan budget and task worksheets.

Related Topics

• Miscellaneous Rate Component Columns and User-Defined Columns

• Overview of Worksheet Display in Workforce Compensation Plans

• When to Use a Fast Formula or Dynamic Column to Display Information in a Worksheet Column

• Formula Type Is Compensation Default and Override

Cross-Reference Column Properties

You can use values from another column as default values for a column as long as neither column is a percentage
column.

That other column can be in the same worksheet, a different worksheet in the same plan, or a worksheet in a different
plan. For example, you want your managers to see all compensation for the workforce compensation cycle when they're
planning salary and bonus changes. Because they use separate plans to make these changes, you cross-reference the
relevant amounts from the other plan.

•

•

In the salary plan worksheet, you enable a column, such as a miscellaneous rate or user-defined column, to
show the bonus amounts as default values.

In the bonus plan worksheet, you enable a similar column to show the salary amounts as default values.

Or maybe you want to generate a single compensation change statement that shows the compensation changes from
the multiple plans managers use in the cycle. You create a plan that has only a communication task worksheet. Then
you enable and configure the columns, as shown here.

298

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 53
Worksheets: Column Properties

Compensation Change Statement
Column

Cross-Reference

Compensation Amount - Component 1

Merit plan, Compensation Amount - Component 1 column

Compensation Amount - Component 2

Bonus plan, Compensation Amount - Component 1 column

Compensation Amount - Component 3

Stock plan, Compensation Amount - Component 1 column

The worksheet with the cross-references shows the latest referenced data as soon as people save their changes to that
data.

Cross-Reference Plan
You can cross-reference a column from any active plan, even plans with no started cycles. You can even cross-reference
the same column in the same plan worksheet to use values from a previous workforce compensation cycle. For
example, you want managers to consider target amounts or bonuses from the previous cycle when they make their plan
changes in the current cycle.

Managers can't see the default values for plans with no started cycles. You need to run the Start Workforce
Compensation Cycle process for the relevant plans and then they can see the default values.

Cycle Matching
Here's how you can specify which started workforce compensation cycle to get the referenced values from. The plan
cycle name and extract dates come from the plan cycles configurations of the plan with this worksheet and the cross-
referenced plan.

Value

Description

Same Cycle Extract Date

Get the reference data from the plan cycle with the same HR data extraction date as this plan's cycle.

Same Cycle Display Name

Get the reference data from the plan cycle with the same name as this plan's cycle.

Previous Cycle Extract Date

Get the reference data from the plan cycle with the HR data extraction date that's closest to, but still
before this plan cycle's extract date.

Latest Cycle Extract Date

Get the reference data from the most recent plan cycle, without regard to this plan cycle's extract date.
Typically, you use this value in a plan that's always available and automatically clears after the new
cycle runs.

Reference
For descriptions of every worksheet column, see Workforce Compensation Worksheet Configuration Definition
(document ID 1450891.1) on My Oracle Support (support.oracle.com). You can also see this information:

• The navigation path for columns that map directly to a field in Oracle Fusion Global HR Cloud Service

•

•

If you can default column values using a plan cross-reference

If people can update the values in their plan budget and task worksheets.

299

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 53
Worksheets: Column Properties

Related Topics

• Default Value Properties of Worksheet Columns

• Overview of Worksheet Display in Workforce Compensation Plans

Formula Type Is Compensation Default and Override

To determine the default values for a worksheet column in a workforce compensation plan, you can create formulas
using the Compensation Default and Override formula type.

Here's a comprehensive list of the contexts available to this type of formula:

• DATE_EARNED

• EFFECTIVE_DATE

• END_DATE

• START_DATE

• HR_ASSIGNMENT_ID

• HR_TERM_ID

• JOB_ID

• LEGISLATIVE_DATA_GROUP_ID

• COMPENSATION_RECORD_TYPE

• ORGANIZATION_ID

• PAYROLL_ASSIGNMENT_ID

• PAYROLL_RELATIONSHIP_ID

• PAYROLL_TERM_ID

• PERSON_ID

The database items available for this type of formula are related to Person, Assignment, Salary, Element Entries,
Compensation Record, and From and End Dates.

These are the input variables available to this type of formula:

Input Value

Data Type

Required

Description

CMP_IV_PLAN_ID

Number

CMP_IV_PERIOD_ID

Number

CMP_IV_COMPONENT_ID

Number

CMP_IV_ITEM_NAME

Char

Y

Y

Y

Y

Unique numeric identifier for the
workforce compensation plan

Unique numeric identifier for the
fiscal calendar period

Unique numeric identifier for the
workforce compensation plan
component

Name for the workforce
compensation plan item

300

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 53
Worksheets: Column Properties

Input Value

Data Type

Required

Description

CMP_IV_PERSON_ID

Number

CMP_IV_PLAN_START_DATE

Date

CMP_IV_PLAN_END_DATE

Date

CMP_IV_PLAN_ELIG_DATE

Date

CMP_IV_PERFORMANCE_EFF_
DATE

Date

CMP_IV_PROMOTION_EFF_DATE

Date

CMP_IV_XCHG_RATE_DATE

Date

CMP_IV_ASSIGNMENT_ID

Number

Y

Y

Y

Y

Y

Y

Y

Y

Unique numeric identifier for the
individual associated with the
workforce compensation plan

Date when the workforce
compensation plan becomes active

Date when the workforce
compensation plan becomes
inactive

Date when the workforce
compensation plan becomes
eligible

Date to use for compensation
performance ratings

Date on which job, grade, and
position changes take effect

Date when the Start Workforce
Compensation Cycle and Refresh
Workforce Compensation Data
processes obtain conversion rates
from the general ledger daily rates
table.

Date to use for assignments

These are the return variables available to this type of formula:

Return Value

Data Type

Required

Description

L_DEFAULT_VALUE

Number/Char/Date

L_DATA_TYPE

Char

Y

Y

Default value from the formula.
The date should be in yyyy/mm/
dd format

Data type of the column

This sample formula determines the value of a column based on its item name.

/***********************************************************
FORMULA NAME : Compensation Default and Override Formula
FORMULA TYPE : Compensation Default and Override
DESCRIPTION : Defaults the value of a column based on its item_name
*************************************************************/

/*=========== INPUT VALUES DEFAULTS BEGIN =====================*/
INPUTS ARE CMP_IV_PLAN_ID (number), CMP_IV_PERIOD_ID (number), CMP_IV_COMPONENT_ID (number),
 CMP_IV_ITEM_NAME (text)
/*=========== INPUT VALUES DEFAULTS ENDS======================*/

/*================ FORMULA SECTION BEGIN =======================*/

DEFAULT FOR CMP_IV_ITEM_NAME IS 'YYYYYYY'
L_DEFAULT_VALUE = to_char(0)
IF (CMP_IV_ITEM_NAME = 'AmountComp1') THEN
(

301

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 53
Worksheets: Column Properties

L_DEFAULT_VALUE = to_char(3333)
)
ELSE IF (CMP_IV_ITEM_NAME = 'AmountComp2') THEN
(
L_DEFAULT_VALUE = to_char(7777)
)
ELSE
(
L_DEFAULT_VALUE = to_char(-999)
)
RETURN L_DEFAULT_VALUE

/*================ FORMULA SECTION END =======================*/

Related Topics

• Default Value Properties of Worksheet Columns

• Formula Compilation Errors

• Formula Execution Errors

• When do I run the Compile Formula process?

• Example of Writing a Fast Formula Using Formula Text

Sample Compensation Default and Override Formulas

You can test setting default values for worksheet columns in a workforce compensation plan using these sample
formulas of type Compensation Default and Override. You can also use these sample formulas to create your own
versions.

CMP_ELIGIBLE_SALARY_PRORATION_DAILY_AVERAGE
Calculates the eligible salary by averaging the daily salary. The formula accounts for number of days that a salary is in
effect during the evaluation period of the workforce compensation cycle.

CMP_ELIGIBLE_SALARY_PRORATION_MONTH_END_AVERAGE
Calculates the eligible salary by averaging the salary on the last day of each month in the evaluation period of the
workforce compensation cycle. The calculation uses the salary on the last day of the evaluation period for midmonth
evaluation end dates.

CMP_ELIGIBLE_SALARY_PRORATION_DAILY_AVERAGE_NINETY_DAY_MIN
Calculates the eligible salary by averaging the daily salary. The formula accounts for the number of days that a salary
is in effect during the evaluation period of the workforce compensation cycle. It returns 0 for people who worked fewer
than 90 days.

CMP_ELIGIBLE_SALARY_PRORATION_DAILY_AVERAGE_USING_FTE
Calculates the eligible salary by averaging the daily salary adjusted for part-timers. The formula accounts for the
number days that a salary is in effect and FTE during the evaluation period of the workforce compensation cycle.

302

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 53
Worksheets: Column Properties

CMP_ELIGIBLE_SALARY_PRORATION_DAILY_AVERAGE_FOR_JOBS
Calculates the eligible salary by averaging the salary for the number of days the person holds a specific job code on the
assignment. The formula accounts for the number of days that a salary is in effect during the evaluation period of the
workforce compensation cycle.

Related Topics

• General Properties of Worksheet Columns

• Formula Type Is Compensation Default and Override

Salary and Element Mapping Properties of
Compensation Amount Columns

You can specify whether approved compensation amount changes for the component transfer to HR as single
payments or as adjustments to people's salary amounts. Use the options in the Element Mapping section of the
Configure Column Properties page.

Single Payment
To pay the changes as a single payment, set Post as Salary to No. Then add the payroll elements to use to pay the
specified compensation amount. You can add multiple payroll elements to accommodate payments in different
currencies and to pay people in different legislative data groups.

Base Pay Adjustment
To adjust base pay by the specified compensation amount, set Post as Salary to Yes. When the Transfer Workforce
Compensation Data to HR process runs, it updates each person's salary with the amount stored in the compensation
amount column of the component. You can also post any itemized adjustments for future reference.

Related Topics

• Compensation Components in Workforce Compensation Plan Worksheets

• Compensation Component Number and Name, and Detail Table of Worksheet Display

• How You Enable Salary Itemization Using Incremental Components

•

Incremental Salary Component Lookups

Post Incremental Itemized Salary Adjustments in a
Workforce Compensation Plan to HR

303

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 53
Worksheets: Column Properties

To post the component amount change as an itemized adjustment, you select the applicable incremental salary
component. The Transfer Workforce Compensation Data to HR process then updates each person's salary. It also
adds the incremental salary component and that component adjustment amount to the salary for future reference.

To post the compensation amounts of all enabled incremental components as a single adjustment to each person's
salary, leave these fields blank:

• Salary Component

• Salary Includes Simple Components

Example Configuration
Your workforce compensation plan has a compensation task worksheet with the Merit and COLA compensation
components enabled. A manager uses the worksheet to give someone a $5,000 merit increase and a $1,500 cost of
living increase. Here's how you configure the column properties so both component amounts increase the person's
salary amount by $6,500. The adjustments also transfer for future reference.

• For both components, set Post as Salary to Yes.

• For the Compensation Amount - Merit component, set Salary Component to Merit.

• For the Compensation Amount - COLA component, set Salary Component to Cost of living.

Related Topics

• Considerations for Using Salary Bases with Incremental Components versus Simple Components

• Salary Amount Is Determined by Incremental Components

• How You Enable Salary Itemization Using Incremental Components

• Compensation Components in Workforce Compensation Plan Worksheets

• Compensation Component Number and Name, and Detail Table of Worksheet Display

Post Salary Compensation Amounts to Simple
Components in a Workforce Compensation Plan to HR

You can distribute and post salary compensation amounts back to people whose salaries include simple components
through the transfer process.

You navigate to the properties for the compensation amount worksheet column you use for your salary increases and
scroll down to the Salary and Element Mapping section.

1. Select the Yes option for Post as Salary.
2. Select the Yes, manager does not enter simple components option for Salary Includes Simple Components.

You may also have Salary Includes Rates enabled.

If you choose the Yes, manager enters simple components option, you need to configure the section on the Individual
Worker Display page instead.

Only those salary bases that use simple components appear in the search. After you select a salary basis, the associated
simple components appear. The derived components that contribute to the overall salary are also listed in the table, but
they don't have any distribution setup support.

304

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 53
Worksheets: Column Properties

Related Topics

• Considerations for Using Salary Bases with Incremental Components versus Simple Components

• Salary Amount Is Determined by Simple Components

• Compensation Components in Workforce Compensation Plan Worksheets

• Compensation Component Number and Name, and Detail Table of Worksheet Display

Rate Application Result Options for Salary Adjustments
to Simple Components

When you run the Transfer Workforce Compensation Data to HR process you select one of the rate application result
options.

Here are the 4 rate application result options:

Rate Application Result Options

Option

Amounts

Percentages

Results

Rate receives a change amount as entered here (which can be an increment or decrement amount to
previous rate value).

Rate receives a change amount as a percentage of the base salary change amount (increment/
decrement in base salary).

Percentage of Remaining

The application first allocates the rates that use Amount or Percentage type of result and arrives at
the remaining increment in base salary. Then it applies the specified percentage on this remaining
increment amount to arrive at the change amount for the rate.

Balances

Rate receives the balance increment remaining after calculating other rates.

Related Topics

• Considerations for Using Salary Bases with Incremental Components versus Simple Components

• Salary Amount Is Determined by Simple Components

• Compensation Components in Workforce Compensation Plan Worksheets

• Compensation Component Number and Name, and Detail Table of Worksheet Display

Considerations for Posting Salary Adjustments to Simple
Components

You need to consider these points when you post salary adjustments to simple components.

305

Oracle Fusion Cloud Human Resources
Implementing Compensation

Consider the following:

Chapter 53
Worksheets: Column Properties

• The Balance rate application result method is required for each salary basis you configure.

• The simple component distribution condition builder uses worksheet columns only.

• Derived components get calculated as usual during transfer process. All other rate types allow for distribution

setup.

• The Transfer process doesn't post the salary if the overall salary after distribution doesn't match the salary

proposed in the worksheet.

• The Overall Salary, Fixed Amount and Fixed Percentage simple components won't have any distribution

setup, so you can't edit the Rate Application Results and Valuefields for those simple components.

• You can edit the rate application results for the simple components of User enters amount and User enters

percentage types.

• Simple components of type Progression Grade Ladder Rate aren’t supported.

Related Topics

• Considerations for Using Salary Bases with Incremental Components versus Simple Components

• Salary Amount Is Determined by Simple Components

• Compensation Components in Workforce Compensation Plan Worksheets

• Compensation Component Number and Name, and Detail Table of Worksheet Display

How to Post Back Salary Changes for People Whose FTE
is Less Than 1

When workers have an FTE that is less than 1 you can let managers edit the Base Salary Change Amount and Base
Salary Percentage Change columns in the worksheet.

When you configure the columns in setup and your plan has a single salary component, you need to deselect the Read-
Only check box to let managers edit the column in the worksheet because the value is selected by default. Managers
enter the salary change amount and the worksheet uses that amount to reverse calculate the compensation amount in
the plan frequency.

Rounding Rule Behavior When You Post Back Salary
Changes for People Whose FTE is Less Than 1

You configure the rounding rules when you set up the salary information columns. The application applies rounding
rules when managers edit the columns in the worksheet.

Here’s how the application rounds the amounts:

• Base Salary – You can configure rounding rules in setup for Base Salary - New, Base Salary Change Amount,

and Base Salary Percentage Change columns.

306

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 53
Worksheets: Column Properties

•

•

•

If all three of the columns have rounding rules, only the rounding rule on Base Salary - New column is honored
and the other rounding rules are ignored.

If there's no rounding rule configured for Base Salary - New, and both Base Salary Change Amount and Base
Salary Percentage Change columns have rounding rules configured, preference is given to Base Salary Change
Amount. Rounding rule configuration on Base Salary Percentage Change is ignored.

If there is no rounding rule on either Base Salary - New or Base Salary Change Amount, a rounding rule on Base
Salary Percentage Change is honored.

• Here's the order of preference for rounding rules. It depends on which column you've configured a rounding

rule:

a. Base Salary - New
b. Base Salary Change Amount
c. Base Salary Percentage Change

Rounding Rule Behavior for Base Salary – Current
Column

You can configure a rounding rule when you set up the Base Salary - Current column. The rule applies when managers
edit the column in the worksheet.

The salary data of the assignment without rounding applies for this column by default. If the data comes from a column
default, like a fast formula, then the rounding rule you configure for the column during setup applies.

307

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 53
Worksheets: Column Properties

308

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 54
Worksheets: Dynamic Columns in Worksheet Display
Configurations

54  Worksheets: Dynamic Columns in
Worksheet Display Configurations

Overview of Dynamic Columns in Workforce
Compensation Plan Worksheets

You can calculate and display values that vary by individual for many worksheet columns, including most percentage
columns. You do this by building conditional expressions for the appropriate columns. For example, you want to base
the bonus eligible salary on the current annual salary.

You can also determine the values in one column using values in another column. For example, as part of the annual
bonus review, you want to show managers the bonus target amounts to consider during allocations. You build a
dynamic calculation that varies the Bonus Target Amount by each individual's performance rating. For example, people
with an Outstanding performance rating have a bonus target amount that's 10% of their bonus eligible salary. People
with a Meets rating have an amount that's 5%.

Validation and Testing
You can validate each condition as you build it and test all conditions and column results on the Dynamic Calculation
page. You can also export the conditions on the page to review and validate them outside of the worksheet
configuration.

Column Information Sourced Outside the Plan
When the information source for a column is outside the workforce compensation plan, you might need to run the
Refresh Workforce Compensation Data process. For example, dynamic columns that depend on the performance
management overall rating might not show the actual performance rating until after you run the refresh process.

Evaluation Order, Sequence, and the Default Condition
of Dynamic Worksheet Columns

The evaluation order of dynamic columns identifies the calculation order when the condition of one column uses the
results of another column.

For example, you build the dynamic column condition of the Target Compensation Amount Minimum component
column to use eligible salary. You set the evaluation order to 1 for the dynamic column of the Eligible Salary component
column. And you set the evaluation order to 2 for the corresponding Target Compensation Amount Minimum
component column. This way the dynamic column for target compensation uses the appropriate eligible salary in its
conditions.

309

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 54
Worksheets: Dynamic Columns in Worksheet Display
Configurations

Sequence and Default Condition
The sequence identifies the calculation order for conditions on the same Dynamic Column page. The worksheet
evaluates every condition for the column in sequence order. The default condition is the condition to use when no
other conditions are met, so it has to always be the highest sequence. For example, condition 1 gives people with a
performance rating of 5 a 10% bonus. For people who don't have a 5, condition 2 checks to see if they have a 4. If they
do, they get a 5% bonus. Condition 3, the default condition, says that everyone else doesn't get a bonus. If you don't
select a default condition and no conditions are met, the column displays no values.

Configure conditions that cover the most workers with the highest sequence numbers to improve worksheet and batch
process performance. Test a few dynamic calculations at a time to assess the performance impact and decide what level
of impact the plan audience can accept.

Related Topics

• Configure the Compensation Amount Dynamic Column of the Bonus Component to Reward High Performers

Triggering Events for Conditions of Dynamic Columns
and Alerts

You specify when to evaluate the conditions of dynamic columns and alerts by selecting one or more of these triggering
events:

Triggering Event

Description

Dynamic Column Example

Alerts Example

Calculate the eligible salaries that
managers use during the cycle.

Let the worksheet managers know
that an individual got a recent pay
increase and isn't eligible.

Re-evaluate people's eligibility
for the workforce compensation
plan and worksheet compensation
components.

Let the worksheet manager know
that performance management
ratings were updated and target
ranges were adjusted.

Calculate people's total
compensation amount after
managers make changes to current
salary amounts.

Let the worksheet manager know
that they're giving an individual
more than the target and they
need to provide a justification.

Start compensation cycle

Refresh data

Change worksheet data

When the Start Workforce
Compensation Cycle process
runs, it calculates the results for
all dynamic column and alert
conditions.

When the Refresh Workforce
Compensation Data process
runs, it re-evaluates all dynamic
conditions, fast formulas, and
the HR data used in dynamic
conditions. It also re-evaluates all
alert conditions.

When managers enter or change
the value and leave the field,
the worksheet re-evaluates the
condition and corresponding
results.

This trigger might slow worksheet
performance. The more dynamic
columns you use or the more
conditions for the dynamic column,
 the longer the worksheet takes
to respond. For example, you
select this option on four dynamic
columns, each with five conditions.
When the manager tabs out of a

310

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 54
Worksheets: Dynamic Columns in Worksheet Display
Configurations

Triggering Event

Description

Dynamic Column Example

Alerts Example

worksheet field, the worksheet
evaluates all 20 conditions,
 regardless of whether the column
has dynamic column settings.
Use it for only column results that
depend on data that changes in the
worksheet.

Related Topics

• Configure the Compensation Amount Dynamic Column of the Bonus Component to Reward High Performers

Descriptions for Dynamic Worksheet Column Conditions

You can add up to 1600 characters of meaningful description for the dynamic column condition. Make it clear to
people reviewing the worksheet column configuration in later workforce compensation cycles what the purpose of the
condition is.

You can also explain from where or when information from outside the worksheet came. Click the Edit icon next to the
field to add or change text.

Related Topics

• Configure the Compensation Amount Dynamic Column of the Bonus Component to Reward High Performers

Basic and Advanced Tabs When Building a Condition for
a Dynamic Column or an Alert

You can build a condition by selecting worksheet columns, operators, and values in the appropriate order. Use the
Basic tab of the Edit Condition dialog box. You can build or edit a condition directly in the Column Results field on the
Advanced tab.

Reference
For descriptions of every worksheet column, see Workforce Compensation Worksheet Configuration Definition
(document ID 1450891.1) on My Oracle Support (support.oracle.com). You can also see this information:

• The navigation path for columns that map directly to a field in Oracle Fusion Global HR Cloud Service

•

•

If you can default column values using a plan cross-reference

If people can update the values in their plan budget and task worksheets.

311

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 54
Worksheets: Dynamic Columns in Worksheet Display
Configurations

To help you locate columns, the document Worksheet Configuration tab organizes information in the same groupings
as the Configure Worksheet Page Layout pages.

Related Topics

• Configure the Compensation Amount Dynamic Column of the Bonus Component to Reward High Performers

Configure the Compensation Amount Dynamic Column
of the Bonus Component to Reward High Performers

Here's how you can configure the dynamic column of the Compensation Amount - Bonus component to calculate
bonuses according to performance ratings.

For example, people with outstanding performance ratings get a bonus that's 10% of their annual salary. People who
exceed expectations get a 5% bonus. People with other performance ratings don't get any bonus.

Before you start

You need to complete these configuration tasks before you can configure the dynamic column:

1. Create a workforce compensation plan using the Workforce Compensation Plans task.
2. Configure a bonus compensation component using the Configure Compensation Components task.
3. Configure performance management or compensation performance ratings that use a scale of 1 to 5 where 5 is

Outstanding and 4 is Exceeds. Use the Configure Performance Ratings task.

4. Enable the appropriate performance rating columns and the Compensation Amount column of the bonus

component using the Configure Worksheet Display task.

Here's what to do

1. Configure the dynamic compensation amount column.

a.
In the row for the bonus component Compensation Amount column, click the Dynamic Column icon.
b. On the Dynamic Column page, select the Start compensation cycle and Refresh data triggering events.

2. Build the condition for people with a 5 rating.

This condition identifies people with a performance management rating of 5 and awards them a bonus that's 10% of
their annual full-time salary.

a. Click the Add icon.
b.
c.

In the Sequence field, enter 1.
Identify the eligible people.

In the Column field, select Performance Management Overall Rating.
In the Operation field that appears, select Equals.
In the Fixed Value field that appears, enter 5.

i. Under Condition, the Create or Edit Expression icon.
ii. On the Edit Condition dialog box, Basic tab, click Build Condition.
iii.
iv.
v.
vi. Click Done.
vii. Optionally, click Validate. On the confirmation, click OK.
viii. Click Apply.
d. Award the 10% bonus.

312

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 54
Worksheets: Dynamic Columns in Worksheet Display
Configurations

In the Column field that appears, select Annualized Full-Time Salary - Current.

i. On the Dynamic Column page, under Column Results, click the Create or Edit Expression icon.
ii. On the Edit Column Result dialog box, Basic tab, select Equation.
iii. Click Switch to Column.
iv.
v. Click Next.
vi.
vii.
viii. Click Done.
ix. Click Apply.

In the Operation field that appears, select Multiplied by.
In the Fixed Number field, enter .1.

e. Add the description.

i. On the Dynamic Column page, under Description, click the Create or Edit Description icon.
ii. On the Description dialog box, enter Award a 10% bonus to people with a performance rating of 5,

which identifies them as outstanding.

iii. Click Apply.

3. Build the condition for people with a 4 rating.

This condition identifies people with a performance management rating of 4 and awards them a bonus that's 5% of
their annual full-time salary.

a. Click the Add icon.
b.
c.

In the Sequence field, enter 2.
Identify the eligible people.

In the Column field, select Performance Management Overall Rating.
In the Operation field that appears, select Equals.
In the Fixed Value field that appears, enter 4.

i. Under Condition, the Create or Edit Expression icon.
ii. On the Edit Condition dialog box, Basic tab, click Build Condition.
iii.
iv.
v.
vi. Click Done.
vii. Optionally, click Validate. On the confirmation, click OK.
viii. Click Apply.
d. Award the 5% bonus.

In the Column field that appears, select Annualized Full-Time Salary - Current.

i. On the Dynamic Column page, under Column Results, click the Create or Edit Expression icon.
ii. On the Edit Column Result dialog box, Basic tab, select Equation.
iii. Click Switch to Column.
iv.
v. Click Next.
vi.
vii.
viii. Click Done.
ix. Click Apply.

In the Operation field that appears, select Multiplied by.
In the Fixed Number field, enter .05.

e. Add the description.

i. On the Dynamic Column page, under Description, click the Create or Edit Description icon.
ii. On the Description dialog box, enter Award a 5% bonus to people with a performance rating of 4,

which identifies them as exceeds expectations.

iii. Click Apply.

313

Oracle Fusion Cloud Human Resources
Implementing Compensation

4. Build the condition for people with lower ratings.

Chapter 54
Worksheets: Dynamic Columns in Worksheet Display
Configurations

This condition identifies people with a performance rating that's less than 4 and doesn't award them any bonus.

In the Sequence field, enter 3.

a. On the Dynamic Column page, click the Add icon.
b.
c. Select Default.
d. Award no bonus to everyone who failed to meet the other two conditions.

i. Under Column Result, click the Create or Edit Expression icon for the expression you just created.
ii. On the Edit Column Results dialog box, Basic tab, in the Fixed Value field, enter 0.
iii. Click Done.
iv. Click Apply.

e. Add the description.

i. On the Dynamic Column page, under Description for the condition you just created, click the Create

or Edit Description icon.

ii. On the Description dialog box, enter Don't award any bonus to people with a performance ratings

below 4.
iii. Click Apply.

5. Test the dynamic column conditions.

a. On the Dynamic Column page, click the Test Condition and Column Results icon.
b. On the Test Condition dialog box, complete the fields, as shown here.

Variable Name

Test Value

Performance Management Overall

5

Rating

Annualized Full-Time Salary -

50000

Current

c. Click Test.
d. Verify that the results are what you expected and click OK.

Related Topics

• Overview of Dynamic Columns in Workforce Compensation Plan Worksheets

When to Use a Fast Formula or Dynamic Column to
Display Information in a Worksheet Column

You can vary worksheet column results using fast formulas and dynamic columns. The best method depends on the
data you use, the complexity of the calculation, and how frequently you refresh worksheet data.

314

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 54
Worksheets: Dynamic Columns in Worksheet Display
Configurations

Data Used
Fast formulas can use any Oracle Fusion application data with a database item. Dynamic columns conditions can use
other worksheet columns.

Calculations
Fast formulas can be anywhere from simple to complex with multiple compound conditions or multiple database
records. Dynamic columns have simple if-then conditions or a few compound conditions.

Initializing and Refreshing Values
For both fast formulas and dynamic columns, the Start Workforce Compensation Cycle process sets the initial column
values. The Refresh Workforce Compensation Data process re-evaluates column values every time it runs with one of
these options selected:

• Refresh column defaults

• Full refresh

Dynamic column values are also re-evaluated if the refresh process runs with the Refresh dynamic columns option
selected. And they're re-evaluated every time a manager leaves a column field if the dynamic column configuration has
Change worksheet selected.

Configuration Process
You create formulas using the Fast Formulas task. You link them to worksheet columns using the Properties icon of the
worksheet column. You build dynamic conditions using the Dynamic Columns icon of the worksheet column.

Related Topics

• Overview of Dynamic Columns in Workforce Compensation Plan Worksheets

• Formula Type Is Compensation Default and Override

• Overview of Using Formulas

Copy Dynamic Column Configurations

You can copy dynamic column configurations from one plan to another or from one column to another within the same
plan.

Here’s how you copy dynamic column configurations from one plan to another or from one column to another within
the same plan:

1. Navigate to the Dynamic Column configuration page for the column you want to copy from.

2. Select the copy or duplicate icon on the toolbar. The Copy Dynamic Expressions page opens. On this page, you can

copy dynamic calculation expressions from the current plan or select a different plan.

3. Select the plan. The Source Display Name list of values lets you select a dynamic calculation to copy. Only the

columns that have dynamic calculations configured appear in the Source Display Name list of values. The Column
Names From columns shows the column names used in the dynamic expression based on the selection.

315

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 54
Worksheets: Dynamic Columns in Worksheet Display
Configurations

4. Show either the Current Plan names or the Source Plan names. If more than one dynamic expression exists for a

selected dynamic calculation, you can select and copy all or select some dynamic expressions to copy.

5. Select an option. The dynamic expressions are copied to the target column, and you receive a confirmation message.

6. Click Done to return to the Dynamic Column configuration page to view the copied expressions.

7. Save your changes. Newly added dynamic expressions have an icon to the left of the sequence number.

Related Topics

• Overview of Dynamic Columns in Workforce Compensation Plan Worksheets

316

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 55
Worksheets: Configuration Guidance for Salary and Budget
Component Columns, and Promotion Effective Date

55  Worksheets: Configuration Guidance for
Salary and Budget Component Columns, and
Promotion Effective Date

Guidelines to Configure the Eligible Salary Component
Columns

Many fast formulas and dynamic column conditions use eligible salary to determine percentages, such as allocation,
target, and worker budget percentages. So when you use percentage columns, you need to configure the Eligible Salary
column for each component enabled in the plan.

For example, you make eligible salary equal to each individual's current base pay. Or you might prorate their eligible
salary according to various factors, such as length of service or geographic location. You need to configure the Eligible
Salary column when the component budget pool stores budgets as percentages.

• To use a fast formula or derived factor to determine default values, you configure the column properties. You

can copy and modify delivered samples of eligible salary proration formulas using the Fast Formula task in the
Compensation work area. Use the samples with the Compensation Default and Override formula type.

• To build conditions that determine each individual's eligible salary, you configure the dynamic column settings.

• Worker budget percentages

Related Topics

• Default Value Properties of Worksheet Columns

• Overview of Dynamic Columns in Workforce Compensation Plan Worksheets

• Compensation Components in Workforce Compensation Plan Worksheets

• Formula Type Is Compensation Default and Override

Guidelines to Configure the Budget Amount - Worker
Component Columns

You can use compensation fast formulas to calculate the default monetary amounts shown in the Budget Amount -
Worker column of each enabled plan component. Or you can use dynamic column conditions to calculate the amounts.

Both formulas and conditions calculate the amounts in the individual's currency, determined by the local currency
determination code of the compensation component. But, budget and task worksheets store the amounts in the plan
currency. To calculate and show the correct results, dynamic column conditions need to divide the local currency value
by the corresponding Currency Conversion Rate component column.

317

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 55
Worksheets: Configuration Guidance for Salary and Budget
Component Columns, and Promotion Effective Date

Related Topics

• Default Value Properties of Worksheet Columns

• Overview of Dynamic Columns in Workforce Compensation Plan Worksheets

• Compensation Components in Workforce Compensation Plan Worksheets

• Formula Type Is Compensation Default and Override

Guidelines to Allocate Compensation as Percentage of
Budget

You can allocate compensation as a percentage of the budget pool instead of as a percentage of eligible salary or a flat
amount.

If you enable the Percentage of Budget column for any component, here's what else you need to do:

• On the Configure Worksheet Page Layout page, Detail Table tab, disable the Percentage of Eligible Salary

column for the corresponding component. Also make sure that the Value remains unchanged and Rounding
Rule column properties aren't selected. Use the Configure Worksheet Display task.

• On the Configure Modeling page, disable these allocation methods using the Configure Modeling task.

◦ Allocate n percent of eligible salary
◦ Increase n percent of eligible salary

Rounding Rules
The rounding rule set for the corresponding Compensation Amount column affects the amount calculated for
the Percentage of Budget Pool column. For example, a manager whose overall budget is 900 USD enters 4 in the
Percentage of Budget Pool column. Here are the amounts when the corresponding Compensation Amount column
does and doesn't have a rounding rule of Round to the nearest 10.

Column

Calculation

Amount with Rounding

Amount without Rounding

Component Amount

Entered Percentage / 100 * Overall
Budget Amount

40

(4 / 100) * 900

Percentage of Budget

Compensation Amount / Overall
Budget Amount

4.44

36

4

If you set a rounding rule for a Compensation Amount column, don't set a rounding rule for the corresponding
Percentage of Budget Pool column. Or if you select Use currency rounding for the Compensation Amount column,
don't select it and the rounding rule property for the Percentage of Budget Pool column. If you want to round the
percentage instead of the compensation amount, you do the opposite. Set either the Rounding Rule or the Use
currency rounding property for the Percentage of Budget Pool column. And make sure that neither property is set for
the Compensation Amount column.

318

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 55
Worksheets: Configuration Guidance for Salary and Budget
Component Columns, and Promotion Effective Date

Guidelines to Configure Default Values for the Promotion
Effective Date Column

The batch processes for workforce compensation use promotion effective dates in plan worksheets to get new salary
ranges and compa-ratios.

The processes also use the dates to get other salary metrics when the promotion includes a change to the person's
grade. You can set a default effective date for everyone promoted through a workforce compensation plan using the
Configure Plan Cycles task. Then, you can enable the Promotion Effective Date column in the appropriate task
worksheets and configure the column properties.

• Let managers override the default date for individuals they promote during the compensation cycle.

• Specify whether the Refresh Workforce Compensation Data process refreshes the Promotion Effective Date

column values.

Subject to Refresh

What Happens

Yes

No

a. A manager overrides the default promotion effective date.
b. The Refresh Workforce Compensation Data process changes the worksheet column

date back to the default promotion effective date set for the plan cycle.

c. The process uses the default date to refresh the corresponding salary metrics.

The Refresh Workforce Compensation Data process uses the promotion effective date to

refresh the corresponding salary metrics. The date in the worksheet column is from either of

these sources:

◦ Default promotion effective date for the plan cycle
◦ Manager-entered date

Related Topics

• Workforce Compensation Plan Cycle Dates

• Default Value Properties of Worksheet Columns

• Overview of Worksheet Display in Workforce Compensation Plans

• Refresh Workforce Compensation Data Process

Update Grade Step as Part of a Workforce Compensation
Cycle

You can let managers update a person's Grade Step as a part of a workforce compensation cycle when you configure the
worksheet display.

319

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 55
Worksheets: Configuration Guidance for Salary and Budget
Component Columns, and Promotion Effective Date

As a part of the column properties, only the Proposed Grade Step is included in the audit trail and allowed for updates.
The Proposed Grade Step column is read only by default. You must explicitly choose to allow worksheet managers
to update the column. All 3 new columns can be initially hidden, enabled, allow for role-based column access to be
configured, and used in dynamic calculations and alerts. The columns are available for display in Individual Worker
Display and Administer Workers.

Proposed Grade Column When You Update the Grade
Step

Depending on the criteria met for the assignment, values are shown from one of these sets: All Grades of the set, Valid
Grades of Position and Job, or Grades of the assignment grade ladder.

• When the assignment doesn't have a Grade Ladder and if the profile option PER_ENFORCE_VALID_GRADES is

disabled the Proposed Grade list of values shows all the Grades available for the respective set.

• When the assignment doesn't have a Grade Ladder and if the profile option PER_ENFORCE_VALID_GRADES is
enabled the Proposed Grade list of values shows all Valid Grades available depending on the Position or Job for
the respective set.

• When the assignment has a Grade Ladder, regardless of the value of the profile option

PER_ENFORCE_VALID_GRADES, the Proposed Grade list of values shows the Grades with respect to the Grade
Ladder.

Worksheet Effects When You Update the Grade Step

The Proposed Grade Step column shows the steps of a Grade if the Grade is part of a Grade Ladder configured to use
Grade and Steps.

When you select a Grade using the Proposed Grade column, and if the Grades are from a Grade Ladder configured to
use Grade and Steps, the first Step in the sequence shown by default. Worksheet managers can change or override it
with any of the Steps from the list of values. When the Proposed Grade column isn’t filled with a selected Grade and if
the current Grade is part of a ladder that configured to use Grade and Steps, the Proposed Grade Step drop down shows
the respective Steps for the current Grade. In a scenario where the Proposed Grade or Current Grade doesn't have Steps,
the Proposed Grade Step list of values remains blank.

Note:  The Compensation Amount Column you selected to post as salary is READ-ONLY for people with a Grade
Ladder with Include salary updates set to Yes. Their compensation amount is calculated based on the value selected
in the Grade Step column.

320

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 55
Worksheets: Configuration Guidance for Salary and Budget
Component Columns, and Promotion Effective Date

Base Salary - New Column When You Update the Grade
Step

When a Grade Step is proposed in the worksheet, it automatically fetches the Step value as the new base salary, subject
to these conditions:

• The Grade Ladder should be of type Grade and Step.

• The Grade Ladder should have Include salary updates set to Yes.

• The Grade Ladder should have Salary Calculation Method set to Use grade step rate.

• There should be only one component in the Workforce Compensation plan that has its compensation amount

set to Post as salary.

• Worker's salary basis type isn’t Salary Rates or Simple Components.

If the Proposed Grade Step's value can't be determined, the Base Salary - New column in the worksheet (along with the
associated compensation amount column) is set to null. This happens in these cases:

• The Grade Ladder's currency doesn't match the base salary currency of the worker.

• The Proposed Grade Step doesn't have a value defined in the Grade Ladder.

The Base Salary - New (along with the associated compensation amount column) becomes read-only. You can only
propose it by selecting a Proposed Grade Step when these conditions are met:

• The Grade Ladder is of type Grade and Step.

• The Grade Ladder has Include salary updates set to Yes.

In other cases, the column behavior remains as before. The application calculates the Base Salary - New based on the
Step value using this formula:

Base Salary - New = (Step Value * Step Annualization Factor) / (Pay Annualization Factor)

If the base salary frequency of the worker isn't hourly and Salary Adjustment Type of the ladder is set to a value other
than blank (FTE less than 1 only OR FTE not equal to 1) and the FTE of the worker's assignment matches the selection,
then FTE adjustment happen using this formula:

Base Salary - New = (Step Value * Step Annualization Factor * FTE of the worker's assignment) / (Pay
 Annualization Factor)

Downloaded Workbook When You Update the Grade
Step

If you select the Manage in Workbook option the downloaded workbook has these columns: Current Grade Ladder,
Current Grade Step, and Proposed Grade Step.

The first 2 are read-only columns and the last one is editable according to how you set up the preferences. The
downloaded workbook works the same way the worksheet does.

321

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 55
Worksheets: Configuration Guidance for Salary and Budget
Component Columns, and Promotion Effective Date

People can select Proposed Grade Step values either from the list of values of the Proposed Grade Step column by
double-clicking on the respective cell or by entering a value in the cell and uploading it.

Note:  The Proposed Grade Step list of values shows the values according to the existing Grade or Proposed Grade
value. If people select a new Proposed Grade in the downloaded workbook the Proposed Grade Step list of values
shows step values according to the old Grade or Proposed Grade value until the new Proposed Grade is uploaded.

If people enter a valid Proposed Grade value but an invalid Proposed Grade Step value, the upload fails.

322

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 56
Worksheets: Miscellaneous Rate Component Columns,
User-Defined Columns, and External Data in Task
Worksheets

56  Worksheets: Miscellaneous Rate
Component Columns, User-Defined Columns,
and External Data in Task Worksheets

Miscellaneous Rate Component Columns and User-
Defined Columns

You can include your own numeric, text, and list information in worksheet columns of workforce compensation plans.

Miscellaneous Rate Component Columns
You can share numeric values with managers and let them enter their own values using the six miscellaneous rate
columns under the component groups. For example, you want to use a target stored outside the plan to calculate
bonuses. All six columns are updatable and you can default values for them using a plan cross-reference. But, if an
individual isn't eligible for the component, managers can't edit their value.

With these columns, you can show totals for the detail table population in the summary table view.

User-Defined Columns
You can share numeric, text, and list values with managers and let them enter or select their own values by configure
user-defined columns. For example, you want to include external stock data, such as vested and unvested shares
and the vesting date. All user-defined columns are updatable and you can default values for them using a plan cross-
reference.

The numeric columns can display any numeric value and the text columns can display any text value. List Column 46
displays the values that you define in the CMP_CWB_CUST_COL_46_LIST lookup type. List Column 47 displays the
values that you define in the CMP_CWB_CUST_COL_47_LIST lookup type, and so on, for list columns 48 -- 50. You can
override the default lookup type and use a different lookup type. To edit the default lookup types and create your own,
use the Lookups task in the Compensation work area.

You can't show totals for these columns in the summary table view because they aren't available to enable there.

Related Topics

Configure User-Defined Columns of a Workforce
Compensation Plan Worksheet to Show External Data

Here's how you configure user-defined worksheet columns to show external data in a workforce compensation plan.

1.

In the Compensation work area, click Workforce Compensation Plans.

323

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 56
Worksheets: Miscellaneous Rate Component Columns,
User-Defined Columns, and External Data in Task
Worksheets

2. On the Workforce Compensation Plans page, create the plan or search for and open an existing plan.

3. On the Define Workforce Compensation page, under Worksheets, click Configure Worksheet Display.
4. On the Configure Worksheet Display page, in the worksheet task row, click the Configure Task Layout icon.

5. On the Configure Worksheet Page Layout page, click the Detail Table tab.

6. Expand the User-Defined Columns group.

7. Enable the text, numeric, or list column, depending on what type of external data you're showing in the column.

8. Give the column a meaningful display name, such as Prior Bonus Amount or Target Information.

9. Configure the external data record type and column properties.
10. Save your changes and configure more columns or save and close the task worksheet.

Related Topics

• Record Type Lookups for External Compensation Data

324

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 57
Worksheets: Default Worksheet Display and Individual
Worker Display

57  Worksheets: Default Worksheet Display
and Individual Worker Display

Default Display Settings for Workforce Compensation
Plan Worksheets

You determine display defaults for worksheets when you configure the default worksheet display. For example, you can
set the team filter to default to Direct reports or to Direct reports if total workers exceeds 30, else show all.

Setting the team filter to an option other than All workers improves worksheet performance when managers switch
from list to tree view in the detail table.

You can also set default visible rows and row height and frozen columns. You can set the detail table to show as a list or
tree by default. And you can specify whether worksheet information, worksheet summary, and table filters are open or
closed by default.

Tip:  Managers can override these plan-level defaults by specifying their own default display settings in their
worksheets.

Related Topics

• Overview of Worksheet Display in Workforce Compensation Plans

Overview of Individual Worker Display in Workforce
Compensation Plan Worksheets

You can let managers view information about each individual in their worksheet by configuring the individual worker
display. Depending on how you configure the page, managers can also allocate compensation, promote the individual,
add notes and attachments, and view alerts.

You start by specifying whether the page shows the individual's information using up to 10 infotiles or as a single
scrolling page. You can include up to 15 sections on the scrolling page and per infotile. If you have more than 15 sections
that you want to share with managers, you need to use infotiles. Managers click each infotile to see the related sections.

You can also use infotiles to provide managers with more focused information to review and possibly change. For
example, you configure one infotile to show person information. You add a section that shows the individual's details,
such as their country, eligibility status, and email. And you add another section to show their assignment details, such
as legal employer, location, department, direct manager, and years employed. Then you configure another infotile to
show salary information. It has one section that shows summary information and another section that shows current
salary. A third section lets managers allocate salary.

325

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 57
Worksheets: Default Worksheet Display and Individual
Worker Display

After you decide how you want to present information on the individual worker page, you add sections. Then you
configure the content for each section. At any point along the way, you can save your current settings and preview what
managers would see. The data fields are blank because the preview doesn't know about any specific individual.

Individual Worker Page Content in Workforce
Compensation Plan Worksheets

You add content to the individual worker page by adding sections. The single scrolling page and each infotile can have
up to 15 sections.

Content Type

Content Source

Predefined Content

• Specific worksheet columns that are also available when you configure a task worksheet display,

 such as alerts, attachments, notes, job, performance, and salary histories.

• Oracle Transactional Business Intelligence reports. Use the Properties icon to add any OTBI

and Oracle Business Intelligence Enterprise Edition reports from the /shared/Custom/Human
Capital Management/Compensation folder.

Salary Simple Components

The same summary columns that are available when you configure a task worksheet display and all of
the simple components in the salary table. You can configure column properties, but any changes also
affect the summary columns of the task worksheets.

Not every simple component that you enable applies to every individual. Managers see only the
components configured for the individual's salary basis.

Summary

Worksheet Columns

The same summary columns that are available when you configure a task worksheet display. You
can configure column properties, but any changes also affect the summary columns of the task
worksheets.

The same worksheet columns that are available when you configure a task worksheet display. You
can configure column properties and dynamic columns, but any changes also affect the detail table
columns of the task worksheets.

Salary Rates

Rate data from the salary tables as of the HR data extraction date

You use different sections with different content types to add a mix of information about the individual to the page. For
example, you add an employment section with worksheet columns. You add job and performance history sections with
predefined content. And you add a salary summary section with summary columns.

Tip:  The predefined content renders best when you add one option per section. For example, if you want to include
alerts and attachments, add one section for alerts and another section for attachments. Don't combine them in a
single section.

326

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 57
Worksheets: Default Worksheet Display and Individual
Worker Display

Related Topics

• Overview of Worksheet Display in Workforce Compensation Plans

• Detail Table Configuration for Compensation, Detail Table Only, Performance, and Promotion Worksheets

• Overview of Dynamic Columns in Workforce Compensation Plan Worksheets

• Configure the Summary Display for Compensation Task Worksheets

• Configure the Summary Displays for Communication, Performance, and Promotion Task Worksheets

327

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 57
Worksheets: Default Worksheet Display and Individual
Worker Display

328

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 58
Worksheets: Alerts

58  Worksheets: Alerts

Overview of Alerts in Workforce Compensation Plan
Worksheets

You can use alerts to let worksheet managers know about issues that require their attention. You enable alerts to appear
in the task worksheets of workforce compensation plans using the Configure Worksheet Display task.

You enable predefined alerts and build and enable your own alerts using the Configure Alerts task. The triggering
events for the alerts that you build are the same as the events for dynamic columns. And how you build alert conditions
is the same as building dynamic column conditions. To test each alert condition that you build, use the Test alert
conditions icon on the toolbar.

Alert names are the actual alert that managers see in their worksheets. You show them additional information, such
as how to fix an issue, in the description. For example, you have an alert titled Can't allocate more than target. The
description is Adjust this individual's allocation to be less than or equal to the target.

Related Topics

• Triggering Events for Conditions of Dynamic Columns and Alerts

• Basic and Advanced Tabs When Building a Condition for a Dynamic Column or an Alert

•

Include Alerts in Task Worksheets

Predefined Alerts for Workforce Compensation Plan
Worksheets

To notify managers about issues in their worksheet that need their attention, you can enable predefined alerts using the
Configure Alerts task.

Predefined Alert

When the Alert Appears in a Worksheet

Salary changed in HR

Salary amount changed in HR

Allocation outside target range

Compensation amount for the component is less than the target minimum or greater than the target
maximum configured in the column properties

Grade changed in HR

Grade changed in HR

Worksheet manager does not match line
manager

Worksheet manager doesn't match line manager on the individual's employment record

New salary outside salary range

New salary amount is less than the salary range minimum or greater than the salary range maximum
for the individual's current grade

Worker was terminated

Individual's employment was terminated in HR

329

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 58
Worksheets: Alerts

Predefined Alert

When the Alert Appears in a Worksheet

Outside Defined Limits

Compensation minimum or maximum amount is outside of the limits set for the column

Alert Types for Workforce Compensation

When you create an alert, you select an alert type from several options.

Most are just informational but Error preventing save and Error preventing submit affect worksheet actions. For
these two alert types the best practice is to use only the Change worksheet data trigger event. If you select one or both
of the other triggering events the error prevention save or submit won’t take place.

Example Alert to Warn Managers That Their Allocated
Compensation Amounts Changed

You want to warn managers when someone else changes a component compensation amount that they entered for an
individual.

Field

Name

Type

Criteria

Value

Someone changed the compensation amount

Warning

Original Amount Updated By - Component 1 column is not equal to Compensation Amount Last
Updated By - Component 1 column

Description

Someone overrode the compensation amount that you entered.

Triggering Events

NA

Related Topics

• Triggering Events for Conditions of Dynamic Columns and Alerts

• Basic and Advanced Tabs When Building a Condition for a Dynamic Column or an Alert

Example Alert to Prevent Managers from Allocating
More Than the Targeted Compensation

Your company policy prohibits managers from allocating more compensation than is targeted for an individual.

330

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 58
Worksheets: Alerts

Field

Name

Type

Criteria

Description

Value

Allocation can't exceed the target

Error preventing submit

Note:  This type prevents managers from saving or submitting their worksheet until they resolve the
issue.

Compensation Amount - Component 1 column is greater than Compensation Target - Component 1
column

You need to adjust the compensation amount you allocated to this person because it can't exceed the
target amount.

Triggering Events

NA

Related Topics

• Triggering Events for Conditions of Dynamic Columns and Alerts

• Basic and Advanced Tabs When Building a Condition for a Dynamic Column or an Alert

Example Alert to Notify Managers When the New Base
Salary Is Greater Than the Range Maximum

Your company policy prohibits managers from allocating more compensation than is targeted for an individual.

Field

Name

Type

Criteria

Value

New base is over the range maximum

Information

New Base Salary column is greater than the Salary Range Maximum - Current column

or

New Base Salary column is greater than the Salary Range Maximum - New column

Description

The individual's new salary exceeds their salary range maximum.

Triggering Events

NA

Related Topics

• Triggering Events for Conditions of Dynamic Columns and Alerts

• Basic and Advanced Tabs When Building a Condition for a Dynamic Column or an Alert

331

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 58
Worksheets: Alerts

332

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 59
Worksheets: Assignment Segments

59  Worksheets: Assignment Segments

Overview of Assignment Segments in Workforce
Compensation Plan Worksheets

You can include prorated values for relevant component worksheet columns is a separate table in the worksheet when
you configure assignment segments.

Rather than multiple columns in the detail table, you can show the information using separate rows for each segment.
And you can let managers make changes in the relevant fields. For example, the bonus amount for this person is
calculated according to their eligible earnings and target percentage for 2 segments of time during the workforce
compensation cycle.

Start Date

End Date

Salary

Currency

Days
Eligible

Proration
Factor

Eligible
Earnings

Target %

Target
Amount

Modifier

Payout
Amount

Jan 1

Mar 14

75,000

USD

73

.2

15,000

15

2,250

1.1

2,473

(73/365)

Mar 15

Dec 31

82,500

USD

292

.8

66,000

20

13,200

1.1

14,520

(292/365)

The segment values, in this case payout amounts, are summed and shown in the table footer. When the manager clicks
Apply, the total passes to the read-only worksheet column that you specified.

Tip:  It's important that when you configure assignment segments, you start with the end in mind. Identify what data
you need to store, what you want to calculate, and what data is and isn't editable.

16,995

Basic Process to Configure Worksheet Assignment
Segments

Here's the basic process to include assignment segments in a compensation, detail table only, performance, or
promotion task worksheet. All tasks are in the Compensation work area.

1. Load your assignment segments using the External Data task.

2. Make sure that all the compensation cycles are closed for the workforce compensation plan. This way you have all

configuration options available because certain options aren't available to open cycles.

333

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 59
Worksheets: Assignment Segments

3.

Identify the compensation component you want to use for assignment segment. Also identify the amount column to
use for the assignment segments. It can be the Compensation Amount column or one of the six miscellaneous rate
columns for the component. This column is how you can feed segment totals to worksheet summary views. You can
also use the totals as default values for the selected column in the detail table of the worksheet.

4. Configure only one of the five available compensation components for assignment segments. Use the Configure

Compensation Component task. You need to configure a component that isn't mapped to salary rates and doesn't
have salary rates mapped to it.

5. Enable the Assignment Segments column in the Additional Information group of the detail worksheet table using

the Configure Worksheet Display task.

6. Enable and configure the assignment segments using the Configure Assignment Segments task. To reduce

horizontal scrolling, enable try to enable no more than 10 columns. To give managers a more robust view of the
assignment segment table, select Show detach icon.

Just like for all worksheet columns, you can set meaningful display names and change the default sequence. You can
also set properties for assignment segment columns. The specific properties you can set depend on the column.

◦ General, such as column shading, rounding rule, and decimal precision

- For one numeric segment column, you need to set Selected for Totaling to Yes.
- For each segment column you want to include in worksheet audit trails, you need to select Include in

audit trail.

◦ Visibility and access, such as line managers can only read the column data but compensation

administrators can read and edit it

◦ Default value, such as a specific number or text, or values provided by a specified formula, compensation

derived factor, or from a cross-referenced column

- For each segment column the Refresh Workforce Compensation Data process should update after

people make changes, you need to select Default value subject to refresh.

◦ Information, such as the calculation or dynamic column condition used to determine the segment column

amounts or the source of the segment column data

For many segment columns, you can also build dynamic conditions, for example, to determine the proration factor.

To let managers view changes to assignment segments in worksheet audit trails, for only one segment column,
select Audit Differentiator.

If you change Enable Assignment Segments to No, you delete all segment configurations. Changing it back to
Yes won't restore the configurations. If you leave the page before saving the change to No, you can restore any
configurations saved before you set Enable Assignment Segments to No.

Related Topics

• Detail Table Configuration for Compensation, Detail Table Only, Performance, and Promotion Worksheets

• Default Value Properties of Worksheet Columns

• Overview of Dynamic Columns in Workforce Compensation Plan Worksheets

• Configure Assignment Segments Options of a Compensation Component

• Configure the Summary Displays for Communication, Performance, and Promotion Task Worksheets

334

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 59
Worksheets: Assignment Segments

Data for Worksheet Assignment Segments

Assignment segment data can come from HR or from third-party or legacy application. To use it in worksheet columns
of a workforce compensation plan, it has to be in the external data table.

To use the external data specifically in assignment segments, each row needs to include all of this information:

• An end date

• An assignment number

• A job

When you load monetary segment amounts, you need to convert them to the same currency the individuals use, as of
the HR data extraction date.

You can use up to 50 of the available 65 user-defined assignment segment columns at a time. The user-defined
columns are 50 numeric, 15 text, and 5 date columns. Keep in mind you’re repeating data in rows instead of in columns
and most likely won't need all 50.

You can also use these columns. They're automatically available on the Configure Assignment Segments page and you
don't need to map them to user-defined columns:

• Person Name

• External Worker Data ID

• Assignment Number

• Legal Employer

• Worker Number

• Job

• Record Type

• Start Date

• End Date

• Eligibility Status

• Sequence Number

• Currency Code

The column that you use to show the assignment segment totals needs to be read-only in the worksheet.

Related Topics

• External Compensation Data

• Default Value Properties of Worksheet Columns

• Configure User-Defined Columns of a Workforce Compensation Plan Worksheet to Show External Data

• Example of Loading External Data

335

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 59
Worksheets: Assignment Segments

Visibility, Ability to Update, and Restrictions for
Worksheet Assignment Segments

Compensation administrators can see all assignment segment columns of a workforce compensation plan when they
administer workers. This includes where segment data that's loaded but not showing for the worksheet manager.

Whether managers can see assignment segments depends on the configuration. This includes whether you specify to
Show ineligible rows when you configure assignment segments. Also, managers need to have the detail table in list,
not tree, view to see the Assignment Segments table configured for the worksheet. And even if managers can see rows
with a status of Ineligible, they can't make changes to any values in those segment rows. They also have read-only
access to segment rows where the individual's assignment is processed or partially processed and if they have read-
only worksheet access.

You can specify Role-Based Overrides for assignment segment columns. Role based overrides take precedent over the
main column visibility and access settings, which determine visibility and access for all other roles.

Here's what else managers can't do when you enable assignment segments for the worksheet:

• Reorder columns, apply filters, or sort rows in the assignment segments table. The table columns appear

according to the assignment segments setup.

• Freeze columns in either the detail or the assignment segments table.

• Export the detail table content using the Export to Excel icon.

•

Include assignment segment content using Manage in Spreadsheet.

Related Topics

• Default Display Settings for Workforce Compensation Plan Worksheets

• Visibility and Access Properties of Worksheet Columns

• Detail Table Configuration for Compensation, Detail Table Only, Performance, and Promotion Worksheets

Eligibility of Worksheet Assignment Segments

You can use the configured workforce compensation plan or compensation component eligibility when you configure
eligibility for assignment segments. Both eligibility configurations use the segment end date to validate if the segment
is eligible or not.

Or you can load a value in an external data column and map it to the Eligibility Status column on the Configure
Assignment Segments page. If a row in the assignment segment table has a value in the external data column, the
segment status is Eligible. If the row is blank, the status is Ineligible.

Only the Refresh Workforce Compensation Data process or a compensation administrator using the Administer
Workers task can change segment eligibility. The manager eligibility change action doesn't affect the assignment
segment table.

336

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 59
Worksheets: Assignment Segments

Related Topics

• Workforce Compensation Plan Eligibility

• How Required and Optional Profiles Determine Compensation Eligibility

• Eligibility Profiles of Compensation Components

The Start Workforce Compensation Cycle Process and
Assignment Segments

Data has to exist in the external data table before you run the initial Start Workforce Compensation Cycle process for a
workforce compensation plan. Running the process again won't fill in any missing rows or add new external data rows.

• They meet the selected criteria.

• They have an end date between the evaluation period start date of the plan cycle and the process effective

date.

When you run the Start Workforce Compensation Cycle process, it considers only those external data rows specific to
the plan assignments. The rows need to have an end date. And the end date has to be between the evaluation period
start date and the HR data extraction date.

The process considers data in the external data table as a part of assignment segments if these conditions are true:

• The end date of the row is between the evaluation period start date and HR data extraction date. Or, the
row end date is between the evaluation period start date of the plan cycle and the person's employment
termination date. This way the process gets assignment segment rows for terminated workers.

• The date columns use the format YYYY/MM/DD.

After you run the Start Workforce Compensation Cycle process, you can change certain editable plan configuration
settings, including these:

• Record Type on the Configure Assignment Segments page

• Amount Column for Assignment Segments on the Edit Component dialog box opened from the Configure

Compensation Component page

Related Topics

• Basic Process to Configure Worksheet Assignment Segments

• Configure Assignment Segments Options of a Compensation Component

337

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 59
Worksheets: Assignment Segments

The Refresh Workforce Compensation Data Process and
Assignment Segments

To support assignment segments, you can run the Refresh Workforce Compensation Data process with one or more of
these parameters selected:

• Refresh assignment segments data: Includes updating dynamic columns for assignment segments, the

worksheet, and summary totals.

• Re-evaluate assignment segment eligibility.

• Refresh dynamic columns for assignment segments.

When you select Full Refresh, you select all assignment segment options.

Before you can refresh assignment segment data, has to exist in the external data table. Also, the Start Workforce
Compensation Cycle process has to have evaluated it.

You can't delete a segment row and use the refresh process to remove the information. You can use the refresh process
to update the worksheet after managers update data. The appropriate segment columns have to have with the Default
value subject to refresh property selected for the refresh to work.

Related Topics

• Basic Process to Configure Worksheet Assignment Segments

338

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 60
Modeling, Reports, Filters, and Plan Analytics

60  Modeling, Reports, Filters, and Plan
Analytics

Overview of Modeling in Workforce Compensation Plan
Worksheets

Let managers and administrators explore scenarios and align their budgets and compensation allocations with
organizational pay practices using worksheet models in their workforce compensation plans.

First, you enable the create, update, and apply worksheet actions when you configure worksheet display. Then you set
general options and enable model sharing, usage, and allocation methods when you configure modeling. Each method
determines the values that managers and administrators can enter in their models, and how the model calculates and
applies the results.

For example, you specify whether only administrators or both managers and administrators can access models. You
also specify whether managers can create their own models, manage models in the integrated workbook, and how they
can share models. For both managers and administrators, you enable model usages that determine how they can apply
model results. You can let them apply the results as actual compensation, budget, and target amounts, or a combination
of these options.

Numeric Properties
The general properties of numeric columns in models vary depending on where managers and administrators view
the model information. For example, model numeric columns on the Model Summary page have properties from the
summary table view of the corresponding budget or task worksheet. This includes the Overall Compensation Amount
summary component columns. Model numeric columns in the detail table have properties from the detail table of the
corresponding budget or task worksheet.

Related Topics

• General Properties of Worksheet Columns

• Actions Configuration for Communication, Compensation, Detail Table Only, Performance, and Promotion

Worksheets

• Performance Considerations for Workforce Compensation Plans

•

Include Models in Task Worksheets

• Allocation Methods in Workforce Compensation Models

Overview of Reports in Workforce Compensation Plans

Let administrators and managers view key information in their workforce compensation plans when you configure
reports.

339

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 60
Modeling, Reports, Filters, and Plan Analytics

For example, give administrators the reports they need to optimize compensation budgets and allocations across their
client groups. Give line managers reports with contextual and background information about their people so they can
make informed compensation allocations.

You can use delivered reports or add Oracle Transactional Business Intelligence (OTBI) and Oracle Business Intelligence
Enterprise Edition (OBIEE) reports. You can add any OTBI and OBIEE reports save in the shared/custom/HCM/
Compensation folder to a workforce compensation plan. And you can give the reports display names that are
meaningful to the plan audience. Removing OTBI and OBIEE reports from the Configure Reports page removes them
from only the plan. The source reports remain unaffected.

Tip:  Each workforce compensation plan can include up to 25 reports.

Related Topics

• Performance Considerations for Workforce Compensation Plans

Administrator and Line Manager Access to OTBI and
OBIEE Reports Used in Workforce Compensation Plans

To view and create Oracle Transactional Business Intelligence (OTBI) and Oracle Business Intelligence Enterprise Edition
(OBIEE) reports, people need to have the Compensation or Line Manager role. To set up workforce compensation plans,
they also need the Compensation Administrator role.

To view OTBI and OBIEE reports in their workforce compensation plans, people need the Compensation Transaction
Analysis duty role. This role is included in both the Compensation and Line Manager job roles.

Related Topics

• Overview of Reports in Workforce Compensation Plans

How You Add Dashboard OTBI Reports to the Workforce
Compensation Landing Page

Here’s how you can use Page Composer to add dashboard OTBI reports to the Workforce Compensation landing page.

1. Go to Navigator > Tools > Reports and Analytics.

2. Create your first analysis using the Workforce Compensation subject area.

3. Create your dashboard prompts.

4. Create a dashboard and add both.

5. Go to the worksheet landing page and select your plan.

6. Go to Settings and Actions > Edit Pages > Activate Sandbox > Enable Page Composer.

7. On the Add Content tab, click Add Content.

8. Go to Reports and Analytics, find your dashboard, and click Add.

340

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 60
Modeling, Reports, Filters, and Plan Analytics

9. Review your dashboard and publish your sandbox.

Related Topics

• Overview of Reports in Workforce Compensation Plans

• Overview of Landing Page Analytics in Workforce Compensation Plans

• Create a Sandbox and Make It Active

Dimensions and Range Increments in Worksheet Models
and Plan Reports

Dimensions are attributes that you use to group data in reports for workforce compensation plans. You also use them as
criteria when building worksheet models.

For example, reports can analyze compensation allocations by country and job dimensions to see how average
allocations vary. Models can automatically allocate salary adjustment amounts to people who work in specified country
and location dimensions.

You enable the dimensions that have meaning to your organization within the context of the plan when you configure
reports. Here are some examples of delivered dimensions:

• Country

• Department

• Years of service

• Performance management rating

• Location

• Job

• Position

• Grade

You can also use delivered job attributes, grade attributes, user-defined worksheet columns, and compensation
attributes, to define your own dimensions for reports and modeling criteria.

Range Increments
Instead of showing a separate data point for each person, report graphs and tables and model tables show aggregated
data for groups of people. You set compa-ratio, salary range position, years employed, and performance management
calculated rating range increments as appropriate for the plan reports and models. For example, you have a plan that
uses compa-ratio to group data in increments of 10 percentage points. The plan reports and models group together
everyone whose compa-ratio falls between 10 and 20, 20 and 30, 30 and 40, and so on.

341

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 60
Modeling, Reports, Filters, and Plan Analytics

Related Topics

• Overview of Modeling in Workforce Compensation Plan Worksheets

• Overview of Reports in Workforce Compensation Plans

•

Include Models in Task Worksheets

• Create a Workforce Compensation Model

Overview of Filters in Workforce Compensation Plan
Worksheets and Reports

Let managers sort the populations in the worksheets of their workforce compensation plans by configuring filters. For
example, you can enable Alerts, Country, Department, Location, and Job filters. The filters you can enable include 6 job
attribute, 3 grade attribute, and 15 text column filters.

You can also enable advanced filters by building relevant conditions that only compensation administrators, or both
administrators and plan managers can use. Filter conditions have only the Basic tab, while alerts and dynamic columns
also have the Advanced tab.

Related Topics

• Basic and Advanced Tabs When Building a Condition for a Dynamic Column or an Alert

• Overview of Reports in Workforce Compensation Plans

Overview of Landing Page Analytics in Workforce
Compensation Plans

You can include analytics for the entire workforce compensation plan at the bottom of the plan page. Be sure that
when you make the predefined titles more meaningful for the plan audience, the changes don't exceed 40 characters,
including spaces.

Analytic

Description

Average Allocation Amount

Workers Compensated

A meter gauge analytic available per component that shows the average allocation amount for that
component. The percentage is calculated from the total number of individuals that report to the
primary plan manager.

A meter gauge analytic available per component that shows the percentage of compensated
individuals. The percentage is calculated from the total number of individuals that report to the
primary plan manager.

Budget Usage

A bar chart showing how much budget remains for the primary plan manager. The budget amount is
based on the total budget for the manager.

342

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 60
Modeling, Reports, Filters, and Plan Analytics

Analytic

Description

Manager Submitted

Workers Promoted

A meter gauge analytic showing the number of subordinate plan managers who have submitted their
plan changes for approval. The number is the total number of subordinate managers who report to the
primary plan manager, including managers who report indirectly.

A meter gauge analytic showing the number of people promoted as a part of the compensation cycle.
The number is based on the total number of eligible individuals reporting to the primary plan manager.

Related Topics

• General Structure of Workforce Compensation Plans

343

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 60
Modeling, Reports, Filters, and Plan Analytics

344

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 61
Validation and Processing

61  Validation and Processing

Overview of Plan Validation and Starting the Workforce
Compensation Cycle

After you finish the foundation, budgets, worksheets, and models and reports configurations for the workforce
compensation plan, you validate the plan. Then you start the compensation cycle.

Validate Plan Setup
To check dependencies among the various plan configurations and make sure that all existing conditions work, use
the Validate button. Correct any errors listed on the Validation Results page and validate the plan again, repeating as
needed until you don't get any errors.

Tip:  This validation doesn't include the formulas, payroll elements, eligibility profiles, and other objects linked to the
plan.

Start Workforce Compensation Cycle
After you finish validating the plan setup, you build the task worksheets for this plan using the Start Compensation
Cycle button.

• The first time you run the Start Workforce Compensation Cycle process for the plan, you might want to make

it a trial run.

•

•

If you have issues with running the process, you may want to include trace statements in the log file.

If you're using compensation tables in Oracle Transactional Business Intelligence (OTBI), you want to start the
Synchronize Hierarchy process after the cycle process completes.

• For a thorough test, you might want to include recently terminated workers to check that the various task

worksheets show what you expect.

Related Topics

• Eligibility Profile Testing for a Workforce Compensation Plan

• Eligibility Profile Testing for a Compensation Component

• Formula Execution Errors

345

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 61
Validation and Processing

346

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 62
Global Compensation Settings

62  Global Compensation Settings

General and Watchlist Global Settings for Workforce
Compensation Plans

You can configure global settings that affect all workforce compensation plans and plan managers. You can override
various global settings when you configure workforce compensation plans.

General
You can let managers switch to a subordinate manager and move among that manager's plans. You can also validate
country budgets, set how many recently searched managers to display, and enable click-to-edit in task worksheets. And
you can include the Save and Close button on task worksheets, either as an additional option on the standard Save
button or beside it. To aid managers with worksheets for different assignments, you can enable up to two assignment
differentiators, such as Job and Location. The differentiators then show in hover text for the plan switcher as well as in
plan, budget, and worksheet headers.

Watchlist
You can show managers the number of active budget pools and plans in their watchlists. You can also show them
their newly published budgets and newly active plans. And you can set the number of days that the budget and plan
information remains in their watchlists.

Global Setting Options for Workforce Compensation Plan
Notifications

Here's a full list of the options you can select when you configure global notification settings for workforce
compensation plans. You can also select these options when you override the global settings using the Configure
Approvals and Notifications task.

The available options in both tasks depend on the setting.

Notification Option

Description

Notify

Always send notifications, such as when budgets and plans are published or withdrawn, or when
changes are approved.

Prompt manager

Send notifications for actions only if the initiating manager selects, such as when plan access changes.

Approval required

Require approval, such as for eligibility changes and worker reassignments.

Disable

Disable notifications so that none are sent, such as when individuals are delegated or removed from
delegation.

347

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 62
Global Compensation Settings

Related Topics

• Configure Notifications for Workforce Compensation Plan Worksheets

How Workforce Compensation Plan Notifications Work

Here's an explanation of how and when each notification for a workforce compensation plan is sent. The explanation
covers who initiates sending the notification, who gets it, and what the recipient can do with it.

It also covers when notifications are bypassed. You enable these notifications using the Configure Global Settings task.
You can override the settings in workforce compensation plans using the Configure Approvals and Notifications task.

Notification

Initiating Action

Initiator

Recipient

Budget Published

Manager's plan status
changes from Not
Started to Budget
Available

Manager who
published a budget to
subordinate managers

Subordinate manager
receiving a published
budget amount

Actions Available to
the Recipient

Condition
Causing Bypass of
Notification

Close

None

Worksheet Submitted Manager's plan status
changes to Submitted

Primary worksheet
manager or switched
to manager

Worksheet Returned
for Correction

Manager's approval
status for the plan
changes to Return for
Correction

Worksheet Approved
by Higher-Level
Manager

Manager's worksheet
status changes to In
Approvals

Final Approval
Obtained

Manager's plan status
changes to Fully
Approved

Higher-level manager,
specified alternate
approver, or switched
manager who returned
the subordinate
manager's plan

Higher-level manager
or specified alternate
approver who
approved plan
changes using the
submit notification,
or switched manager
who approved the
changes in their own
plan approval task.
The higher-level
manager isn't the final
approver

Top-level approver
or specified
alternate approver
who approved a
subordinate manager's
plan changes using
the submit for
approval notification

Manager one level
above the submitter in
the plan hierarchy, or
the specified alternate
approver

Approve

Reject

Submitting manager
is the highest-level
approver in the
hierarchy

Manager whose plan
was returned for
correction

Close

None

Manager whose plan
status changed to In
Approvals

Close

Manager's plan access
is No Access

Manager whose plan
is approved and all
of their subordinate
managers

Close

Manager's plan access
is No Access

348

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 62
Global Compensation Settings

Notification

Initiating Action

Initiator

Recipient

Actions Available to
the Recipient

Condition
Causing Bypass of
Notification

Plan Access Changed

Higher level manager
selects Change
Access for All
Managers or Change
Access for Selected
Managers from the
worksheet

Worksheet Withdrawn Manager clicks

Withdraw Submission

or the approval action
from the worksheet

Manager who changed
another manager's
plan access

Manager whose plan
access was changed

Close

None

Primary worksheet
manager who
previously submitted
the worksheet

Approver who received
the original worksheet
submitted notification
from a subordinate
manager

Close

None

Budget Withdrawn

Due Date Changed

Worksheet Overridden
by Higher Manager

Request for
Information

Delegate Worker

Remove Worker
Delegation

Manager clicks
Withdraw All Budgets
or Withdraw Selected
Budgets

Manager who
previously published
a budget to a
subordinate manager

Subordinate manager
for whom a budget
amount was
previously published

Close

None

Manager changes
a due date for an
individual manager or
selects Change Due
Date for All Managers

on the Action menu

Manager or
administrator changes
a compensation
amount column that
another manager
supplied, and clicks
Save

Manager selects one
or more managers
on the approval task
page, and clicks
Request Information

Manager selects one
or more individuals
on the worksheet
and selects Delegate
Workers on the
Action menu

Manager selects one
or more individuals
on the worksheet
and selects Remove
Delegations on the
Action menu

Higher-level manager
or administrator

Subordinate manager
whose worksheet due
date changed

Close

None

Manager who
modified an amount
or administrator

Manager or
administrator who
originally supplied the
amount

Close

None

Manager who
requested information

Selected managers

Reply, which opens a
dialog box to reply to
the sender

None

Primary worksheet
manager

Manager selected to
review the individuals

Primary worksheet
manager who
previously delegated
the individuals

Manager who
previously delegated
the individuals

Close

Dismiss

Approve

Reject

Dismiss

Approve

Reject

None

None

349

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 62
Global Compensation Settings

Related Topics

• Global Setting Options for Workforce Compensation Plan Notifications

• Configure Notifications for Workforce Compensation Plan Worksheets

Header and Message Text for All Workforce
Compensation Plan Notifications

Here's the header and message text for each notification for a workforce compensation plan. You can enable these
notifications using the Configure Global Settings task. The notification name identifies the manager action that sends
the notification.

You can't change the header and message text.

Notification

Header Text

Message Text

Budget Published

Compensation Budget Published for {manager
who received the budget} ({budget amount}
{currency code})

{manager who published the budget} published
a budget to you for the plan {plan name}. You
can publish budgets to lower managers or
begin allocating compensation.

Worksheet Submitted

Approval of {plan name} for {submitting
manager}

Worksheet Returned for Correction

Your {plan name} Worksheet is Returned for
Correction

Worksheet Approved by Higher Manager

Your {plan name} Worksheet is Approved

{submitting manager} submitted {plan name}
worksheet for approval. Review it and take the
appropriate approval action.

{submitting manager} returned your worksheet
for correction. Review it, make the necessary
changes, and resubmit for approval

Your worksheet was approved by {approving
manager}. It is still in the approval process until
final approval is obtained.

Final Approval Obtained

{plan name} Worksheet is Fully Approved

Your worksheet has obtained final approval.

Plan Access Changed

{plan name} Worksheet Access Was Changed

Your access to the plan and cycle was changed.

Worksheet Withdrawn

{plan name} Worksheet was Withdrawn by
{manager name}

{withdrawing manager} withdrew the {plan
name} worksheet. {withdrawing manager} will
resubmit the worksheet when it is ready for
your approval.

Budget Withdrawn

Compensation Budget Withdrawn by {manager
name}

{manager name} withdrew your budget for
{plan name}. Your worksheet will display a zero
available budget.

Due Date Changed

{plan name} Worksheet Due Date Changed

Worksheet Overridden by Higher Manager

Your {plan name} Worksheet was Modified by
{manager name}

Your due date changed. Submit your worksheet
on or before the new due date shown.

Compensation allocations for one or more
of your workers was overridden by {manager
name}. View details of the override from the
plan worksheet.

350

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 62
Global Compensation Settings

Notification

Header Text

Message Text

Request for Information

Eligibility Change

Information Request from {manager name}
Regarding {plan name}

{manager name} requested additional
information about your worksheet. Review the
comments and provide a response.

Eligibility Change Requested by {manager
name} ({worker name})

{manager name} requested to change worker
eligibility for the plan or component. Review the
request and take the appropriate action

Worker Reassignments

Worker Reassignment Requested by {manager
name} ({plan name})

{manager name} requested to reassign the
following workers to your worksheet. The
reassignment is only effective for the plan and
cycle shown and does not affect the manager
relationship in worker employment records.
Review the request and take the appropriate
action

Delegate Worker

Used to notify managers only

Remove Worker Delegation

Used to notify managers only

Workers Added to Your Compensation
Worksheet

No predefined text.

Workers Removed from Your Compensation
Worksheet

No predefined text.

Delegate Worker

Worker Delegation Requested by {0} ({1})

The following workers will be added to your
compensation worksheet.

Used when approval is required

Remove Worker Delegation

Used when approval is required

Worker Delegation Removal Requested by {0}
({1})

The following workers will be removed from
your compensation worksheet.

Related Topics

• Global Setting Options for Workforce Compensation Plan Notifications

• Configure Notifications for Workforce Compensation Plan Worksheets

How can I configure the content that appears in
the workforce compensation submit for approval
notification?

To configure worksheet summary tables, use the Configure Worksheet Display task. The setup determines the content
in the Compensation Summary, Performance Summary, and Promotions Summary sections of the notification.

To configure the Related Links and Comments sections content, use the Manage Task Configurations for Human
Capital Management task. You can't configure the Details and Summary sections content.

351

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 62
Global Compensation Settings

Related Topics

• How Workforce Compensation Plan Notifications Work

• Header and Message Text for All Workforce Compensation Plan Notifications

• How You Define Approvals for Human Capital Management

352

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 63
Workforce Compensation Administration Overview

63  Workforce Compensation Administration
Overview

Prepare to Start a Workforce Compensation Cycle

Administering workforce compensation is an iterative process. It involves preparing for the cycle, administering
individuals and workforce compensation plans during the cycle, and closing the cycle. Follow these steps to prepare for
the cycle. The tasks are in My Client Groups > Compensation unless otherwise specified.

Start Cycle Preparation

Step

Task

docs.oracle.com > Human Resources > Learn What's New in Your Update

Manager Feedback

Eligibility Profiles

Workforce Compensation Plans

Identify new features and enhancements
released since you last prepared to start
a workforce compensation cycle that you
want to include in this cycle.

Determine what configuration changes to
make to workforce compensation plans
based on feedback survey results from the
previous cycle.

Assess and update eligibility profiles
used in the eligibility configurations for
the workforce compensation plans and
compensation components.

Review existing workforce compensation
plans and create additional plans for
the upcoming compensation cycle, as
appropriate.

• Create the plan cycle. Plans

and cycles share compensation
performance ratings and promotions
according to the Performance
Rating Date and Default Promotion
Effective Date plan cycle dates.
If you aren't planning to view
and change ratings and promote
individuals during the new cycle, set
different dates in the new plan cycle
configurations.

• Validate the hierarchies and default

access levels.

• Review the corporate currency and

currency switching settings.

• Validate the plan access.

353

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 63
Workforce Compensation Administration Overview

Step

Task

• Update feedback survey and plan
information to reflect current
language and policies.

• Validate the budget pools and display

settings.

• Validate the enabled compensation
components and make sure that the
appropriate component is linked to
the plan budget pool.

• Validate the performance ratings.
Integration with Performance
Management is common across plan
cycles. This means that people use
the same rating model across plan
cycles and they see the most recent
performance management ratings in
the plan worksheets.

• Review the remaining worksheets
configurations. To view current
and revised configurations, use
the Preview option whenever it's
available.

• Validate your changes thoroughly
and resolve any errors that might
affect processing.

See how the plan and compensation
component eligibility affects the plan
worksheet populations.

View Administration Reports > Status and Monitoring > Worker Eligibility Details

Administer Individuals and Plans During a Workforce
Compensation Cycle

Administering workforce compensation is an iterative process. It involves preparing for the cycle, administering
individuals and workforce compensation plans during the cycle, and closing the cycle. Follow these steps to administer
individuals and plans during the cycle. The tasks are in My Client Groups > Compensation.

Step

Administration Report or Task

Validate the global models.

Global Models

Review various plan statuses and monitor
plan data:

Status and Monitoring:

• See how the plan and compensation
component eligibility affects the plan
worksheet populations.

• make sure that there aren't any
breaks in the hierarchies for all

• Worker Eligibility Details report

• Workers Without Managers report

• Alert Summary report

• Manager Status report

354

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 63
Workforce Compensation Administration Overview

Step

Administration Report or Task

workforce compensation plans active
during the compensation cycle.

• Review and address alerts for all

workforce compensation plans active
during the compensation cycle.

• Track the progress of submitted
changes through the approvals
process for all workforce
compensation plans active during the
compensation cycle.

Make sure that allocations fall within
compensation policies and any defined
targets for all workforce compensation
plans active during the compensation
cycle. This includes any defined target
amounts and ranges as well as pay equity
rules.

Monitor budget pools for all workforce
compensation plans active during the
compensation cycle.

Review and address and performance
rating and promotion issues for all
workforce compensation plans active
during the compensation cycle.

Refresh workforce compensation data
for all workforce compensation plans
active during the compensation cycle,
 at the determined intervals and for the
determined refresh options.

The process updates existing worksheet
data for the specified workforce
compensation plan and cycle. You
might need to run it if you let salary
changes happen outside the workforce
compensation cycle, or if the HR data had
many changes.

Determine if or when to start the cycle to
evaluate new assignments for a specific
workforce compensation plan active
during the compensation cycle.

Monitor the apply model process if you
let managers create and apply models
for workforce compensation plans
active during the compensation cycle.
Monitoring is especially important when
worksheet population sizes might be
larger than the configured batch limit.

Monitor individuals who were reprocessed
or added to a new plan manually, for any
processing issues.

Compensation Analysis reports

Budget Consumption Report

Promotions and Performance reports

Task: Run Batch Processes > Refresh Workforce Compensation Data

Supporting report: Batch Process Monitoring > Refresh Workforce Compensation Data Process

Report: Batch Process Monitoring > Start Compensation Cycle Process

Supporting task: Run Batch Processes > Start Workforce Compensation Cycle

Report: Batch Process Monitoring > Apply Model Process

Supporting task: Workforce Compensation Plans > Configure Models

Batch Process Monitoring > Reprocess or Add New Plan Data

355

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 63
Workforce Compensation Administration Overview

Close a Workforce Compensation Cycle

Administering workforce compensation is an iterative process. It involves preparing for the cycle, administering
individuals and workforce compensation plans during the cycle, and closing the cycle. Follow these steps to close the
cycle. The tasks are in My Client Groups > Compensation.

Step

Task

Confirm that all primary managers for the
workforce compensation plan submitted
their plan changes and the changes are
approved.

Release centrally managed and stored
compensation change statements to
managers and then individuals.

Reduce transfer errors for changes to
the workforce compensation plans by
refreshing workforce compensation data
before transferring changes to HR. You
should also refresh data if you let salary
changes happen outside the workforce
compensation cycle or the HR data had
many changes.

Transfer workforce compensation
data to HR. You can transfer data by
compensation type, such as elements,
 salary, stock, performance ratings, and
promotion. You can also use different HR
actions with each transfer and transfer
data for specific populations using
inclusion criteria.

Tip:  Changes that you make to
an individual's HR data using the
Administer Workers task apply to only
that assignment, plan, and cycle. They
don't transfer back to HR. To make
the changes permanent, you need
to change the data in Global Human
Resources.

Track transferred workforce compensation
data and resolve any errors. To get an
overall view of the processed assignments
and assignments remaining to process,
 you can use the Consolidated Posting
Summary report.

View Administration Reports > Status and Monitoring > Manager Status report

Run Batch Processes:

• Process Workforce Compensation Change Statements

• Refresh Workforce Compensation Data

• Transfer Workforce Compensation Data to HR

View Administration Reports > Data Processed reports

Close the workforce compensation cycle
for each plan by setting the Cycle Status
to Closed.

Active Plans

356

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 64
Workforce Compensation Batch Processes to Start a
Compensation Cycle and Refresh Data

64  Workforce Compensation Batch Processes
to Start a Compensation Cycle and Refresh
Data

Start Workforce Compensation Cycle and Synchronize
Hierarchy Processes

To build the worksheets that make up the specified workforce compensation plan for the specified cycle, you run the
Start Workforce Compensation Cycle process.

Eligibility, Including People with Employment Termination Dates
To determine which employment records to evaluate for eligibility, the start cycle process uses these plan
configurations:

• Employment records specified in the plan details

• Eligibility determination date set in the plan cycles

It then uses the eligibility criteria configured at the plan and compensation component levels to evaluate the relevant
employment records and determine eligibility. To narrow the employment records used in the eligibility evaluation, set
population filters, such as Country and Legal Employer when you start the cycle.

The process includes eligible people with an employment termination date between the evaluation period start date and
HR data extraction dates, in the cycle. And it uses the employment termination date rather than the HR data extraction
date to extract HR data. You can also include assignments terminated between plan cycle evaluation period start date
and HR data extraction date that are due to a global transfer.

During the Start Compensation Cycle process, the application fetches the Current Grade Ladder and Current Grade Step
values from Global HR as of the plan cycle's HR data extraction date.

Status
For a specific plan and cycle combination, you can set the cycle to either Administrative or Open the first time you start
the cycle. To change the cycle status after that, you need to use the Active Plans task. For example, to finalize a plan for
a new focal compensation cycle, you start the cycle with Status set to Administrative. At the time designated by your
policies, you use the Active Plans task to change the cycle status to Open.

Synchronize Hierarchy
To populate the OTBI reports included in the plan configuration, you need to run the Synchronize Hierarchy process.
You can have the start cycle process run it for you by selecting the Launch Synchronize Hierarchy process once this
process is complete option. You can also run that process manually, for example, to populate OTBI reports with the
most recent plan hierarchy data.

357

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 64
Workforce Compensation Batch Processes to Start a
Compensation Cycle and Refresh Data

Related Topics

• Workforce Compensation Plan Cycle Dates

• Employment Records to Use in the Compensation Cycle

• Workforce Compensation Plan Eligibility

• Overview of Reports in Workforce Compensation Plans

• Formula Type Is Compensation Person Selection

Plan Not in the Choice List of the Start Workforce
Compensation Cycle Process

If you can't see the plan you're looking for in the Plan choice list, verify the following:

• The Configure Plan Access task for the plan doesn't restrict access for the Compensation Administrator role.

• You have the Compensation Administrator role or the appropriate security to run the compensation batch

processes.

Refresh Workforce Compensation Data Process

To include the most recent changes to person, HR, salary, assignment segment, and terminated worker data, run the
Refresh Workforce Compensation Data process. Also run this process to re-evaluate eligibility and to refresh plan
hierarchies, due dates, currency conversion rates, dynamic columns, alerts, and summary section totals.

Refresh Date
You specify the date the process uses to refresh the data, calculations, and evaluations associated with the selected
refresh options.

• Actual Process Run Date: Use the system date at the time the process runs for all refreshes, including

eligibility.

• Plan Cycle Dates: Use the specified eligibility determination date to refresh eligibility and the specified HR data

extraction date for all other refreshes.

• Specific Date: Use the selected date for all refreshes, including eligibility.

Predefined alerts appear according to the alert type instead of the refresh date. Also, salary metrics associated with a
promotion to a new grade, such as new salary ranges and compa-ratio, use the promotion effective date. They don't use
the refresh date. The Worksheet manager does not match line manager predefined alert is retained when you run the
Refresh Workforce Compensation Data process. Make sure to use the Refresh primary manager hierarchy parameter
when the Primary Hierarchy source in plan setup is set to something other than Primary manager hierarchy.

To run a onetime refresh, you can select any of these refresh dates. For example, you want people to use recently
updated assignment segment data. You can use any refresh date to specify when to push those changes out to plan
managers and other reviewers.

358

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 64
Workforce Compensation Batch Processes to Start a
Compensation Cycle and Refresh Data

To schedule a recurring refresh, you probably want to use the Actual Process Run Date or Play Cycle Dates options.
For example, you want people to see the most current employment changes, such as terminations and transfers, and
summary totals on their worksheets. You schedule a recurring nightly refresh of HR data using the actual process run
date because this becomes the system date when the process runs. Each refresh changes by 1 day every time it runs.

When you run the Refresh Process with either the Full refresh or Refresh HR data options selected, Current Grade
Ladder and Current Grade Step values for workers part of the plan are refreshed from Global HR as of the effective date
selected during refresh process run.

Refresh Options
You can select one or more refresh options to process. For many options, when you select one option, you also select
interconnected refreshes. For example, if you select Refresh column defaults, you automatically select the options to
refresh dynamic columns, alerts, and worksheet summary section totals too.

Tip:  Typically, manual primary plan manager and worker eligibility changes revert to their original values. You can use
the Administer Workers task to identify the changes you don't want overridden.

Related Topics

• Workforce Compensation Plan Cycle Dates

• Employment Records to Use in the Compensation Cycle

• Workforce Compensation Plan Eligibility

• Reprocess an Individual or Add Them to a Workforce Compensation Plan and Cycle

• Formula Type Is Compensation Person Selection

Refresh Options for the Refresh Workforce
Compensation Data Process

Here's a comprehensive list of the refresh options you can select when you run the Refresh Workforce Compensation
Data process. Because of the interconnections between workforce compensation plan objects and worksheet columns,
often selecting one option also selects other options.

Option

Full refresh

Refresh HR data

Refresh base and eligible Salary

Description

When you select this option, you also select all other refresh options except the last few. You don't
refresh active plan data, currency conversion rates, or terminated worker data using the process date.
You do refresh everything else.

Refresh all person and HR-related data, except the primary plan manager. Refresh the summary
section totals of the plan worksheets and the predefined alerts. Also refresh all alerts and dynamic
worksheet columns with the Refresh Data triggering event selected.

Refresh base salary, salary basis, salary range columns, and any related data stored in the workforce
compensation tables. This stored data includes base salary frequency, adjusted salary, FTE salary, and
compa-ratio. Refresh default values for eligible salary and local currency if using input currency, the
summary section totals of the plan worksheets, and the predefined alerts.

359

Oracle Fusion Cloud Human Resources
Implementing Compensation

Option

Description

Chapter 64
Workforce Compensation Batch Processes to Start a
Compensation Cycle and Refresh Data

Also refresh all alerts and dynamic worksheet columns with the Refresh Data triggering event
selected.

Refresh column defaults

Refresh column defaults for the plan worksheets, the summary section totals of the plan worksheets,
 and the predefined alerts. Also refresh all alerts and dynamic worksheet columns with the Refresh
Data triggering event selected.

Recalculate eligible salary derived using a formula or dynamic column. Don't override existing column
values that aren't from HR and don't have a column default or dynamic calculation defined.

Refresh assignment segments data

Refresh the external data used to configure the assignment segments. Also refresh the dynamic
worksheet columns with Default value subject to refresh selected.

Refresh primary manager hierarchy

Refresh the primary plan manager and rebuild the corresponding hierarchy. Also refresh the summary
section totals of the plan worksheets and the predefined alerts

Refresh secondary manager hierarchy

Refresh the secondary plan manager and rebuild the corresponding hierarchy. Also refresh the
predefined alerts.

Refresh other reviewer hierarchy

Refresh the other reviewers and rebuild the corresponding hierarchy. Also refresh the predefined alerts.

Reevaluate eligibility

Re-evaluate the plan-level and component-level eligibility of everyone already included in the plan,
which if you track ineligible people, might change their eligibility status. Also refresh the summary
section totals of the plan worksheets, and all alerts and dynamic worksheet columns with the Refresh
Data triggering event selected.

If you don't track ineligible people and want to add eligible people to the plan, use the Start Workforce
Compensation Cycle process.

Reevaluate assignment segment eligibility

Re-evaluate people's eligibility for the assignment segment. Also refresh the dynamic worksheet
columns with Default value subject to refresh selected.

Reevaluate limited eligibility

Re-evaluate which plan managers have a status of Limited. Refresh the summary section totals of the
plan worksheets, the predefined alerts, and all alerts with the Refresh Data triggering event selected.
Also refresh the dynamic worksheet columns with Default value subject to refresh selected or the
Refresh Data triggering event selected.

Refresh due dates

Refreshes due dates set in the plan cycle configuration, including the hierarchy due dates.

Refresh dynamic columns for assignment
segments

Refresh the dynamic worksheet columns for assignment segments with Default value subject to
refresh selected.

Refresh dynamic columns and alerts

Refresh the summary section totals of the plan worksheets and all alerts and dynamic worksheet
columns with the Refresh Data triggering event selected.

Refresh predefined alerts

Refresh the predefined alerts.

Refresh summary totals

Refresh the period totals in the summary section of the plan worksheets. The refresh includes the total
count and eligible counts for all managers and their direct reports.

Refresh terminated worker data using
process date

Refresh active plan data

Refresh terminated people's HR data using the batch process date.

Refresh the compensation components and component post as salary option. Also refresh the
configuration data of the budget pool for the plan and period. Budget pool data includes status,
 budgeting style, submit mode, and approval mode.

Refresh currency conversion rates

Refresh the conversion rate data for the plan and period as of the refresh date.

360

Oracle Fusion Cloud Human Resources
Implementing Compensation

Option

Description

Chapter 64
Workforce Compensation Batch Processes to Start a
Compensation Cycle and Refresh Data

Lock worksheet while the process runs

Prevents people from changing their worksheets and possibly introducing data corruptions, while
their worksheets are getting refreshed. If you submit the refresh process without this option selected,
 people can make changes during the refresh.

Related Topics

• Guidelines to Configure Default Values for the Promotion Effective Date Column

• Option to Track People Ineligible for a Workforce Compensation Plan

• How the Options to Track and Hide Ineligible People Affect Plan Worksheets

• Workforce Compensation Plan Eligibility

• Eligibility Profiles of Compensation Components

Formula Type Is Compensation Person Selection

To determine the person selected for an associated workforce compensation plan, you can create formulas using the
Compensation Person Selection formula type. You select the formula when you run these batch processes:

• Start Workforce Compensation Cycle

• Refresh Workforce Compensation Data

• Transfer Workforce Compensation Data to HR

Here's a comprehensive list of the contexts available to this type of formula:

• DATE_EARNED

• EFFECTIVE_DATE

• END_DATE

• START_DATE

• HR_ASSIGNMENT_ID

• HR_TERM_ID

• JOB_ID

• LEGISLATIVE_DATA_GROUP_ID

• COMPENSATION_RECORD_TYPE

• ORGANIZATION_ID

• PAYROLL_ASSIGNMENT_ID

• PAYROLL_RELATIONSHIP_ID

• PAYROLL_TERM_ID

• PERSON_ID

The database items available for this type of formula are related to Person, Assignment, Salary, Element Entries,
Compensation Record, and From and End Dates.

These are the input variables available to this type of formula:

361

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 64
Workforce Compensation Batch Processes to Start a
Compensation Cycle and Refresh Data

Input Value

Data Type

Required

Description

CMP_IV_PLAN_ID

CMP_IV_PERIOD_ID

CMP_IV_PLAN_START_DATE

CMP_IV_PLAN_END_DATE

CMP_IV_PLAN_ELIG_DATE

CMP_IV_PERFORMANCE_EFF_
DATE

Number

Number

Date

Date

Date

Date

CMP_IV_PROMOTION_EFF_DATE

Date

CMP_IV_XCHG_RATE_DATE

Date

CMP_IV_ASSIGNMENT_ID

Number

CMP_IV_PERSON_ID

Number

Y

Y

Y

Y

Y

Y

Y

Y

Y

Y

Plan ID

Period ID

Plan Start Date

Plan End Date

Plan Eligibility Date

Performance Effective Date

Promotion Effective Date

Currency Conversion Date

Assignment ID

Worker ID

These are the return variables available to this type of formula:

Return Value

Data Type

Required

Description

L_SELECTED

Char

N

Y or N

This sample formula determines if a person is selected for a workforce compensation plan based on their
assignment_id.

/******************************************************************
FORMULA NAME : Compensation Selection Formula
FORMULA TYPE : Compensation Person Selection
DESCRIPTION: Assignment_id based selection fast formula
*******************************************************************/

/*=========== INPUT VALUES DEFAULTS BEGIN =====================*/
INPUTS ARE CMP_IV_ASSIGNMENT_ID (number), CMP_IV_PLAN_ID (number)
/*=========== INPUT VALUES DEFAULTS ENDS======================*/

/*================ FORMULA SECTION BEGIN =======================*/
DEFAULT FOR CMP_IV_ASSIGNMENT_ID IS 0
l_selected = 'Y'
/* 100000008154095 - Ariel.Aimar@oracle.com - GBI data*/
if (CMP_IV_ASSIGNMENT_ID = 100000008154095) THEN
(
l_selected = 'N'
)
else
(
l_selected = 'Y'
)
RETURN l_selected
/*================ FORMULA SECTION END =======================*/

362

Oracle Fusion Cloud Human Resources
Implementing Compensation

Related Topics

• Formula Compilation Errors

• Formula Execution Errors

• When do I run the Compile Formula process?

• Example of Writing a Fast Formula Using Formula Text

Chapter 64
Workforce Compensation Batch Processes to Start a
Compensation Cycle and Refresh Data

363

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 64
Workforce Compensation Batch Processes to Start a
Compensation Cycle and Refresh Data

364

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 65
Workforce Compensation Batch Process to Transfer
Workforce Compensation Data

65  Workforce Compensation Batch Process to
Transfer Workforce Compensation Data

Transfer Workforce Compensation Data to HR Process

To post base pay adjustments to salary records and element entries to payroll, use the Transfer Workforce
Compensation Data to HR process. Also use this process to post stock grants to stock history and job, grade, and
position changes to the assignment records specified in the plan. Depending on the plan worksheet configurations,
some of the transfer details pages might not have any data to transfer.

• To transfer all data, select and configure all relevant element, salary, stock, and promotion details.

• To transfer specific data, configure those details and unselect the details on all other pages except Other

Details. For example, to transfer just stock grants, configure the stock details and unselect all element, salary,
and promotion details.

You need to post the same types of details for a person, in the same transfer process. For example, post all of Lynn's
element details in a single transfer. You can't post some of their element details with one transfer process and the post
more element details with a later transfer process. You can post all of their element details with one transfer process and
then post all of their stock details with a later transfer process.

When you run the Transfer Workforce Compensation Data to HR process the process transfers the Proposed Grade Step
attribute along with existing Job, Grade, Position, and Assignment Name Change attributes of a person's assignment.
The Transfer process skips salary transfers for those workers who are on a Grade Ladder of Type Grade and Steps
and the Grade Ladder has Include salary updates checked. The Transfer process log shows the reason an update was
skipped. After a Proposed Grade Step is transferred to an assignment from a plan cycle, the Rate Synchronization
process needs to run separately to update the new salary on the assignment because the Transfer process doesn't
update the salaries.

View Statistics
You can better understand the raw data related to the plan, cycle, and action you're transferring data for by expanding
the View Statistics section. You can see the total, eligible, processed, partially processed, and unprocessed assignments
included in the transfer process configuration. You can also see how many assignments are marked to not process and
processed assignments for salary, stock, promotion, and elements column.

People Whose Employment Was Terminated
To post single compensation payments and salary adjustments for people whose employment was terminated, run
the Transfer Workforce Compensation Data to HR process when the compensation cycle is over. Make sure that the
plan cycle is still open though. The effective date of the compensation allocations must be before or on the person's
employment termination date. The transfer process fails to post any payments and adjustments with an effective date
after the person's payroll last standard process date.

365

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 65
Workforce Compensation Batch Process to Transfer
Workforce Compensation Data

Element and Salary Details of Transfer Workforce
Compensation Data to HR Process

The salary and element mapping property configurations of the compensation amount columns determine where the
Transfer Workforce Compensation Data to HR process posts the data. The configurations also determine the step
where you configure the transfer details.

If Post as Salary is No, the changes post to the element entry of the specified payroll element. You include or exclude
this data in the transfer using the Element Details page. If none of the compensation amount columns in the plan have
this property configuration, then the Element Details page of the transfer process is blank.

If Post as Salary is Yes, the changes update people's salary records. If the column also has a salary component
specified, such as Merit or Cost of Living, the salary changes include that component for future reference. If none of
the compensation amount columns in the plan have this property configuration, then the Salary Details page of the
transfer process is blank.

Given that plans can have up to five compensation amount columns, the transfer might have all amounts post to either
elements or salary records. Or the transfer might have some amounts post to elements and others to salary records.

Related Topics

• Salary and Element Mapping Properties of Compensation Amount Columns

• Other Details of Transfer Workforce Compensation Data to HR Process

• Transfer Workforce Compensation Data to HR Process

Stock Details of Transfer Workforce Compensation Data
to HR Process

To post stock granted in workforce compensation plans to people's stock history, configure the stock details of the
Transfer Workforce Compensation Data to HR process. People can see their stock history in the Shares section of
their Compensation page. Depending on change statement configurations for the plan, they might also be able to see
the history in their workforce compensation change statement.

You don't have to set up payroll elements to post stock grants.

Related Topics

• Transfer Workforce Compensation Data to HR Process

• Other Details of Transfer Workforce Compensation Data to HR Process

366

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 65
Workforce Compensation Batch Process to Transfer
Workforce Compensation Data

Promotion Details of Transfer Workforce Compensation
Data to HR Process

To post changes to people's jobs, grades, and positions, you configure the promotion details of the Transfer Workforce
Compensation Data to HR process. If the promotion includes compensation changes, you configure that part of the
data transfer on either the Element Details or Salary Details page, or both.

To mark people's compensation changes as part of a promotion, post promotion data in a separate transfer process
with the Promotion action reason. You still configure any related element and salary details separately from the
promotion details.

Related Topics

• Element and Salary Details of Transfer Workforce Compensation Data to HR Process

• Salary and Element Mapping Properties of Compensation Amount Columns

• Other Details of Transfer Workforce Compensation Data to HR Process

• Transfer Workforce Compensation Data to HR Process

Other Details of Transfer Workforce Compensation Data
to HR Process

To filter the people whose data you want to transfer to HR, configure the other details of the Transfer Workforce
Compensation Data to HR process. For example, you can specify to include only the subordinates of specific managers
and build a condition that identifies inclusion criteria to apply. You can also use a person selection formula and include
people who's changes were approved to a specific level.

Tip:  The statistics you can view contain only the people included using the manager hierarchy and worker inclusion
criteria. The statistics don't contain people included using the person selection formula or people with changes
approved to the specified level.

Workers Approved at Least N Levels Up
To include people's changes in the transfer process, the changes need to be part of Approved plans in the specified
levels. For example, if you select 1, the transfer process includes the approved plan changes from the lowest level of the
plan hierarchy.

If you select 3, the transfer process includes the approved plan changes from the three lowest levels of the plan
hierarchy. If plan changes for the third level up are In Approvals, the transfer process includes only the approved
changes for the first two levels. It excludes the changes for the third level because they're pending approval.

367

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 65
Workforce Compensation Batch Process to Transfer
Workforce Compensation Data

Mark Assignments as Processed
Every time you run the transfer process, you need to specify whether to mark assignments as processed.

• No: When the process successfully posts the assignments, it process marks them as partially processed. This

option lets a future transfer process post changes for other unprocessed details. For example, you transfer only
stock details in a process that doesn't mark assignment as processed. Later, for the same people, you transfer
salary and promotion details.

• Yes: When the process successfully posts the assignments, it marks them as fully processed. To process any
further changes, you need to run the Back Out Workforce Compensation Data process, for the appropriate
transfer process ID. You can find that process ID in various reports available using the View Administration
Reports.

Related Topics

• Basic and Advanced Tabs When Building a Condition for a Dynamic Column or an Alert

• Configure Approvals for Workforce Compensation Plan Worksheets

• Alternate Approver Table in Worksheet Approval Configuration

• Transfer Workforce Compensation Data to HR Process

• Formula Type Is Compensation Person Selection

368

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 66
Workforce Compensation Batch Processes to Back Out
and Purge Data, Notify Managers, and Process Change
Statement

66  Workforce Compensation Batch Processes
to Back Out and Purge Data, Notify Managers,
and Process Change Statement

Back Out and Purge Workforce Compensation Data
Processes

To reverse the transfer of data from the workforce compensation plan to HR, you run the Back Out Workforce
Compensation Data process. For example, you run the process to remove transferred element and salary data so that
you can transfer newer changes for processing. When you run the process, you can do a full back out to reverse all of
data transfers for the specified plan and cycle. You also do a full back out to reverse all plan hierarchy synchronizations.
Or you can reverse the data transferred by a specific process. Various administrative reports that you access using the
View Administrative Reports task include process IDs for just this purpose. To honor the work that plan managers put
into creating models, you can specify that the back out process preserve any plan models.

To remove unneeded data from previous cycles for the specified plan, you run the Purge Workforce Compensation
Data process. You can select a specific plan and cycle. Or you can provide an HR data extraction date range. The
process purges the data from all plans with HR data extraction dates on or during the process start and end dates. After
you set the range, the process tells you how many cycles it will purge.

The Back Out Workforce Compensation Cycle process reverts any Grade Step changes that are done as a part of
Transfer Workforce Compensation Data to HR process.

Related Topics

• Transfer Workforce Compensation Data to HR Process

Notify Managers About Workforce Compensation Plan
Due Dates and Cycle Status Change Processes

To remind primary plan managers of upcoming due dates, you run the Notify Managers of Approaching Due Dates
process. You can notify them that due dates are approaching in 15, 10, 5, 4, 3, and 2 days as well as tomorrow and today.
You can also notify them that a due date is past. When you configure the notification process, you select a specific due
date or multiple due dates, as appropriate to your policies.

To let primary plan managers know that the plan cycle is open or closed, run the Notify Managers That Cycle Is Open
or Closed process. When you configure the process, you can optionally specify when to communicate plan changes to
affected individuals. You can also refine the people affected by the cycle status change using population filters, such as
to meet country-specific regulatory requirements. For example, you configure an instance of the process to notify only
managers in France that the plan cycle is closed for people in France. And you configure another instance of the process
to notify only managers in Germany that the plan cycle is closed for people in Germany.

369

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 66
Workforce Compensation Batch Processes to Back Out
and Purge Data, Notify Managers, and Process Change
Statement

Related Topics

• Workforce Compensation Plan Cycle Dates

• Overview of Plan Validation and Starting the Workforce Compensation Cycle

• Start Workforce Compensation Cycle and Synchronize Hierarchy Processes

Process Workforce Compensation Change Statements
Process

To generate and store the compensation change statements configured for central management, you run the Process
Workforce Compensation Change Statements process.

For the specified combination of workforce compensation plan and cycle, you specify the mode of the process, such as
Delete, Update Expiration, or Replace. You need to specify visibility, such as only administrators; administrators and
managers; or administrators, managers, and workers for the Update Visibility, Replace, and New modes. And for all
modes, you need to specify the change statement template the process uses when it runs.

You can also refine the people to generate the compensation change statements for using population filters, such as
to meet country-specific regulatory requirements. For example, you configure an instance of the process to generate
statements for only people in France. And you configure another instance of the process to generate statements for
only people in Germany.

Related Topics

• Overview of Compensation Change Statements in Workforce Compensation Plan Worksheets

• Statement Generation Timing and Output Format for Compensation Change Statements

• Delivery Options for Compensation Change Statements

People Can't See Their Workforce Compensation Change
Statements

To let people see their workforce compensation change statements, review and change these settings, as appropriate:

• Enable worker statements using the Configure Global Settings task.

• Make the expiration date of the Process Workforce Compensation Change Statements process after the

process date. Also set Visibility to Administrators, managers and workers.

370

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 67
View Compensation Administration Reports

67  View Compensation Administration
Reports

Compensation and Budget Analysis Reports for
Workforce Compensation

Here’s a list of reports that analyze compensation and budgets.

Compensation and Budget Analysis Reports

Report

How to Use

Compensation Allocations

Review allocations by component. The summary shows allocations by Legal Employer. The details are
by person.

Allocations Deviating From Target

Review allocations compared to targets, and percentage deviations from targets. Validate that
allocations line up with set targets. Percentage deviation refers to the difference between the
Percentage of Eligible Salary and the Target Compensation Percentage, expressed as a percentage of
eligible salary.

Allocations Compared to Target Ranges

See amount and percentage of eligible salary allocated, and where awards fall within target ranges.
Validate that allocations are within set compensation target ranges.

Budget Consumption

See manager allocations compared to published budgets. Review how managers use their budgets. If
you use worker-level budgets, you can see the breakout by country by manager.

You can view worker-level budget amounts by country in the Budget Consumption report in View
Administration Reports. Click the icon in the Budget Usage by County column to see a window with
the amounts listed by country. When you use manager-level budgets, only compensation amounts are
listed by country.

Related Topics

• Cycle Overview Reports for Workforce Compensation Managers

• Salary Analysis Reports for Workforce Compensation Managers

• Target Analysis Reports for Workforce Compensation Managers

• Distribution Analysis: Allocations by Manager Report for Workforce Compensation Managers

Promotions and Performance Reports for Workforce
Compensation

Here’s a list of reports that summarize performance info.

371

Oracle Fusion Cloud Human Resources
Implementing Compensation

Promotions and Performance Reports

Reports

How to Use

Chapter 67
View Compensation Administration Reports

Promotion Summary

See all job, grade, and position changes made during a compensation cycle. Review all promotions.
The summary shows changes by grade, job or position.

Performance Rating Summary

See deviations from profile rating model targets for each performance rating. Review performance
ratings against the rating profile distribution in the summary.

Review all ratings for all workers in the details. Use the "No Rating" option to find workers without a
rating.

Related Topics

• Pay for Performance Reports for Workforce Compensation Managers

Status and Monitoring Reports for Workforce
Compensation

Here’s a list of reports that show various compensation statuses.

Report

How to Use

Manager Status

Alert Summary

Manager Feedback

See where managers are in the compensation plan’s cycle. Identify which managers haven’t started
their work.

View all alerts triggered for all workers in this compensation cycle. The summary shows the breakout of
alerts by type. The details allow you to refine the list of people by alert type.

Review the feedback that managers gave after they submitted their plan changes for a given plan
cycle. The report is separated by rating summary, rating details, and then the responses to any
configured questions.

Workers Without Managers

Review workers without a worksheet manager that create a gap in the reporting hierarchy. Validate that
there’re no gaps in the primary hierarchy.

Worker Eligibility Details

Review plan and component level eligibility details of the workers in a compensation cycle. Review how
eligibility configuration has affected the plan population. The summary shows 2 graphs: plan eligibility
and component eligibility. You can switch between components to review any other configured
component level eligibility impacts.

The details lets you refine the list of ineligible people by plan or component ineligibility reason. You can
also see which eligibility profile and criteria caused a person to be found ineligible for the component
or plan.

Worker Statement Actions

Review the actions taken by people on their stored compensation change statements. If no one has
taken an action, you’re notified of the same and the report does not run.

You can view the status of the actions taken by workers on their compensation change statements in
employee self-service. To use the report, you must configure the workforce compensation plan to use
the centrally managed and stored option for statements and run the Process Workforce Compensation
Statements process.

372

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 67
View Compensation Administration Reports

Data Processed Reports for Workforce Compensation

Here’s a list of reports that show processing info.

Data Processed Reports

Report

How to Use

Salary Adjustments Posted

See processing details and total salaries adjusted. Review posted salary adjustments. The summary
shows the adjustments by Legal Employer and Salary Basis. The details shows them by person.

The report generates a batch process ID. You can back out by the ID if there are problems.

You can view amounts in the Salary Adjustments Posted report in the same decimal precision as in the
worksheet.

Element Entries Posted

Review total allocations posted element entries. The summary shows the adjustments by Legal
Employer and payroll element. The details shows them by person.

The report generates a batch process ID. You can back out by the ID if there are problems.

Assignment Changes Posted

See job, grade and position changes transferred to core HR by assignment. Review posted assignment
changes. The summary shows info by Legal Employer and number of changes. The details shows the
changes by person.

The report generates a batch process ID. You can back out by the ID if there are problems.

Stock Grants Posted

Review stock grants posted to the Stock table. The summary shows stock posted by Legal Employer
and Grant Type. The details shows info by person.

The report generates a batch process ID. You can back out by the ID if there are problems.

Posting Error Summary

See cycle close errors that may require manual processing. Review posting errors by batch process ID.
The summary shows overall errors by type and the number. The details shows which people had the
error.

Consolidated Posting Summary

See an overall view of all posted data. The summary graph shows the number of assignments, number
of eligible assignments, how many are fully process or partially processed, how many are pending
processing and how many assignments were marked to not process. The details shows what was
posted for each batch process ID.

Back Out Cycle Error Summary

See all errors that occurred when backing out data that were transferred to HR. The report is separated
by batch process ID.

Consolidated Posting Summary Report Data

This report in the Compensation work area, Administrative Reports task lets you see an overall view of all posted data.

Within the report, you are able to see the following for each batch run:

• Process ID

• Run Mode

373

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 67
View Compensation Administration Reports

• Run Start Time

• Who submitted the batch process

•

If unhidden, you can see if assignments were marked as "Processed"

For each allocation type (element, promotion, salary, stock) within the batches the following is available:

• How many were posted

• How many failed

• How many were backed out

• How many had no action taken

This report displays only overall data processed and if assignments are still marked to allow for more processing. You
need to review the Posting Error Summary report to find out why data transfers fail.

Exports for Workforce Compensation

Here’s a list of reports you can use to export info by parameters you select.

Report

How You Use

Worksheet Export

See worksheet details exported to a workbook. Export worksheet data using the following parameters:
Name, Country, Legal Employer, Business Unit, Department, and Manager Hierarchy.

Generate Real Time Statements

Audit Export

Generate statements for a selected manager hierarchy. After you select a manager hierarchy, you
can further refine the population by country. Generate statements all at once for a selected template.
This export doesn’t take into account any statement criteria in plan setup. It uses criteria within the
template.

Generated files are only available for the time shown on the page. The system currently sets the
availability to 7 days.

Use the following parameters to view and export audit trail data to a workbook from a plan cycle:
Person Name, Column Updated, Updated By, Component, Last Update Date, Department, Business
Unit, Legal Employer, Country, and Manager Hierarchy. The Advanced option lets you search by Update
Date Range instead of Last Update Date.

You must enable the "Include in audit trail" column property before you run the Start process. This is
the same as with the Audit report on the worksheet.

Batch Process Monitoring for Workforce Compensation

Here’s a list of reports you can use to moni9tor workforce compensation processing.

Report

How to Use

Start Compensation Cycle Process

See history of Start Workforce Compensation Cycle batch process submissions. Use this report to see
these details:

374

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 67
View Compensation Administration Reports

Report

How to Use

• Efficiency of the start process ran based on plan setup details and selected parameters.

• Number of workers processed and the time taken.

• Number of fast formulas used in plan setup and access additional info.

If you enable the start compensation cycle trigger during setup, you can also see how many
dynamic calculations are configured.

Refresh Workforce Compensation Data
Process

See history of Refresh Workforce Compensation Data batch process submissions. Use this report to see
these details:

• Efficiency of the refresh process ran based on plan setup details and selected parameters.

• Number of workers processed and the time taken.

• Number of fast formulas used in plan setup and access additional info.

If you enable the refresh data trigger during setup, you can also see how many dynamic calculations
are configured.

Reprocess or Add New Plan Data

See history of Reprocess or Add New Plan batch process submissions. Administrators can see details
from the Reprocess or Add New Plan Data process. It shows info about the submission itself and if any
errors occurred.

Apply Model Process

See history about the Apply Model Process including any submissions done by worksheet managers.
Administrators use this report when people have difficulty applying a model through the batch
process.

Discrimination Detection Report

You can analyze classes of people who are protected from pay discrimination using the Discrimination Detection report.
For example, you can compare compensation for men and women who work in the US.

The report calculates the averages and medians using standard statistical methods.

Summary
You can view calculated values for the entire plan cycle in the Cycle Summary section. By default, the report shows
everyone for the entire cycle. But, you can limit the people you're comparing using criteria in the Define Comparison
Group section.

You can refine the report in the Protected Class Analysis section to show only people in the comparison group who
belong to protected classes, such as gender and age. Most of the values in the table are self-evident. But, the Amount
Difference, under the Variance from Group Average header, is calculated as follows: Class Average Amount - Group
Average Amount.

The class amount is in the table, under the Compensation for this Group header. The group amount is in the Cycle
Summary section.

Details
Here's the source of some of the data in the table on the Details tab.

375

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 67
View Compensation Administration Reports

Field

Data Source

Discrimination Reporting Code

HR tables

Group Median Amount

Same value as the field in the Cycle Summary section of the Summary tab. It's the same for everyone.
You can use it as a reference to compare with the person's Compensation Amount.

Difference from Group

A result of this calculation: Compensation Amount - Group Median Amount.

376

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 68
Active Workforce Compensation Plans and Manual
Currency Conversion Rates

68  Active Workforce Compensation Plans and
Manual Currency Conversion Rates

Active Workforce Compensation Plans

To see the active workforce compensation plans and the status of their plan cycles, use the Active Plans task in the
Compensation work area. You can also use this task to make these changes for a specific plan cycle:

• Cycle status

• Approval, submit, and withdraw modes

• Plan, component, and budget pool display order

• Currency conversion rates

The changes you make with this task don't apply to the source plan configuration.

Currency Conversion Rates
Plan worksheets can show converted currency amounts and the currency conversion rates. They also use the rates to
calculate the amounts in the Budget Amount - Worker column. And the Transfer Workforce Compensation Data to
HR process posts amounts in each person's local currency. Thus, the plan cycle has to include currency conversion rates.
If you don't populate the rates using the Manage Daily Rates task, you can manually add them on the plan cycle Active
Plans page.

When you first run the Start Workforce Compensation Cycle process for the plan cycle, the process populates the
appropriate workforce compensation table. It loads the daily rates in effect at that date and time. Here's how you can
update the table and plan cycle worksheets with the most recent daily rates:

1. On the Active Plan page, Currency Conversion Rates tab, click the Refresh button. To update the table with

manually added and changed currency conversion rates, save the changes you made on the tab.

2. Run the Refresh Workforce Compensation Data process with the Refresh summary totals option selected to

update the plan cycle worksheets with the most recent rates.

Related Topics

• Add and Change Currency Conversion Rates for a Workforce Compensation Plan Cycle

• Guidelines for Creating Conversion Rate Types

• Overview of GL Currency Rates Upload

Add and Change Currency Conversion Rates for a
Workforce Compensation Plan Cycle

All compensation areas, such as salary, individual and workforce compensation, and total compensation, convert values
using general ledger daily rates. More specifically, the selected plan cycle uses these daily rates to convert the plan

377

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 68
Active Workforce Compensation Plans and Manual
Currency Conversion Rates
currency to people's local currencies in the enabled worksheets. Here's how you can manually manage specific currency
conversion rates for the plan cycle, as needed:

1. On the plan cycle Active Plans page, Currency Conversion Rates tab, add a row. To change an existing rate, skip to

step 3.

2. Select the To Currency code, such as CAD - Canadian Dollar.

3. Enter the conversion rate, such as 1.00695.

4. Repeat steps 1 through 3 to add other currencies. Repeat step 3 to change other conversion rates.

5. When you finish, save your changes.

6. Refresh the summary data in the plan cycle worksheets with these changes.

a. On the Run Batch Processes page, in the Refresh Workforce Compensation Data row, click the Run icon.
b. Select the appropriate plan, cycle, and refresh date.
c. Optionally select a person selection formula.
d. Select the Refresh summary totals option.

378

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 69
Administer Workforce Compensation for Workers

69  Administer Workforce Compensation for
Workers

Administer Individuals During Workforce Compensation
Cycles

To reprocess the data used in workforce compensation for a specific person or add them to a new plan, you use the
Administer Workers task. The changes that you can make depend on the person's HR data, plan configuration, and
whether the person is a manager. Here's what else you can do with the task:

All of the information that you see and the changes you make apply only to the selected person, assignment, workforce
compensation plan, and plan cycle. They don't apply for anyone else. They also don't apply for the same person in these
situations:

• Review the person's information, such as employment details and any employment terminations.

• Review and change details about the person's budget, compensation, promotion, performance, hierarchies and

statuses, and eligibility. You can also review and change user-defined data, notes, alerts, and audit history.

• Review any generated statements or stored statements, and add stored statements.

Tip:  To keep any changes you make for the specific person, assignment, plan, and cycle, you can select the Exclude
worker from the refresh process option. This option is above the Person Information section of the Administer
Workers page with the various tabs, starting with Worker Information and Budget. The refresh processes preserve any
changes until you unselect the option.

Related Topics

• Refresh Workforce Compensation Data Process

Reprocess an Individual or Add Them to a Workforce
Compensation Plan and Cycle

You can reprocess the data for a specific person, assignment, and effective date used in a specific workforce
compensation plan and cycle. For example, someone transferred into or out of your organization after the workforce
compensation cycle starts. Now, you want to re-evaluate their eligibility for a specific plan and cycle with an effective
date that's the day the transfer was complete.

1. Use the Administer Workers task to search for the person and get a list of their assignments.

2.

In the row with the appropriate assignment, click the person's name.

3. On the Administer Workers: Select Plan page, use the Reprocess or Add New Plan button to complete any of these

tasks:

◦ Re-evaluate the person's eligibility for a plan and cycle they're already participating in.

379

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 69
Administer Workforce Compensation for Workers

◦ Evaluate their eligibility for a plan they're already participating in, but a cycle they aren't.
◦ Evaluate their eligibility for a plan and cycle they aren't participating in.

Related Topics

• Refresh Workforce Compensation Data Process

Administer an Individual's Hierarchies and Access for a
Workforce Compensation Plan Cycle

Manager and reviewer responsibilities during a workforce compensation cycle depend on the plan hierarchy and access
settings.

• Primary managers finalize and approve workforce compensation plan changes submitted by their subordinate

managers. They also finalize their own changes and then submit all of these changes to their approver.

• Secondary managers and other reviewers view plans delegated by the primary manager. Depending on the

setup, they can suggest changes to the primary manager. The delegated individuals they review might appear
in a different reporting structure than they do in the primary hierarchy.

Sometimes you might need to change the manager or reviewer. For example, the current primary manager is the
new line manager for the person as the result of a recent internal transfer. You want the primary manager for this
assignment, plan, and cycle to be their previous line manager because that manager knows this person better. Any
hierarchy changes don't change the line manager for the assignment.

As needed, you can override the access levels configured for these hierarchies. For example, you want to remove all
access for the primary manager. And you do want to give the secondary manager access and let them make changes.

You can change the plan hierarchies and access on the Administer Workers page, Status and Hierarchy tab. The changes
apply only for the selected person, assignment, workforce compensation plan, and plan cycle.

Tip:  To keep any changes you make for the specific person, assignment, plan, and cycle, you can select the Exclude
worker from the refresh process option. This option is above the Person Information section of the Administer
Workers page with the various tabs, starting with Worker Information and Budget. Future reprocess and refresh
processes preserve any changes until you unselect the option. You can also use the Don’t refresh option for each
relevant hierarchy to let future reprocess and refresh processes update other changes you made.

Related Topics

• Workforce Compensation Plan Hierarchies

• Options to Configure Workforce Compensation Plan Hierarchies

380

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 69
Administer Workforce Compensation for Workers

Administer an Individual's Manager and Processing
Statuses, and Due Date for a Workforce Compensation
Plan Cycle

When you administer an individual, you can administer them and an assignment as being part of a primary manager's
plan worksheets for the cycle. You might also administer them in such a way for a secondary manager or other reviewer.
And for those individuals who are also a primary manager for the workforce compensation plan and cycle, you can
administer their plan and approval statuses.

To change the status for their plan, you use the Manager Status field. To see what work the individual has finished so
far in their role as primary manager, you can review their action history. You can also change the due date by when they
need to submit their plan changes for approval.

Again administering the individual as part of a primary manager's plan worksheets, you can also review and change
their processing status. The status indicates how much of the plan changes to the individual's workforce compensation
data were transferred to HR.

To review the current statuses and due date, and make any necessary changes, use the Administer Workers page, Status
and Hierarchy tab.

Administer an Individual's Eligibility for a Specific
Workforce Compensation Plan Cycle

When the Start Workforce Compensation Cycle process runs, it determines people's eligibility status for the workforce
compensation plan and enabled compensation components. Depending on the refresh and population options you
select, the Refresh Workforce Compensation Data process re-evaluates their eligibility status. It's also re-evaluated for
an individual when you Reprocess or Add New Plan for them.

You can manually override the eligibility status for a specific person, assignment, plan, and cycle using the Administer
Workers task. On the Eligibility tab of the Administer Workers page, you can set the eligibility status for the plan or for
specific components. You can also specify that future reprocess and refresh processes can't update your changes.

When administrators run the Reprocess or Add New Plan process, the application fetches the Current Grade Ladder
and Current Grade Step values from Global HR as of effective date selected during the process run. When you run the
Refresh Data process for any person, the Current Grade Ladder and Current Grade Step values are also refreshed.

Related Topics

• Workforce Compensation Plan Eligibility

• How Required and Optional Profiles Determine Compensation Eligibility

• Option to Track People Ineligible for a Workforce Compensation Plan

• How the Options to Track and Hide Ineligible People Affect Plan Worksheets

• Eligibility Profiles of Compensation Components

381

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 69
Administer Workforce Compensation for Workers

Adjust Manager-Level Budgets Stored as Percentages

You might need to adjust a manager level budget stored as a percentage after you’ve started the compensation cycle.

The best way to do this is to use a model to redistribute the desired percentage. First, on the Allocate Budgets page, use
Adjust Budgets to reduce the budget level of the top-level manager to the new percentage level. Then, create a model
that reduces the remaining managers’ amounts. Finally, run the Refresh process to sync the Summary Totals. Review
the results to make sure they are as desired.

382

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 70
Examples of When to Reprocess an Individual after Starting
a Workforce Compensation Plan Cycle

70  Examples of When to Reprocess an
Individual after Starting a Workforce
Compensation Plan Cycle

Someone Transfers into an Organization After the
Workforce Compensation Cycle Starts

Maria transfers into your organization after the workforce compensation cycle starts and may be eligible for
compensation changes.

You use the Administer Workers task to find the appropriate assignment. And you use the Reprocess or Add New
Plan button to evaluate her eligibility for the specified plan and cycle. If the process finds Maria eligible, it adds her to
the appropriate primary plan managers' worksheets.

Someone's Data Is Corrected in HR After the Workforce
Compensation Cycle Starts

Michael was ineligible for a workforce compensation plan and cycle because of incorrect employment data.

After HR corrects the data, you use the Administer Workers task to find the appropriate assignment. And you use the
Reprocess or Add New Plan button to re-evaluate his eligibility for the specified plan and cycle. If the process finds
Michael eligible based on the corrected data, it adds him to the appropriate primary plan managers' worksheets.

Someone Leaves an Organization After the Workforce
Compensation Cycle Starts

Janice is eligible for a workforce compensation plan when the cycle starts. A week later, she leaves your organization
making her no longer eligible for compensation changes in that plan and cycle.

You use the Administer Workers task to find the appropriate assignment. And you use the Reprocess or Add New
Plan button to re-evaluate her eligibility for the specified plan and cycle. The process finds her ineligible because she
isn't in the organization anymore, and removes Janice from her primary plan managers' worksheets.

383

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 70
Examples of When to Reprocess an Individual after Starting
a Workforce Compensation Plan Cycle

A Contingent Worker Becomes a Regular Worker After
the Workforce Compensation Cycle Starts

Ravi, a contingent worker, isn't eligible for compensation changes when the cycle starts for a specific workforce
compensation plan. But Ravi manages people who are eligible. Thus his status in the plan worksheets is Limited and he
can only propose compensation changes for his subordinates and approve subordinate managers' plan changes. A few
weeks later, Ravi becomes a regular worker and should now be eligible for compensation changes.

You use the Administer Workers task to find the appropriate assignment. And you use the Reprocess or Add New
Plan button to re-evaluate his eligibility for the specified plan and cycle. If the process finds him eligible, it changes
Ravi's status to Eligible in the appropriate primary plan managers' worksheets.

384

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 71
Total Compensation Statement Overview

71  Total Compensation Statement Overview

Guidelines to Create Total Compensation Statement
Definitions

The statement definition acts as a template and determines the layout and content of the generated statement. The
statement definition configures the display of compensation items added to compensation categories.

This topic explains:

• Statement definition approaches

• Reuse of statements and components

• Editing categories

• Statement display flexibility

•

Iterative design process

Statement Definition Approaches
You can create statement definitions using either of the following approaches:

• Create the item and category components as you the build statement hierarchy.

• Define the item and category building block components first, and then associate them hierarchically.

The second approach promotes reuse of items and categories across multiple statements.

You can also share statement definitions across environments or with your colleagues by using the Export XML and
Import XML actions. When you import you'll have objects that are in progress. If you share statement definitions with
colleagues, then your sources will be different. Categories and subcategories display partially completed icons. You
need to complete any unfinished items or categories. Then, generate statements using the newly imported Statement
Definition.

Reuse of Statements and Components
You can:

•

Include multiple legal employers, multiple countries, and multiple currencies in one statement.

• Add compensation items with sources that belong to different legal employers.

• Use the same categories in multiple statements.

• Reuse statement definitions by adding new statement periods and then modify the definition for subsequent

periods.

• Duplicate a definition as the starting point for other definitions.

385

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 71
Total Compensation Statement Overview

Editing Categories
Edits to categories affect all statement definitions that use that category (as a category or subcategory). This applies
whether you make the edits from the Manage Compensation Categories page or the Manage Statement Definitions
page. Exception: Compensation category display names are local to the statement definition where you create or edit
the name and don't impact the compensation category.

Statement Display Flexibility
Top-level categories in the statement definition appear in the optional summary page and as separate pages in the
statement.

The optional summary page:

• Provides workers with high-level view of their total compensation in graphs and tables

• Displays summed totals of top-level categories included in monetary and nonmonetary sections

Viewers can drill down to detailed category pages from the summary page or use regional area navigation links,
depending on how you configure the category.

Iterative Design Process
Configuring top-level compensation categories and statement definitions is an iterative process. You generate, view,
purge, and regenerate your statements multiple times while editing category and statement definition and display
options.

Overview of Creating a Total Compensation Statement

Configure the design, content, and delivery of a total compensation statement that includes pay such as base pay,
variable compensation, fringe benefits, cost of benefits, and paid time off.

The following figure shows the construction of a total compensation statement and how it displays items and
categories.

386

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 71
Total Compensation Statement Overview

To construct a total compensation statement, application implementors and compensation administrators:

1. Define compensation items that map to sources of estimated or actual amounts paid to workers or costs

incurred by the company.

2. Arrange compensation items into categories such as cash compensation, base pay, benefits, or company stock.
3. Assemble categories into statement definitions.

◦ Top-level categories in the statement definition appear in the optional summary page and as separate

pages in the statement.

◦ Display category details on a single page or enable recipients to drill to details in the statement.
◦ Configure optional graphical displays of data, worker instructions, and supplemental information such as

compensation policies or benefit plan details.

◦ Define periods for which statement data is valid and add an optional welcome message for each period.

4. Configure settings that control statement availability and the default stock price and currency used for

estimated values.

5. Generate statements by selected population filters, including manager hierarchy, for review by compensation

manager.

387

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 71
Total Compensation Statement Overview

6. Monitor process logs.
7. Make statements available for workers to view.
8. Purge unneeded statements and monitor processes with summary and detailed online reports.
9. Enable feedback and configure ratings and questions. Feedback lets you gauge employee satisfaction with total

compensation thereby improving the total compensation package.

To define total compensation statements, use the Total Compensation Statements task list in the Compensation work
area.

Related Topics

• Compensation Items and Sources

• Compensation Category Types

• Compensation Categories and Subcategories

• Guidelines to Create Total Compensation Statement Definitions

• Best Practices for Planning Statement Definitions

Display Options in Statements

Options for Display and Layout of Total Compensation Statements

You have many options to control the layout and display of tables and categories in total compensation statements.
Additional options control graphic displays, descriptive text, and supplemental information.

In general, you configure display options for:

• Category detail pages during category setup

• Top-level categories and the summary page during statement definition setup

The following table describes and compares the display options available when creating or editing compensation
categories and compensation statement definitions.

Display Option

Category Setup

Statement Definition Setup

Hide table columns

Rename table columns

Configure display of zero or no values

Configure graph display

Add descriptive text

Yes

Yes

Yes

Yes

Yes

Yes: summary page columns

Yes: top-level categories only

Yes: top-level categories only

Yes: in summary page

Yes: in summary page

388

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 71
Total Compensation Statement Overview

Display Option

Category Setup

Statement Definition Setup

Add supplemental text

Change vertical display order

Hide regions for graphs or descriptions

Yes

Yes

Yes

Yes: in summary page

Yes: in summary page

Yes: in summary page

Exclude category from statement summary

No

Yes: top-level categories only

Hide or show estimated amount indicator

No

Include and hide statement summary page

No

Include and hide welcome message

Select printable statement options

Display job or position, or both, in the
statement header

No

No

Yes

Yes

Yes

Yes

Yes

Yes: in statement options

Related Topics

• Best Practices for Hiding Columns in a Statement

• Options to Handle Display of Statement Categories When Zero or No Values Exist

• Options for Displaying Graphs in Total Compensation Statement

Best Practices for Hiding Columns in a Statement

You can edit the column properties to hide a column in the category or statement summary page. When you hide a
column, the data that the column would display isn't included in summary or detail tables or graphs.

Hiding Columns
You can hide:

• Unused or not applicable columns, such as the worker contribution column in a cash compensation category

• Description columns

You can show a category's row in the statement even when it contains only zero values. However, you should show at
least the Description column and enter an explanation, otherwise viewers see only a row of zeros. You can't hide all
columns in a category if you configure the category level of details to show all details on a single category overview
page.

389

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 71
Total Compensation Statement Overview

Options to Handle Display of Statement Categories When Zero or
No Values Exist

When you design categories for a statement, you can decide how to handle display when a worker has zero or no values
to display during the statement period. You design categories using the Manage Compensation Categories task.

Contribution Values
Zero or no values might occur when a worker:

• Didn't receive any stock options during the period

•

Isn't participating in a compensation or benefit plan

The following table describes the zero or no value display options.

Statement Element

Display Options When All Contribution Values are Zero or No Value

Top-level categories page

Do not display category if zero values or no values exist

Display category if values are zero; hide if no value exists

Always display the category page

Stock subcategory rows

Do not display row when no values exist or values are zeroes

Display row if values are zeroes and allow subcategory drill

Display and allow drill if historical values are over zero

Always display the row and prevent drilling to subcategory

Always display the row and allow drilling to subcategory

Items in categories

Do not display row when no values exist or values are zeroes

Display row if values are zeroes; hide if no values exist

Always display the row

If you decide to display the row or category page with zero or no values, you can optionally compose a statement
message to:

• Explain the lack of values

• Call attention to missed opportunities, such as participation in a stock purchase plan

390

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 71
Total Compensation Statement Overview

Options for Displaying Graphs in Total Compensation Statement

You can display up to two graphs for each category. If you include a summary page in the statement, you can also
include up to two graphs each in the Monetary and Nonmonetary sections of the summary.

For each graph that you decide to display, you must specify:

• Graph type: Pie chart or various types of bar chart

• Columns included in the graph: Worker contributions, company contributions, or both.

Graphs: Restrictions
A graph must not include columns containing:

• Text or dates

• More than one nonmonetary unit of measure

• A combination of monetary and nonmonetary values

For example, a graph that mixes shares of stock, a company car, and fitness membership doesn't provide clear
information.

If you try mixing combinations of items that use different units of measure you get a warning. You make these
configuration happen on either the category or summary. Graphs with incompatible items are hidden on the total
compensation statement.

Options to Display Title and Salary

You can display the latest title and salary for successive jobs in the statement header.

Here's when title and salary appear in the header:

• Person has only 1 assignment

• Person has only 1 assignment for the employer

• Person has more than 1 assignment, but the entire data of the statement comes from 1 assignment

• The data comes from more than 1 assignment but the person has only 1 valid or active assignment at the end of

the period

This applies to both online and printable statements. This doesn't apply to multiple concurrent jobs where the data will
only appear in the detail and not in the header, as per usual. In that case use the job column in category table to clarify
what amount pertains to what job in the category table.

391

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 71
Total Compensation Statement Overview

392

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

72  Total Compensation Statement
Components

Compensation Items and Sources

Compensation items are the lowest level of compensation detail in the total compensation statement. Map each
item to the specific source from which the statement retrieves compensation information. Items can hold monetary,
nonmonetary, date, or text values. You can use them across statement definitions.

This topic explains the following significant aspects of compensation items:

• Source type

• Type of compensation and unit of measure

• Estimated values

• Rounding

• Proration

• Compensation item testers

• Relationship in the statement

Source Type
Using the Manage Compensation Items task, you map compensation items to the source of the compensation to
retrieve the compensation information. This table describes the source types and special data entry requirements for
each.

Source Type

Benefit Balance

Calculated Item

Element Entry

External Data

Description

Additional Data Entry Requirements

Compensation such as data obtained from a
legacy compensation application entered as a
one-time benefit balance.

Type of Compensation

Create a calculation to define the value of an
item and display it as descriptive text.

Item Value, Operation, Fixed Number

Compensation such as salary and bonus
earnings retrieved from element entry whose
pay period end dates fall within the statement
period.

Legislative Data Group, Payroll Element, and
Input Value

Compensation such as data internal to the
organization from another system, or data from
a third party supplier.

Record Type, Column, and Type of
Compensation.

393

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

Source Type

Formula

Payroll Balance

Description

Additional Data Entry Requirements

Create a formula to retrieve compensation
information that isn't stored in the other
predefined source types.

Type of Compensation, nonmonetary Unit
of Measure, Rounding Rule, and Currency.
(Formula unit or currency overrides item
definition)

Compensation such as commissions or
company-paid taxes retrieved from payroll
balance records. We support these payroll
balance dimensions:

Legislative Data Group

• Relationship Period to Date

• Relationship Year to Date

• Term Period to Date

• Term Year to Date

• Assignment Period to Date

• Assignment Year to Date

• Fiscal Year to Date

•

Inception to Date

• Rolling 12 Months

Salary

Compensation such as overall salaries.

Salary Basis, or all Salary Basis from a
particular Legislative Data Group, or All
Salaries

Salary Rates

Salary amount based on incremental
components

Base Salary or Allowances or Other

Salary Simple Components

Salary amount based on standard components

Base Salary or Allowances or Other

Compensation Type and Unit of Measure
The compensation item inherits from the source:

• Default type of compensation, such as monetary or nonmonetary

• Monetary currency

• Nonmonetary unit of measure (UOM)

In some cases you can override the default compensation type and nonmonetary UOM when defining the item.

•

If a formula that retrieves compensation also specifies currency or nonmonetary unit of measure, the formula
configuration overrides the currency or unit selections in the item definition.

• The currency defined in the benefit balance overrides the currency on the item definition.

Estimated Values
For each item, you can select the Estimated amount option to indicate that this compensation isn't the actual amount
paid. In the statement definition, you can specify whether to display the estimated amount indicator for amounts
designated as estimated.

394

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

Rounding
You can specify how to round nonmonetary amounts.

Proration
You can control whether proration occurs for element entry style compensation items. You can enable proration or not
for salary, and also enable it for other element entries. Use the Allow Proration radio buttons on the compensation item
when the source type is Element Entry and Type of Compensation is Monetary. We recommend that you always select
Yes for any element entries linked to a salary basis.

Compensation Item Testers
Use the Test buttons to verify that the results are what you expect before you generate the statements.

Items in the Statement Hierarchy
You can't add items to statement definitions directly. To include them on statements, you must add items to a
compensation category.

Related Topics

• Overview of Using Formulas

Formula Type for Total Compensation Item

The Total Compensation Item formula determines compensation information that isn't stored in the other predefined
item source types.

You select the formula when you manage compensation items on the Create or Edit Compensation Items page. Click the
Validate button to validate your expectations for compensation items before you generate the statements.

The following contexts are available to formulas of this type:

• DATE_EARNED

• EFFECTIVE_DATE

• END_DATE

• START_DATE

• HR_ASSIGNMENT_ID

• HR_TERM_ID

• JOB_ID

• LEGISLATIVE_DATA_GROUP_ID

• COMPENSATION_RECORD_TYPE

• ORGANIZATION_ID

• PAYROLL_ASSIGNMENT_ID

• PAYROLL_RELATIONSHIP_ID

395

Oracle Fusion Cloud Human Resources
Implementing Compensation

• PAYROLL_TERM_ID

• PERSON_ID

Chapter 72
Total Compensation Statement Components

Database items related to Person, Assignment, Salary, Element Entries, Compensation Record, and From and End Dates
are available to formulas of this type.

The following input variables are available to formula of this type.

Input Value

Data Type

Required

Description

CMP_IV_PERIOD_ID

Char

CMP_IV_PERIOD_START_DATE

Date

CMP_IV_PERIOD_END_DATE

Date

Y

Y

Y

Period ID

Statement Period Start Date

Statement Period End Date

The following return variables are available to formula of this type.

Return Value

Data Type

Required

Description

COMPENSATION_DATES

Date

VALUES

Char

ASSIGNMENTS

Char

LEGALEMPLOYERS

Char

UNIT

Char

COMPENSATION_DATES1

Date

Y

Y

N

N

N

Y

One to 15 transaction dates
delimited by semicolon, maximum
250 characters.

One to 15 transaction values
delimited by semicolon, maximum
250 characters. Must be the same
number of values as dates.

One to 15 transaction assignments
delimited by semicolon, maximum
250 characters. Must be the same
number of assignments as dates.
Can return an empty space with a
delimiter (; ;).

One to 15 legal employer IDs
delimited by semicolon, maximum
250 characters. Must be the same
number of assignments as dates.
Can return an empty space with a
delimiter (; ;).

4 optional variables for every value
and every variable can have more
than one value delimited by “;”.
Can return currency code from
monetary units.

Second variable for transaction
dates from 16 to 30 if limit of 250
characters is exceeded.

396

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

Return Value

Data Type

Required

Description

VALUES1

Char

ASSIGNMENTS1

Char

LEGALEMPLOYERS1

Char

UNIT1

Char

COMPENSATION_DATES2

Date

VALUES2

ASSIGNMENTS2

LEGALEMPLOYERS2

UNIT2

Char

Char

Char

Char

COMPENSATION_DATES3

Dates

VALUES3

ASSIGNMENTS3

LEGALEMPLOYERS3

UNIT3

Char

Char

Char

Char

Y

N

N

N

Y

Y

N

N

N

Y

Y

N

N

N

This sample formula returns one date and one value based on the worker ID.

Second variable for transaction
values from 16 to 30 if limit of 250
characters is exceeded.

Second variable for transaction
assignments from 16 to 30 if limit
of 250 characters is exceeded.

Second variable for legal employer
IDs from 16 to 30 if limit of 250
characters is exceeded.

4 optional variables for every value
and every variable can have more
than one value delimited by “;”.
Can return currency code from
monetary units.

Transaction dates from 31 to 45.

Transaction values from 31 to 45.

Transaction assignments from 31 to
45.

Legal employers from 31 to 45.

4 optional variables for every value
and every variable can have more
than one value delimited by “;”.
Can return currency code from
monetary units.

Transaction dates from 46 to 60.

Transaction values from 46 to 60.

Transaction assignments from 46
to 60.

Legal employers from 46 to 60.

4 optional variables for every value
and every variable can have more
than one value delimited by “;”.
Can return currency code from
monetary units.

397

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

/*******************************************************************
FORMULA NAME : Total Compensation Simple Item Formula
FORMULA TYPE : Total Compensation Item
DESCRIPTION : Returns one date and one value.
*******************************************************************/

/*=========== INPUT VALUES DEFAULTS BEGIN =====================*/
INPUTS ARE CMP_IV_PERSON_ID (text), CMP_IV_PERIOD_START_DATE (date), CMP_IV_PERIOD_END_DATE (date)
DEFAULT FOR CMP_IV_PERSON_ID IS '-1'
DEFAULT FOR CMP_IV_PERIOD_START_DATE IS '4712/12/31' (date)
DEFAULT FOR CMP_IV_PERIOD_END_DATE IS '4712/12/31' (date)
/*============ INPUT VALUES DEFAULTS ENDS =====================*/

/*=================== FORMULA SECTION BEGIN =================*/
COMPENSATION_DATES = '2005/01/01'
VALUES = '500.00'

ASSIGNMENTS = to_char(get_context(HR_ASSIGNMENT_ID,-1))

RETURN COMPENSATION_DATES, VALUES, ASSIGNMENTS

/*================ FORMULA SECTION END =======================*/

This sample formula returns multiple variables.

/*******************************************************************
FORMULA NAME : Total Compensation Multi Item Formula
FORMULA TYPE : Total Compensation Item
DESCRIPTION : Returns multiple variables.
*******************************************************************/

/*=========== INPUT VALUES DEFAULTS BEGIN =====================*/
INPUTS ARE CMP_IV_PERSON_ID (text), CMP_IV_PERIOD_START_DATE (date) , CMP_IV_PERIOD_END_DATE (date)
/*=========== INPUT VALUES DEFAULTS ENDS =====================*/

/*================= FORMULA SECTION BEGIN =================*/

COMPENSATION_DATES = '2009/01/01;2009/02/01;2009/03/01'
COMPENSATION_DATES1 = '2009/07/01;2009/08/01;2009/09/01'
COMPENSATION_DATES2 = '2009/10/01;2009/11/01;2009/12/01'
COMPENSATION_DATES3 = '2009/10/01;2009/11/01;2009/12/01'

VALUES = '200.00;200.00;300.00'
VALUES1 = '300.00;500.00;500.00'
VALUES2 = '500.00;500.00;600.00'
VALUES3 = '600.00;600.00;700.00'

/* Returns only first two assignment */
ASSIGNMENTS = ';1234567890;1234567890'
ASSIGNMENTS1 = '1234567890;1234567890;1234567890'

/* Returns last two assignments */
ASSIGNMENTS2 = ';1234567890;1234567890'
/* Returns first and last assignments */
ASSIGNMENTS3 = '1234567890;;1234567890'

LEGALEMPLOYERS = '0123456789;;0123456789'
LEGALEMPLOYERS1 = '0123456789;0123456789;0123456789'
LEGALEMPLOYERS2 = '0123456789;0123456789;0123456789'
LEGALEMPLOYERS3 = '0123456789;0123456789'

UNIT = 'USD'
UNIT1 = 'EUR'
UNIT2 = 'AUD'
UNIT3 = 'CAD'

398

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

RETURN
 COMPENSATION_DATES,VALUES,COMPENSATION_DATES1,VALUES1,COMPENSATION_DATES2,VALUES2,COMPENSATION_DATES3,VALUES3,ASSIGNMENTS,ASSIGNMENTS1,ASSIGNMENTS2,ASSIGNMENTS3,L
GALEMPLOYERS,LEGALEMPLOYERS1,LEGALEMPLOYERS2,LEGALEMPLOYERS3,UNIT,UNIT1,UNIT2,UNIT3

/*================ FORMULA SECTION END =======================*/

Related Topics

• Formula Compilation Errors

• Formula Execution Errors

• When do I run the Compile Formula process?

• Example of Writing a Fast Formula Using Formula Text

Compensation Category Types

The compensation category type determines the table columns and general layout of the category page in the total
compensation statement, as well as whether the category can include subcategories. This topic explains the category
types and provides an example of a user-defined category.

Types
The following table shows the category types with default column and configuration details.

Category Type

Default Columns

Configurable

• Benefits

• Worker contributions

• Add compensation items

• Cash Compensation

• Employer contributions

• Nest categories within the category as

• Savings

• Retirement

• Description

subcategories

• Hide columns that don't apply

Time Off

• Type of time off

• Edit column labels

• Monetary value of the time off

• Configure category table row names as

• Accrued balance

links to more information

• Can't nest categories as subcategories

Stock History

Select columns of data from the database table
that stores workers' stock details

• Select which types of stock to include in

the category

• Alter which columns are hidden or only
available optionally in statement view
menu

• Edit column labels

• Can't nest categories as subcategories

Other

Same basic structure as the Cash
Compensation or Benefits category type

You can use it for any type of compensation

399

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

Category Type

User-Defined

Default Columns

Configurable

Specify the number of columns, up to five, that
you want to include in the category

• Configure column labels

• Select compensation items for the table

rows

• Can't nest categories as subcategories

User-Defined Category Example
You might use the user-defined category type to display information about commissions by including columns, such as:

• Sales target

• Units sold

• Percentage over target

• Percentage under target

• Commission amount

Related Topics

Compensation Categories and Subcategories

Compensation categories display information in tables. Use categories to group similar or related compensation
items, such as Cash Compensation, Benefits, Time Off, or Stock History. You can use the same categories in multiple
statements. You can also display categories directly on the summary page.

Consider the following factors when planning how to group compensation items and categories for display:

• Category type

• Contribution type and unit of measure

• Level of detail

Category Type
Consider these points:

• Category type determines the table columns and general layout of the page in the statement.

• You can't add categories as subcategories to the Stock History, User-Defined, or Time Off category types.

• After you use a category in any statement, you can't change the category type.

Contribution Type and Unit of Measure
The contribution type and unit of measure of the associated items or subcategories determines:

• Category's contribution type (monetary or nonmonetary)

• Category's nonmonetary unit of measure

400

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

All items and subcategories within a nonmonetary category must share the same unit of measure.

Level of Detail
When you create a category, you specify how you want to display the category details in the statement.

Select one of these level of detail values:

• Viewers drill into line items to see details

• Viewers see all details on one page

Related Topics

• Options to Display Category Details in a Compensation Statement

• Best Practices for Hiding Columns in a Statement

• Options to Handle Display of Statement Categories When Zero or No Values Exist

• Options for Displaying Graphs in Total Compensation Statement

Options to Display Category Details in a Compensation
Statement

Use the Manage Compensation Categories task in the Compensation work area to specify how to display the category
details in the statement. Select from two level of display options, depending on category type and design preference.

Viewers Drill Into Line Items to See Details
Provide links from a high-level category page that drill down to specific details for each item or subcategory row in the
category.

Example: You can create a Benefits category that displays high-level information for different health benefits, such as:

• Medical

• Dental

• Life Insurance

To see the details of each row in the category, such as medical, viewers can drill into the row to a separate details page.

Viewers See All Details on One Page
Display the full detail of the category's content on a single page in the statement. For example, you can create a Bonus
category that displays the amount of different bonuses (such as new hire and quarterly) as rows on the category page.

If you select to show all details on a single page:

• The name column doesn't show in the statement for rows in the category.

• You can't hide all columns in the category.

401

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

• You can't add subcategories to these category types: Benefits, Cash Compensation, Savings and Retirement, or
Other. However, you can add subcategories to these category types if the level of detail enables drilling to see
details.

It's best not to show all details on a single page for recurring information.

Best Practices for Planning Statement Definitions

You need to consider certain statement elements and options when you plan how many different total compensation
statement definitions to create and the presentation of content in each.

These are the statement elements and options to consider:

• Statement audience

• Statement definition details

• Statement periods

Statement Audience
You can create different statement definitions for different statement audiences. Use the following two methods,
individually or in combination, to limit the statement audience:

• Attach an eligibility profile to the statement on the Statement Options tab.

Example: Within a business unit, you create separate statement definitions for individual contributors and
executive level workers by:

a. Creating eligibility profiles that differentiate between individual contributors and executive workers.
b. Attaching each eligibility profile to the corresponding statement definition.

• Use the following population filter parameters to specify your audience when you generate statements:

◦ Business unit
◦ Benefits group
◦ Legislative data group
◦ Country
◦ A person selection formula that you define
◦ A single person that you select

Statement Definition Details
Build the statement hierarchy of categories and items appropriate for the audience. Configure table and graphical
displays, descriptive text, and supplemental information.

402

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

Statement Periods
Configure statements to cover any period of time by specifying start and end dates on the statement definition Periods
tab. You can create multiple periods at one time. For each statement period, further specify:

• An optional statement period display name

Example: Name the period 2011 Annual Statement rather than the default display of start and end date.

• The date that statements become available to workers

• The conversion rate date for currency conversions

• An optional welcome message.

Total Compensation Statement Options

You can configure an optional summary page, estimated amount indicator, and welcome message for each statement.

Summary Page
On the statement definition Options tab, you can configure the summary page. The optional summary page consists of
the following optional features:

• Monetary and Nonmonetary sections, each containing section-level descriptive text, graphs, and tables

• Summary page descriptive text that can include rich text formatting and hyperlinks

Include placeholder fields for values that vary among workers, such as the first name, a compensation item
amount, or work location. These placeholder fields enable you to use the same text for different workers.

• Summary page supplemental information, such as hyperlinks to company policies and resources, which are

displayed in a separate window

If you include a graph in the Nonmonetary section, all top-level categories in the nonmonetary summary should share
the same unit of measure. You can exclude individual top-level categories from the summary.

Estimated Amount Indicator
Displaying an estimated amount indicator in the statement requires two configuration steps:

•

Item definition: When creating compensation items, identify whether the item amounts are estimates.

• Statement definition: On the statement definition Options tab, specify whether to display or hide the indicator

that visually denotes amounts as estimated.

Welcome Message
For each statement period, you can compose an optional welcome message on the statement definition Periods tab. In
the welcome message you can:

• Personalize the greeting with each worker's name

• Use rich text and include hyperlinks

403

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

•

Include placeholder fields for values that vary among workers, such as the first name, a compensation item
amount, or work location. These placeholder fields enable you to use the same text for different workers.

• Use the Preview Text in Printable Statements option to see what the statement looks like with placeholders, not

real-time data.

If included, the welcome message is the first page the worker sees in the statement.

Online and Printable Statements
You can configure either online or printable statements or both. Some options are available in certain statements.

Online and Printable Statements

Option

Statement Type

Detail sections defined in the online
statement drill downs

Estimated stock values

Both

Both

Display person mailing address columns

Both

Include category line item detail section
option

Left-click menu navigation

Online

Online

Links within the statement navigation

Printable

Mass generate statements

Printable

Options to Include Descriptive Text in Compensation
Statements

You can include descriptive text in the Welcome, Summary, and Descriptive Text sections of total compensation
statements.

You can also insert fields into your descriptive text that act as placeholders. When you generate statements for your
workers, these fields are replaced with the actual values for each worker.

For example, you can insert the <FIRST_NAME> field, which the generate process then replaces with the worker's first
name, such as Marie. Or, you use descriptive text to inform the employee of company-specific information, such as
company policies.

Here's a list of fields you can insert as part of the descriptive text. You can access these fields from the Insert Field
menu on the Descriptive Text tab.

Option

Description

Person Name

Name information, such as <FIRST NAME>, <MIDDLE NAME>, and <LAST NAME>.

404

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

Option

Description

Employment

Location information, such as <DEPARTMENT>, <BUSINESS UNIT>, and <EMPLOYER>.

Job information such, as <JOB>, <GRADE>, and <POSITION>.

Compensation Item

Compensation item information, such as bonus or car allowance.

For example, you can select the <BONUS> compensation item.

Conditional Text

Compensation item information that appears when it meets the conditions that you create.

For example, you can show the monthly salary: <Most recent [Pay Monthly] * 12 Is not blank) Or
(Sum[Pay Monthly] Is not blank)>.

Miscellaneous

Date information, such as <STATEMENT START DATE> and <STATEMENT END DATE>

You can use the Fields icon to manage or reuse fields already created. You need to recreate the Conditional text from
period to period.

Related Topics

• Total Compensation Statement Options

Options to Configure Statement Periods, Welcome
Message, and Feedback

Using the Statement Definitions Periods tab, you configure statement periods, an optional welcome message for each
statement and feedback.

Statement Periods
Configure statements to cover any period of time by specifying start and end dates on the Periods tab. You can create
multiple periods at one time.

For each statement period, further specify:

• A recommended statement period display name

Example: Name the period 2022 Annual Statement, rather than the default display of start and end date.

• The date that statements become available to workers

• The conversion rate date for currency conversions

• An optional welcome message

405

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

Use the item tester to validate your expectations for compensation items before you generate the statements. The item
tester is available for all source types.

Optionally, you can enable feedback when people view their online statement. You can configure ratings and questions.
People complete the feedback, and then compensation administrators and line managers can view it.

Statement Periods to Display
Use the Configure Total Compensation Global Settings task to control the statement periods available to workers. If you
don’t enter a number, the worker sees all statements. If you enter 0, the worker doesn’t see any statements. Finally, if
you enter a number greater than 0, the worker sees that many statements.

Welcome Message
For each statement period, you can compose an optional welcome message by clicking the Welcome Message button
on the Periods tab. If included, the welcome message is the first page the worker sees in the statement.

In the welcome message you can:

• Personalize the greeting with each worker's name

• Use rich text and include hyperlinks

Feedback
You can find out how your people feel about total compensation. You start by enabling feedback on the Statement
Periods tab. Then, configure your ratings and questions. You generate statements in the usual manner. The feedback
appears on online statements only. People complete the feedback, so compensation analysts, compensation managers,
and line managers can view the results.

Here's where you can see the feedback results:

• Compensation Work Area > Total Compensation > View Total Compensation Statement Reports

• My Team > Show More > Compensation > Total Compensation Statement Feedback

Options to Configure Statement Eligibility and Summary
Page

On the Statement Definition Statement Options tab, configure an optional summary page, eligibility profile, and
visibility of the estimated amount indicators.

Summary Page
Top-level categories in the statement definition appear in the optional summary page and as separate pages in the
statement.

The optional summary page provides workers with a high-level view of their total compensation in monetary and
nonmonetary sections. Viewers can drill down to detailed category pages from the summary page or use regional area
navigation links, depending on how you configure the category.

406

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

On the Statement Options tab, configure the following optional features of the summary page:

• Monetary and Nonmonetary sections, each containing section-level descriptive text, graphs, and tables

• Summary page descriptive text that can include rich text formatting and hyperlinks

• Summary page supplemental information, such as hyperlinks to company policies and resources, which are

displayed in a separate window

Tip:  If you include a graph in the Nonmonetary section, all top-level categories in the nonmonetary summary should
share the same unit of measure. You can exclude individual top-level categories from the summary.

Eligibility Profile
Attach an eligibility profile to limit the audience of the statement. The eligibility profile works as a further refinement to
statement generation process parameters, such as business unit or legislative data group.

Example: Within a business unit, you create separate statement definitions for individual contributors and executive-
level workers by:

1. Creating eligibility profiles that differentiate between individual contributors and executive workers.
2. Attaching each eligibility profile to the corresponding statement definition.
3. Selecting the Business Unit parameter when generating either statement.

Estimated Amount Indicator
Displaying an estimated amount indicator in the statement requires two configuration steps:

•

Item definition: When creating compensation items, identify whether the item amounts are estimates.

• Statement definition: On the Statement Options tab, specify whether to display or hide the indicator that

visually denotes amounts as estimated.

Printable Statement Templates

You can maintain, preview, and upload your printable statement templates using the Manage Template task in the
Compensation work area.

You can use the delivered template as is or you can modify it, for example by adding your company logo. Then, you can
click the upload action to upload the modified template. You can preview your uploaded template. Finally, on the Create
or Edit Statement Definition page, Printable Statement Options tab, you can verify which template is used.

Using the Printable Statement Templates task to modify the delivered template ensures you follow the best practices for
business intelligence customize feature.

407

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

FAQs

How can I change whether the category displays zero or no values
in the statement?

Edit the top-level category only on the Edit Statement Definition page. Or, edit the subcategory and item rows on the
Edit Compensation Categories page.

Follow these steps:

1. Select the category or item row.
2. Select the zero value display option in the Actions menu.

The Display Zero Rows column shows the current setting for each category.

How can I display a hidden column?

Edit the summary table column properties only on the summary page. Or, edit each individual category's column
properties on the Edit Compensation Category page.

Follow these steps:

1. Click the Column Properties button.
2. Select the column from the menu.
3. Update the option to display the column in the statement.

How can I hide or show the welcome message in total
compensation statements?

You can use the Manage Statement Definitions task in the Compensation work area to hide or show the message.

Follow these steps:

1. Select the statement definition and click Edit.
2. On the Periods tab, select the button in the Welcome Message column.
3. Edit the Do not display welcome message option.

How can I change welcome message text in total compensation
statements?

Use the Manage Statement Definitions task in the Compensation work area to change the message.

408

Oracle Fusion Cloud Human Resources
Implementing Compensation

Follow these steps:

Chapter 72
Total Compensation Statement Components

1. Select the statement definition and click Edit.
2. On the Periods tab, select the Edit button in the Welcome Message column.

Why can't I delete or edit some items?

If the item is in use in a compensation category, you can't delete it. Also, you can't edit some attributes, such as the type
of compensation and nonmonetary unit of measure.

Why did the default stock details change?

More than one administrator might have access to these settings.

The following tasks use the stock price and currency information:

• View compensation history

• Manage workforce compensation

• Generate total compensation statements

How can I import stock data sent to me by my supplier?

On the Manage Stock Grants page, use the Prepare Import Spreadsheet button to generate the stock table spreadsheet.
Enter your supplier's data, ensuring that each row contains a unique Grant Date, Grant ID, and Grant Number. Upload
the information into the stock table.

Can I reuse a previous year's statement?

Yes. You can reuse an existing statement definition by adding new periods.

You might also want to:

• Update the welcome message

• Add or edit the items and categories included

• Hide or update the display of graphs, descriptive text, and supplementary information

Can I correct the definition after workers received statements?

Yes. You can correct the statement definition and regenerate the statements, which makes the newer version available
to workers.

409

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 72
Total Compensation Statement Components

What's the difference between total compensation statements and
workforce compensation change statements?

Total compensation statements show base and variable pay, fringe benefits, and perks for a specified period of time,
typically a year. These statements are available both online and in PDF format. You configure these statements using
the Total Compensation Statement tasks in the Compensation

You configure these statements using the Total Compensation Statement tasks in the Compensation work area.
Workforce compensation statements show recent changes to base and variable pay. They apply to a statement group,
which has RTF templates that can include criteria to identify which people get the template.

For example, people in Spanish-speaking countries get the Spanish version of the statement. The workforce
compensation plan containing the statement configuration determines the statement content. You configure
these compensation change statements for a specific plan using the Workforce Compensation Plans task in the
Compensation work area.

410

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 73
Total Compensation Examples

73  Total Compensation Examples

Create a Bonus Category

This example demonstrates how to create a bonus category that includes a profit sharing bonus, a new hire bonus, and
a quarterly bonus. The new hire and quarterly bonus items already exist and are reused in this category.

The following table summarizes key decisions for the Profit Sharing compensation item in this scenario.

Decision to Consider

Item in This Example

What compensation does the item
represent?

Profit sharing bonus

What's the source type?

Payroll element

What's the legislative data group?

USA

The following table summarizes key decisions for the category in this scenario.

Decision to Consider

Category in This Example

What's the category type?

Cash Compensation

Display category details in the statement
at what level?

Viewers see all details on one page.

Add items?

Yes: Profit sharing bonus, new hire bonus, and quarterly bonus.

Display graphs? How many? What type?

Yes. Two: Bar and stacked bar.

Hide or edit any columns in the category?

Hide worker contributions because this is a cash compensation category. Edit company contribution
column name to make it familiar to workers.

Before you start

1. Create a payroll element named Profit Sharing Bonus using the USA legislative data group.
2. Create the following compensation items using payroll elements in the USA legislative data group:

◦ New Hire Bonus
◦ Quarterly Bonus

Here's what to do

411

Chapter 73
Total Compensation Examples

Oracle Fusion Cloud Human Resources
Implementing Compensation

1. Create a compensation item.

a. Click the Manage Compensation Items task.
b. Click Create.
c. Complete the fields as shown in this table:

Field

Value

Item Name

Source Type

Profit Sharing Bonus

Element entry

Legislative Data Group

USA

Payroll Element

Profit Sharing Bonus

Input Value

Pay Value

d. Click Save and Close.

2. Enter category details and add items.

a. Click the Manage Compensation Categories task.
b. Click Create.
c. Complete the fields, as shown in this table.

Field

Name

Value

Bonus

Category Type

Cash Compensation

d. Click Continue.
e. Select Viewers see all details on one page in the Level of Detail field.
f. Click Add Items three times to add three new rows.
g. Complete the fields for each new row as shown in this table.

Name

Description

Company Contribution (Items)

Profit Sharing

Profit Sharing Bonus

Profit Sharing Bonus

New Hire

Quarterly

New Hire Bonus

New Hire Bonus

Quarterly Bonus

Quarterly Bonus

h. Click Edit Column Properties and select the Your Contribution column.
i. Select Do not display in the statement.
j. Click OK.
k. Click Edit Column Properties and select the Company Contribution column.
l. Enter Amount in the Column Label field.

m. Click OK.

412

Oracle Fusion Cloud Human Resources
Implementing Compensation

3. Configure display options.

Chapter 73
Total Compensation Examples

a. On the Graphs tab, Complete the fields for two graphs, as shown in this table.

Field

Graph Title

Graph Type

Graph Items

Value for the First Graph

Value for the Second Graph

Your Bonuses

How Your Bonuses Add Up

Bar

Amount

Bar - stacked

Amount

b. Click Save.
c. Click OK in the confirmation.
d. Select the Descriptive Text tab.
e. Enter any text here to describe what's included in this category or details about policies, and format it

appropriately.

f. Click Reorder Components at the top of the page.
g. Select Descriptive Text and click the downward arrow until Descriptive Text appears below Graphs.
h. Click OK.
i. Click Save and Close.

Related Topics

• Create a Total Compensation Statement

Create a Salary Category

This example demonstrates how to create a salary category that includes All salaries, with Salary as a Source Type.

The following table summarizes key decisions for a salary compensation item in this scenario.

Decision to Consider

Item in This Example

What compensation does the item
represent?

Salary

What's the source type?

Salary

What's the selection criteria?

All salaries

What's the salary basis type?

All

The following table summarizes key decisions for the category in this scenario.

413

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 73
Total Compensation Examples

Decision to Consider

Category in This Example

What's the category type?

Cash Compensation

Display category details in the statement
at what level?

Viewers drill into details

Add items?

Yes: Salary

Display graphs? How many? What type?

No

Hide or edit any columns in the category?

Hide worker contributions because this is a salary category.

Before you start

1. Check whether you have at least 1 salary basis configured and assigned to employees.

Here's what to do

1. Create a compensation item.

a. Click the Manage Compensation Items task.
b. Click Create.
c. Complete the fields as shown in this table:

Field

Item Name

Source Type

Value

Salary

Salary

Selection Criteria

All salaries

Salary Basis Type

All

Estimated Amount

Not checked

d. Click Save and Close.

2. Enter category details and add items.

a. Click the Manage Compensation Categories task.
b. Click Create.
c. Complete the fields, as shown in this table.

Field

Name

Value

Salary

414

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 73
Total Compensation Examples

Field

Value

Category Type

Cash Compensation

d. Click Continue.
e. Select Viewers drill into details in the Level of Detail field.
f. Click the Salary compensation item.
g. Complete the fields for each new row as shown in this table.

Name

Salary

Description

Your Salary

Company Contribution (Items)

Salary

h. Click Edit Column Properties and select the Your Contribution column.
i. Select Do not display in the statement.
j. Click OK.
k. Click Save and Close.

Related Topics

• Compensation Items and Sources

• Create a Total Compensation Statement

Create a Benefits Category

This example demonstrates how to create a benefits category that includes medical, dental, vision, disability insurance,
and life insurance. The following table summarizes key decisions for the compensation items in this scenario.

Decision to Consider

First Item

Second Item

What compensation does the item represent?

Worker contribution for medical benefit

Company contribution for medical benefit

What's the source type?

Payroll element

What's the legislative data group?

USA

Payroll element

USA

The following table summarizes key decisions for the category in this scenario.

Decision to Consider

Category in This Example

What's the category type?

Benefits

Display category details in the statement
at what level?

Display details of item rows on separate pages that viewers drill to for details.

415

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 73
Total Compensation Examples

Decision to Consider

Category in This Example

Add items? (Describe)

Yes: Both worker and company contributions for medical, dental, vision, disability insurance, and life
insurance benefits.

Add other categories as subcategories?
Describe

No

Display graphs? (No or Yes?) One or two?
What type?

Yes. Two: Stacked bar and pie chart.

Hide or edit any columns in the category?

No

Display the row if values are zero in the
period?

No

Create items for medical insurance, then create a benefits category and attach the items you created along with eight
existing benefits items and configure display options. Use the default values except where otherwise indicated.

Before you start

1. Create the following payroll elements using the USA legislative data group.

◦ Medical Worker Contribution
◦ Medical Company Contribution

2. Create the following compensation items using payroll elements in the USA legislative data group:

◦ Dental Worker Contribution
◦ Dental Company Contribution
◦ Vision Worker Contribution
◦ Vision Company Contribution
◦ Disability Worker Contribution
◦ Disability Company Contribution
◦ Life Insurance Worker Contribution
◦ Life Insurance Company Contribution

Here's what to do

1. Create a compensation item. Use the default values except where indicated.

a.

In the Compensation work area, click Manage Compensation Items to open the Manage Compensation
Items page.

b. Click Create.
c. On the Create Compensation Item page, complete the fields as shown in this table:

Field

Value

Item Name

Medical Worker Contribution

Source Type

Element entry

416

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 73
Total Compensation Examples

Field

Legislative Data Group

Value

USA

Payroll Element

Medical Worker Contribution

Input Value

Pay Value

d. Click Save and Create Another.
e. On the Create Compensation Item page, complete the fields as shown in this table:

Field

Value

Item Name

Medical Company Contribution

Source Type

Element entry

Legislative Data Group

USA

Payroll Element

Medical Company Contribution

Input Value

Pay Value

f. Click Save and Close.

2. Enter category details and add items.

a.

In the Compensation work area, click Manage Compensation Categories to open the Manage
Compensation Categories page.

b. Click Create.
c. On the Create Compensation Categories page, complete the fields, as shown in this table.

Field

Name

Value

Benefits

417

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 73
Total Compensation Examples

Field

Category Type

Value

Benefits

d. Click Continue.
e. On the Create Category page, Table tab, select Viewers drill into line items to see details in the Level of

Detail field.

f. Click Add Items five times to add five new rows.
g. Complete the fields for each new row, entering a name and description of the category row and selecting

compensation items for each contribution column in the category, as shown in this table.

Name

Description

Your Contribution (Items)

Company Contribution

(Items)

Medical

Dental

Vision

Amounts reflect your coverage. Medical Worker Contribution

Medical Company Contribution

Amounts reflect your coverage. Dental Worker Contribution

Dental Company Contribution

Amounts reflect your coverage. Vision Worker Contribution

Vision Company Contribution

Disability Insurance

LTD provides income

Disability Worker Contribution

Disability Company

protection.

Contribution

Life Insurance

Life insurance is a core benefit.

Life Insurance Worker

Life Insurance Company

Contribution

Contribution

3. Configure display options.

a. Select the Graphs tab.
b. Complete the fields for two graphs, as shown in this table.

Field

Graph Title

Graph Type

Graph Items

Value for the First Graph

Value for the Second Graph

Employee Versus Company Contributions

Total Contribution Comparison

Bar

Pie

Your Contribution, Company Contribution

Your Contribution, Company Contribution

c. Click Save.
d. Click OK in the confirmation.
e. Select the Descriptive Text tab.
f. Enter any text here to describe what's included in this category or details about policies, and format it

appropriately.

g. Click Reorder Components at the top of the page.
h. Select Descriptive Text and click the downward arrow until Descriptive Text appears below Graphs.
i. Click OK.
j. Click Save and Close.

418

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 73
Total Compensation Examples

Related Topics

• Create a Total Compensation Statement

Create a User-Defined Category for Commissions

This example demonstrates how to create a Commissions category using the User-Defined category type. The following
table summarizes key decisions for the category in this scenario.

Decision to Consider

Category in This Example

What's the category type?

User-Defined

Display category details in the statement
at what level?

Viewers see all details on one page.

Add items?

Yes: Sales target, sales revenue, and commissions items for year end.

Display graphs? How many? What type?

Yes. Two bar charts, one for revenue generated and one for commissions earned.

Hide or edit any columns in the category?

Edit column labels.

To create the user-defined category for commissions complete the following tasks. Use the default values except where
otherwise indicated.

1. Create a User-Defined category.
2. Attach existing compensation items.
3. Configure display options.

Before you start

Create the following compensation items:

• Sales Target Year End

• Sales Revenue Year End

• Commission Year End

Here's what to do

1. Enter category details and add items.

a. Click the Manage Compensation Categories task.
b. Click Create.
c. Complete the fields, as shown in this table.

Field

Name

Category Type

Value

Commissions

User-Defined

419

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 73
Total Compensation Examples

Field

Value

Number of Item Columns

3

d. Click Continue.
e. Select Viewers see all details on one page in the Level of Detail field.
f. Click Edit Column Properties and select the Your Contribution column.
g. Enter Sales Target in the Column Label field.
h. Click OK.
i. Click Edit Column Properties and select the Company Contribution column.
j. Enter Sales Revenue in the Column Label field.
k. Click OK.
l. Click Edit Column Properties and select the User-Defined Column 3 column.

m. Enter Commission in the Column Label field.
n. Click OK.
o. Click Add Items.
p. Complete the fields for the new row, as shown in this table.

Name

Row 1

Description

Sales Target (Item)

Sales Revenue (Item)

Commission (Item)

Year End Activity

Sales Target Year End

Sales Revenue Year End

Commission Year End

The Name column doesn't show in the statement when the level of detail is configured to display all details
on a single page.

2. Configure display options.

a. Select the Graphs tab.
b. Complete the fields for two graphs, as shown in this table.

Field

Graph Title

Graph Type

Graph Items

Value for the First Graph

Value for the Second Graph

Revenue Generated

Commissions Earned

Bar

Bar

Sales Revenue

Commissions

c. Click Save.
d. Click OK in the confirmation.
e. Select the Descriptive Text tab.
f. Enter any text here to describe what's included in this category or details about policies, and format it

appropriately.

g. Click Reorder Components at the top of the page.
h. Select Descriptive Text and click the downward arrow until Descriptive Text appears below Graphs.
i. Click OK.
j. Click Save and Close.

420

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 73
Total Compensation Examples

Related Topics

• Create a Total Compensation Statement

Create a Stock History Category

This example shows how to create a stock history category for nonqualified stock options with vesting information. You
create a stock history category and configure column visibility and graphs.

The following table summarizes key decisions for the category in this scenario.

Decision to Consider

Category in This Example

What's the category type?

Stock History

Display category details in the statement
at what level?

Viewers see all details on one page.

Display graphs? How many? What type?

Yes.

• One Pie to display Nonmonetary (Shares)

• One Bar to display Monetary (Estimated Values

Hide or edit any columns in the category?

Accept most default column visibility settings. Make some adjustments to visibility of vested share
columns and grant number. Edit some column labels for display on the statement.

The Stock Details table must contain stock data. Use the default values except where otherwise indicated.

1. Enter category details and configure columns.

a. Click the Manage Compensation Categories task.
b. Click Create.
c. Complete the fields, as shown in this table.

Field

Name

Value

Stock History

421

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 73
Total Compensation Examples

Field

Value

Category Type

Stock History

d. Click Continue.
e. Select Non-Qualified Stock Option  in the Grant Type  field.
f. Edit the column labels and availability of column types, as shown in this table, using the default values of

columns not listed.

Sequence

Column Type

Column Label

Available for Displaying

Online Statement

1

3

10

16

17

18

20

25

Original Grant Date

Grant Date

(Use default)

Grant Number

(Use default)

Select

Original Value at Grant

Grant Value

(Use default)

Estimated Market Value of

Estimated Market Value

(Use default)

Total Shares

Vested Shares

(Use default)

Exercised Shares

(Use default)

Select

Select

Estimated Gain from Vested

(Use default)

Deselect

Shares

Exercise Date

(Use default)

Select

2. Configure display options.

a. Select the Graphs tab.
b. Complete the fields, as shown in this table.

Field

Graph Title

Graph Type

Value for the First Graph

Vested Versus Unvested Shares

Pie

Nonmonetary Graph Items

Vested Shares, Unvested Shares

Graph Title

Graph Type

Estimated Values

Bar

Monetary Graph Items

Estimated Market Value of Total Shares, Estimated Gain from Vested Shares

c. Click Save.
d. Click OK in the confirmation.
e. Select the Descriptive Text tab.

422

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 73
Total Compensation Examples

f. Enter any text here to describe what's included in this category or details about policies, and format it

appropriately.

g. Click Reorder Components at the top of the page.
h. Select Descriptive Text and click the downward arrow until Descriptive Text appears below Graphs.
i. Click OK.
j. Click Save and Close.

Related Topics

• Create a Total Compensation Statement

Create a Total Compensation Statement

This example demonstrates how to create, generate, and view a total compensation statement that contains two top-
level categories, one for cash compensation and one for stock.

The statement definition is for individual contributors whose salaries are quoted on an annual basis. The categories
added as subcategories were created for other statement definitions and are reused in this definition. The following
table summarizes key decisions for the compensation item in this scenario.

Decision to Consider

Item in This Example

What compensation does the item
represent

Base pay for exempt workers with annual salary

What's the source type?

Payroll element

What's the legislative data group?

USA

The following table summarizes key decisions for the categories in this scenario.

Decision to Consider

Cash Compensation Category

Stock Category

What's the category type?

Cash Compensation

Other

Display category details in the statement at
what level?

Display details of item and subcategory rows on
separate pages that viewers drill to for details.

Display details of item and subcategory rows on
separate pages that viewers drill to for details.

Add items?

Yes: Base pay for exempt workers

Not directly, only through subcategories.

Add other categories as subcategories?

Yes. One: Bonuses Exempts

Yes. Two: ESPP Exempts and Stock History
Exempts

Display graphs? How many? What type?

Yes. Two: Bar and stacked bar.

No

Hide or edit any columns in the category?

Hide worker contributions because this is a
cash compensation category. Edit subcategory
names to make them familiar to workers.

Edit subcategory names to make them familiar
to workers.

Display the row if values are zero or no in the
period?

No

Display the Employee Stock Purchase Plan row
but prevent drilling to details.

423

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 73
Total Compensation Examples

The following table summarizes key decisions for the statement definition in this scenario.

Decision to Consider

Statement Definition in This Example

Include which top-level categories?

Cash Compensation and Stock

What's the statement period?

Calendar year 2015Also create a second annual period to be ready for the next year.

Include welcome message?

Yes. Address recipients by first name.

Include summary page?

Yes

What's the statement audience for
eligibility?

Individual contributors whose salaries are quoted on an annual basis

What's the population for statement
generation?

Legal employer: Infusion USA

Before you start

1. Create a payroll element named Base Pay Exempts that represents base pay earnings for salaried exempt

workers in the USA legislative data group.

2. Create the following compensation categories with items:

◦ Bonuses Exempts
◦ ESPP Exempts
◦ Stock History

3. Create an eligibility profile named IC Annual Salary that identifies individual contributors who are salaried with

annual salary basis.

Here's what to do

1. Create the compensation item.

a. Click the Manage Compensation Items task.
b. Click Create.
c. Complete the fields as shown in this table:

Field

Value

Item Name

Source Type

Base Pay Exempts

Element entry

Legislative Data Group

USA

Payroll Element

Base Pay Exempts

Input Value

Pay Value

d. Click Save and Close.

2. Create a cash compensation category and attach the base pay item you created along with two existing cash

categories with items.

a. Enter category details and add an item.

424

Chapter 73
Total Compensation Examples

Oracle Fusion Cloud Human Resources
Implementing Compensation

b. Add and configure subcategories.
c. Configure display options.

3. Create a stock category.

a. Enter category details.
b. Add and configure subcategories.
c. Configure display options.

4. Create a statement definition.

a. Enter statement details and add top-level categories.
b. Configure table display options.
c. Define statement periods and welcome message.

5. Configure optional eligibility and statement summary page.

In the Eligibility Profile field, select IC Annual Salary.

a. Select the Statement Options tab.
b.
c. Click Configure Summary Page.
d.
e. Select the Graphs tab.
f. Complete the fields, as shown in this table.

In the Monetary Compensation section, select the Table tab and verify the table contents.

Field

Graph Title

Graph Type

Graph Items

Value for the First Graph

Value for the Second Graph

Your Total Compensation

How Your Compensation Adds Up

Bar

Bar - stacked

Company Contributions

Company Contributions

g. Click Save.
h. Click OK.
i. Select the Descriptive Text tab.
j. Enter any text that you want to appear in the summary page specifically related to monetary compensation.
k. Scroll down to the Summary Page Descriptive Text section and expand it.
l. Enter some text, such as: The summary provides you an overview of your compensation package. Click

each category name to view additional details.

m. Click Save and Close.
n. Click OK.
o. Click Finish to validate the statement.

425

Oracle Fusion Cloud Human Resources
Implementing Compensation

Chapter 73
Total Compensation Examples

426

