Oracle Fusion
Cloud Human
Resources

Using Global Human Resources

Oracle Fusion Cloud Human Resources
Using Global Human Resources

G34740-05

Copyright © 2011, 2025, Oracle and/or its affiliates.

Author: Alison Firth, Jyothi Meruva, Sweta Bhagat, Megan Wallace, Suzanne Kinkead, Hema Hardikar, Richard Kellam, Angela Brown, Srinivas Vellikad,
Lakshmi Venkat, Phyllis Simons, Timothy Bisset, Carla Fabrizio, Jan Somers, Janet McCandless, Tina Brand, Kathryn Wohnoutka, Asra Alim, Jacqui
Wood, Essan Ni Jirman, Barbara Snyder, Santosh Radhakrishnan, Gayathri Akkipeddi, Malini Sampathkumar

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Contents

Get  Help  ................................................................................................................................    i

1 Introduction to Global Human Resources

1

Overview of Using Global Human Resources ...........................................................................................................................  1

Quick  Actions  ..................................................................................................................................................................................     2

FAQs  ...................................................................................................................................................................................................    2

2 Users and Roles

5

User Management ..........................................................................................................................................................................  5

Role Management ..........................................................................................................................................................................   8

3 Departments, Divisions, Organizations, Locations, and Worker Unions

13

Overview of Workforce Structures ............................................................................................................................................   13

List of Values in Workforce Structures .....................................................................................................................................  13

Departments, Divisions, and Organizations ...........................................................................................................................   19

Locations  ........................................................................................................................................................................................    48

Worker  Unions  ...............................................................................................................................................................................    53

4 Jobs and Positions

59

Jobs  .................................................................................................................................................................................................     59

Examples of Jobs .........................................................................................................................................................................  59

Examples of Positions ................................................................................................................................................................   60

Considerations for Using Jobs and Positions ........................................................................................................................  62

Job and Position Structures ......................................................................................................................................................   64

Scheduling Group Attribute for Jobs ......................................................................................................................................   66

Associate Legal Employers with a Job ....................................................................................................................................  67

Workforce Structures Code Generation Methods .................................................................................................................  68

View Details of Associated Profiles and Open Profiles Pages from Redwood Job or Position Pages ........................  69

Create a Position Profile .............................................................................................................................................................  70

Associate Action Reasons in Position with Role ...................................................................................................................   70

How FTE is Calculated in Positions ..........................................................................................................................................   71

Work Hours and Duration ..........................................................................................................................................................   72

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Workday Information Defaults ..................................................................................................................................................   73

How You Match Position Valid Grades with Job Grades .....................................................................................................   75

Position Budgeting .......................................................................................................................................................................  75

Position Costing for Redwood Positions Pages ....................................................................................................................   75

Position Synchronization ............................................................................................................................................................  76

Set Up Position Synchronization ..............................................................................................................................................   78

How Assignment Values Are Inherited from Position .........................................................................................................   79

How Position Synchronization Impacts Assignments ..........................................................................................................   81

Business Unit and Position in When and Why ......................................................................................................................  82

Position Override in Redwood Employment Processes .......................................................................................................  83

Behavior of Position Override ...................................................................................................................................................  84

Synchronize Assignment Action Reason From Position .....................................................................................................   86

Example of Action Reason Synchronization in Assignments ............................................................................................   87

Synchronize Assignment Flexfields From Position Flexfields ............................................................................................  88

Considerations for Flexfield Mapping in Position Synchronization ..................................................................................  90

Synchronize Person Assignment from Position Process .....................................................................................................   91

HCM Position Hierarchy ..............................................................................................................................................................  92

Graphical Position Hierarchy .....................................................................................................................................................   93

How You Create a Graphical Position Hierarchy ...................................................................................................................   94

Parent Position Isn’t Defaulted for Professional Users ........................................................................................................  98

Considerations for Using Position or Position Hierarchy for Synchronizing Assignment Manager ...........................   98

Filter Managers Using Parent Position Hierarchy .................................................................................................................  99

How You Route Position Approvals .......................................................................................................................................   100

Jobs  Search  .................................................................................................................................................................................     104

Positions Search .........................................................................................................................................................................   105

Upload Workforce Structures Using a Spreadsheet ...........................................................................................................   105

FAQs for Jobs and Positions ...................................................................................................................................................   106

5 Grades

111

Grades, Grade Rates, and Grade Ladders ...............................................................................................................................  111

6 Person Information

113

Person Records ............................................................................................................................................................................   113

Personal Information ..................................................................................................................................................................  122

7 Employment Information

133

List of Values in Employment Processes ...............................................................................................................................  133

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Assignments  ................................................................................................................................................................................     136

Employment Dates .....................................................................................................................................................................   175

Eligible  Jobs  .................................................................................................................................................................................    190

8 Areas of Responsibility

193

How You Assign Areas of Responsibility ...............................................................................................................................  193

Autoprovision Areas of Responsibilities ................................................................................................................................  194

Areas of Responsibility Integration with Work Contacts ...................................................................................................   196

Examples of Setting Scope of Responsibility .......................................................................................................................  196

Areas of Responsibility Templates ..........................................................................................................................................  197

FAQs for Areas of Responsibility ............................................................................................................................................   198

9 Hire and Manage Workers

201

Overview of the Workforce Lifecycle .....................................................................................................................................   201

Employment Processes .............................................................................................................................................................   201

Hire  People  ..................................................................................................................................................................................     203

Promote and Transfer People ..................................................................................................................................................   219

Employment Contracts .............................................................................................................................................................   246

Add and Reassign Direct Reports ...........................................................................................................................................   251

Terminate Work Relationships ................................................................................................................................................   256

10 Seniority Dates

269

Overview of Seniority Dates ....................................................................................................................................................  269

Seniority Dates ............................................................................................................................................................................  272

Adjust a Seniority Date .............................................................................................................................................................   272

Examples of Calculating Seniority Dates ..............................................................................................................................   273

How Cumulative Seniority Dates Are Calculated ................................................................................................................  276

Examples of Calculating Cumulative and Noncumulative Seniority Dates ...................................................................   278

Hours-Based Seniority Calculation ........................................................................................................................................   283

Examples of Calculating Hours-Based Seniority ................................................................................................................   283

Process to Calculate Seniority Dates .....................................................................................................................................   285

V1 Seniority Dates ......................................................................................................................................................................   287

11 Document Records

291

Overview of Document Records ..............................................................................................................................................  291

How You Scan Attachment to Prefill Document Record Attributes ................................................................................   292

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Mass Download Document Records ......................................................................................................................................  293

Archive and Purge Document Records .................................................................................................................................  296

Change Publish Date for Document Records ......................................................................................................................   297

Sources of Creating Document Records ..............................................................................................................................   298

Preview Document Records ....................................................................................................................................................   298

Audit Access to Document Records Pages ..........................................................................................................................  299

FAQs for Document Records ..................................................................................................................................................   300

12 Workforce Records

303

Overview of Workforce Records .............................................................................................................................................   303

Directory and Person Spotlight ..............................................................................................................................................   303

Connections  .................................................................................................................................................................................     317

Activity Centers ...........................................................................................................................................................................   321

Mass  Updates  ..............................................................................................................................................................................    323

Work Schedules ..........................................................................................................................................................................   327

13 Workforce Deployment Analysis

331

Generate Workforce Deployment Intelligence ......................................................................................................................   331

FAQs for Evaluate Workforce Deployment Performance ..................................................................................................   338

14 HR Help Desk Service Requests Classic

341

HR Help Desk Classic Documentation ...................................................................................................................................  341

15 Troubleshooting

343

Reverse a Termination ..............................................................................................................................................................   343

How do I unlock a worker’s employment record? ..............................................................................................................   343

Oracle Fusion Cloud Human Resources
Using Global Human Resources

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
Using Global Human Resources

Get Help

ii

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 1
Introduction to Global Human Resources

1  Introduction to Global Human Resources

Overview of Using Global Human Resources

This overview outlines the tasks you can do through the workforce deployment cycle, from setting up workforce
structures, creating and maintaining person records, hiring and managing your workforce to analyzing the workforce
deployment.

Set Up Workforce Structures
You set up basic workforce structures such as divisions, departments, jobs, positions, and grades to manage your
workforce. You can revise the initial setup of your enterprise if you want to add more workforce structures to your
enterprise.

Create and Maintain Person Records
If you're an HR specialist, you can create person records, maintain user accounts, and hire people. Managers can
manage their teams, promote, transfer, and terminate their direct reports. As a worker, you can manage your personal
information, give feedback to coworkers, and report time off.

Hire and Manage Your Workforce
You can get new hires onboard, manage their employment cycle within the enterprise, associate employment contracts
with assignments, and award compensation.

1

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 1
Introduction to Global Human Resources

Analyze Workforce Deployment
You can view statistical and employment-related information for your workforce and generate reports in OTBI and
deliver the reports using dashboards, Infolets, or email.

Quick Actions

Quick actions are links on the Home page that enable you to initiate actions quickly on yourself, your team, or your
client groups. You can view the quick actions grouped under the following tabs:

• Me - This tab lists actions to manage your own information.

• My Team - This tab lists actions to manage your team.

• My Client Groups - This tab lists actions to manage people within your area of responsibility.

Click the Show More link to view all the available actions grouped under a specific head.

The set of actions that you see are displayed based on your security privileges. The people that you can act on differ
based on the tab you're on. Consider that you're both a line manager and an HR Specialist. You can access the Promote
action from both the tabs: My Team and My Client Groups. Also, you will see a different set of employees on each tab
whom you can promote. You can promote only your direct reports using the Promote task in the My Team tab. You can
promote only those employees that you have access to as an HR Specialist, using the Promote task in the My Client
Groups tab.

Related Topics

• Create and Edit Quick Actions

FAQs

Why can't I see some quick actions on landing pages after an
upgrade?

These responsive landing pages are redesigned:

• Absences

• Career Development

• Compensation

• Data Exchange

• Goals

• Mass Updates

• New Person

• Performance

2

Oracle Fusion Cloud Human Resources
Using Global Human Resources

• Profiles

• Workforce Structures

Chapter 1
Introduction to Global Human Resources

Quick action tasks available on the My Client Groups tab are also available from the new landing pages as well. If you
don't see a task in the list of quick actions, you won't see it on the landing page and vice-versa. You need to enable the
quick actions to see these tasks in the landing pages. Here are the steps to enable the quick actions.

1. Navigate to Configuration > Sandboxes.
2. Click Create Sandbox.
3. Enter a name and description for the sandbox.
4. Add Structure and any other tools you require.
5. Click Create and Enter.
6. Navigate to Configuration > Structure.
7. Click My Client Groups and then click the Quick Actions tab.
8. Select the quick action you want to configure.
9. Change the Visible or other settings as needed.
10. Click Save and Close.

3

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 1
Introduction to Global Human Resources

4

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 2
Users and Roles

2  Users and Roles

User Management

How You Manage an Incomplete Request for an HCM User
Account

This topic describes the Process User Account Request action, which may appear on the Manage User Account page for
users who have no user account.

The Process User Account Request Action
The Process User Account Request action is available when the status of the worker's user account is either
Requested or Failed. These values indicate that the account request hasn't completed.

Selecting this action submits the request again. Once the request completes successfully, the account becomes
available to the user. Depending on your enterprise setup, the user may receive an email containing the user name and
password.

Role Provisioning
Any roles that the user will have appear in the Roles section of the Manage User Account page. You can add or remove
roles before selecting the Process User Account Request action. If you make changes to roles, then you must click
Save.

The Send Pending LDAP Requests Process
The Process User Account Request action has the same effect as the Send Pending LDAP Requests process. If Send
Pending LDAP Requests runs automatically at intervals, then you can wait for that process to run if you prefer. Using
the Process User Account Request action, you can submit user account requests immediately for individual workers.

User Names

By default, user names are generated automatically in the format specified for the default user category when you
create a person record. Users who have the human resource specialist (HR specialist) role can change user names for
existing HCM users.

This topic describes the automatic generation of user names and explains how to change an existing user name.

User Names When Creating Users
You create an HCM user by selecting a task, such as Hire an Employee, in the New Person work area. The user name is
generated automatically in the format specified for the default user category. This table summarizes the effects of the
available formats for Oracle Fusion Cloud HCM users.

5

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 2
Users and Roles

User-Name Format

Description

Email

The worker's work email is the user name. If you don't enter the work email when hiring the worker,
 then it can be entered later on the Security Console. This format is used by default. A different default
format can be selected on the Security Console.

FirstName.LastName

The user name is the worker's first and last names separated by a single period.

FLastName

The user name is the worker's last name prefixed with the initial of the worker's first name.

Person number

If your enterprise uses manual numbering, then any number that you enter becomes the user name.
Otherwise, the number is generated automatically and you can't edit it. The automatically generated
number becomes the user name.

Note:  If the default user-name rule fails, then a system user name can be generated. The option to generate a system
user name is enabled by default but you can disable it on the Security Console.

Existing User Names
HR specialists can change an existing user name on the Manage User Account page.

To change a worker's user name:

1. On the My Client Groups tab, find and select the Manage User Account quick action. You may have to click

Show More if it is not visible by default. Line Managers can use the quick action on the My Team tab.

2. Search for and select the worker.
3. On the Manage User Account page, select Actions > Edit User Name.
4. Select Actions >

The updated name, which can be in any format, is sent automatically to your Identity Store. The maximum length of the
user name is 80 characters.

Tip:  When you change an existing user name, the user's password and roles remain the same. However, the user
receives no automatic notification of the change. Therefore, you're recommended to send details of the updated user
name to the user.

FAQs for User Management

What happens if I reset a user's password?
A notification containing a reset-password link is sent to the user's work email. If the user has no work email, then the
notification is sent to the user's line manager. Notification templates for this event must exist and be enabled.

How can I reset a user's password?
If you're a human resource specialist, then you can reset a user's password by selecting Actions Reset Password on the
Manage User Account page.

6

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 2
Users and Roles

You must have security access to the person whose password you want to reset.

How can I notify users of their user names and passwords?
You can run the Send User Name and Password Email Notifications process in the Scheduled Processes work area. For
users for whom you haven't so far requested an email, this process sends out user names and reset-password links.

The email goes to the work email of the user or the user's line manager. You can send the user name and password
once only to any user. A notification template for this event must exist and be enabled.

Where do default user names come from?
User names are generated automatically in the format specified on the Security Console for the user category. The
default format is the worker's primary work email, but you can override this value for each user category.

For example, your enterprise may use person number as the default user name for the default user category.

What happens when I link a user account?
The request to link the person or party record to the account goes automatically to your LDAP directory. Once the
account status is Active, current roles appear in the Roles section of the Manage User Account or Edit User page.

At this point, the user can sign in. You're recommended to notify the user when the account is linked.

How can I create a user account for an existing worker?
On the Manage User Account page, select Create User Account. Update account details, if appropriate, and click Save.
Once the request is processed successfully, the account becomes available.

If automatic creation of accounts is disabled, then you can't use the Create User Account action. Instead, authorized
users can create user accounts on the Security Console.

What happens if I edit a user name?
The updated user name is sent to your LDAP directory for processing when you click Save on the Manage User Account
or Edit User page. The account status remains Active, and the user's roles and password are unaffected.

As the user isn't notified automatically of the change, you're recommended to notify the user. Only human resource
specialists can edit user names.

What happens when I copy personal data to Identity Store?
User accounts are defined in your Identity Store. The Identity Store also holds some personal information about users,
such as name, work phone, and work location address. Changes to personal information in Oracle HCM Cloud are
copied automatically at intervals to your Identity Store.

Why does this worker have no user account?
Automatic creation of user accounts may be disabled in your enterprise. In this case, your enterprise may be managing
user accounts outside Oracle HCM Cloud.

You can link such an account to the worker's person record on the Manage User Account, Create User, or Edit User
page.

7

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 2
Users and Roles

Role Management

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

8

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 2
Users and Roles

The user who's terminating a work relationship specifies when the user loses roles. Deprovisioning can occur:

• On the termination date

• On the day after the termination date

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

FAQs for Role Management

What's the provisioning method?
The provisioning method identifies how the user acquired the role. This table describes its values.

Provisioning Method

Meaning

Automatic

The user qualifies for the role automatically based on his or her assignment attribute values.

Manual

External

Either another user assigned the role to the user, or the user requested the role.

The user acquired the role outside Oracle Applications Cloud.

9

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 2
Users and Roles

Why did some roles appear automatically?
In a role mapping:

• The conditions specified for the role match the user's assignment attributes, such as job.

• The role has the Autoprovision option selected.

Why can't I see the roles that I want to assign to a user?
You can see the roles that you want to assign, if the role satisfies all of the following conditions:

• A role mapping exists for the role. For more information on creating a role mapping, see the topic Create a Role

Mapping.

• The Requestable option is selected for the role in the role mapping. For more information, see the topic How do

I provision HCM data roles to users?.

• At least one of your assignments satisfies the role-mapping conditions.

Why can't I see the roles that I want to request for myself?
Before you can request a role:

• The role must appear in a role mapping where it's Self-requestable.

• At least one of your assignments must match all conditions, such as job and location, in the role mapping.

Typically, an application administrator or IT security manager creates and maintains role mappings.

What happens if I deprovision a role from a user?
The user loses the access to functions and data that the removed role was providing exclusively. The user becomes
aware of the change when he or she next signs in.

If the user acquired the role automatically, then future updates to the user's assignments may mean that the user
acquires the role again.

Why is the user losing roles automatically?
The user acquired these roles automatically based on his or her assignment information. Changes to the user's
assignments mean that the user is no longer eligible for these roles. Therefore, the roles no longer appear.

If a deprovisioned role is one that you can provision manually to users, then you can reassign the role to the user, if
appropriate.

What happens when I autoprovision roles for a user?
The role-provisioning process reviews the user's assignments against all current role mappings.

The user immediately:

• Acquires any role for which he or she qualifies but doesn't have

• Loses any role for which he or she no longer qualifies

You're recommended to autoprovision roles to individual users on the Manage User Account page when new or
changed role mappings exist. Otherwise, no automatic updating of roles occurs until you next update the user's
assignments.

10

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 2
Users and Roles

What happens if I delegate a role?
The proxy user to whom you delegate the role can perform your tasks on your data. For example, you may be a line
manager who manages the absence records of reports. If you delegate the line manager role, then the proxy user can

You don't lose the role while it's delegated.

Can I delegate any role?
No. You can delegate any role that you either have currently or can provision to other users. Also, delegation must be
allowed for the role. Not all roles are enabled for delegation.

What happens if I delegate approvals?
Approval notifications for tasks in the selected category go automatically to the selected worker during the specified
period. That worker approves transactions, for example, in your place. You don't receive approval notifications for the
task category while approvals are delegated.

You may want to delegate approvals if you're also delegating a role in which you approve transactions. However, you can
delegate roles and approvals independently of each other.

You now have an option to restrict or allow the person who is being delegated to, to approve their own transactions. You
can enable this feature by selecting the checkbox Allow this user to approve their own transaction on the Approval
Delegations page.

What's a delegated role?
A job, abstract, or data role that a user, known as the delegator, assigns to another user, known as the proxy user.

You can delegate a role either for a specified period, such as a planned absence, or indefinitely.

11

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 2
Users and Roles

12

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

3  Departments, Divisions, Organizations,
Locations, and Worker Unions

Overview of Workforce Structures

You can review and revise the initial setup if there are changes in your enterprise structure. As a part of this activity,
you can add or revise workforce structures. For example, you may add new departments, create jobs, or revise rates for
grades.

You add and edit workforce structures using the Workforce Structures work area.

• Departments

• Divisions

• Disability organizations

• Organization trees

• Department trees

• Position trees

• Locations

• Jobs

• Positions

• Grades

• Grade rates

• Grade ladders

Although you create payroll statutory units, legal employers, and tax reporting units from the Manage Legal Entity task
in the Setup and Maintenance work area, you can revise them using the Manage Legal Entity HCM Information task in
the Workforce Structures work area.

Related Topics

• How do I default the effective start date on Redwood workforce structures pages?

List of Values in Workforce Structures

List of Values (LoVs) in workforce structures can be filtered based on certain criteria and are formatted on certain
parameters.

For the departments, job families, jobs and locations Redwood pages, the LOVs are displayed in a column format,
which can be sorted. They’re filtered based on additional attributes such as user roles, effective start date, and so on as
applicable.

13

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

List of Values on the Department Pages
This table lists the LoVs on the department pages, along with the formatting (querying attributes) and the filtering
criteria for each.

LoV

Action Reason

Format

• Name

• Code

Filtering Criteria

• Department Effective Start Date

• User roles

• Profile option -

PER_LOV_SEARCH_ACTIONREASONS_STARTSWITH

Status (Active/Inactive)

• Meaning

• Department Effective Start Date

Department Set

Location

• Name

• Code

• Name

• Code

• City or Town

• Country

None

• Department Effective Start Date

• Status (Active/Inactive)

List of Values on the Disability Organization Pages
This table lists the LoVs on the disability organization pages, along with the formatting (querying attributes) and the
filtering criteria for each.

LoV

Action Reason

Format

• Name

• Code

Filtering Criteria

• Disability Organization Effective Start Date

• Status (Active/Inactive)

• Action

• User roles

• Profile option -

PER_LOV_SEARCH_ACTIONREASONS_STARTSWITH

Status (Active/Inactive)

• Meaning

• Disability Organization Effective Start Date

Location

• Name

• Code

• City or Town

• Country

• Disability Organization Effective Start Date

• Status (Active/Inactive)

14

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

List of Values on the Division Pages
This table lists the LoVs on the division pages, along with the formatting (querying attributes) and the filtering criteria
for each.

LoV

Action Reason

Format

• Name

• Code

Filtering Criteria

• Division Effective Start Date

• Status (Active/Inactive)

• Action

• User roles

• Profile option -

PER_LOV_SEARCH_ACTIONREASONS_STARTSWITH

Status (Active/Inactive)

• Meaning

• Division Effective Start Date

Location

• Name

• Code

• City or Town

• Country

• Division Effective Start Date

• Status (Active/Inactive)

List of Values on the Enterprise HCM Information Pages
This table lists the LoVs on the Enterprise HCM Information pages, along with the formatting (querying attributes) and
the filtering criteria for each.

LoV

Action Reason

Format

• Name

• Code

Filtering Criteria

• Enterprise Effective Start Date

• Status (Active/Inactive)

• Action

• User roles

• Profile option -

PER_LOV_SEARCH_ACTIONREASONS_STARTSWITH

Status (Active/Inactive)

• Meaning

• Enterprise Effective Start Date

Location

• Name

• Code

• City or Town

• Country

• Enterprise Effective Start Date

• Status (Active/Inactive)

15

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

List of Values on the Job Family Pages
This table lists the LoVs on the job family pages, along with the formatting (querying attributes) and the filtering criteria
for each.

LoV

Action Reason

Format

• Name

• Code

Filtering Criteria

•

Job Family Effective Start Date

• User roles

• Profile option -

PER_LOV_SEARCH_ACTIONREASONS_STARTSWITH

Status (Active/Inactive)

• Meaning

•

Job Family Effective Start Date

List of Values on the Job Pages
This table lists the LoVs on the job pages, along with the formatting (querying attributes) and the filtering criteria for
each.

LoV

Action Reason

Format

• Name

• Code

Filtering Criteria

•

Job Effective Start Date

• User roles

• Profile option -

PER_LOV_SEARCH_ACTIONREASONS_STARTSWITH

Status (Active/Inactive)

• Meaning

•

Job Effective Start Date

Job Set

Job Family

Full time or Part time

Job Function

Regular or Temporary

Management Level

Scheduling Group

Progression Job

• Name

• Code

• Name

• Code

• Meaning

• Meaning

• Meaning

• Meaning

• Meaning

• Name

• Code

• Family

None

•

Job Effective Start Date

• Status (Active/Inactive)

•

•

•

•

•

•

Job Effective Start Date

Job Effective Start Date

Job Effective Start Date

Job Effective Start Date

Job Effective Start Date

Job Effective Start Date

• Status (Active/Inactive)

16

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Format

Filtering Criteria

LoV

Benchmark Job

Requisition Template

• Name

• Code

• Family

• Name

• Code

Frequency

• Meaning

Annual working duration units

• Meaning

Grade Ladder

Valid Grades

• Name

• Type

• Name

• Code

• Set Name

•

Job Effective Start Date

• Status (Active/Inactive)

• Benchmark Flag

None

•

•

•

Job Effective Start Date

Job Effective Start Date

Job Effective Start Date

• Status (Active/Inactive)

•

Job Effective Start Date

• Status (Active/Inactive)

• Set of the Job

List of Values on the Legislative Data Group Pages
This table lists the LoVs on the legislative data group pages, along with the formatting (querying attributes) and the
filtering criteria for each.

LoV

Country

Currency

Cost Structure Allocation

Format

Filtering Criteria

• Flag

• Code

• Name

• Name

• Name

Worker Union Effective Start Date

None

None

List of Values on the Location Pages
This table lists the LoVs on the location pages, along with the formatting (querying attributes) and the filtering criteria
for each.

LoV

Action Reason

Format

• Name

• Code

Filtering Criteria

• Location Effective Start Date

• User roles

17

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

LoV

Format

Status (Active/Inactive)

Location Set

Frequency

Designated Receiver

Inventory Organization

Ship to location

Timezone

• Meaning

• Name

• Meaning

• Name

• Business Title

• Work Email

• Person Number

• Status

• Name

• Name

• Code

• City or Town

• Country

• Timezone Code

• Timezone

Official Language

• Meaning

Filtering Criteria

• Profile option -

PER_LOV_SEARCH_ACTIONREASONS_STARTSWITH

• Location Effective Start Date

None

• Location Effective Start Date

• Location Effective Start Date

None

• Ship-to-site as "No"

None

None

List of Values on the Reporting Establishment Pages
This table lists the LoVs on the reporting establishment pages, along with the formatting (querying attributes) and the
filtering criteria for each.

LoV

Action Reason

Format

• Name

• Code

Filtering Criteria

• Reporting Establishment Effective Start

Date

• Status (Active/Inactive)

• Action

• User roles

• Profile option -

PER_LOV_SEARCH_ACTIONREASONS_STARTSWITH

Status (Active/Inactive)

• Meaning

• Reporting Establishment Effective Start

Date

18

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

LoV

Location

Format

• Name

• Code

• City or Town

• Country

Filtering Criteria

• Reporting Establishment Effective Start

Date

• Status (Active/Inactive)

List of Values on the Worker Union Pages
This table lists the LoVs on the worker union pages, along with the formatting (querying attributes) and the filtering
criteria for each.

LoV

Action Reason

Format

• Name

• Code

Filtering Criteria

• Worker Union Effective Start Date

• Status (Active/Inactive)

• Action

• User roles

• Profile option -

PER_LOV_SEARCH_ACTIONREASONS_STARTSWITH

Status (Active/Inactive)

• Meaning

• Worker Union Effective Start Date

Location

Country

• Name

• Code

• City or Town

• Country

• Flag

• Code

• Name

• Worker Union Effective Start Date

• Status (Active/Inactive)

• Worker Union Effective Start Date

Departments, Divisions, and Organizations

Guidelines for Using Single or Multiple Classifications for an
Organization

Organization classifications define the purpose of the organization, whether it's a department, a division, or a legal
entity. In some enterprises, organization classifications overlap, which means that the same organization can be
assigned multiple classifications.

19

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

For example, one organization within an enterprise might be both a project organization and a department. The
classifications of organizations vary according to business objectives, legal structure, industry, company culture, size
and type of growth. You can create organizations in Oracle Fusion with one or more classifications to reflect your
enterprise structure.

Defining an Organization with One Classification
Define each organization in your enterprise as a separate organization with a single classification to reflect your
enterprise structure and provide flexibility for expansion. The advantage of setting up separate organizations is the
ability to add further organizations to expand the enterprise easily. For example, if your enterprise acquires another
company which has a different line of business in a country in which you employ people, you can create a division, a
legal entity, and additional departments. Classify the new legal entity as a legal employer and payroll statutory unit for
the company's payroll tax and social insurance.

Defining an Organization with Multiple Classifications
Define an organization with multiple classifications if the organization has multiple purposes. For example, use an
organization within the sales applications as a department that employs salespeople and classify it as a department and
a sales organization. Or, if your enterprise operates and employs people in multiple business verticals, create a division
for each such business using the Manage Divisions task. Then use the Manage Departments task to classify the division
as a department.

Related Topics

• Model Your Financial Reporting Structure

How You Configure Your Enterprise Structure After an Acquisition

The InFusion Corporation is a global company with organizations in the United States (US), the United Kingdom (UK),
France, China, Saudi Arabia, and the United Arab Emirates (UAE).

Its main area of business is in the high tech industry, but it recently acquired a financial services business, based in
Germany. InFusion wants to retain the financial services company as a separate business with all the costs and reporting
managed by the Financial Services division.

You need to set up organizations to reflect the newly acquired company and its organizations.

20

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

The following figure illustrates how to set up the new division for Germany, and how the new division fits into the

enterprise.
The following table summarizes the key decisions for setting up the new division:

Decisions to Consider

In This Example

Create a separate division?

Yes, as you want to keep the Financial Services company as a separate line of business. By creating a
separate division, you can manage the costs and reporting separately from the InFusion Corporation.
Additionally, you don't have to modify any existing organizations in your enterprise setup.

How many departments?

The Financial Services company currently has three departments for sales, accounting, and marketing.
As InFusion has no plans to downsize or change the company, you can create the three departments to
retain the structure.

How many cost centers?

Three, to track the costs of each department.

How many legal entities?

You need one legal entity defined as a legal employer and payroll statutory unit. As the new division
operates only from Germany, you can configure the legal entity to suit Germany's legal and statutory
requirements.

21

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Decisions to Consider

In This Example

Create legislative data group?

Yes, you need a legislative data group as you currently don't employ or pay people in Germany. Create
one legislative data group to run payroll for your workers in Germany.

Create location?

Create a new location address for each organization located differently. The financial services company
is based in Frankfurt, and the headquarters and departments are all in the same location.

You can use the following tasks to set up the enterprise structures that you need to include in the new Financial Services
company:

• Creating a Location

• Creating a Division

• Creating Departments

• Creating a Legislative Data Group

• Creating Legal Entities

• Defining Legal Employer and Payroll Statutory Unit Information

Creating a Location

In the Workforce Structures work area, click the Manage Locations tab to open the Manage Locations page.

1.
2. On the Manage Locations page, click Create, and complete the fields shown in the following table. Use the

default values except where indicated.

Field

Name

Code

Value

Germany

DE

Country

Germany

Address Line 1

Hauptstrasse 85

Postal Code

6000

City

Frankfurt

3. Click Submit.

Creating a Division

In the Workforce Structures work area, click Manage Divisions to open the Manage Divisions page.

1.
2. On the Manage Divisions page, click Create.

22

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

3. On the Create Division: Division Description page, select the Create New option to create a division with a

4.

single classification.
In the Division Description region, complete the fields shown in the following table. Use the default values
except where indicated.

Field

Name

Value

Germany Financial Services

Location

Germany

5. Click Next.
6. On the Create Division: Division Details page, complete the fields shown in the following table. Use the

default values except where indicated.

7. Click Next.
8. On the Create Division: Review page, review the division details, and click Submit.
9. Click Yes.
10. Click OK.

Creating Departments

1.

In the Workforce Structures work area, click the Manage Departments tab to open the Manage Department
page.

2. On the Manage Departments page, click Create.
3. On the Create Department: Description page, select the Create New option to create a department with a

single classification.

4. Enter the details of the accounting department by completing the fields shown in the following table. Use the

default values except where indicated.

Field

Value

Department Name

Accounting

Location

Germany

5. Click Next.
6. Associate a cost center in the Create Department: Department Details page.
7. Click Next.
8. On the Create Department: Review page, review the details of the department, and click Submit.
9. Repeat steps 2 through 8 to create the sales and marketing departments.

Creating a Legislative Data Group

1.

In the Setup and Maintenance work area, locate the Manage Legislative Data Groups task. Click Go to Task
to open the Manage Legislative Data Group page.

2. On the Manage Legislative Data Groups page, click Create.
3. On the Create Legislative Data Groups page, complete the fields shown in the following table. Use default

values except where indicated.

23

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Field

Name

Value

Germany Financial Services

Country

Germany

Currency

Eur

4. Click Submit.

Creating Legal Entities

1.

In the Setup and Maintenance work area, locate the Manage Legal Entity task. Click Go to Task to open the
Manage Legal Entity page.

2. On the Manage Legal Entity page, click Create.
3. On the page, complete the fields shown in the following table. Use default values except where indicated.

Field

Name

Value

Legal Entity

Legal Entity Identifier

123456

Payroll Statutory Unit

Selected

Legal Employer

Selected

Legal Address

EIN or TIN

Registration Number

123

123

123

4. Click Save and Close.

Defining Legal Employer and Payroll Statutory Unit Information

1.

In the Setup and Maintenance work area, locate the Manage Legal Entity HCM Information task. Click Go to
Task to open the Manage Legal Entity page.

2. Search for the new legal entity that you created in the "Creating Legal Entities" task.
3. Enter the payroll statutory unit and legal employer details.

24

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

4. Associate the legislative data group with the payroll statutory unit.
5. Click Save.

Related Topics

• How do I default the effective start date on Redwood workforce structures pages?

Divisions

Managing multiple businesses requires that you segregate them by their strategic objectives and measure their results.

Responsibility to reach objectives can be delegated along the management structure. Although related to your legal
structure, the business organizational hierarchies don't reflect directly the legal structure of the enterprise. The
management entities and structure can include:

• Divisions and subdivisions

• Lines of business

• Other strategic business units

• Their own revenue and cost centers

These organizations can be included in many alternative hierarchies and used for reporting, as long as they have
representation in the chart of accounts.

Divisions
A division refers to a business-oriented subdivision within an enterprise, in which each division organizes itself
differently to deliver products and services or address different markets. A division can operate in one or more
countries, and can be many companies or parts of different companies that are represented by business units.

A division is a profit center or grouping of profit and cost centers, where the division manager is responsible for
achieving business goals including profits. A division can be responsible for a share of the company's existing product
lines or for a separate business. Managers of divisions may also have return on investment goals requiring tracking of
the assets and liabilities of the division. The division manager generally reports to a corporate executive.

By definition a division can be represented in the chart of accounts. Companies can use product lines, brands, or
geographies as their divisions: their choice represents the primary organizing principle of the enterprise.

Historically, divisions were implemented as a node in a hierarchy of segment values. For example, Oracle E-Business
Suite has only one balancing segment, and often the division and legal entity are combined into a single segment where
each value stands for both division and legal entity.

Use of Divisions in Oracle Fusion Cloud Human Capital Management (HCM)
Divisions are used in HCM to define the management organization hierarchy, using the generic organization hierarchy.
This hierarchy can be used to create organization-based security profiles.

Related Topics

• Can I view the address details of the location on the Redwood pages for organizations?

• Can I select an existing organization when I'm creating a new organization in Redwood?

• Can I view the Other Classifications section on the Redwood pages for organizations?

25

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Example of Adding a New Division After Acquiring a Company

This example describes how you can restructure your enterprise after acquiring a new division.

Scenario
You are part of a senior management team at InFusion Corporation. InFusion is a global company with organizations in
the following countries:

• United States (US)

• United Kingdom (UK)

• France

• China

• Saudi Arabia

• United Arab Emirates (UAE)

The company's main area of business is in the high tech industry, and it recently acquired a new company. You must
analyze the company's current enterprise structure and determine the new organizations to create in the new company.

Details of the Acquired Company
The acquired company is a Financial Services business based in Germany. The Financial Services business differs
significantly from the high tech business. Therefore, you want to keep the Financial Services company as a separate
business with all the costs and reporting managed by the Financial Services division.

The following table summarizes the key decisions that you must consider when determining what new organizations to
set up and how to structure the enterprise.

Decision to Consider

In This Example

Create location?

The Financial Services company and its departments are based in Frankfurt. Therefore, you only have
to create one location.

Create separate division?

Yes. Although the new division will exist in the current enterprise structure, you want to keep the
Financial Services company as a separate line of business. By creating a separate division, you can
manage the costs and reporting separately from the InFusion Corporation. Additionally, you don't have
to modify any organizations in the enterprise setup.

Create business unit?

Yes. The Financial Services business requires you to create several jobs that don't exist in your high
tech business. You can segregate the jobs that are specific to financial services in a new business unit.

How many departments?

The Financial Services company currently has departments for sales, accounting, and marketing. As
you have no plans to downsize or change the company, you can create three departments to retain the
structure.

How many cost centers?

Although you can have multiple cost centers to track the department costs, you decide to create one
cost center for each department.

26

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Decision to Consider

In This Example

How many legal entities?

Define a legal entity for each registered company or some other entity recognized by law. Using the
legal entity, you can:

• Record assets

• Record liabilities

• Record income

• Pay transaction taxes

• Perform intercompany trading

In this case, you only need one legal entity.

You must define the legal entity as a legal employer and payroll statutory unit. As the new division
operates only from Germany, you can configure the legal entity to suit Germany's legal and statutory
requirements.

Note:
You can identify the legal entity as a payroll statutory unit. When you do so, the application transfers
the legal reporting unit associated with the legal entity to Oracle Fusion HCM as a tax reporting unit.

Create legislative data group?

Yes. Because you currently don't employ or pay people in Germany, you must create one legislative
data group to run payroll for the workers in Germany.

Resulting InFusion Enterprise Structure
Based on the analysis, you must create the following:

• One new division

• One new location

• Three new departments

• Three new cost centers

• One new legal entity

• One new legislative data group

27

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

The following figure illustrates the structure of InFusion Corporation after adding the new division and the other

organizations.

Departments

A department is an organization to which you assign workers. It is an organization with one or more operational
objectives or responsibilities that exist independently of its manager.

You track the department's financial performance through one or more cost centers. For example, sales, research and
development, and human resources. You can report and keep track of headcount by creating a department hierarchy
using Oracle Fusion Trees.

Departments and cost centers example:

28

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

This figure illustrates how departments belong to legal entities within the enterprise structure.

Departments and Cost Centers
A cost center represents the smallest segment of an organization for which you allocate and report on costs. The
manager of a department is typically responsible for cost control by meeting a budget and may be responsible for the
assets used by the department. You can track the financial performance of a department through one or more cost
centers.

Uploading Departments Using a Spreadsheet
If you have a list of departments already defined for your enterprise, you can upload them from a spreadsheet. To use
this option, you first download a spreadsheet template, add your department information to the spreadsheet, and
then upload directly to your enterprise configuration. You can upload the spreadsheet multiple times to accommodate
revisions.

Related Topics

• Upload Workforce Structures Using a Spreadsheet

• Can I view the address details of the location on the Redwood pages for organizations?

• Can I select an existing organization when I'm creating a new organization in Redwood?

• Can I view the Other Classifications section on the Redwood pages for organizations?

How You Create a Chart of Account to Create a Department

In this example you can see how to create a chart of account for HCM implementations. You must set up a minimal
chart of account to associate a company and cost center with departments.

29

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

This topic describes a simple scenario primarily intended for use within HCM. For more detailed information on setting
up a chart of account, refer to the Financials product documentation.

Vision Corporation US is a US-based legal entity with cost centers in Arizona and California. In this example, we will
create a Arizona cost center and associate it with the Sales Department.

The following table summarizes key decisions that you must consider when creating a chart of .

Decisions to Consider

In this Example

What should be the validation type for the
value set?

Independent. Only this type is supported for creating General Ledger (GL) cost center information for
departments in HCM.

What should be the segment labels for the
chart of account?

The first segment is Primary Balancing Segment and the second segment is Cost Center Segment.
Selecting these labels in this order is crucial in specifying the General Ledger cost center information
for a department.

Summary of Tasks
In the Setup and Maintenance work area, create a chart of account and cost center value sets to create a chart of
account structure and instance, and then associate it with the department.

1. Create the chart of account value set for the Vision Corporation US enterprise.
2. Specify Arizona and California as the values for the chart of account value set
3. Create the cost center value set for the Vision Corporation US enterprise.
4. Specify Arizona and California as the values for the cost center value set.
5. Create the chart of account structure by associating it with the chart of account and cost center value sets you

created earlier.

6. Create the chart of account structure instance by associating it with the structure.
7. Specify the General Ledger cost center information by associating it with the chart of account and the cost

center you created earlier, for creating the sales department.

Create a Chart of Account Value Set

1.

In the Setup and Maintenance work area, go to the following:.

◦ Offering: Workforce Deployment
◦ Functional Area: Financial Reporting Structures
◦ Task: Manage Chart of Accounts Value Sets

2. Click Create.
3. Complete the fields as shown in this table.

Field

Value

Value Set Code

Vision Corporation US Value Set 1

Description

Vision Corporation US Value Set 1

30

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Field

Module

Value

Common Shared Setups

Validation Type

Independent

Value Data Type

Character

Value Subtype

Maximum Length

Text

5

4. Click Save and Close.

Specify Values for the Chart of Account Value Set

1. On the Manage Chart of Accounts Value Sets page, search and select Vision Corporation US Value Set 1 from

the search results.
2. Click Manage Values.
3. Click Create.
4. Complete the fields as shown in this table.

Field

Value

Value

AZ

Description

Arizona

Enabled

Select the check box

5. Click Save and Close.
6. Create additional values for the Vision Corporation US Value Set 1 as shown in this table.

Field

Value

Value

CA

Description

California

Enabled

Select the check box

31

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

7. On the Manage Values page, click Save and Close.

Create a Cost Center Value Set

1.

In the Setup and Maintenance work area, go to the following:

◦ Offering: Workforce Deployment
◦ Functional Area: Financial Reporting Structures
◦ Task: Manage Chart of Accounts Value Sets

2. Click Create.
3. Complete the fields as shown in this table.

Field

Value

Value Set Code

Vision Corporation US Cost Center Value Set 1

Description

Vision Corporation US Cost Center Value Set 1

Module

Common Shared Setups

Validation Type

Independent

Value Data Type

Character

Value Subtype

Maximum Length

Text

5

4. Click Save and Close.

Create a Chart of Account Structure

1.

In the Setup and Maintenance work area, go to the following:.

◦ Offering: Workforce Deployment
◦ Functional Area: Financial Reporting Structures
◦ Task: Manage Chart of Accounts Structures

2. Search and select the GL# key flexfield code.
3. Click Manage Structures.
4. Click Create.

32

Oracle Fusion Cloud Human Resources
Using Global Human Resources

5. Complete the fields as shown in this table.

Field

Value

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Structure Code

Vision Corp CoA Cost Center

Name

Vision Corp CoA Cost Center

Description

Vision Corporation Chart of Account Cost Center

Delimiter

Select any value

6. Click Save.
7.
In the Segments section, click Create.
8. Complete the fields as shown in this table.

Field

Value

Segment Code

Vision_Corp_COA

API Name

visionCorpCoa

Name

Vision Corporation COA

Sequence Number

1

Prompt

Vision Corporation COA

Short Prompt

Vision

Enabled

Select the check box

Display Width

Range Type

1

Low

Column Name

SEGMENT1

Default Value Set Code

Vision Corporation US Value Set 1

33

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Field

Value

Selected Labels

Primary Balancing Segment

9. Click Save and Close.
10. Create another segment with the following values

Field

Value

Segment Code

Vision_Corp_CostCenter_COA

API Name

visionCorpCostcenterCoa

Name

Vision Corporation Cost Center COA

Sequence Number

2

Prompt

Vision Corporation Cost Center COA

Short Prompt

Vision1

Enabled

Select the check box

Display Width

Range Type

1

Low

Column Name

SEGMENT2

Default Value Set Code

Vision Corporation US Cost Center Value Set 1

Selected Labels

Cost Center Segment

11. Click Save and Close.
12. On the Create Key Flexfield Structure page, click Save and Close.

Create a Chart of Accounts Structure Instance

1.

In the Setup and Maintenance work area, go to the following:

34

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

◦ Offering: Workforce Deployment
◦ Functional Area: Financial Reporting Structures
◦ Task: Manage Chart of Accounts Structure Instances

2. Search and select the GL# key flexfield code.
3. Click Manage Structure Instances.
4. Click Create.
5. Complete the fields as shown in this table.

Field

Value

Structure Instance Code

Vision COA Structure Instance

API name

VisionCoaStructureInstance

Name

Vision Corporation COA Structure Instance

Structure Name

Vision Corp CoA Cost Center

6. Click Save and Close.

Specify the General Ledger Cost Center Information for Creating a Department

In the Workforce Structures work area, click the Manage Departments tab.

1.
2. Click Create.
3. Select the Create new option.
4. Enter Sales Department in the Name field.
5. Click Next.
6.

In the GL Cost Center Information section, complete the fields as shown in this table.

Field

Record Identifier

Value

10

Company Value Set

Vision Corporation US Value Set 1

Company

AZ

Cost Center Value Set

Vision Corporation US Cost Center Value Set 1

Cost Center

AZ

35

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

7. Click Next to review the specified information.
8. Click Submit.

Cost Centers and Departments

The two important components to be considered in designing your enterprise structure are cost centers and
departments.

A cost center represents the smallest segment of an organization for which you collect and report costs. A department
is an organization with one or more operational objectives or responsibilities that exist independently of its manager
and has one or more workers assigned to it.

Cost Centers
A cost center represents the destination or function of an expense rather than the nature of the expense which is
represented by the natural account. For example, a sales cost center indicates that the expense goes to the sales
department.

A cost center is generally attached to a single legal entity. To identify the cost centers within a chart of accounts
structure use one of these two methods:

• Assign a cost center value in the value set for each cost center. For example, assign cost center values of

PL04 and G3J1 to your manufacturing teams in the US and India. These unique cost center values allow easy
aggregation of cost centers in hierarchies (trees) even if the cost centers are in different ledgers. However, this
approach requires defining more cost center values.

• Assign a balancing segment value with a standardized cost center value to create a combination of segment
values to represent the cost center. For example, assign the balancing segment values of 001 and 013 with
cost center PL04 to represent your manufacturing teams in the US and India. This creates 001-PL04 and 013-
PL04 as the cost center reporting values. The cost center value of PL04 has a consistent meaning. This method
requires fewer cost center values to be defined. However, it prevents construction of cost center hierarchies
using trees where only cost center values are used to report results for a single legal entity. You must specify a
balancing segment value in combination with the cost center values to report on a single legal entity.

Departments
A department is an organization with one or more operational objectives or responsibilities that exist independently of
its manager. For example, although the manager may change, the objectives don't change. Departments have one or
more workers assigned to them.

A manager of a department is typically responsible for:

• Controlling costs within their budget

• Tracking assets used by their department

• Managing employees, their assignments, and compensation

The manager of a sales department may also be responsible for meeting the revenue targets.

The financial performance of departments is generally tracked through one or more cost centers. In Oracle Fusion Cloud
Applications, departments are defined and classified as Department organizations. Oracle Fusion Cloud Human Capital
Management (HCM) assigns workers to departments, and tracks the headcount at the departmental level.

36

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

The granularity of cost centers and their relationship to departments varies across implementations. Cost center
and department configuration may be unrelated, identical, or consist of many cost centers tracking the costs of one
department.

Department Classifications

A department can be classified as a project organization, sales and marketing organization, or cost organization.

A point to note is that a department name must be unique. This rule applies even when the department is classified as
a project organization or an inventory organization. For example, if you create a department with name Vision Corp.
Sales, you can't create another department with the same name. Also, if you classify this department as a project
organization, you can't create another project organization as well with the same name.

Or, if you create a division with the name Vision Corp. Marketing that is classified as a department, which in turn is
classified as a project organization, you can't create another division, department or project organization with the same
name.

Oracle Fusion Cloud Human Capital Management (HCM) uses trees to model organization hierarchies. It provides
predefined tree structures for department and other organizational hierarchies that can include organizations with any
classification.

Project Organization
Classify departments as a project owning organization to enable associating them with projects or tasks. The project
association is one of the key drivers for project access security.

In addition, you must classify departments as project expenditure organizations to enable associating them to project
expenditure items. Both project owning organizations and project expenditure organizations can be used by Oracle
Subledger Accounting to derive accounts for posting Oracle Fusion Cloud Project Management accounting entries to
Oracle General Ledger.

Sales and Marketing Organization
In sales applications, you can define sales and marketing organizations. Sales organization hierarchies are used to
report and forecast sales results. Salespeople are defined as resources assigned to these organizations.

In some enterprises, the HCM departments and hierarchies correspond to sales organizations and hierarchies.
Examining the decision on how to model sales hierarchies in relationship to department hierarchies when implementing
Customer Relationship Management to eliminate any possible redundancy in the definition of the organizations is
important.

The following figure illustrates a management hierarchy, in which the System Components Division tracks its
expenses in two cost centers, Air Compressors and Air Transmission. At the department level, two organizations with a
classification of Department are defined, the Marketing Department and Sales Department. These two departments can
be also identified as a Resource Organizations, which enable assigning resources, such as salespeople, and other sales
specific information to them. Each department is represented in the chart of accounts by more than one cost center,
enabling granular as well as hierarchical reporting.

37

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Cost Organization
Oracle Project Costing uses a cost organization to represent a single physical inventory facility or group of inventory
storage centers, for example, inventory organizations. This cost organization can roll up to a manager with responsibility
for the cost center in the financial reports.

A cost organization can represent a costing department. Consider this relationship when determining the setup of
departments in HCM. No system dependencies are required for these two entities, cost organization and costing
department, to be set up in the same way.

How You Configure the Department Title

The Title field for a department is hidden and optional, by default. You need to do these 2 steps to enable the field and
make it mandatory.

Enable Title Field
These are the steps to set the value of the profile option ORA_PER_ENABLE_DEPARTMENT_TITLE to Y.

1. Navigate to the Setup and Maintenance work area.
2. Search for and click the Manage Administrator Profile Values task.
3. Search for the ORA_PER_ENABLE_DEPARTMENT_TITLE profile option code and select the profile option in

the search results.
In the Profile Values section, enter Y in the Profile Value field.

4.
5. Click Save and Close.

Once you set the profile option value to Y, you can see the Title field in all the department pages, including Create,
Update, Correct, and Review pages.

38

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Note:  On the Redwood department pages, the Title field appears by default and it's not controlled by the profile
option.

Here's how the Department Title is displayed in the Departments LoV:

• On the Redwood Employment flows, the Department Title is displayed in the Departments LoV by default.

• On the responsive Employment flows, the Department Title isn’t displayed in the Departments LoV by default.
Use the Search Configuration option in the HCM Experience Design Studio to enable the Department Title in
the Departments LoV.

Make Title Field Mandatory
Prerequisite Tasks:

1. Create a sandbox and add the Page Composer tool.
2. Create a department from the Workforce Structures work area on the My Client Groups tab.

Do these steps to make the title field mandatory:

1. Click Edit Pages from the Settings and Actions menu.
2. Click Structure and place your cursor in the Title field.
3. Click Edit in the Confirm Shared Component Edit window.
4. Search for InputText:Title in the component list and click the Edit icon.
5. Scroll down to the Required field in the Edit Properties window and click the down arrow.
6. Select Expression Builder.
7. Add the #{pageFlowScope.makeTitleMandatory eq 'Y'} condition in the expression editor.
8. Click OK.
9. Scroll down to the Show Required field in the Edit Properties window and click the down arrow.
10. Select Expression Builder.
11. Add the #{pageFlowScope.makeTitleMandatory eq 'Y'} condition in the expression editor.
12. Click OK.

Associate Legal Employers with a Department

You can now associate multiple legal employers with a department using the Legal Employers That Share This
Department extensible flexfield (EFF) context. If you have enabled Oracle Search for Departments LoV, this will help in
filtering the departments based on the selected legal employer, on pages that will implement this feature in the future.

Here are some key points to note:

• You can associate multiple legal employers with a department, but you can't associate the same legal employer

twice with the same department.

• You can associate the same legal employer with different departments.

• You can delete the legal employer - department association.

• This legal employer - department mapping is copied when you duplicate a department.

• You can associate legal employers when creating, updating, or correcting a department.

• The legal employer list of values will display all active and inactive legal employers configured. There isn't any

filtering for only active legal employers.

39

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

• Legal employers are listed in the ascending order of legal employer name.

• A department must have at least one associated legal employer, for the department to be filtered based on a

legal employer.

• You can associate departments with legal employers using classic Manage Department page but you can use

the department filtering only on Redwood pages because this feature is delivered for REST LOVs only.

• You can also use HCM Data Loader (HDL) to associate legal employers with a department.

• The department - legal employer association is also migrated when you migrate your Department

configuration using the Functional Setup Manager (FSM) export/import functionality.

• An extra parameter is added on the REST departmentsLovV2 as follows:

◦ LegalEmployerId in findByWord finder.

•

If you have enabled Oracle Search for Departments LoV, only pages that have implemented this feature will
demonstrate this additional filtering.

In this example, Vision Enterprise has 3 legal employers: Vision Corporation, Vision US, and Vision Consulting,
associated with multiple departments in the US. You want to filter departments associated with Vision Corporation.

Let's look at the steps to update this association.

Associate Vision Corporation with the Administrative Computing Department

1. Go to My Client Groups > Quick Actions > Workforce Structures.
2. Click the Manage Departments task.
3.
4. On the Create Department page, in the Department Details section, enter the required details to create a

In the Manage Departments page, click +Create.

department.

Field

Effective Start Date

Name

Title

Value

8/25/21

Administrative Computing

Admin Computing

5.

In the Organization Information EFF: Department Details section, click Add in the Legal Employers That Share
This Department section to associate the Vision Corporation legal employer with this department.

6. Select Vision Corporation from the Legal Employer list.

Note:  As a prerequisite, the legal employer must already exist.

7. Click OK.
8. Click Submit.

Related Topics

• Departments

• Configure Extensible Flexfields

• Guidelines for Loading Organizations

• Departments List of Values V2

• Extending HCM Redwood Applications Using Visual Builder Studio

40

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Disability Organizations

You can set up disability organizations to identify the external organizations with which disabled employees are
registered, and assess the degree of disability in the employee.

You set up disability organizations using the Manage Disability Organizations task in the Workforce Structures work area
under My Client Groups.

Purpose of Disability Organizations
Disability organizations provide information and support to people with disabilities, for example, the Royal National
Institute of Blind People. You can create a disability organization as a Trading Community Architecture party using the
Manage Integration of Additional Applications task in the Setup and Maintenance work area. You can then select a
disability organization party usage code.

For employees with disability, you can select the disability organization in their person records, identify the registration
and expiration dates, and enter any other descriptive or legislative information about the disability.

Related Topics

• Person Records

• Can I view the address details of the location on the Redwood pages for organizations?

• Can I select an existing organization when I'm creating a new organization in Redwood?

• Can I view the Other Classifications section on the Redwood pages for organizations?

Departments Search

As a professional user, you can use the Departments Search that uses Oracle Search and a customizable interface for an
enhanced search experience.

Here's what you can do with the departments search:

• Leverage Oracle Search to search for departments quickly and easily.

• Use the name, title, and location keywords to search for departments.

• Filter the results using various department filters, for example, Effective Date, Status, Set Name, and Location

Name.

• View the search results in a grid pattern and customize the grid columns.

• Navigate to the details page of a department from the search results where you can perform tasks depending

on your role.

For a filter category, the top 10 values are displayed in the LOV. If you don’t see the value that you need, you can start
typing the value in the LOV to find it. After you apply relevant filters, click the See Results button to view the filtered
data.

The fields listed under Hide are not shown in the results. If you want to view a field from this list as a column, you can
drag and drop it in the column configurator or select the check box next to the field.

41

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

HCM Trees

Trees graphically represent the hierarchical structures of your organization. You manage trees in the Workforce
Structures work area under My Client Groups.

These tree structures are supported - department, organization, position, and geography. What nodes can be added
to the tree is controlled by each structure type. With the exception of geography trees, you can create multiple trees for
each HCM tree type, and multiple versions of each tree. However, only one version of a tree is active at any time.

Each tree version contains a root node that's at the highest level in the hierarchy. The lines connecting the elements in
a tree structure are branches and the elements are referred to as nodes. These relationships are explained as follows: a
node is a parent of another node if it's one step higher in the hierarchy. Child nodes share the same parent node.

For example, in the Department Tree figure, Operations is the parent of Human Resources, Legal, and Finance, which
are its child nodes.

Department Trees
A department tree is a hierarchical representation of your departments. You can create versions of department trees but
only one tree version is active at a time. A department can’t be added more than once in the same tree version.

Department Tree Uses

• Maintain a hierarchy of all departments under one or multiple trees.

• Select the department hierarchy tree structure in the Secure by Organization Hierarchy setup of the

organization security profiles to secure access to departments within that tree.

• Secure Areas of Responsibility (AOR) data using the Hierarchy Type list. The areas of responsibility defined

for a hierarchy type can be used in securing by areas of responsibility while creating person security profiles to
secure person records.

• Use the responsibility types defined in the AOR setup to define approval rules so that representatives defined

using department tree can be approvers.

• Use the department hierarchy in your analysis to build roll-up analysis reports.

• Default the line manager from the department manager in a worker assignment using the department tree. You

can use the PER_DEPARTMENT_TREE_FOR_MANAGER profile option to configure this setting.

Example of a Department Tree

The following figure illustrates a department hierarchy that you can establish using a department tree.

42

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Organization Trees
An organization tree is a hierarchical representation of your various organizational entities. You can select any
organization including divisions, legal employers, business units, departments, and so on to create your organization
tree. You can create versions of organization trees but only one tree version is active at a time. An organization can’t be
added more than once in the same tree version.

Organization Tree Uses

• Maintain a hierarchy of different organizational structures.

• Select the Generic organization hierarchy tree structure option in the Secure by Organization Hierarchy setup

of organization security profiles to secure access to organizations within that tree.

• Secure Areas of Responsibility (AOR) data using the Hierarchy Type list. The areas of responsibility defined

for a hierarchy type can be used in securing by areas of responsibility while creating person security profiles to
secure person records.

• Use the responsibility types defined in the AOR setup to define approval rules so that representatives defined

using organization tree can be approvers.

• Use the organization hierarchy in your analysis to build roll-up analysis reports, if departments are at the lowest

level of the hierarchy.

Example of an Organization Tree

The following figure illustrates an organization hierarchy that you can establish using an organization tree.

43

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Position Trees
You can create multiple position trees using the predefined position tree structure in the Workforce Structures work
area. You can then create multiple versions to establish reporting relationships among positions. Position trees can have
only one top node.

Position Tree Uses

• Use position hierarchies for budgeting and organizational planning.

• Secure access to positions by identifying a position hierarchy in a position security profile. For example, you
can create a position security profile that includes all positions in a position hierarchy under a specified first
position. You can also include the position security profile in a person security profile to secure access to person
records. In this case, the person security profile includes the person records of the people who occupy the
positions in the position security profile.

Example of a Position Tree

44

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

The following figure illustrates a position hierarchy that you can establish using a position tree.

Geography Trees
You can create versions of the predefined geography tree structure to represent countries in which your enterprise
operates. For each country, you can define lower-level nodes such as states and cities. For example, United Kingdom -
England - London. You manage trees in the Workforce Structures work area.

Although you can create multiple versions, you can create only one tree in the hierarchy. Geography trees also have only
one first node.

Calendar Events

You use the geography tree to specify the locations to which calendar events apply. You can create the tree using these
conditions.

•

•

•

If an event applies to your entire enterprise, you can attach it to the first node in the tree, for example, Global.

If an event applies only to specific countries in your enterprise, you can attach it to the nodes for those specific
countries, for example, United Kingdom.

If an event applies only to specific states or cities in a country, you can attach it to the state or city level nodes.
For example, England, London.

Example of a Geography Tree

45

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

This figure illustrates the geographical hierarchy that you can establish using a geography tree.

Related Topics

• Guidelines for Managing Trees and Tree Versions

• Employment Profile Options

FAQs for Departments, Divisions, and Organizations

What's a reporting establishment?
A reporting establishment is an organization that's used for statutory reporting other than tax and social insurance
reporting. In some countries, such as France, a reporting establishment can also be a tax reporting unit.

A reporting establishment and a legal employer share a parent-child relationship with the legal employer being the
parent organization. A legal employer can be the parent of multiple reporting establishments. You create reporting
establishments using the Manage Legal Reporting Unit HCM Information task in the Setup and Maintenance work area.

46

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Related Topics

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

• Can I select an existing organization when I'm creating a new organization in Redwood?

• Can I view the Other Classifications section on the Redwood pages for organizations?

How do I create a disability organization?
Use the Manage Integration of Additional Applications task in the Setup and Maintenance work area. Disability
organizations are one of the choices when creating third-party organizations.

What's the difference between department name and title?
A department name is unique but the department title is non-unique and can be the same across departments. You
can't have 2 or more departments with the same name, but you can have multiple departments with the same title.

For example, you can have a Human Resources department (title) that can be common across the enterprise but there
can only be one unique US Human Resources department (name) in the enterprise. A department name is mandatory
but the title is hidden and optional, by default. You can enable the Title field and make it mandatory.

Can I delete an organization?
No you can't. However, you can disable an organization if it's no longer required. For example, if the enterprise is
downsizing, then you can set the status of the organization to inactive.

Changing the status of the organization disables the organization and the organization is no longer available to select.

How can I identify my organization in a report?
Use the organization manager information in the Create and Edit Department pages to enter a reporting name to
identify the organization in a report. You use organization hierarchies for statutory, legal and management reporting.

You can see all employees in the Manager list.

What's the purpose of the legislative action attributes?
When you create transfer or termination related actions using the Configure Actions task in the Workforce Structures
work area, you can also enter legislative attributes for the actions. You can use the attributes to:

•

Indicate whether an action is transfer-related.

• Specify the termination type for termination-related actions.

For example, the termination-related action Resignation can have the termination type as voluntary and the action
Reduction in Force can have the termination type as involuntary. Typically you enter this information to meet specific
legislative requirements or for reporting purposes.

Can I change the set of a department, location, job, or grade?
No, you can't change the set of a department, location, job, or grade because it may cause corruption in data that relies
on business unit and set partitioning. However, you can inactivate the current workforce structure and create a new set
respectively.

47

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

What's business unit and set partitioning?
Each business unit has its own reference data set for departments, locations, jobs, and grades. When you assign
reference data sets to business units, you assign a default reference data set to use for all reference data types for that
business unit.

You can override the set assignment for departments, jobs, locations, and grades.

When using jobs, grades, departments, and locations at the transaction level, users can select data from the set that
corresponds to the business unit they enter on the transaction, and any data assigned to the Common Set.

Locations

Locations

A location identifies physical addresses of a workforce structure, such as a department or a job. You create and manage
locations using the Location Details quick action in the Workforce Structures area on the My Client Groups tab.

You can also create locations to enter the addresses of external organizations that you want to maintain, such as
employment agencies, tax authorities, and insurance or benefits carriers.

When specifying the location address, you can default the country in the location responsive pages. You configure the
default location country on the Manage Enterprise HCM Information page. If you don't configure any default country,
then the country is automatically defaulted to United States in the location address.

The locations that you create exist as separate structures that you can use for reporting purposes, and in rules that
determine employee eligibility for various types of compensation and benefits. You enter information about a location
only once. Subsequently, when you set up other workforce structures you select the location from a list.

A point to note is that the Ship-to Site, Receiving Site, Bill-to Site, Office Site, and Designated Receiver fields in the
Shipping Details section of a location setup are for information purpose only and can be used to report upon. They
aren’t currently used by any feature or process within HCM.

Location Sets
When you create a location, you must associate it with a set. Only those users who have access to the set's business unit
can access the location set and other associated workforce structure sets, such as those that contain departments and
jobs.

Note the following:

• You can also associate the location to the common set so that users across your enterprise can access the

location irrespective of their business unit.

• You can also configure a location as an employee location on the Location Details page.

• When users search for locations, they can see the locations that they have access to along with the locations in

the common set.

48

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

The following figure shows how locations sets restrict access to users.

Upload Locations Using a Spreadsheet
If you have a list of locations already defined for your enterprise, you can upload them from a spreadsheet.

To use this option:

• Download a spreadsheet template

• Add your location information to the spreadsheet

• Upload directly to your enterprise configuration

You can upload the spreadsheet multiple times to accommodate revisions.

Update Location Details
If you need to update or correct the details of a location, here's how you can do that:

1. Go to My Client Groups > Location Details.
2. On the page, click Show Filters.
3. Search for the location you need to correct or update using the filters and select it.
4. On the location's details page, click Actions and select Update or Correct.
5. Update the details as required and click Submit.

Related Topics

• Why can't I see my location in the search results?

• What happens if I inactivate a location?

• Upload Workforce Structures Using a Spreadsheet

• How do I default a country when creating locations?

49

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Locations Search

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

As a professional user, you can use the Departments Search that uses Oracle Search and a customizable interface for an
enhanced search experience.

Here's what you can do with the locations search:

• Leverage Oracle Search to search for locations quickly and easily.

• Use the name, code, city, and other address fields to search for locations.

• Filter the results using various location filters, for example, Effective Date, Status, City or Town, Country, and

Location Set.

• View the search results in a grid pattern and customize the grid columns.

• Navigate to the details page of a location from the search results where you can perform tasks depending on

your role.

For a filter category, the top 10 values are displayed in the LOV. If you don’t see the value that you need, you can start
typing the value in the LOV to find it. After you apply relevant filters, click the See Results button to view the filtered
data.

The fields listed under Hide are not shown in the results. If you want to view a field from this list as a column, you can
drag and drop it in the column configurator or select the check box next to the field.

Associate Legal Employers with Locations

You can associate multiple legal employers with a location. This enables filtering locations by legal employer on pages
that have implemented this feature. You use the Legal Employers Operating At This Location extensible flexfield (EFF)
context for the legal employer - location association.

These are some key points to note:

• A location must have at least one associated legal employer to filter the location by legal employer.

• You can associate multiple legal employers operating at a location, but can't associate the same legal employer

twice with a location.

• You can associate the same legal employer with different locations.

• You can delete the legal employer - location association.

• The legal employer - location mapping is copied when you duplicate a location.

• You can associate legal employers when creating, updating, or correcting a location.

• The legal employer list of values displays all active and inactive legal employers configured. There isn't any

filtering for only active legal employers. Similarly, there is no filtering of legal employers by matching the legal
employer country with the location address country.

• Legal employers are listed in the ascending order of legal employer name.

• Locations are first filtered based on the set. And thereafter, if an association exists, they're filtered based on the

legal employers.

In this example, Vision Enterprise has 3 legal employers Vision Corporation, Vision US, and Vision Consulting operating
at multiple locations in the US. You want to filter locations from where Vision Corporation is operating.

50

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Let's look at the steps to update this association.

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Associate Vision Corporation with the Pleasanton Location

1. Go to My Client Groups > Quick Actions > Workforce Structures.
2. Click the Location Details task.
3. Click Add.
4. Select the Additional Info option on the questionnaire page and click Continue.
5. Enter these required details to create a location.

Section

Field

Value

When and Why

When does this location start?

8/25/21

Location Details

Name

Code

Main Address

Address Line 1

ZIP Code

City

State

County

Pleasanton

PLS

603

94588

Pleasanton

CA

Alameda

6.

In the Additional Info section, click Add in the Legal Employers Operating At this Location section to associate
the Vision Corporation legal employer to this location.
7. Select Vision Corporation from the Legal Employer list.

Note:  As a prerequisite, the legal employer should already exist.

8. Click OK.
9. Click Submit.

Related Topics

• Filter Locations Based on Legal Employers

51

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

FAQs for Locations

Why can't I see my location in the search results?
You can search for approved locations only. Also, if you created a location in Oracle Fusion Trading Community Model,
then you can't access that location from Oracle Fusion Global Human Resources.

For use in Oracle Fusion HCM, you must recreate the location from the Manage Locations page.

How can I associate a location with an inventory organization?
From the Oracle Fusion Global Human Resources, go to the Manage Locations page. Use the Manage Locations task in
the Workforce Structures work area.

To appear on the Create or Edit Location pages, your inventory organization must be effective as of the current date and
must exist in the location set that you selected.

What happens if I select an inventory organization when I am creating or editing a
location?
The location is available for selection in purchase documents of that inventory organization in Oracle Fusion Inventory
Management. If you don't select an inventory organization, then the location is available in purchase documents across
all inventory organizations.

What happens if I select a geographic hierarchy node when I create or edit a location?

The calendar events that you created for the geographic node start to apply for the location and may impact the
availability of worker assignments at that location.

You manage locations using the Manage Locations task in the Workforce Structures work area.

The geographical hierarchy nodes available for selection on the Locations page display from a predefined geographic
hierarchy.

Related Topics

• How an Individual's Schedule Is Identified

What happens if I inactivate a location?
Starting from the effective date that you entered, you can no longer associate the location with other workforce
structures, assignments, or applications.

If the location is already in use, it will continue to be available to the components that currently use it.

52

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Worker Unions

Worker Union Management

These three components manage worker union information in Human Capital Management (HCM) Cloud:

• Worker Unions

• Bargaining Units

• Collective Agreements

Worker Unions
The worker union is a HCM organization. The details of a worker union are country-specific and the country value is
mandatory for a worker union. You can optionally attach any supporting documents for the worker union. A worker
union holds date-effective attributes. Therefore, you can track the changes to the worker union over a period of time.
You can also inactivate the worker union. You can configure additional attributes specific to any legislation or customer
using the available descriptive flexfields and extensible flexfields.

You can optionally associate worker unions with their affiliated bargaining units. The values in the Bargaining Unit and
Location fields are filtered to match the country you selected. You can add more than one work union contact and enter
the contact details, such as contact name, union title, work phone, and work Email.

This figure illustrates the association between worker union, bargaining unit, and collective agreement:

A worker union can be associated with multiple bargaining units. However, a bargaining unit can be associated with only
one worker union. A collective agreement can be associated with only one worker union and bargaining unit. A worker
union or bargaining unit can be associated with multiple collective agreements.

53

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

This figure illustrates the association between position or assignment and worker union, bargaining unit, and collective
agreement:

A position or worker assignment can be associated with only one collective agreement, bargaining unit, and worker
union. However, a bargaining unit, worker union, or collective agreement can be associated with multiple positions or
worker assignments.

Bargaining Units
A bargaining unit is a specific group of employees who are represented by one authorized union or association for
purposes of collective bargaining. A bargaining unit is defined as a lookup type.

Collective Agreements
A collective agreement is a special type of commercial agreement that's negotiated collectively between the
management (on behalf of the company) and trade unions (on behalf of employees). The agreement regulates the
terms and conditions of employees in their workplace, their duties, and the duties of the employer.

Let's take a look at the collective agreement details:

A collective agreement is country-specific. You may enter the bargaining unit, legal employer, and union values
depending on the country. For example, you can create a collective agreement without the bargaining unit and legal
employer, or only with the legal employer. When you select the value in the Country field, the values in the Bargaining
Unit, Legal Employer, and Union fields are filtered to match the country selected. You can optionally associate collective
agreements with worker unions and attach documents to the collective agreement.

54

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

You can provide details of the parties negotiating the collective agreement, such as the employee and employer
organizations. The employee organization can be the trade union or bargaining unit representing the employee while
the employer organization is represented by the company management.

A collective agreement is date-effective, therefore, you can track changes to a collective agreement over time.
You can also inactivate the collective agreement. You can configure additional attributes specific to a legislation or
customer using the available descriptive flexfields and extensible flexfields. If you specify a Valid To date for a collective
agreement, it lapses after that date and you can't link it to an employee.

Note:  If the collective agreement is linked to an assignment, you can't edit the Identification Code, Country,
Bargaining Unit, Union, and Legal Employer fields. Additionally, you can't delete the collective agreement.

Here's how you can link collective agreements:

You can link a collective agreement to an assignment provided the bargaining unit, country, and legal employer of the
collective agreement are consistent with the assignment. If you created a collective agreement without associating
it with a legal employer or bargaining unit, you can link the collective agreement to any assignment within the same
country.

You can link a union, bargaining unit, or collective agreement with a worker assignment provided that its country and
legal employer is consistent with the assignment.

The union, bargaining unit, and collective agreement list of values (LOV) that you can select for linking with an
assignment or position are filtered as described in this table:

Attribute

Union

Linking Object

Filter Conditions

Assignment

Union

Position

Bargaining Unit

Assignment

Bargaining Unit

Position

The LOV is filtered to show unions that are
active as of the start date and whose country
matches the country of the legal employer on
the worker assignment.

The LOV is filtered to show unions that are
active as of the position start date. As there is
no legislation context available for a position,
 the LOV isn't filtered based on the union
country. All unions configured in the application
are listed in the LOV.

•

•

If you don't select a union, the LOV is
filtered to show bargaining units that are
active as of the start date, and whose
country matches the legal employer
country or have no country tag itself.

If you select a union, the LOV is filtered to
show bargaining units that are active as of
the start date and are associated with the
selected union.

As there is no legislation context available for a
position, the LOV isn't filtered based on country
tags configured for the bargaining unit lookup
codes.

55

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Attribute

Linking Object

Filter Conditions

Collective Agreement

Assignment

Collective Agreement

Position

•

•

If you don't select a union, the LOV is
filtered to show bargaining units that are
active as of the position start date.

If you select a union, the LOV is filtered to
show bargaining units that are active as of
the position start date and are associated
with the selected union.

Note:
The LOV is filtered to show only those values
that match the country of the legal employer
on the worker assignment.

If you don't select a union or bargaining unit,
 the LOV is filtered to show all active collective
agreements as of the start date.

If you select a union without selecting a
bargaining unit, the LOV is filtered this way:

• Shows collective agreements that are

active and match the selected union, but
don't have an associated bargaining unit
(union-specific values).

• Shows collective agreements that are

active and don't have an associated union
or bargaining unit value (global values).

If you select a bargaining unit without selecting
a union, the LOV is filtered this way:

• Shows collective agreements that are

active and match the selected bargaining
unit, but don't have an associated union
(bargaining unit-specific values).

• Shows collective agreements that are

active and don't have an associated union
or bargaining unit value (global values).

If you select a union and a bargaining unit, the
LOV is filtered this way:

• Shows collective agreements that are

active and match the selected union and
bargaining unit (union and bargaining
unit-specific values).

• Shows collective agreements that are

active and don't have an associated union
or bargaining unit value (global values).

As there is no legislation context available on
for a position, the LOV isn't filtered based on
the collective agreement country.

If you don't select a union or bargaining unit,
 the collective agreement LOV is filtered to

56

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Attribute

Linking Object

Filter Conditions

show all active collective agreements as of the
position start date.

If you select a union without selecting a
bargaining unit, the LOV is filtered this way:

• Shows collective agreements that are

active and match the selected union, but
don't have an associated bargaining unit
(union-specific values).

• Shows collective agreements that are

active and don't have an associated union
or bargaining unit value (global values).

If you select a bargaining unit without selecting
a union, the LOV is filtered this way:

• Shows collective agreements that are

active and match the selected bargaining
unit, but don't have an associated union
(bargaining unit-specific values).

• Shows collective agreements that are

active and don't have an associated union
or bargaining unit value (global values).

If you select a union and a bargaining unit, the
LOV is filtered this way:

• Shows collective agreements that are

active and match the selected union and
bargaining unit (union and bargaining
unit-specific values).

• Shows collective agreements that are

active and don't have an associated union
or bargaining unit value (global values).

57

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 3
Departments, Divisions, Organizations, Locations, and
Worker Unions

Attribute

Linking Object

Filter Conditions

Note:

• The global collective agreement values

can be used on a position by configuring
the following profile option:

CAGR_ON_POSITIONS

◦ Code: ORA_PER_ALLOW_GLOBAL_
◦ Display Name: Allow Global Collective

Agreements on Position

• By default, the profile value is set to
N. In this case, the global collective
agreement values can't be used on a
position even though the values are
available for selection in the LOV. If you
select a global collective agreement
value, the application will display an
error message when you submit the
position change or creation.

•

If you set the profile value to Y, the
global collective agreement values can
be used on a position.

Related Topics

• Can I view the address details of the location on the Redwood pages for organizations?

• Can I select an existing organization when I'm creating a new organization in Redwood?

• Can I view the Other Classifications section on the Redwood pages for organizations?

58

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

4  Jobs and Positions

Jobs

Jobs are typically used without positions by service industries where flexibility and organizational change are key
features. As part of your initial implementation, you specify whether to use jobs and positions, or only jobs.

Basic Details
Basic details for a job include an effective start date, a job set, a name, and a code.

A job code must be unique within a set. Therefore, you can create a job with the code DEV01 in the US set and another
job with the same code in the UK set. However, if you create a job with the code DEV01 in the Common set, then you
can't create a job with the same code in any other set.

Benchmark Information
You can identify a job as being a benchmark job. A benchmark job represents other jobs in reports and salary surveys.
You can also select the benchmark for jobs. Benchmark details are for informational purposes only.

Progression Information
A progression job is the next job in a career ladder. Progression jobs enable you to create a hierarchy of jobs and are
used to provide the list of values for the Job field in the Promote Worker and Transfer Worker tasks.

The list of values includes the next job in the progression job hierarchy. For example, assume that you create a job called
Junior Developer and select Developer as the progression job. Progression jobs show as suggested jobs; so when you
promote a junior developer, the Suggested Jobs list of values for the new job will show Developer. You can select this
value, or select another one.

Jobs and Grades
You can assign grades that are valid for each job. If you're using positions, then the grades that you specify for the job
become the default grades for the position.

Related Topics

• Guidelines for Using Desktop Integrated Excel Workbooks

• Considerations for Enforcing Grades at Assignment Level

Examples of Jobs

Jobs are typically used without positions by service industries where flexibility and organizational change are key
features.

59

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Software Industry
For example, XYZ Corporation has a director over the departments for developers, quality assurance, and technical
writers.

• Recently, three developers have resigned from the company.

• The director decides to redirect the headcount to other areas.

•

Instead of hiring all three back into development, one person is hired to each department, quality assurance,
and technical writing.

In software industries, the organization is fluid. Using jobs gives an enterprise the flexibility to determine where to use
headcount, because the job only exists through the person performing it. In this example, when the three developers
leave XYZ Corporation, their jobs no longer exist, therefore the corporation has the flexibility to move the headcount to
other areas.

This figure illustrates the software industry job setup.

Examples of Positions

Positions are typically used by industries that use detailed approval rules, which perform detailed budgeting and
maintain headcounts, or have high turnover rates.

Retail Industry
ABC Corporation has high turnovers. It loses approximately 5% of its cashiers monthly. The job of the cashier includes
three positions: front line cashier, service desk cashier, and layaway cashier. Each job is cross-trained to take over
another cashier's position. When one cashier leaves from any of the positions, another existing cashier from the
front line, service desk or layaway can assist where needed. But to ensure short lines and customer satisfaction, ABC
Corporation must replace each cashier lost to turnover. Since turnover is high in retail it's better for this industry to use
positions.

60

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Note the following:

Chapter 4
Jobs and Positions

• You have to create a vacancy manually when position synchronization is used and an employee terminates

employment (when an incumbent moves out of the position).

• The position exists even when there are no holders. Having the position continue to exist is important if the

person who leaves the company is a manager or supervisor with direct reports.

• All direct reports continue reporting to the position even if the position is empty.

• You don't have to reassign these employees to another manager or supervisor. The replacement manager is

assigned to the existing position.

Also, an added advantage to using Positions is when you hire somebody new, many of the attributes are inherited from
the position. This speeds up the hiring process.

This figure illustrates the retail position setup.

Health Care Industry
Health care is an industry that must regulate employment, roles, and compensation according to strict policies and
procedures. Fixed roles tend to endure over time, surviving multiple incumbents. Industries that manage roles rather
than individuals, where roles continue to exist after individuals leave, typically model the workforce using positions.

The hospital has a structured headcount and detailed budgeting. For example, a specific number of surgeons, nurses,
and interns of various types are needed. These positions must be filled in order for the hospital to run smoothly. Use
jobs and positions when you apply detailed headcount rules.

61

Oracle Fusion Cloud Human Resources
Using Global Human Resources

This figure illustrates the hospital position setup.

Chapter 4
Jobs and Positions

Considerations for Using Jobs and Positions

Jobs and positions represent roles that enable you to distinguish between tasks and the individuals who perform those
tasks.

Note the following:

• The key to using jobs or positions depends on how each is used.

• Positions offer a well-defined space independent of the person performing the job.

• Jobs are a space defined by the person.

• A job can be defined globally in the Common Set, whereas a position is defined within one business unit.

• You can update the job and department of a position at any time. For example, if you hire someone into a new

role and want to transfer the position to another department.

During implementation, one of the earliest decisions is whether to use jobs or a combination of jobs and positions. The
determinants for this decision are:

• The primary industry of your enterprise

• How you manage your people

Primary Industry of Your Enterprise
The following table outlines information about Primary industries and how they set up their workforce.

Primary Industry

Workforce Setup

Mining

Utilities

Positions

Positions

62

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Primary Industry

Workforce Setup

Manufacturing

Retail Trade

Positions

Positions

Transportation and Warehousing

Positions

Educational Services

Positions

Public Transportation

Positions

Agriculture, Forestry, Fishing, and Hunting

Jobs

Construction

Wholesale Trade

Information

Finance and Insurance

Professional, Scientific, and Technical
Services

Management of Companies and
Enterprises

Jobs

Jobs

Jobs

Jobs

Jobs

Jobs

Administrative and Support and Waste
Management and Remediation Services

Jobs

Arts, Entertainment, and Recreation

Jobs

Accommodation and Food Services

Jobs

Other Services (Except Public
Administration)

Jobs

Management of People
Consider the following scenarios how industries manage their employee turnover:

• Scenario 1: Replace employees by rehiring to the same role.

• Scenario 2: Replace headcount but the manager uses the headcount in a different job.

63

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

• Scenario 3: Rehire employees to the same position, but the manager requests reallocation of budget to a

different post.

The following table displays suggestions of what the industry should use, either jobs or positions, in these three
scenarios:

Industry

Project (An industry that
supports project-based forms of
organization in which teams of
specialists from both inside and
outside the company report to
project managers.)

Controlled (An industry that's
highly structured in which all
aspects of work and remuneration
are well organized and regulated.)

Scenario 1

Positions

Scenario 2

Scenario 3

Jobs

Jobs

Positions

Positions

Positions

Manufacturing

Positions

Positions

Positions

Positions

Retail

Education

Other

Related Topics

Jobs

Jobs

Jobs

Jobs

Positions

Positions

Positions

Jobs

• How Grades and Grade Rates Work with Jobs, Positions, Assignments, Compensation, and Payroll

Job and Position Structures

Job and position structures identify the descriptive flexfield structure that enables you to specify additional attributes
that you want to capture when you define jobs and positions.

Job and position attributes provide further detail to make jobs and positions more specific. You also use attributes to
define the structure of your jobs and positions. You can specify attributes at the enterprise level for jobs and positions,
at the business unit level for positions, and at the reference data set level for jobs. Job and position structures are
optional.

Enterprise-Level Job Attributes
When you define a job, you enter a value for the name of the job. To make job names more specific, set up attributes
to identify additional details about the job. This includes the nature of the work that is performed or the relative skill

64

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

level required. If these attributes apply to all jobs within your enterprise, set up enterprise-level job attributes. Standard
capabilities mean that you can use the different segments of the name to:

•

Identify common jobs or job holders for analysis or compensation.

• Group records in reports, such as to find all jobs of a specific job type.

Don't use attributes with values that change regularly, for example, salary ranges or expense approval levels that change
every year.

This figure illustrates how job type and job level provide further details for the HR Application Specialist job.

Enterprise-Level Position Attributes
Position attributes at the enterprise level are similar to those for jobs. Each position that you define identifies a specific
role in the enterprise, which you can manage independently of the person in the position. A position belongs to one
specific department or organization. The name of each position must be unique. To simplify the process of managing
unique names for positions, set up enterprise-level attributes to identify separate components of the position name.
For example, you can set up an attribute for position title and one for position number. When defining the attributes
that make up the structure of a position name, consider whether any of your attributes are part of the definition of
a common job type. Using job types for a position can help you manage common information that applies to many
different positions.

For example, you can:

1. Define a job type of Manager.Level 1.
2. Use it for comparison of positions across departments or lines of business or for setting common job

requirements.

3. Define multiple manager-type positions in your HR department, each of which has responsibility for a different

management function or group.

65

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

This figure illustrates how title and position number provide further details for the manager position.

Business Unit-Level Attributes for Positions
If you have information that you want to capture for positions that are specific to each business unit, then you can
define attributes at the business unit level for positions. When you create positions, these attributes appear in addition
to any enterprise-level attributes. For example, you might want to identify the sales region for all positions in the sales
business unit. You can set up a text attribute called Sales Region and use it to enter the necessary information when
creating positions for the sales business unit.

Reference Data Set-Level Attributes for Jobs
If you have information for jobs that applies to specific reference data sets, set up attributes for jobs at the reference
data set level. When you create jobs, these attributes appear in addition to any enterprise-level attributes. For example,
you might want to identify all information technology (IT) jobs within a specific set. You can set up a text attribute called
Function and use it to enter IT in jobs that you create that perform an IT function within a specific set.

Scheduling Group Attribute for Jobs

You can use scheduling groups to group similar jobs for the purpose of workforce scheduling.

For example: In healthcare, the skill set of a Registered Nurse or RN may include multiple jobs in HCM such as
Registered Nurse (RN), Charge Nurse (CN), and Certified Nurse Assistant (CNA). A staffing need for an RN can be
fulfilled by any one of these different jobs defined in HCM.

Scheduling group is an optional attribute that you can add to jobs. It’s defined as a lookup, and it's supported by the
ORA_PER_SCHEDULING_GROUP lookup type. You can define the lookup values according to your requirement by using
the Manage Common Lookups task.

Here are some more details about this attribute:

• Scheduling group isn't a required attribute.

•

Its default value is blank.

66

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

•

In the Job Duplicate flow, the value of this field is copied from the source job.

• You can upload data for this attribute using HCM Data Loader (HDL) and HCM Spreadsheet Data Loader

(HSDL).

• The Scheduling Group attribute is also migrated when you migrate your job configuration using the export and

import functionality in Functional Setup Manager (FSM).

• You can make date-effective updates and correct the existing value of this attribute.

• The Scheduling Group attribute is added to the ManageJobs data model. You can add this attribute to the

UpdateJobReport, CreateJobReport, and DTDeleteJobReport reports by customizing the BIP templates, if
required.

Associate Legal Employers with a Job

You can associate multiple legal employers with a job using the Legal Employers That Use This Job extensible flexfield
(EFF) context. If you have enabled Oracle Search for Jobs LoV, this will help in filtering the jobs based on the selected
legal employer, on pages that will implement this feature in the future.

Here are some key points to note:

• You can associate multiple legal employers with a job, but you can't associate the same legal employer twice

with the same job.

• You can associate the same legal employer with different jobs.

• You can delete the legal employer - job association.

• This legal employer - job mapping is copied when you duplicate a job.

• You can associate legal employers when creating, updating, or correcting a job.

• The legal employer list of values will display all active and inactive legal employers configured. Filtering isn’t

done for only active legal employers.

• Legal employers are listed in the ascending order of legal employer name.

• Jobs are first filtered based on the set. And thereafter, if an association exists, they're filtered based on the legal

employers.

• A job must have at least one associated legal employer, for the job to be filtered based on a legal employer.

• You can associate jobs with legal employers using both classic and responsive job pages but you can use the job

filtering only on Redwood pages because this feature is delivered for REST LOVs only.

• You can also use HCM Data Loader (HDL) to associate legal employers with a job.

• The job - legal employer association is also migrated when you migrate your Job configuration using the

Functional Setup Manager (FSM) export/import functionality.

• An extra parameter is added on the REST jobsLovV2 as follows:

◦ LegalEmployerId in findByWord finder.

•

If you have enabled Oracle Search for Jobs LoV, only pages that have implemented this feature will demonstrate
this additional filtering.

In this example, Vision Enterprise has 3 legal employers Vision Corporation, Vision US, and Vision Consulting associated
with multiple jobs in the US. You want to filter jobs associated with Vision Corporation.

Let's look at the steps to update this association.

67

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Associate Vision Corporation with the Assistant Trainer Job

1. Go to My Client Groups > Quick Actions > Workforce Structures.
2. Click the Job Details task.
3. Click Add.
4. Select the Additional Info option on the questionnaire page and click Continue.
5. Enter the required details to create a job.

Section

Field

When and Why

When does this job start?

Job Details

Job Details

Name

Code

Value

8/25/21

Assistant Trainer

ASST_TRAINER

6.

In the Additional Info section, click Add in the Legal Employers That Use This Job section to associate the
Vision Corporation legal employer with this job.

7. Select Vision Corporation from the Legal Employer list.

Note:  As a prerequisite, the legal employer must already exist.

8. Click OK.
9. Click Submit.

Related Topics
• Jobs

• Configure Extensible Flexfields

• Guidelines for Loading Jobs

• Jobs List of Values V2

• Extending HCM Redwood Applications Using Visual Builder Studio

Workforce Structures Code Generation Methods

A code uniquely identifies either a position or a job. Currently, you can generate a code for position and job workforce
structures. Use the Manage Enterprise HCM Information task in the Workforce Structures work area to configure the
code generation method for positions and jobs.

You can generate the position code or the job code in one of these 3 ways:

• Manually

• Automatically prior to submission

• Automatically upon final save

Manual: Use this method to manually enter the code when creating a position or a job. You can update the code in the
Details page. This is the default method for generating the position and job code.

68

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Automatic prior to submission: Use this method to automatically create and display the code when you create a
position or job. This method may create gaps in the code sequence if the transaction is canceled after the position or
job code is generated.

Automatic upon final save: Use this method to create position or job codes only after the create transaction is
approved. You can't see the position or job code when you're creating the respective workforce structure, but can see it
on the Details page after the transaction is approved. This method has less possibility of creating gaps in the generated
codes.

The Automatic prior to submission and Automatic upon final save methods use an enterprise number sequence. All
workforce structures' codes that are generated using the automatic methods are numeric only. By default, the sequence
starts from 1; however, you can change the starting number. The code increments by one for each new position or job
created.

You can change the position or job code generation method from Automatic prior to submission method to the
Automatic upon final save method and the other way around. You can also change from the automatic method to the
manual method and the other way around but you must be careful which method you choose if you have existing data.
You can't edit an automatically generated position or job code.

Initial Position and Job Code
You can specify the initial position or job code for your enterprise when you generate the code automatically. The
application uses this number for the first record that you create using the automatic position and job code setting and
increments the number by one for subsequent records. By default, the initial code is 1. The validation on the initial
position and job code helps you identify the starting code in automatic code generation when the method is changed
from manual to automatic.

Using the initial position and job code, you can retain the legacy codes for existing positions and jobs respectively.
Additionally, you can automate the number generation for new positions and jobs, starting from the last legacy person
number plus one. You can change the initial code.

Note:  To avoid duplicate codes being generated, follow these recommendations.

•

If you have been using the manual method of position or job code generation for sometime and now moving
to the automatic method, we recommend setting an initial code to a value higher than the old position or job
codes that were specified manually.

• When using HDL to load positions or jobs, the position and job code can be automatically generated, hence we

recommend you leave the code blank in the dat file.

View Details of Associated Profiles and Open Profiles
Pages from Redwood Job or Position Pages

On the read-only, create, and edit pages for jobs and positions in Redwood, you can see a read-only view of all the
associated profiles. You can view all the profile details without leaving the job or position page.

This feature is available only in the Redwood job and position pages.

69

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

The Associated Profiles section of the job or position page shows all the profiles associated with a job or position. For
each of the associated profiles, an individual Profile details link is displayed. When you click the link for an associated
profile, a panel drawer opens, showing the entire details for that particular associated profile.

Note:  The Associated Profiles read-only section appears in the view, create, and edit pages for jobs and positions. If
you add an associated profile to this section while creating or editing a job or position, the Profile details link for the
profile that you’re adding will appear only after you click the Save button for that profile.

You can also open the job profiles and position profiles search pages from within a view-only job or position page
respectively in Redwood. All the profiles associated with that particular job or position will show up by default on the
profiles page. If you clear this search by closing the Job Name or Position Name filter chip, you will see a list of all the
available job profiles or position profiles respectively.

You can create or edit a profile on the profile page, and then associate it with the same job or position, or with any other
job or position. Clicking the Back arrow will take you back to the same view page.

Create a Position Profile

Profiles help you in identifying the requirements and competencies for a position. You can associate an existing profile.
You can also create a new profile and associate it with the position by updating or correcting the position.

You can associate a profile to a position using any of these pages - Position Details, Position Change, and Request a
New Position. Here's how you create a position profile.

1. On the Home page, click My Client Groups.
2. Navigate to the quick actions and click the Show More link.
3. Under Workforce Structures, click Position Details.
4. Search for and click the position for which you want to associate the profile.
5. On the Position Details page, click Create Profile under the Actions menu.
6. On the Create Position Profile page, enter these details.

Field

Description

Position Responsibility

Responsibilities that are required for the position.

Position Qualifications

Qualifications that are required of the people in the position.

7. Click Save.

Associate Action Reasons in Position with Role

70

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

You can make the action and action reason role-specific on these position pages by selecting the applicable roles when
you configure the action and action reason.

• Request a New Position

• Request a Position Change

• Update Position (from Position Details)

• Correct Position (from Position Details)

• Duplicate Position (from Position Details)

After the configuration, the position pages will display the action and action reason that are specific to the worker's
logged in user role. You need to associate the action reasons on the Configure Actions page. In these steps, we will
create a new action reason and associate the role.

1. On the Home page, click My Client Groups > Workforce Structures > Action Reasons.
2. Click Add.
3. Enter a name, code, and description for the action.
4. Click Submit.
5. On the Home page, click My Client Groups > Workforce Structures > Configure Actions.
6. Search and click the action with which you want to associate the specific action reason, for example, Update.

This table lists the flows associated with the action.

Action

Create

Update

Code

Applies to

PER_POS_NEW

PER_POS_UPD

◦ Request a New Position
◦ Duplicate Position

◦ Update Position
◦ Correct Position
◦ Request a Position Change

7. On the Edit Action page, click Continue in the Action section.
8. Click Associate.
9. Select the action reason you created.
10. Enter a start date for the association.
11. Select the roles you want to associate.
12. Click Submit.

In addition to the action reasons associated with the role, you can also see the action reasons that are available for all
users and not associated with any role in the Action Reasons LOV.

How FTE is Calculated in Positions

The full-time equivalent (FTE) value is the result of multiplying the working hours with the headcount and dividing by
the standard working hours.

For example, if the working hours are 30, the headcount is 2 and the standard working hours are 40, then the FTE value
is 1.5.

71

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Ways to Calculate the FTE
You can either enter the FTE manually or calculate it automatically.

• Manually: Use the FTE field in the Budget Details section to enter a FTE value manually. If an FTE value is
already provided, you can update it based on the ratio of the working hours to standard working hours.

• Automatically: Select the Calculate FTE option in the Budget Details section to automatically calculate the FTE.
This check box is shown only when the Enable FTE Calculation in Positions profile option is set to Yes. Earlier,
the FTE value was automatically calculated only when a position was created. However, when this check box is
deselected automatic FTE calculation is disabled even when a position is created.
When the Calculate FTE option is selected and you edit the working hours or the headcount in the position
pages, the FTE is automatically calculated and the FTE field becomes read-only. However, you can override the
automatic calculation of FTE by deselecting the Calculate FTE option on the position pages.
This check box is available in these flows - Request a New Position, Request a Position Change, Update or
Correct Position, and Duplicate Position flows.

The Calculate FTE Option
Here are some points to note about Calculate FTE option.

• The Calculate FTE option is disabled for positions created before enabling automatic FTE calculation.

• The Calculate FTE setting is copied when a position is duplicated.

•

If FTE is configured as hidden in the Transaction Design Studio (TDS), then the Calculate FTE option is also
hidden even though the profile option is enabled.

Work Hours and Duration

Full-time equivalent (FTE) is the number of hours worked by an employee on a full-time basis.

It’s calculated by dividing the working hours by standard working hours. For example, if the working hours are 20 and
the standard working hours are 40, the FTE is 0.5.

Organizations use FTE to determine their employees’ workload; specifically the number of part-time employees
required and the hours they work to add up to the same number of hours worked by full-time employees. Hence, the
general assumption is that an employee works 2,080 hours annually. This value is derived by calculating the number of
hours worked by a full-time worker in a week multiplied by the number of weeks in a year - 8 hours per day x 5 days per
week x 52 weeks per year = 2,080 hours.

However, the working hours duration might vary across industries. For example, in the manufacturing sector, an annual
number of working hours contract may be in place due to seasonal fluctuations, with only premium pay applicable when
the prorated annual hours exceed the specified annual hours. In the education sector, the duration may be linked to the
academic teaching timetable.

In such cases, the FTE calculation needs to be adjusted for such employees. These work hours attributes defined in a
position help in determining the adjusted FTE.

Standard Working Hours - Standard working hours are usually those of a full-time worker. You define them for the
enterprise, legal employer, department, location, job, or position.

72

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

If you define standard working hours for more than one work structure, the application uses this hierarchy to derive
standard working hours for the position: Job > Location > Department > Enterprise. The application uses this hierarchy
to derive standard working hours for the worker assignment: Position > Job > Location > Department > Legal Employer
> Enterprise.

Working Hours - Working hours are the same as standard working hours, by default.

Working hours and standard working hours may remain the same. For example, if an employee is working the
department's standard working hours, standard working hours and working hours are the same. For part-time workers,
there is usually a difference between standard working hours and working hours. Where there is a difference, you
update the working hours for the position and the assignment.

Standard Annual Working Duration – You define the standard annual working duration for the enterprise, legal
employer, department, location, job, or position.

If you define the standard annual working duration for more than one work structure, the hierarchy to derive the
standard annual working duration is same as standard working hours.

Annual Working Duration – Annual working duration is same as the standard annual working duration. The value may
differ but the duration is the same as the duration defined for the standard annual working duration.

Workday Information Defaults

The Full-Time Equivalent (FTE) is the number of hours worked by a worker on a full-time basis and is typically used to
determine the workload.

You can either specify your own values or default the standard working hours, standard annual working duration, and
the unit of measure (UOM) values. The workday information is used to calculate the full-time equivalent (FTE) of a
worker.

You can default the workday information attributes from these entities in this order.

1. Job
2. Location
3. Department
4. Enterprise

Let’s look at how this works with the help of a diagram.

73

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

The defaulting logic for the standard working hours, frequency, standard annual working duration, and units of
measure is given below.

Entity

Job

Location

Department

How it Works

The first check is on the job specified in the position. If values for any of these attributes are available
in the job, then these values are defaulted on the position.

If any of the attribute values aren't specified on the job, then the check is done on the location
specified in the position. If these values are specified in the location, then these values are defaulted on
the position.

If any of the attribute values aren't specified on the location, then the check is done on the department
specified in the position. If these values are specified in the department, then these values are
defaulted on the position.

74

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Enterprise

If any of the attribute values aren't specified on the department, then the check is done on the
enterprise. If these values are specified in the enterprise, then these values are defaulted on the
position.

If you change the business unit, department, location, or job in the position, then the existing defaulted workday
information is also removed, if they are defaulted from any of these objects. However, this doesn't apply when you
duplicate a position.

In addition, the defaulting hierarchy gets recalibrated when you provide a value in any of the entities. For example, if
the standard annual working duration was earlier defaulted from the enterprise and you have specified a value for the
standard annual working duration for a department now. The latest standard annual working duration value will now be
defaulted from the department.

How You Match Position Valid Grades with Job Grades

You can enforce that valid grades of the position match with valid grades of the associated job by setting this profile
option value to yes: Validation to Match Position's Valid Grades With Job Valid Grades Enabled.

When the profile option is enabled, only valid grades specified in the selected job can be added in the position. An error
is shown when you add grades that aren’t specified for the job.

A new position inherits the valid grades defined in the selected job. Valid grades for the position are those that are
active and associated with the common set or the set associated with the business unit. Valid grades are used in
assignments that use the position and subsequently in payroll calculation.

Position Budgeting

Position Budgeting helps to capture the budgetary values and to enforce them while creating or updating budgets for
positions. You can now define a budgetary period and measure your activity against these values.

For more information about position budgeting, see How do I set up position budgeting?

Position Costing for Redwood Positions Pages

You can manage the position costing information in the newly added Costing region in the Redwood Position pages and
processes. The Costing region is hidden by default. You need to enable it using business rules.

The costing information can be managed when creating or updating a position, or while requesting a new position or
requesting a position change.

The costing of position is specific to a legislative data group. You need to have access to the legislative data group to
add or modify the costing of the position. The changes to the position costing are within the context of a legislative data
group.

75

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

To update an existing position costing, search for and click the position on the Positions search page. On the position
page, go to the Costing region. Open the costing record that you want to update, and click Update Record in the Select
an action drop-down list. Modify the data as required. Click +Add to add another costing LDG. Click Save.

To delete an existing position costing, on the position page, open the costing record and click Delete Record in the
Select an action drop-down list.

Note:  If you delete a date effective record for a position, the costing doesn’t get deleted.

Similarly, you can add the position costing information and modify the position costing in the Costing step of the
Request a New Position and Request a Position Change processes respectively.

Here are some key points about position costing:

• You can't create costing for a position if no cost allocation structure is attached to the legislative data group.

• You can't create costing when costing exists in a future date.

• The total percentage of cost allocations must be between 0 and 100. If it's less than 100, a warning message
is displayed, stating that the remaining allocation goes to Default Account, and you can proceed further after
you confirm. If the total percentage of cost allocations is above 100, an error message is shown, and you can’t
proceed further until you correct it.

•

If you enter a percentage and don't enter any costing segments, an error message is displayed.

• Position costing isn’t a child of the position. It’s a separate object on its own. So whatever operations you’re

doing on the position won’t impact the costing.

• A position has its own effective start date and effective end date, and position costing has its own effective

start date and effective end date. The position dates and the position costing dates are different and
independent of each other.

•

If costing is already existing for a position, all the costing records that lie between the effective start date and
effective end date for the position are displayed in the Position Costing section.

• When you duplicate a position, the costing data won’t be copied to the duplicated position. You need to add the

costing data manually.

• Position costing can also be managed from the position costing pages of payroll. Any changes made in payroll

will reflect here and vice versa.

Related Topics
• Jobs

• Extending HCM Redwood Applications Using Visual Builder Studio

Position Synchronization

If position synchronization is enabled, assignments inherit specified values from the associated position.

Synchronized Attributes
You can select any of the following attributes for synchronization when position synchronization is enabled:

• Department

76

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

• Job

• Location

• Grade

• Grade Ladder

• Manager

• Full Time or Part Time

• Regular or Temporary

• Assignment Category

• FTE and Working Hours

• Start Time and End Time

• Probation Period

• Union, Bargaining Unit and Collective Agreement

• Synchronize Mapped Flexfields

Position Changes
All active assignments that are synchronized from position automatically inherit changes from the position. Assignment
attributes synchronized from position automatically inherit changes from the position. For those attributes not
synchronized from position, you can either retain the existing values or update values from the position.

The Review page in the Edit Position page displays the list of impacted assignments with a status for each assignment.
The status indicates if there are any issues due to the position change. You must correct all errors before submitting the
position changes.

Assignment Changes
When you change the position in existing assignments you have a choice whether to inherit the values for those
attributes which aren't synchronized from the position. If you choose not to inherit, then the previous values remain
unchanged.

Position Synchronization Configuration Changes
If the position synchronization configuration is changed after person and assignments are created, then the
Synchronize Person Assignment from Position process must be run to apply the changes in assignments.

Position Hierarchy Configuration Changes
When the manager is synchronized from the HCM position hierarchy and you change the parent position, all
assignments inherit the new manager from the current parent position. When you remove a position from the hierarchy,
all child positions move one level up in the hierarchy. Hence, the grandparent position is the new parent position.

The incremental flattening process is triggered when you add or change a parent position. The flattening process will
update the changes in the position hierarchy.

When you change the position in an existing assignment, the manager value is updated based on the parent position of
the changed position. If the parent position doesn't have an incumbent, the incumbent in the position in the next level
up in the hierarchy is the new manager.

77

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Uploading Changes Using HCM Data Loader and Workers REST API
When you create or update assignments using HCM Data Loader or Workers REST API, you can synchronize them from
positions. In this case, you must:

• Enable position synchronization before you load the assignments. If you enable it after the assignments are

loaded, then you can synchronize from positions for current and future dates only.

• Set the Synchronize from Position (Position Override) attribute on the employment terms or assignment

object to Y.

After loading the assignments using HCM Data Loader or Workers REST API, you must run the Synchronize Person
Assignments from Position process to synchronize the assignments.When you run the process, set the Past Period
to Be Considered in Days parameter to an appropriate value. For example, if you set this parameter to 60 days, then
any assignment records with start dates during the previous 60 days are synchronized from positions. By default, Past
Period to Be Considered in Days is set to 30 days.

Note:  If you're using the Compensation Workbench to promote your workers and have enabled position
synchronization, then after running the Transfer Workforce Compensation Data to HR process, you need to also
run the Synchronize Person Assignments from Position process. This will update the other synchronized position
attributes in the assignment.

Related Topics

• How Assignment Values Are Inherited from Position

• Synchronize Person Assignment from Position Process

Set Up Position Synchronization

Position synchronization is inheritance of values in an assignment from the values specified in the associated position.

You can enable position synchronization at the enterprise and legal entity levels using the Manage Enterprise HCM
Information and Manage Legal Entity HCM Information tasks (in the Setup and Maintenance work area) respectively.

Enterprise Level Setup
You can enable position synchronization either at the enterprise or the legal employer levels. Select the Enable Position
Synchronization attribute in the Edit Enterprise page to enable position synchronization for the enterprise. By default,
this attribute is deselected. You can also specify whether the inherited values can be overridden at the assignment level.

If you enable position synchronization at the legal entity and the enterprise levels, then the settings specified at the
legal employer level takes precedence over the settings specified at the enterprise level.

Legal Employer Level Setup
Set the Enable Position Synchronization attribute to Yes in the Position Synchronization page to specify the attributes to
be configured with the position for the legal employer.

Select No for the Enable Position Synchronization attribute, to exclude a specific legal employer.

78

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

You can also use the same settings as defined for the enterprise. In this case, you must select the Use Enterprise
option, which is the default value. If position synchronization is configured at the enterprise level, then the assignment
inherits the attribute values from the position selected. You can also override these values at the assignment level.

Enabling Position Synchronization Post Setup
Here are the steps to enable position synchronization for the enterprise or legal entity post setup..

1. On the Home page, under My Client Groups tab, click the Show More link to access more quick actions.
2. Navigate to Workforce Structures > Manage Enterprise HCM Information page or Manage Legal Entity

HCM Information page.

3. Under Position Synchronization Configuration section, select the attributes that you want to synchronize.
4. Select the Allow Override at the Assignment option if you want to exclude an assignment from

synchronization.

5. Using HCM Data Loader, you need to update all assignments that you want to must be synchronized from the

position (as of the date you want to enable position synchronization).

6. Set the Synchronize from Position (position override check in HCM Data Loader) attribute on these

assignments to Y. This enables position synchronization even if you don't want to allow override at the
assignment.

7. Run the Synchronize Person Assignments from Position process to synchronize the assignments.

Related Topics

• Synchronize Person Assignment from Position Process

How Assignment Values Are Inherited from Position

If you enable position synchronization, assignments inherit specified values from the associated position. You can also
specify whether the inherited values can be overridden in the assignment.

You can specify this at the enterprise and legal entity levels using the Manage Enterprise HCM Information and Manage
Legal Entity HCM Information tasks respectively.

Overriding of Assignment Values
When you enable position synchronization, you specify which attributes the assignment inherits from the position
due to synchronization. Assignment attributes synchronized from position inherit their values from the position and
aren't editable. The restriction on editing values in the assignment applies only to the information that's entered in the
position. For example, if the Bargaining Unit isn't entered in the position, you can edit this value in the assignment even
though it's one of the attributes inherited from the position. If override is allowed at the assignment level, then you can
specify at the assignment level whether you want to synchronize from position or not. By default, the Synchronize from
Position attribute on the Edit Assignments page is set to Yes. If you prevent override at the assignment level, users can't
update the specified attributes that the assignment has inherited from the position. You can use personalization to
enable managers to specify a value for the Synchronize from Position field.

You can choose to either retain the existing values in the assignment or update the values from the position for any
attributes that aren't synchronized. So, if you don't select the grade attribute for synchronization and update the grade
value in the position, you can either retain the existing grade value in the assignment or update it from the position.

79

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

If a synchronized attribute is empty at the position, then this attribute won't be synchronized in the assignment. You can
enter any value for this attribute in the assignment. If a value already exists for this attribute, it will be retained and you
can change it to any other value.

Let’s see how assignments are impacted when position and position synchronization details are modified using
different applications.

Parameters

Responsive
Employment Flows

HDL or HSDL

REST

Request a Position
Change - Impacted
Assignments

Synchronize Person
Assignment from
Position Process

Position Attributes

Position Flexfields

Yes

Yes

Note:  Only if the
mapping is defined
for the assignment
flexfield.

Manager from
Position Hierarchy

Manager from
Position

Synchronize Reports
from Position
Hierarchy

Calculate FTE as per
Position Working
Hours

Yes

Yes

N/A

Yes

Yes

N/A

N/A

N/A

N/A

N/A

Yes

N/A

N/A

N/A

N/A

N/A

Yes

N/A

N/A

Yes

N/A

N/A

Yes

Yes

Yes

Yes

Yes

Yes

For example, if position synchronization is enabled and you change the position in the responsive employment flows,
all position parameters are synchronized except direct reports. If you load the position parameters changes using HCM
Data Loader (HDL), HCM Spreadsheet Data Loader (HSDL), or REST, then only the position attributes are synchronized.
The Synchronize Person Assignment from Position process updates all assignments irrespective of the application used.

These are some key points to note.

• Position attributes are synchronized irrespective of the application used for the update.

• Position flexfields are synchronized in responsive employment flows and when you run the Synchronize Person

Assignment from Position process. Flexfield data can also be updated in employment flows.

• Line manager is defaulted from the position hierarchy in employment flows, and when you run the Synchronize

Person Assignment from Position process.

• Line manager is defaulted from the position in employment flows, when there is change in the position, and

when you run the Synchronize Person Assignment from Position process.

• Direct reports can be synchronized only when you run the Synchronize Person Assignment from Position

process.

• The assignment FTE is recalculated when you change the standard working hours, and the FTE and working

hours are selected attributes for synchronization.

80

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

• FTE is calculated based on the position working hours in employment flows and when you run the Synchronize

Person Assignment from Position process.

For more information on the attributes that can be synchronized, refer to the topic Position Synchronization.

Note:  If you choose to specify your own values for an assignment, then that assignment won't be synchronized with
any future position changes.

How Position Synchronization Impacts Assignments

If you're using positions and have enabled position synchronization, then assignments will inherit values from the
associated position.

Any change in the synchronization configuration, position attributes, or the position hierarchy (manager) impact the
assignment. Let's look at some of the scenarios that impact assignments because of position synchronization

Scenario

Description

Initiating Object

Impacted Object

Change in Position synchronization
configuration on the Enterprise
HCM Information page

Change in position synchronization
configuration on the Manage Legal
Entity HCM Information page

Change in position hierarchy
configuration (manager from
position hierarchy)

Change in position manager

Change in position attributes

Change in position flexfields

You update the enterprise HCM
information and enable position
synchronization for certain
attributes such as job, department,
 location, and grade. Any change
in the above position attributes will
impact worker assignments.

You update the enterprise HCM
information and enable position
synchronization for certain
attributes such as job, department,
 location, and grade. Any change
in the above position attributes will
impact worker assignments.

Any change in the parent position
leads to the new manager
(incumbent of the new parent
position) being assigned to all
incumbents associated to the child
position.

Any change in the position
manager leads to all incumbents
inheriting the new manager.

Any change in attributes such
as job, department, or any other
attribute, which is part of position
synchronization being updated on
the position leads to an update in
incumbent worker assignments.

Any change in position flexfields
(add or update), which are part of
position synchronization being
updated on the position leads to

Enterprise HCM Information

Assignment

Manage Legal Entity HCM
Information

Assignment

Position

Assignment

Position

Assignment

Position

Assignment

Position

Assignment

81

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Scenario

Description

Initiating Object

Impacted Object

Change in Full Time Equivalent
(FTE)

Change in manager's assignment
affecting direct reports

Change in worker assignment

an update in incumbent worker
assignments.

The new FTE is calculated based
on position working hours and is
synchronized in the incumbent
worker assignments.

If a manager is terminated, or
position change takes place on
manager's assignment, then the
assignment change of manager
impacts the direct reports'
assignments

Date-effective assignment splits
of workers assignment will be
synchronized based on the new
position's attributes

Position

Assignment

Assignment

Assignment

Assignment

Assignment

Related Topics

• Position Synchronization

• How Assignment Values Are Inherited from Position

• Synchronize Person Assignment from Position Process

Business Unit and Position in When and Why

Positions are specific to a business unit. You must select the business unit and the associated position in the When and
why step of Redwood employment processes instead of the Assignment step.

The business unit and position selection is moved from the Assignment step to the When and why step for these
reasons.

• Streamline execution of business rules based on business unit and position instead of doing this in the

Assignment step.

• Simplify the transaction when workers are managed using positions, as you have the ability to manage the

position upfront in When and Why step.

• The business unit attribute will always have a value whether it's available, by default (as in Add Person

processes) or hidden (as in update employment processes).

The business unit and associated position selection is available in these processes.

• Add Assignment

• Add Contingent Worker

• Add Nonworker

• Add Pending Worker

• Change Assignment

• Change Location

82

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

• Change Working Hours

• Correct Employment Details

• Create Work Relationship

• Edit Pending Worker

• Hire an Employee

• Local and Global Transfer

• Promote

• Promote and Change Position

• Transfer

Some key points to note about the business unit and position selection are as follows:

• The business unit and position attributes are read-only in the Assignment step. You can update these values

only in the When and why step.

•

If you change the business unit on the When and why step the second time, then you need to visit the
Assignment step as there may be attributes dependent on the business unit that become invalid on the change.

• You need to select the position again if you change the business unit.

Position Override in Redwood Employment Processes

In Redwood employment processes you can select the business unit and position relevant to the selected business unit.
Once you select the position, the Position override section is displayed in the employment processes.

In this section, the switch is disabled when position synchronization is enabled for an attribute.

• Set the switch to off when position synchronization is disabled, and you want to retain the value on the

assignment.

• Set the switch to on when position synchronization is disabled, and you want to override the value on the

assignment with the value on the position.

Here are some key points to note about the behavior of Union, Bargaining Unit, and Collective Agreement attributes in
the Position override step:

•

•

•

If you select Collective Agreement to be defaulted, then both Union and Bargaining Unit also get selected, by
default.

If you select Bargaining Unit to be defaulted, then Union gets selected, by default and you have the choice to
select or deselect Collective Agreement.

If you select Union to be defaulted, then you have the choice to select or deselect Bargaining Unit and
Collective Agreement.

Another point to note is that all position attributes will be displayed even if the values in the position and assignment
are the same.

83

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Behavior of Position Override

The Position Override step is displayed when a position exists in the When and why step of the Redwood employment
processes. Here we will learn about how it behaves in different scenarios.

Behavior of Position Override Step in Different Scenarios For Redwood
Employment Update Processes
This table lists the behavior of the Position Override step in different scenarios.

Scenario

Applies To

Application Behavior of Position Override
Step

No position exists in When and why step.

All update processes except Promote and
Change Position

Position Override step isn't shown.

Position exists in When and why step and
there's no change in position but there's change
in the existing position details in the Position
Details step.

Promote and Change Position

Position exists in When and why step and
there's no change in position.

All update processes

Position exists in When and why step and
there's a change in position.

All update processes

Position exists in When and why step and
there's no change in position but the position
was modified in the standalone page and
position synchronization isn't configured.

All update processes

Position Override step is shown and you
can default the attributes based on position
synchronization setup. The attributes show the
updated values from the Position Details step.

Position Override step is shown and you
can default the attributes based on position
synchronization setup.

Position Override step is shown and you
can default the attributes based on position
synchronization setup.

Position Override step is shown with the latest
attributes. The check boxes are deselected.
If you select a particular change row then
only that position value is defaulted to the
assignment.

User crosses the Position Override step.

All update processes

This step won't appear in the step navigation.

After reaching the Assignment step user revisits
the When and why step and removes the
position.

All update processes except Promote and
Change Position

Position Override step isn't shown and
assignment changes are retained.

After reaching the Assignment step user revisits
the When and why step and selects a position
(If previously null).

All update processes except Promote and
Change Position

After reaching the Assignment step user revisits
the When and why step and changes the
position.

All update processes

After reaching the Assignment step if the user
revisits the Position Details step and updates
the existing position details.

Promote and Change Position

Position Override step is shown and you
can default the attributes based on position
synchronization setup. The assignment
changes are retained except the changes
impacted by the position change.

Position Override step is shown and you
can default the attributes based on position
synchronization setup. The assignment
changes are retained except the changes
impacted by the position change.

Position Override step is shown and you
can default the attributes based on position
synchronization setup. The assignment

84

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Scenario

Applies To

Chapter 4
Jobs and Positions

Application Behavior of Position Override
Step

changes should be retained except the changes
impacted by the position change.

Edit by Approver

All the above scenarios are valid for edit by approver with the following deviation:

Scenario

Applies To

Application Behavior of Position Override
Step

Approver doesn't change the position.

All update processes

This step won't appear in the step navigation.

Behavior of Position Override Step in Different Scenarios For Add
Assignment
This table lists the behavior of the Position Override step in different scenarios for Add Assignment process.

Scenario

Position Exists in
Source Assignment

Position
Synchronization
Configuration

Allow Override at
Assignment Setting

Copy Data from
Source Assignment
Setting

Expected Behavior

User launches Add
Assignment

Yes

User launches Add
Assignment and
selects a position

No

Yes

Yes

N/A

Yes

No

No

No

Yes

Yes

No

User launches Add
Assignment and
selects a position

User launches Add
Assignment and
doesn’t change the
position

User launches Add
Assignment and
changes the position

Yes

Yes

Yes

Yes

Yes

Yes

Yes

Yes

The Position override
step appears in read-
only mode with
the synchronized
attributed selected.

The Position override
step appears in read-
only mode with
the synchronized
attributes selected.

The Position override
step should appear in
read only mode. With
the synced attributes
selected.

The Position override
step is enabled
and attributes to
be synchronized
(defaulted) from the
step are deselected.

The Position override
step is enabled
and attributes to
be synchronized
(defaulted) from the
step are selected.

85

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Scenario

Position Exists in
Source Assignment

Position
Synchronization
Configuration

Allow Override at
Assignment Setting

Copy Data from
Source Assignment
Setting

Expected Behavior

User launches the
Add Assignment and
selects a position

No

No

N/A

Yes

User launches Add
Assignment and
doesn’t change the
position

N/A

No

N/A

No

The Position override
step is enabled
and attributes to
be synchronized
(defaulted) from the
step are selected.

The Position override
step is enabled
and attributes to
be synchronized
(defaulted) from the
step are deselected.

Synchronize Assignment Action Reason From Position

You can synchronize the action reason in assignments with the action reason specified when a position is updated using
these flows and process.

• Update Position (from Position Details)

• Request a Position Change

• Synchronize Person Assignments from Position ESS process

The action reason is synchronized in the assignment if these conditions are satisfied.

• Position synchronization is enabled at the legal entity level.

• Action reason attribute is selected for synchronization in the position synchronization setup.

• Action reason is specified in the selected position.

• Synchronization from Position action has associated reasons configured.

• Action reason specified in the position is one of the reasons associated with Synchronization from Position

(ORA_POS_SYNC) action and to action of type Update Position (PER_POS_UPD)

• At least one of the synchronized attributes is updated in the position apart from action reason.

A point to note is that the action reason is synchronized only when the first position synchronization record is created in
the assignment. If there’s a correction in the position, then all changed attributes from position will be synchronized in
the assignment apart from the action reason.

How You Enable Action Reason Synchronization
You need to enable position synchronization at the enterprise or legal entity level. These are the steps to enable position
synchronization at the enterprise-level.

1. On the Home page, click My Client Groups > Workforce Structures.
2. Click the Manage Enterprise HCM Information task.
3. Click Edit > Update.
4. Click OK.

86

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

5.

In the Position Synchronization Configuration section, select Enable Position Synchronization and Action
Reason check boxes. Select any other attributes for synchronization.

6. Click Review to check your changes.
7. Click Submit.
8. Click OK.

After position synchronization is enabled, let's add action reasons to the Synchronization from Position and Update
position actions.

In the Action Reasons section, Click Associate to associate the action reasons with the action.

1. On the Home page, click My Client Groups  > Workforce Structures.
2. Click the Configure Actions task.
3. Search for Synchronization from Position (ORA_POS_SYNC) action.
4. Click Continue.
5.
6. Click Ok.
7. Click Submit.
8. Click Configure Actions task
9. Search for and click Update (PER_POS_UPD) action.
10. Click Continue in the Action section.
11. Click Associate and add the same action reason you added to the Synchronization from Position action, for

example, Promotion.

12. Click Ok.
13. Click Submit.

Example of Action Reason Synchronization in
Assignments

You can synchronize the action reason in the position with the action reason in the assignment. Let's understand how
this works with an example.

Position synchronization is enabled at the Global Business Institute enterprise level and department, job, full time or
part time, and action reason attributes are enabled for synchronization.

There are 3 positions - Architect, Sales Manager, and Director with these action reasons and jobs respectively.

Position Info

Position Name

Action Reason

Job

Architect

Sales Manager

Director

Promotion

Software Development

Organization Change

Sales Manager - SAAS

Assignment Change

Director - Operations

The Synchronization from Position action is associated with only promotion and Organization Change action reasons
and the Update Position action is associated with Assignment Change and Organization Change action reasons.

Action Reason Info

87

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Action

Associated Action Reason

Synchronization from Position

• Promotion

Update Position

Assignment Info

• Organization Change

• Assignment Change

• Organization Change

Person

Position

Job

Action Reason

Updated Job

John Doe

Architect

Software Development NA

NA

Updated Action
Reason

(no update in the
assignment action
reason)

Bonnie Vickers

Sales Manager

Sales Manager - SAAS NA

Software Development Organization Change

David Steward

Director

Director - Operations

NA

Software Development

(no update in the
assignment action
reason)

Action Reason Synchronization in Assignment

• John Doe - There is no update in the assignment action reason because none of the attributes were updated in

the Architect position.

• Bonnie Vickers - The Sales Manager position was updated with a new job and the action reason specified
in the position is Organization Change. The Organization Change action reason is associated with both -
Synchronization from Position and Update position actions. Since all conditions are met, the assignment is
updated with the Organization Change action reason.

• David Steward - Though the Director position was updated with a new job, but the action reason (Assignment
Change) wasn't updated in the assignment because the action reason is associated only with Update Position
action type and not the Synchronization from Position action.

Synchronize Assignment Flexfields From Position
Flexfields

You map position flexfields with assignment flexfields using the Manage Assignment Flexfields Mapping task in the
Functional Setup Manager.

Use the task to map assignment descriptive flexfield segments to position descriptive flexfield segments. Synchronizing
mapped flexfields includes the following steps:

1. Define flexfield mapping
2. Enabling flexfield synchronization
3. Synchronizing assignment flexfields from position flexfields

88

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Define Flexfield Mapping
To map flexfields, follow these steps.

Chapter 4
Jobs and Positions

In the Functional Setup Manager, click the Manage Assignment Flexfields Mapping task.

1.
2. Specify the following information.

Field

Description

Source Context

The context for the position descriptive flexfield. If you want to map a global position flexfield

segment, leave the source context blank

Source Segment

The position descriptive flexfield segment of the selected context or the global segment if the

context was left blank

Destination Context

The context for the assignment descriptive flexfield you want to map the position flexfield to.

If you want to map it to a global assignment flexfield segment, leave the destination context

blank.

Destination Segment

The assignment descriptive flexfield segment of the selected assignment context or the global

segment if the context was left blank.

Enterprise Configuration: Enable

Specify whether you want to use this flexfield mapping for position synchronization for the

Position Synchronization

enterprise. Leave this field blank if the flexfield mapping applies to a specific legal employer.

Legal Employer Configuration: Legal

Use this option if the flexfield mapping doesn't apply to the enterprise. You can select multiple

Employer

legal employers. Select the legal employer.

Legal Employer Configuration: Enable

Specify whether you want to use this flexfield mapping for position synchronization for the

Position Synchronization

selected legal employer.

3. Add more mappings as required and specify information described in step 2 for each row.
4. Save the mapping.

Enabling Flexfield Synchronization
To enable flexfield synchronization, follow these steps.

1.

In the Setup and Maintenance work area, click the Manage Enterprise HCM Informationtask to enable the
setting for the enterprise, or click the Manage Legal Entity HCM Information task to enable the setting for a
specific legal entity.

2. Click Edit and select Update.
3. Select the Enable Position Synchronization and Synchronize Mapped Flexfields check boxes in the Position

Synchronization Configuration section.

4. Click Submit.

89

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Synchronizing Assignment Flexfields from Position Flexfields
To synchronize assignment flexfields from position flexfields, follow these steps.

In the Navigator, click Scheduled Processes.

1.
2. Click Schedule New Process.
3. Run the Synchronize Person Assignments from Positions process.

Related Topics

• Position Synchronization

• Considerations for Flexfield Mapping in Position Synchronization

• Synchronize Person Assignment from Position Process

Considerations for Flexfield Mapping in Position
Synchronization

You map position descriptive flexfields to assignment descriptive flexfields using the Manage Assignment Flexfield
Mapping task in Oracle Fusion Functional Setup Manager.

Use this mapping to automatically populate values for those assignment flexfields mapped to the position flexfields,
when position synchronization is enabled. This topic describes what to consider when you're mapping flexfields.

Enterprise or Legal Entity Levels
Before you map flexfields, you must decide whether you want the mapping to be available for the enterprise or for
specific legal entities only. You can reuse a mapping across different legal entities. Settings at the legal employer level
takes precedence over enterprise settings, if both are specified.

You need to define the enterprise or legal employer mapping for each position flexfield segment by selecting each row
corresponding to the flexfield segment.

Note:  If you have defined position synchronization at the legal employer level and haven’t defined flexfield mapping
for a legal employer, the position flexfields won’t be synchronized at the assignment for that legal employer.

Context Specific or Global
You must decide whether to map context specific or global flexfield segments because you can't map a context specific
flexfield segment to a global flexfield segment. You can't map two or more segments of different contexts or multiple
position segments to the same assignment segment.

When you change the position value in an assignment, all synchronized global segments inherit the value from the new
position. You can manually update those segments that have a blank value in the position.

When you change the position value in an assignment, all context specific segments inherit the value from the new
position. If the new position has similar values to the old position and additional contexts defined, the assignments
retain the same values and inherit the additional values from the new position.

90

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Selecting and removing a position in an assignment makes the context and segments editable but the current values
aren't removed if they're synchronized from the position.

Numeric or Character
You can map flexfields of the same type (for example, numeric-to-numeric or character-to-character only), same
precision, and the same value set (same value set ID).

Related Topics

• Position Synchronization

• Considerations for Managing Descriptive Flexfields

Synchronize Person Assignment from Position Process

To synchronize the position changes with the affected assignments, run the Synchronize Person Assignments
from Position process. The Initialize Position Synchronization process to load position synchronization changes is
incorporated into the Synchronize Person Assignments from Position process.

The Synchronize Person Assignments from Position process is triggered in these scenarios.

Assignment

• Assignment update causing a date-effective split.

• Direct report assignment change because of change in assignment. This might be due to either position

change or termination of the manager.

Position

• Position update causing a date-effective split.

• Parent position change.

Position Synchronization Configuration

• Position synchronization configuration update either at the enterprise or the legal entity level.

Run the Synchronize Person Assignment from Position to:

• Update affected assignments in the enterprise or legal entity if position synchronization is enabled (either

initially or later, as a change).

• Prevent data corruption

• Synchronize the line manager based on the HCM position hierarchy.

• Synchronize action reason based on the position action reason and the available action reasons under

Synchronization from Position action.

• Update assignments affected by the position changes, uploaded using HCM Data Loader.

Note:  You must schedule this process to run on a regular basis. If you’re synchronizing the manager, then it's
recommended to run this process daily.

Use the Schedule New Process page in the Scheduled Processes work area to run the Synchronize Person Assignment
from Position process.

91

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Before you run the process, you must enable position synchronization on the Manage Enterprise HCM Information or
Manage Legal Entity HCM Information tasks in the Setup and Maintenance work area

Process Parameters
Past Period to Be Considered in Days

Number of days in the past to be considered for updating the attribute in the assignments. The default value is 30
days. Note that even if position synchronization was enabled in the past and you loaded position data with an effective
date of 6 months back, you don’t need to specify 180 days as the number of days. This is because the process detects
the effective date and the last updated date of the position data. You can enter 2 days as the parameter value though
changes are effective 6 months back.

Run at Enterprise Level

Select Yes to run the process for the enterprise, or No to run it for a specific legal entity.

Legal Entity

Legal entity for which you want to run the process.

Process Results
This process updates all affected assignments with the changes from the position. This includes:

• Changes due to position synchronization.

• Past or future-dated changes to the position hierarchy.

• Rollback of line manager changes in assignments for reverse termination.

• Line manager hierarchy changes

• Flexfield-mapping changes.

• Changes in position loaded using HCM Data Loader

HCM Position Hierarchy

Position hierarchy defines positions' relationships. The HCM position hierarchy is built based on these relationships.
You enable the HCM position hierarchy on the Manage Enterprise HCM Information page in the Setup and Maintenance
work area.

When you enable HCM position hierarchy:

• You can specify the parent position for a position on the Create and Edit Position pages in the Workforce

Structures work area. When you search for positions based on a parent position, it will show all child positions
for the specific parent position.

• You can also use the hierarchy to synchronize the line manager in the assignment from the line manager value

in the parent position.

• You can view the positions that are part of the HCM position hierarchy on the My Team page and view the

incumbents for a position.

• You can inactivate a position only if an incumbent with an inactive assignment exists.

92

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Note:  You can open the existing HCM Position Hierarchy from the Redwood Positions read-only page by clicking the
HCM Position Hierarchy option in the Actions drop-down menu.

Updating the Position Hierarchy
You can only correct the HCM position hierarchy. You can enable or disable the position hierarchy configuration by
flattening the existing hierarchy. You must run the Synchronize Person Assignments from Position process to flatten the
position hierarchy.

When the position hierarchy is flattened, then schedule to run the Synchronize Person Assignments from Position
process. This will apply the manager changes in assignments if the position hierarchy is changed after person and
assignments are created. The assignment changes can exist on the current date, date in the future, or in the past.

You can't change the position hierarchy configuration if the line manager is synchronized based on the HCM position
hierarchy. However, if line manager synchronization was configured as of a date in the past, then you can correct the
position hierarchy configuration.

Graphical Position Hierarchy

The HCM position hierarchy shows the relationship between positions and their parent positions. You can view and edit
the hierarchy on the HCM Position Hierarchy page, if your data security profile allows you.

You can identify a position's parent on the Manage Positions page if the Use HCM Position Hierarchy option is enabled
for the enterprise.

The nodes of the position hierarchy represent positions and parent positions. You can:

• Add child positions under a position either by creating a new position or by selecting an existing position as the

child.

• Create a copy of an existing position by specifying a new name and code. The rest of the information is copied

from the original position to the copy. You can change any information that you want.

• Edit the position.

• View the incumbent details including name, person type, person number, position entry and exit dates, and

their status as of the current date.

• Delete any position that doesn't have any incumbents or child positions.

In each position node, you can view:

• Position name and code.

• Business unit, job, department, and location.

• Number of incumbents for the position.

• Open Full Time Equivalent (FTE)

• Current incumbents in the position.

93

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

How You Create a Graphical Position Hierarchy

Vision Corporation is reorganizing its workforce and defining the hierarchy for all positions. You must create a position
hierarchy as shown here.

The following table summarizes the key decisions for this scenario.

Decisions to Consider

In this Example

Which business unit do these positions
belong?

Vision Corp. US

94

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Decisions to Consider

In this Example

What is the method for position code
generation?

Manual

You must do the following before creating the position hierarchy:

1. On the Manage Enterprise HCM Information page, enable HCM Position Hierarchy.
2. Ensure you have the Manage HCM Position Hierarchy privilege, which enables you to update the hierarchy.
3. Create the following positions -Executive Vice President, Vice President, Senior Sales Manager, and Senior

Operations Manager.

4. Display additional fields on the Create and Edit Position pages using personalization, if required.

Add a Parent Position to an Existing Position

1. On the My Client Groups tab, click Workforce Structures.
2. On the Manage Positions page, search and select the Vice President position.
3. On the Position: Vice President page, click Edit and select Update.
4. Select Reorganization.
5. Click OK.
6. Search and select the Executive Vice President position as the parent position.
7. Click Review.
8. Click Submit.
9. Click Yes.
10. Click OK.

Create a New Child Position

1. On the HCM Position Hierarchy page, click the orange arrow icon in the Vice President node and select Create

Child Position.

2. On the Create Child Position page, enter the following details:

Field

Name

Code

Job

Type

FTE

Headcount

Value

Sales Director

SALES_DIR

Director

Single Incumbent

1

1

95

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Field

Value

3. Click Save and Close.
4. For the Vice President node, repeat steps 1 and 2 using the following details:

Field

Name

Code

Job

Type

FTE

Headcount

5. Click Save and Close.

Value

Operations Director

OPS_DIR

Director

Single Incumbent

1

1

Add an Existing Position as a Child Position

In the Sales Director node, click the orange arrow icon and select Add Existing Position as a Child.

1.
2. Search and select the Senior Sales Manager position.
3. Click OK.
4. On the Edit Position: Senior Sales Manager page, click Save and Close.
5.

In the Operations Director node, click the orange arrow icon and select the Add Existing Position as Child
option.
In the Select Position window, search and select the Senior Operations Manager position.

6.
7. Click OK.
8. On the Edit Position: Senior Operations Manager page, click Save and Close.

Create Duplicate Positions

In the Senior Sales Manager node, click the orange arrow icon. and select Duplicate Position.

1.
2. On the Create Duplicate Position page, enter the following details:

Field

Name

Value

Sales Manager

96

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Field

Code

Type

FTE

Headcount

Value

SALES_MGR

Single Incumbent

1

1

3. Click Save and Close.
4.
5. On the Create Duplicate Position page, enter the following details:

In the Senior Operations Manager node, click the orange arrow icon. and select Duplicate Position.

Field

Name

Code

Type

FTE

Headcount

Value

Operations Manager

OPS_MGR

Single Incumbent

1

1

6. Click Save and Close.

Move the Sales Manager Node
You added the Sales Manager node under the Sales Director node instead of under the Senior Sales Manager node. You
can drag the node and drop it on the Senior Sales Manager node.

1. Select the Sales Manager node and drop it on the Senior Sales Manager node. The Sales Manager position

automatically becomes a child of the Senior Sales Manager position.

If you created a node in a wrong place, you can just drag and drop the node to the correct place. The hierarchy
automatically adjusts itself when you do so.

Review and Submit the Position Hierarchy Changes

1. On the HCM Position Hierarchy page, click Review. This page shows the positions that you added to the

hierarchy or the changes made to existing positions.

2. Click Submit.

97

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

3. Click Yes.
4. Click OK. If approval rules are set up, you'll be able to see the hierarchy changes after they are approved/

Parent Position Isn’t Defaulted for Professional Users

In the Request a New Position process and the Create Position page, the parent position is defaulted to the parent
position of the currently logged in user.

This helps managers as they often create a position in their team. A line manager requests a new position from the My
Team tab. In the Position details step of the process, the parent position is defaulted from the logged-in user.

For the professional user, it's less likely that the new position is within their own team. So the parent position isn’t
defaulted in the Request a New Position process if it’s opened from the My Client Groups tab. The parent position is
blank, and you need to select a value from the drop-down list.

Similarly, when a professional user creates a new position from the Positions quick action, the parent position isn’t
defaulted. In the New Position page, the parent position is blank, and it’s not defaulted to the parent position of the
currently logged in user. You need to select the parent position from the drop-down list.

Considerations for Using Position or Position Hierarchy
for Synchronizing Assignment Manager

To select a line manager synchronization option for the enterprise or for individual legal entities, use the Manage HCM
Enterprise Information and Manage HCM Legal Entity Information in the Setup and Maintenance work area respectively.
This topic discusses the line manager synchronization options available.

HCM Position Hierarchy
Use the HCM Position Hierarchy to synchronize the line manager on the assignment with the incumbent of the parent
position in the position hierarchy.

When there is a change in the position hierarchy, you need to run the Synchronize Person Assignments from Position
process to update the affected assignments. Alternately, when you update a position using the HCM Data Loader also
you must run the Synchronize Person Assignments from Position process for the assignments to inherit the position
changes. For example, if a position is moved under a different parent position, if there are any direct reports they're
automatically reassigned to the incumbent in the new parent position. If there is no manager in the parent position, the
application checks for the incumbent in the grandparent position, or until it finds an incumbent. If there are multiple
incumbents in a parent position, the incumbent with the longest tenure in the position is assigned as the new manager,
You can change the manager to the other incumbent on the Employment page.

If you move a position or remove it from the hierarchy, the grandparent position becomes the new parent position for
all the child positions. For example, if you have a hierarchy as follows: Manager (grandparent), Team lead (parent), and
Developer (child), and you move the Team Lead position to a different branch. The Manager position is the new parent
position for the Developer position.

98

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Note:  If you're using HCM position hierarchy, remove the function privilege for the Manage Position Trees task in the
Setup and Maintenance work area for your users. You can also hide the Manager field on the Create Position and Edit
Position pages using personalization if you synchronize the line manager using position hierarchy.

Position Manager
Use the position manager to synchronize the line manager on the assignment with the line manager defined for the
position. You can use this option if you're not using the HCM Position Hierarchy and want to manually maintain the
manager at the position. .

Related Topics

• Guidelines for Loading Positions

Filter Managers Using Parent Position Hierarchy

The Manager list of values (LoV) only displays the incumbents of the parent position when there are multiple
incumbents for the parent position.

This feature applies to responsive employment pages only when the legal employer or enterprise is set up to use
position hierarchy and the line manager is configured to be synchronized based on the position hierarchy.

These points summarize the behavior of the Manager LoV:

•

•

•

If there's no parent position, then the Manager LoV will display all the workers.

If there is only one incumbent in the parent position, then the incumbent is defaulted and the Manager LoV is
non-editable.

If there are multiple incumbents in the parent position, these conditions apply:

◦ The manager will be defaulted according to the setting of the

ORA_PER_POS_INCUMBENT_TENURE_ASG_SUP profile option.

◦ You can edit the Manager LoV. However, when you search the LoV, the search results will only show the

incumbents from the parent position, and those will be default search values.
◦ You can’t select any other person who is not an incumbent of the parent position.

•

If there are no incumbents in the parent position, these conditions apply:

◦ The application searches the position hierarchy until it finds a position with at least 1 incumbent.
◦ If it’s just 1 incumbent, then that person is populated as the manager and the field becomes read-only.
◦ If the delegate position field is populated on the vacant parent position, then the application doesn’t
search the normal position hierarchy to find the next higher position with an incumbent. Instead, the
application will use the delegate position to find the managers to populate.

Here are some points to consider for the feature of filtering managers using parent position hierarchy:

•

If the ORA_PER_POS_INCUMBENT_TENURE_ASG_SUP profile option is set to the default Longest tenure in
Assignment (LTA) value, then the Managers LoV will show both Active and Suspended assignments of the
incumbents. For all other profile option values, the LoV will only show active assignments of the incumbents.

99

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

• The feature will work in both database (DB) and Oracle Search version of the Worker LoV.

Note:  You won’t see some columns in the DB version of the Worker LOV (for example, Assignment Status).

Related Topics

• Considerations for Using Position or Position Hierarchy for Synchronizing Assignment Manager

• Employment Profile Options

How You Route Position Approvals

You can route position approval rules to incumbents in the parent position instead of just the initiator’s hierarchy.

The routing of approvals to incumbents in the parent position is for these processes:

• Create Position

• Edit Position

• Request New Position

• Request Position Change

The position approval can be routed to either All Parent Position Incumbents or to a specific Identified Parent
Position Incumbent.

Routing Options for Position Approvals

Routing Option

Description

All Parent Position Incumbents

Approval notification will be routed to all incumbents in the parent position.

Identified Parent Position Incumbents

Approval notification will be routed to only a specific incumbent in the parent position.
The incumbent to whom the approval will be routed depends on the value defined in the ORA_PER_
POS_INCUMBENT_TENURE_ASG_SUP profile option:

• Longest tenure in assignment

• Longest tenure in enterprise

• Longest tenure in position

• Shortest tenure in enterprise

• Shortest tenure in position

This diagram describes how position approvals work.

100

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

You can define the approvals to be routed to either all incumbents or only a specific incumbent in the parent position. To
route the approval to a specific incumbent only, you need to set the appropriate value in the profile option.

Examples of Tenure Calculation
Let’s look at how the tenure is calculated for the purpose of approval routing to a specific incumbent in some of these
scenarios.

1. Multiple Managers in Parent Position in Single Assignment and Assignment Changes

Two managers, Bob Price and Donna Smith are in the same position. The former spent the longest in the same
assignment and the latter spent the longest tenure in the enterprise but with changes in assignment.

Employee

Action

Date

Position

Status

Tenure

Comments

Bob Price

Hire

1-Jan-2009

Assistant Manager Active

12 years

Active in the
position for 12
years

Donna Smith

Hire

1-Jan-2000

Assistant Manager Active

Donna Smith

Change
Assignment

1-Jan-2005

Sales Analyst

Active

5 years

6 years

NA

NA

101

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Employee

Action

Date

Position

Status

Tenure

Comments

Donna Smith

Change
Assignment

1-Jan-2010

Assistant Manager Active

11 years

Adding the tenure
for the Assistant
Manager position,
16 years (11 + 5)

Even if the profile
value was set to
Longest Tenure
in Enterprise, the
approval will be
routed to Donna
Smith.

2. Multiple Managers in Parent Position in Single Assignment and with Inactive Assignment

Two managers, Bob Price and Jason King are in the same position. The former spent the longest in the same
assignment and the latter spent the longest tenure in the enterprise but was transferred to a different legal employer
(global transfer).

Employee

Action

Date

Position

Status

Tenure

Comments

Bob Price

Hire

1-Jan-2009

Assistant Manager Active

12 years

Active in the
position for 12
years

Jason King

Hire

1-Jan-2005

Assistant Manager Active

6 years

NA

Jason King

End Assignment

31-Dec-2010

Sales Analyst

Inactive

NA

Jason King

Add Assignment

1-Jan-2010

Assistant Manager Active

11 years

The last day of
this assignment
is 31-Dec-2010.
The effective
start date of the
assignment's
inactive status is 1-
Jan-2011.

Adding the tenure
in the Assistant
Manager position
and removing the
overlap period, we
get:
16 years (6 + 11 - 1 )
years

(Overlap Removed)

3. Multiple Managers in Parent Position in Single Assignment and with Rehire

Two managers, Bob Price and Paul Smith are in the same position. The former spent the longest in the same
assignment and the latter spent the longest tenure same assignment and position even after being rehired into the
same position.

102

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Employee

Action

Date

Position

Status

Tenure

Comments

Bob Price

Hire

1-Jan-2009

Assistant Manager Active

12 years

Paul Smith

Hire

1-Jan-1995

Assistant Manager Active

6 years

Paul Smith

Termination

31-Dec-2000

Assistant Manager

Inactive

NA

Paul Smith

Rehire

1-Jan-2010

Assistant Manager Active

11 years

Active in the
position for 12
years

NA

NA

Adding the tenure
the person is
active in the given
position: 17 years
(6 + 11) years

Note:  If more than one incumbent fulfills the tenure criteria, then the person record creation date and time are
considered for approval routing.

Profile Option for Routing Position Approvals
The Identified Parent Position Incumbent option is based on the ORA_PER_POS_INCUMBENT_TENURE_ASG_SUP
profile option.

By default, this profile option is set to Longest tenure in assignment.

Use the Manage Administrator Profile Values task in the Setup and Maintenance work area to configure this profile
option. Search for and select the ORA_PER_POS_INCUMBENT_TENURE_ASG_SUP profile option. Select one of these
profile values as required, to meet your enterprise requirements.

Profile Option Value

Description

Longest tenure in assignment

The approval is routed to the parent position incumbent with the longest tenure in the assignment.
This option considers both, active and suspended assignments.

This is the default value.

Longest tenure in enterprise

The approval is routed to the parent position incumbent with the longest tenure in the enterprise. This
option considers only active assignments.

Longest tenure in position

The approval is routed to the parent position incumbent with the longest tenure in the position. This
option considers only active assignments.

Shortest tenure in enterprise

The approval is routed to the parent position incumbent with the shortest tenure in the enterprise. This
option considers only active assignments.

Shortest tenure in position

The approval is routed to the parent position incumbent with the shortest tenure in the position. This
option considers only active assignments.

103

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Route Position Approvals to the Representative of the Parent Position
Incumbent
You can also route position approvals to the representative of the incumbents of the parent position for these processes:

• Request New Position

• Request Position Change

• Edit Position

• Delete Position

• Delete Date Effective Position Record

Suppose you want to route the Request New Position approval to the representative of the incumbent of the parent
position. While configuring the approval rule for the Request New Position process, select the following:

• Representative in the Approvers list

• A value for Representative Type

•

Identified Parent Position Incumbent's Representative in the Representative Of LOV

Now, when you create a new position using the Request a New Position UI by associating a parent position which has
incumbents with representatives, the approval is routed to the Identified Parent Position Incumbent's Representative.

Related Topics

• Workforce Structures Profile Options

Jobs Search

As a professional user, you can use the Jobs Search that uses Oracle Search and a customizable interface for an
enhanced search experience.

Here's what you can do with the jobs search:

• Leverage Oracle Search to search for jobs quickly and easily.

• Use the name, code, and job family keywords to search for jobs.

• Filter the results using various department filters, for example, Effective Date, Status, Job Set, and Job Family.

• View the search results in a grid pattern and customize the grid columns.

• Navigate to the details page of a job from the search results where you can perform tasks depending on your

role.

For a filter category, the top 10 values are displayed in the LOV. If you don’t see the value that you need, you can start
typing the value in the LOV to find it. After you apply relevant filters, click the See Results button to view the filtered
data.

The fields listed under Hide are not shown in the results. If you want to view a field from this list as a column, you can
drag and drop it in the column configurator or select the check box next to the field.

104

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Positions Search

As a professional user, you can use the Jobs Search that uses Oracle Search and a customizable interface for an
enhanced search experience.

Here's what you can do with the jobs search:

• Leverage Oracle Search to search for positions quickly and easily. You can also find positions to change using

this search.

• Use the name, code, parent position, and incumbent keywords to search for positions.

• Filter the results using various department filters, for example, Effective Date, Status, Hiring Status.

• View the search results in a grid pattern and customize the grid columns.

• Navigate to the details page of a position from the search results where you can perform tasks depending on

your role.

For a filter category, the top 10 values are displayed in the LOV. If you don’t see the value that you need, you can start
typing the value in the LOV to find it. After you apply relevant filters, click the See Results button to view the filtered
data.

The fields listed under Hide are not shown in the results. If you want to view a field from this list as a column, you can
drag and drop it in the column configurator or select the checkbox next to the field.

Upload Workforce Structures Using a Spreadsheet

Using a spreadsheet, you can upload multiple objects at a time, for the following workforce structures:

• Jobs

• Locations

• Departments

For example, to upload multiple jobs at a time:

• Select Manage Jobs in the Workforce Structures work area

• Display the Create menu

• Select Create in Spreadsheet

Uploading Using a Spreadsheet
For each workforce structure, you can do the following:

• Download a predefined spreadsheet template from the application

• Work on the spreadsheet offline, and upload the spreadsheet to the application when your changes are

complete

• Upload the spreadsheet multiple times to accommodate revisions

105

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Effective Start Date
Ensure that the effective start date of the workforce structure is same as or earlier than the hire date of persons
associated with the workforce structure; for example, enter a job start date earlier than the hire date of persons
associated with the job. You may want to consider creating all objects as of a common early date, for example, create all
locations with the start date 1-1-1950.

Entering Descriptive Flexfield Values
Use the Attribute columns in the main sheet to enter values for the descriptive flexfields that are already defined for the
object. Use the DFF Reference sheet to understand which attribute columns map to which descriptive flexfields, since
this information isn't displayed in the main sheet.

Note:  You can't enter values in the DFF Reference sheet, you can only view details of the descriptive flexfields.

Uploading Jobs Using a Spreadsheet
When uploading jobs using a spreadsheet, you:

• Can't create a new job profile

• Can only associate an existing job profile

• Must enter the name of an existing job profile in the spreadsheet

Related Topics

• Guidelines for Using Desktop Integrated Excel Workbooks

FAQs for Jobs and Positions

What's the difference between a job set and a job family?

A job family is a group of jobs that have different but related functions, qualifications, and titles. They are beneficial for
reporting. You can define competencies for job families by associating them with model profiles.

A job set is an organizational partition of jobs. For example, a job set can include global jobs for use in all business units,
or jobs for a specific country or line of business. When you select a job for a position or an assignment, you can view the
available jobs in your business unit set and the common set.

Related Topics

• What's a job set?

106

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Why can't I see the position code for the new position?

Based on your enterprise settings, the position code is generated after the Create Position transaction is approved. For
example, once the transaction is approved, you can see the position code on the Position Details page.

When can I enable position synchronization?

You can enable position synchronization at any time but if there are existing assignments in an enterprise or legal
employer, you can enable it only as of the current or future date.

If you update an assignment as of a past date the values from the new position won't be updated in the assignment.
For example, if you create a transfer as of a past date before enabling position synchronization, the values from the new
position won't be updated in the assignment.

What happens if I specify a parent position?

You can specify a parent position when you enable HCM position hierarchy using the Manage Enterprise HCM
Information task in the Setup and Maintenance work area. A parent position is one, which is the next position up in the
position hierarchy.

On the Manage Positions page, click the parent position link to view the position details and click the icon next to the
parent position to refresh the search with the parent position.

As a prerequisite, you specify a parent position to synchronize the line manager from the parent position. When you
select to synchronize the line manager using the position hierarchy the incumbent in the parent position is populated as
the new manager.

Related Topics

• Position Synchronization

What happens if I specify the standard working hours in a
position?

In an assignment, the standard working hours are inherited from the position. The working hours and the standard
working hours provided in the position are used to calculate the FTE (Full Time Equivalent) in the assignment.

If there is a FTE value already existing in the position, you can choose to update it based on the ratio of the working
hours to standard working hours.

When position synchronization is enabled, even if FTE value exists for the position, it is not copied to the assignment
during synchronization. Instead, the assignment FTE value is calculated as a ratio of working hours to standard working
hours, if specified.

107

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

What happens when grades are synchronized?

The profile options to default or enforce valid grades are ignored when grades are synchronized.

If multiple valid grades exist at the position, then you can select an appropriate grade in the assignment. If you hire a
person into the position, which has an entry grade specified, then the entry grade will be the default value in case of
multiple valid grades.

If the assignment has both position and job, then synchronization from the position always takes precedence and the
values at the job will be ignored. Let's say you haven't defined any valid grades for the position. However, valid grades
are defined for the job and the assignment has a position. Then any valid grades for the job are ignored.

How can I exclude some assignments from position
synchronization?

If you want to use position synchronization only for a section of workers, you need to enable position synchronization at
the legal employer level.

To exclude some assignments from synchronization, select Allow Override at the Assignment in the Position
Synchronization Configuration section on the Manage Enterprise HCM Information page.

To exclude a specific assignment from synchronization, select No in the Synchronize from Position field in the
assignment (even if override is allowed). All read-only fields become editable but the assignment won't be synchronized
and will no longer inherit any changes made at the position level. However, it isn't possible to exclude only some
synchronized attributes.

How do I override position synchronization at the attribute level?

If you want to capture a different value for one attribute only, leave that attribute blank at the position

Let's say the location attribute is synchronized from the position but except in a few cases it doesn't matter into which
location the person is hired, then you can leave the location field blank at the position. Since blank values aren't
synchronized, the location will be editable in the assignment enabling you to select a value manually.

What happens if I select Synchronize Mapped Flexfields?

When you select this option, assignment flexfields are synchronized with the mapped position flexfields.

You must first map position flexfields to assignment flexfields using the Manage Assignment Flexfield Mapping task
in the Functional Setup Manager, and then select this option in the Manage Enterprise HCM Information task. When
position synchronization is enabled, the position flexfields are inherited in the assignments.

108

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

Are converted pending workers displayed as incumbents in the
Position Details page?

No. Converted or terminated pending workers won’t be displayed in the Past Incumbents, Future Incumbents, and
Current Incumbents sections of the Position Details page.

109

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 4
Jobs and Positions

110

Oracle Fusion Cloud Human Resources
Using Global Human Resources

5  Grades

Chapter 5
Grades

Grades, Grade Rates, and Grade Ladders

For more information about grades, grade rates, and grade ladders, see How do I set up grades, grade rates, and grade
ladders?

111

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 5
Grades

112

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

6  Person Information

Person Records

Person Records

All workers, nonworkers, and contacts have a single person record in the enterprise identified by a person number.

You can't create the person record in isolation because it requires one of the following:

• A current, past, or future work relationship with a legal employer

• A current, past, or future contact relationship with a person who has a work relationship with a legal employer

You never terminate a person record. It continues to exist through all of a person's work and contact relationships in the
enterprise.

You create the person record either

• When you create the person's first work relationship in the enterprise (for example, when you first hire the

person)

• Or when you add the person as a contact (for example, as an emergency contact) in another person's record.

Person Records Compared with Work Relationships
The following table compares Person Records and Work Relationship Records.

Information Type

Particulars

Person Records

Holds personal information such as:

• Name

• Date of birth

• Disability information

Work Relationships

Holds employment information such as:

May also apply to more than one work relationship such as National ID.

•

Job

• Payroll

113

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

Information Type

Particulars

• Working Hours

This can vary among work relationships and be specific to a legal employer.

Note:
A person's worker type (for example, employee) is derived from the person's work relationship;
it's not part of the person record. A person with multiple work relationships of different types has
multiple worker types.

Local Information in Person Records
In a single global enterprise, all users who have access to a person see the same person record, but the person record
can contain local variations of some information.

For example, the person record can contain the person's name in a local language and multiple national IDs. You can
also record some information, such as marital status, using terms that are most appropriate for each country in which
the person has work relationships. All local information is visible to anyone who can view the person record.

Access to Person Information
Having security access to a person record doesn't automatically allow access to all of a person's work relationships and
assignments.

For example, your access may be limited to specific legal employers, which may exclude some work relationships.

Related Topics

• Work Relationships

• Person Names and Languages

Examples of Person Records

Multiple people may be able to manage a person record, including human resource (HR) specialists in any of the
person's legal employers and the person to whom the record belongs.

The first of the following examples show how multiple people can manage the person record sequentially; the second
shows how multiple people can manage the person record simultaneously.

Updating the Person Record After a Break in Service
Miguel is an ex-employee of legal employer A in the United States. Today, Miguel starts a contingent worker work
relationship with legal employer B in Brazil, where you're the HR specialist.

114

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

When you attempt to add Miguel as a contingent worker, the application finds his existing person record; therefore, you
need only to create the contingent worker work relationship. You also update his person record as follows:

Details

Action Item

Miguel is married

Do the following:

• Enter his new marital status in the country information for Brazil

• Update his marital status in the US country information.

Miguel has a new emergency contact

Replace his previous emergency contact by doing the following:

• End date the previous contact relationship.

• Create a new one.

Contact relationship information is date-effective, which means you can retrieve his previous
addresses if necessary.

Miguel's address

Update his addresses. Address information is date-effective, which means you can retrieve his
previous addresses if necessary.

Miguel's national ID(s)

Add his Brazilian national ID, therefore the person record now holds two national IDs.

Miguel's local name

As Miguel is living and working in Brazil, you enter a local name using the Brazilian name format.

Miguel can review some of the information in his person record from the Personal Information work area; he can also
correct some information, such as his address, if necessary.

You have no access to legal employer A so you can't see Miguel's work relationship with legal employer A. If you need
more information about his previous work relationship, you must ask Miguel or his previous line manager to share this
information with you.

115

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

Managing the Person Record When Multiple Active Work Relationships Exist
Marie is French but lives in London, where she has an employee work relationship with legal employer A. She also has a
contingent worker work relationship with legal employer B in France. Marie has two contact relationships.

As the HR specialist for legal employer A, you manage Marie's employee work relationship. The HR specialist for legal
employer B manages her contingent worker work relationship. You can both manage all components of Marie's person
record. In addition, Marie can edit the following details in the Personal Information work area:

• Marital status and name

• Addresses

• Contacts

• Document records

• Phone numbers

• Email addresses

• Other communication methods

• Communication methods order of preference

A typical selection of updates to Marie's person record is as follows:

• Marie manages her own contacts and benefits information.

◦ She names her son as a dependent and her husband as an emergency contact.

• Marie manages her home address, which is also her primary mailing address.

◦ The enterprise has defined the address type Local Overseas.
◦ The HR specialist for legal employer B enters a Local Overseas address for Marie in France.

• The HR specialist in legal employer B enters a local name for Marie in French.

116

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

• You enter details of Marie's UK driver's license. The HR specialist in France enters details of Marie's French

driver's license and her passport. Marie can review and update this information.

• You enter Marie's UK national ID, and the HR specialist in France enters her French national ID.

• Both UK and French versions of Marie's marital status exist in her person record. When Marie's marital status

changes, she edits both versions.

Any HR specialist who manages Marie's person record can view, and edit any of this information.

Person Names and Languages

You can define how to display people's names in the application and in which language. You can define whether to
display a person's name in the global or the local language.

Person name has two parts, style and format.

Name Styles
The name style determines these things:

• Which components of a person's name to display. For example, one country may display first name and last

name while another may display the middle name too

• What's the order of display of the components

• Which components are required and which are optional. For example, title may be optional in some countries.

The legal employer sets the legislative context for the person record. So, if the legal employer is a Canadian
legal entity, the Canadian name style is used. When a country-specific name style doesn't exist, a universal
name style (last name, first name, title, and middle names) is used

Note:  A person's contacts have the same name style as the person for whom they're contacts.

Name Formats
A name format is an arrangement of the name components.

• The format is an arrangement of these name components: first name, last name, and title. You can choose from

these predefined name formats: Display name, List name, Full name, and Order name.

• The format can differ based on the display context. For example, in an ordered list of names, last name may

appear before first name, but in other contexts first name appears before last name.

Global or Local
The profile option HR: Local or Global Name Format controls whether users see local names or global names. The
profile option HR: Local or Global Name Format controls whether users see local names or global names by default.
Global names use one name format. Users who manage people across countries may want to see the names displayed
consistently so may use global names for example. Users who view or manage persons in a single country may prefer to
see local names

117

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

Person-Name Languages
Each enterprise has a global-name language. Person names appear in this language by default. When you create a
person record, you can define what language to use for the local name. Names appear in this language for users whose
HR: Local or Global Name Format profile option value matches the language.

Let's look at an example:

• The global-name language for the enterprise is American English.

• You set the local-name language in a person record to Japanese. Users whose HR: Local or Global Name Format

profile option is set to Japanese see the person's name in Japanese.

• All other users (those who are viewing global-format names or whose HR: Local or Global Name Format

profile option is set to a value other than Japanese) see the person's name in American English. Users can set
preferences to select the language in which they want to see person names displayed in.

Person Identifiers for External Applications

A person identifier captures third-party payroll identifier or the time device badge identifier details from an external
application for a person or an assignment.

You can configure person identifiers to capture additional information, for example, to track a person's parking pass
identifier, or track a person's previous Human Resources system person identifier. You add, modify and delete person
identifiers using the Person Identifiers for External Applications task in My Team and My Client Groups tabs.

It is optional whether you want to associate a person identifier with an assignment because the person may have only
one identifier in an external application. For example, a company assigns a badge to a person that grants access to all
the company's buildings. The person may have multiple assignments in the organization, but have only one badge and
one number in the building access system.

You can assign the same person identifier and identifier type only to one person at a time. This is because of integration
with time clocks and to avoid the same identifier being assigned to more than one person at a time simultaneously. If
you want to assign the same identifier to two people, then you have to specify an end date for the identifier for the first
person before assigning it to the second person.

Which person data can I delete?

You can delete person phone numbers, email addresses, and profile information. You can delete these person details
subject to restrictions.

• Employment

• Person and user details

• Person number

• Salary and compensation

• Benefits

You can't delete person names and person legislative data.

118

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

Delete a Person's Compensation and Benefits Data

To delete workforce compensation data (if the Transfer Workforce Compensation Data process wasn't run):

In the Compensation work area, click the Administer Workers task.

1.
2. Make the worker ineligible

To delete individual compensation data, you delete element entries and any stock grants

1. On the My Client Groups tab, click the Element Entries quick action .
2. Delete all prior and future-dated element entries created for awarded individual compensation plans.
3.
4. Search for the worker and delete all stock records.

In the Compensation work area, click the Stock Grants task.

To delete the total compensation statement:

In the Compensation work area, click the Purge Statements task.

1.
2. Select the Statement Definition Name.
3. Select the worker whose statement you want to delete.
4. Run the Purge Statements process for all statements generated for the invalid worker.

To delete salary data.

1. On the My Client Groups tab, click the Salary History task.
2. Search for the invalid worker
3. Delete the salary, starting from the latest record to the earliest one. This deletes the corresponding element

entries also.

To delete benefits data.

•

If a life event isn't created

In the Enrollment work area, click the Benefit Relationship task.

a.
b. Search for the person and delete the benefit relationships..
c. Cancel the work relationship.

•

If a life event is created

In the Enrollment work area, click the Person Life Events task.

a.
b. Search for the person and Delete any life events on the Potential Life Events tab.
c. Delete the benefit relationships and cancel the work relationships

•

If an enrollment records exist

In the Enrollment work area, click the Person Life Events task.

a.
b. Search for the person. On the Life Event tab, void and back out the life event. Click Save.
c.

In the Evaluation and Reporting work area, click the Processes tab, run the Purge Backed-out or Voided
Life Event Data process.
In the Enrollment work area, click the Benefit Relationship task.

d.
e. Delete the benefit relationships.
f. Cancel the work relationship.

119

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

How You Delete a Person's Employment Data

You can delete work relationships, employment terms, and assignment details using the Cancel Work Relationship
action on the Work Relationship page.

You can terminate a work relationship only if the person doesn't have any payroll, benefits or compensation results, and
direct reports. Also, you can terminate work relationship only if there is another active primary work relationship.

To cancel a work relationship.

1. On the My Clients Group tab, click the Cancel Work Relationship quick action.
2. Search and select the person whose work relationship is to be canceled..
3. Click Submit.

You can't access the person from the search results once you cancel the person's work relationship. If you try to rehire
the person by entering the same name, date of birth, and national ID, the person is identified as existing and available
for selection in the hire process

User Information
The Cancel Work Relationship action automatically removes a user's roles except the user account that remains active.

You must manage roles using other applications if they're assigned outside of Oracle Human Capital Management. You
can use Oracle Identity Manager, Microsoft Active Directory, and so on to manage these user roles. You must verify that
the person has no other work relationships. If there are other active work relationships, then you must retain the user
account but if there are no other active work relationships, then you can disable the user account outside of Oracle HCM
to prevent the user from logging in to the application.

Delete Person Number

You may want to delete a person's person number because you want to assign the number to another person.

You can't delete a person number but you can update it if the person number generation method is set to Manual. So,
you can change a person's person number to something different and make the original available for reassignment to
another person.

Here's how you can change the person number generation method to Manual if it's set otherwise.

In the Setup and Maintenance work area, click the Manage Enterprise HCM Information task

1.
2. Click the Go to Task icon.
3. Click Edit and select Correct.
4. Note the current Person Number Generation Method, as you must reset the value once done with the

procedure.

5. Change the Person Number Generation Method to Manual.
6. Click Submit.
7. On the My Client Groups tab, click the Personal Details action.
8. Search and select the person whose person number you want to change.
9. Change the person number and click Submit.
10. Once you change the person number, reset the Person Number Generation Method back to the original value

following steps 1-6.

120

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

Since the person number is a unique identifier, it's recommended that you cancel the work relationship and create the
new person with a new person number

Can I delete a person's mailing address?

Yes, you can delete a person's mailing address even if it's the only mailing address.

If the person has multiple mailing addresses, these points apply:

• You must first identify another address as primary before deleting the current primary address.

•

If one of the addresses has an effective end date as of the current date, you must first delete this address before
deleting the primary mailing address.

FAQs for Person Records

What's the difference between global names and local names?
The following table outlines the difference between global and local names.

Name Type

Global Names

Local Names

Description

Are in a format and language that can be understood throughout a multinational enterprise.

Are understood by users in a single country, but may not be understood throughout a multinational
enterprise.

You can have only one local name at a time. Select the local-name language that is most appropriate
for your primary assignment and reporting requirements. For example, if your home country is
Sweden, you may enter a local name in the Swedish language and format.

What happens if I change the local-name language of a person's name?
A person can have only one local name at a time.

If you change the language of the local name, the new local name replaces the existing local name. For example, if
you change a person's local-name language from Swedish to Greek, the Greek version of the person's name replaces
the Swedish version. Thereafter, users who have chosen to see names in Swedish will see the global version of the
person's name; only users who have chosen to see names in Greek will see the Greek version of the person's name. If
you use local names, select the local-name language that's most appropriate for the user's primary work relationship
and reporting requirements.

What's the effective start date?
Person attributes such as marital status and addresses are referred to as date-effective objects because they are likely to
change over time. When you change a date-effective object, the new change is inserted in the object's history. Typically,
you insert the new change following

121

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

What's the primary mailing address?
The address used by default for correspondence.

The home address is automatically the primary mailing address. To use a different address as the primary mailing
address:

1. Create the new address. This can be of any type; you need not define it as a mailing address.
2. Edit the primary mailing address to select the new address.

Note:
•

If you create a mailing address, that address doesn't automatically become the primary mailing address; you
must still select the new address as the primary mailing address.

• When you create an address, and make it the primary address, you need to close and reopen the Primary

Mailing Address section to see the new address.

Personal Information

Reviewing Your Personal Information

Review Your Personal Information
You can review and quickly update your personal information including addresses, emergency contacts, pay details,
compensation, and benefit details. Use this procedure to review and update your personal information.

1. On the Home page, click Me > Personal Information.
2. On the Personal Details page, click Edit to update your contact information and mailing address. The address
components are validated as per the geography validation and are completed automatically based on the ZIP
code selection.

3. Click the Employment Info tab to view your employment history.

Note:  You can only see information for your current assignment. For example, if you have been rehired, you
can't see information for your past assignments (before the rehire). Only an HR Administrator has access to
your past assignments.

4. Click the Document Records tab to add or modify your documents, such as certificates, and so on.
5. Click the Identification Info tab to view your visas and licenses.
6. Click the Contact Info tab to add or change your phone, email, and address..
7. Click the Family and Emergency Contacts tab to add or change the people to be contacted in case of

emergency,

8. Click the My Compensation tab to view your salary information.
9. Click Save and Close.

122

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

Change Your Photo

People can see your profile photo on your public information page, in the directory search results, and the global
header. You can have only one profile photo at a time.

1. Go to the Personal Details page in Redwood.

Note:  You can also update your photo using the My Photo page in general preferences. Click your user image
or name in the global header and go to Personalization > Set Preferences > My Photo.

2. Click Browse and select the photo to upload. Keep these points in mind when selecting the photo:

◦ The file size should be less than 20 megabytes.
◦ The preferable file format is .png or .jpeg though other image file formats are also supported.
◦ Ensure that the image dimension is 90 x 120 pixels to avoid distortion. If the image isn't of this

dimension, try maintaining an aspect ratio of 3 x 4.

Note:  If the photo appears rotated after upload, check the orientation of the camera when the photo is taken.
If the camera is left-bottom aligned, then you might face this issue. Rotate the photo four times to correct the
alignment.

3. Click Save and Close.

Disability Disclosure

You use the Personal Details page to capture your disability details. You can also specify if there are any specialized
equipment requirements.

When you create a disability record, you must select a country and category. Disability categories are predefined and
vary by country. You can update the list of values for the DISABILITY_CATEGORY lookup type, using the Manage
Common Lookups task in the Setup and Maintenance work area. You can also enter any reasonable accommodation
requests and upload attachments if you have any records to support the disability

Related Topics

• Person Records

How You Manage Contacts

You can add a new contact or identify an existing person as a contact in the Personal Information work area.

As a Human Resources (HR) specialist or an HR analyst, you can edit the personal information of a worker's contact if
you have the PER_CONTACT_PERSON_PII_MA NAGEMENT_DUTY role.

You can enter the national identifier information for correct identification of contacts with whom you have a personal
relationship: spouse, domestic partner, child, adopted child, foster child, and domestic partner child. You can manage
your dependents and beneficiaries using the Benefits page in the Personal Information work area.

123

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

Contact Relationships
The relationship start date is the date when the relationship takes effect. For example, if you enter your spouse as a
contact, enter your marriage date as the relationship start date. If you enter a relationship start date that's earlier than
the person's hire date, the contact start date is changed to the person's earliest effective start date. This is because a
relationship can't be earlier than the effective dates of the two related persons. A point to note is that the relationship
start date isn't stored in the application.

You can view the history of changes made to a contact relationship. If you delete the contact, the contact's own person
record continues to exist, but the contact relationship between the contact and person is deleted. If you end date the
contact relationship, the contact no longer appears in the person record from the specified date, but the history of the
contact relationship is still available.

As an employee, if you delete a contact on the Family and Emergency Contacts page, the application ends the contact
relationship but doesn’t delete the contact’s person record. A history of the contact relationship is still available. If you’re
an HR Specialist, you can either delete the contact relationship or specify an end date for the contact relationship.

How You Add Document Records for Contacts

Use the Family and Emergency Contacts page to add document records for a person’s contacts who don't have any
associated active or inactive work relationships.

When you delete a contact relationship, it doesn’t delete a contact’s document records. You can't add a document
record for a contact whose addition is pending approval. You can add if there are any changes pending approval for an
existing contact.

Security for the document records is based on the person and not the assignment. For example, a contact's document
records are retrieved based on the person's security profile and not the assignment-level security. You can create a
document type security profile and apply it to the role to control the visibility of certain types of document records.
Security defined for the person record applies for the contact record as well.

Here are some key points to note.

• For existing or terminated workers, you can upload documents from the main Document Records page.

• You can’t configure the Document Records action from the Transaction Design Studio.

• You can only use document types that aren’t assignment-based.

Contact Start Date Changes

You can change the start date of a contact on the Family and Emergency Contacts page.

These are key points to consider when changing the contact start date.

Contact Information

Current Scenario

Impact of the Start Date Change

Contact isn't a coworker or a shared contact

The new start date is a past date

All effective-dated objects, such as relationship,
name, address, visa or permit, and legislative
information, will be synchronized with the new
start date.

124

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

Contact Information

Current Scenario

Impact of the Start Date Change

Contact isn't a coworker or a shared contact

Effective-dated objects have effective-dated
changes that are after the new start date

Effective-dated object dates will be
synchronized with the new start date.

Contact isn't a coworker or a shared contact

Effective-dated objects have effective-dated
changes that are before the new start date

An error message will be shown and you
won't be able to make the change. You need
to remove the effective-dated changes before
changing the start date.

Contact isn't a coworker or a shared contact

Effective-dated object start date starts after the
original start date of the contact

Effective start date won't be synchronized.

Contact is a co-worker

The new start date is in the future

Contact is a co-worker

The new start date is in the past

Contact is a contact of another employee or
contingent worker

The new start date is in the future

Contact is a contact of another employee or
contingent worker

The new start date is in the past

The relationship start date will change but any
other effective-dated details of the co-worker
won't change.

The relationship start date will change but
any other effective-dated details of the co-
worker won't change. The new start date can't
be before the actual start of the co-worker's
original start date.

The relationship start date will change but
any other effective-dated details of the co-
worker won't change. The new start date can't
be before the actual start of the co-worker's
original start date.

The relationship start date will change but
any other effective-dated details of the co-
worker won't change. The new start date can't
be before the actual start of the co-worker's
original start date.

How You Share Data Access With Another Person

Use the Share Data Access action to give another person access to your data.

For example, during a transfer, the receiving line manager may need access to your information to initiate the transfer.
After you share access to your data, they can select your assignment to initiate the transfer.

A user with the Employee or Contingent Worker role can share access to their own data. A user with the Line Manager or
Human Resource Specialist role can share data access on behalf of a person who reports to them or a person available
through their person security profile.

When you share your data access, you have to share all your data and can’t choose which attributes to share. Access is
shared at the person-level and you can’t limit access to a single assignment for a person who has multiple concurrent
assignments. It may be useful to use the Notes field to capture details about the reason for the data sharing.

125

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

The recipient receives a notification with a link to the Person Spotlight of the person whose data is shared. Person
Spotlight contains a person’s public information, so most users will have access. Also, it may be a convenient launch
point for the recipient to take other actions, depending on the security configuration of their role. If recipients don’t have
access to Person Spotlight, they can still access the shared person data in other tasks. Share Data Access doesn’t give
the recipient access to any new tasks; it only updates the data security. The recipient can only view or edit the shared
person data using tasks that are already assigned to their role.

When data access is shared, it’s accessible until it’s revoked. You can revoke access to the data when it’s no longer
needed by returning to the Share Data Access action.

Related Topics

• Approval Rules for Share Data Access

• Guidelines for Securing Person Records

•

Include Shared People Information in a Person Security Profile

Approval Rules for Share Data Access

Use the Share Information approval rule to configure the actions so that workers are given the option to approve or
reject the request.

If a worker approves, the Share Information Approval FYI Notification approval rule is used to notify the requester and
the Share Information Reject FYI Notification approval rule is used when a worker rejects the request.

Once the request is approved, the recipient receives a notification indicating that data access or information has been
shared. Configure this notification using the Share Information FYI Notification approval rule.

Related Topics

• How You Share Data Access With Another Person

Bulk Revoke of Share Data Access

The Revoke Share Data Access process will revoke data security that was granted using the Share Data Access task.
This process automates the process of revoking data access that was previously shared.

You can revoke access in bulk by either the expiration date or creation date. To revoke access by expiration date, use the
Expiration Date field on the Share Data Access page to define the last day that the access is valid. Then, schedule the
Revoke Share Data Access process to run daily. The process will remove all records where the expiration date is before
the run date. For example, if you run the process on July 1, all records with an expiration date of June 30 or earlier will be
revoked. If the expiration date is blank, the access won't be revoked.

The Expiration Date field has been added only to the Redwood version of the page and it’s not a required field. So, you
may have records with a blank expiration date. If you have such records, you can revoke them based on the creation
date instead. You need to specify the number of days after the creation date, which the process uses to calculate an
expiration date.

For example, if you set the Number of Days to 15, the process will calculate the expiration date as 15 days after the
record's creation date. A record created on June 15 would have a calculated expiration date of June 30. If you run the
process on July 1, the record would be deleted because the calculated expiration date is earlier than the July 1 run date.

126

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

All records created before June 15 would similarly be deleted. All records created on or after June 16 would remain,
because their calculated expiration dates would be July 1 or later.

Note:  You need to be careful when you choose the Days after creation date option, because it may delete more
records than you intended. For example, if you set the Number of Days to zero, all records that are one day past their
creation date will be deleted. In other words, the only remaining records would be those that were created today. In
general, you can use this option to clean up historical records, or in combination with the Recipient parameter.

You can also choose to narrow the request to revoke the records only for a specific recipient. This feature is useful if the
recipient has moved to another role and no longer needs access to any records that were previously shared.

Steps to Perform Bulk Revoke of Share Data Access
You must run the Revoke Share Data Access process for the data access to be revoked. You can schedule it to run on a
regular basis, or run it ad-hoc.

1. Navigate to Scheduled Processes.
2. Click the Schedule New Process button.
3. Search for and select the Revoke Share Data Access process.
4. Choose a Run Type.

◦ If you choose Expiration date, the process revokes all records with the expiration date before the system

date.

◦ If you choose Days after creation date, the expiration date is ignored. The process calculates an

expiration based on number of days after creation date.
If Run Type is Days after creation date, specify the Number of Days.

5.
6. Optionally select a Recipient.

The recipient parameter will revoke only those records that were shared with the specified recipient.

7. Click Submit to submit the process.

Key Points About Bulk Revoke of Share Data Access
Here are some key points about Share Data Access.

• The Share Data Access task adds rows to PER_SHARE_INFORMATION, and the Revoke Share Data Access

process deletes them.

◦ No audit is done on the table.
◦ Once the data is deleted, it can't be recovered. But you can use the Share Data Access task to manually

add it again.

◦ The data in the table is used by the person security profile. If configured, your person security profile

includes the rows in the table when determining data security for your tasks.

• When Run Type is Days after creation date, the Expiration Date on the record is ignored. If the data meets the

criteria to be deleted based on creation date, it will be deleted even if the expiration date is in the future.

• Schedule the Revoke Share Data Access process so that it runs regularly. If you don't run the process, the access

won't expire even if the expiration date has passed.

• These functional privileges support bulk revoke of share data access:

◦ Run Revoke Share Data Access Process (PER_RUN_REVOKE_SHARE_DATA_ACCESS_PROCESS)
◦ Run Global HR Processes (PER_RUN_HR_PROCESSES_PRIV)

127

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

Note:  This privilege also gives access to other Global HR processes.

How National Identifiers are Validated

A national identifier is unique when it doesn't match any other national identifier in the application.

You can set up validation to check for the country-type-number combination by setting the Person Creation Duplicate
Check enterprise option to one of the options that contains these 3 attributes. For example, when you specify the option
National Identifier Country and National Identifier Type and National Identifier Number as the enterprise option, then
the check for national identifier uniqueness is done on national identifiers having these 3 attributes. A national identifier
- United States, SSN, 887-2234 will be considered unique to the national identifier - United Kingdom, SSN, 887-2234,
simply because the countries don't match even if the type and number are the same.

The national identifier is validated when you add a national identifier during any of the add new person processes or
while changing a person's information. The ID is also validated when you add it when creating a person record using any
of these services:

• Worker v2 service

• Worker REST service

• HCM Data Loader and HCM Spreadsheet Data Loader

A point to note is that Oracle Recruiting candidates aren't included in the check when a person record is created using
the methods mentioned earlier. However, the national identifier of these candidates can be checked against the national
identifiers of all non-candidates when they become pending workers.

Profile Option to Validate the National Identifier
You need to enable the National Identifier Uniqueness Validation Mode profile option to check if the national identifier
in a person record is unique. You can choose any of these values at the site-level.

Profile Option Value

Description

None

Warning

Error

The national identifier isn't checked for uniqueness.

A warning is displayed indicating the national identifier isn't unique. You can continue with the same
value however.

An error message is displayed preventing you from entering a national identifier, which isn't unique.

Duplicate Person Check
The duplicate person check identifies whether a person record is unique based on the first and last names, date of
birth, and national identifier. The national identifier validation checks for the uniqueness of the national identifier in the
person record. The differences between the two are indicated in this table:

128

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

Attribute

National Identifier Validation

Duplicate Person Check

How is it configured?

When is it triggered?

How does it work?

Configured using the National Identifier
Uniqueness Validation Mode profile option.

Configured using the Person Creation Duplicate
Check enterprise option.

When you create or update a person's national
identifier record (excluding Oracle Recruiting
candidates)

When you hire an employee, a contingent
worker, a nonworker, a pending worker, or
when a candidate is transformed into a pending
worker, depending on the configuration in
Oracle Recruiting.

Enabled using a profile option and checks
uniqueness of national identifier.

When enabled, each new or updated national
identifier record is checked for uniqueness
against the records of all other people
(excluding Oracle Recruiting candidates), to
show a warning or error to prevent the action if
a national identifier number is found to belong
to another person.

This is independent of national identifier
uniqueness validation. When enabled, each
new person record will first be checked for
any existing duplicate records. If any possible
duplicates are found, the user can decide
how to proceed. The definition of duplicate is
configured in the enterprise option, and can
include comparing the names, dates of birth,
 and even genders, or the national identifiers
and their countries and types.

Related Topics

• Candidate Duplicate Check and Merge After Job Offers

How Person Addresses Are Validated

When a user enters the postal code from the UI, the other corresponding address fields are updated automatically and a
validation is done to check whether the value entered is correct.

However, from REST and HDL, no such validation is done to check whether the geography hierarchy or the combination
of address values entered are invalid. For such scenarios, you can run the Validate Geographies of Addresses Against
Master Geographies ESS process with these parameters: Location Table Name = PER_ADDRESSES_F, Run Type = ALL,
Country Code. This ESS process will give the list of addresses that don't match the validation. You can then correct these
addresses.

Related Topics

• Guidelines for Loading Person Address

Comparing Items

Use comparison to quickly identify and evaluate differences between items. Compare any person, job, and position
items. For example, you can compare a person with another person or with a job profile.

You can compare items in the Profiles work area and on the talent review dashboard.

129

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

Selecting Items
The first item you select is the comparison base, and the items you select subsequently are secondary items. You can
change the comparison base if required. The comparison displays the base item attributes, and indicates the differences
between the attributes of the secondary items and the base items.

Controlling Results
Data sets control which attributes are displayed for each item in the comparison. For example, you must select the
School Education data set to display and compare a person's education details.

The information displayed in the comparison results is controlled by security access. For example, line managers can
compare their direct reports and view their performance data in the comparison results. HR specialists can perform this
comparison only if they have security access to the persons' performance information. You can change the effective
date of comparison if you're either a line manager or an HR specialist.

FAQs for Personal Information

Can I add additional data sets to the comparison?
No, you can only select from the list of data sets available for an item type.

Can I compare all of the person's assignments?
No, you can compare only the primary assignments of a person.

How are the differences between comparison attributes identified?
The differences are calculated between the attributes of the secondary items and the base item. Differences between
numeric values are calculated and displayed; character differences are indicated using an icon.

When the data includes a range (competency ratings, for example), the comparison displays the differences from
each end of the range. The comparison, however, doesn't display the differences for values that lie within the range.
For example, consider that you're comparing the competency requirements of two job profiles. The competency
requirement of the base job is between 2 and 4 and the secondary job is between 1 and 3. The comparison displays
the difference between the minimum competency requirement of the secondary job (1) and the base job (2) as -1.
The comparison doesn't display the difference between the maximum values because the maximum competency
requirement of the secondary job (3) lies within the competency requirement of the base job (between 2 and 4).

How is risk of loss assessed?
Line managers and human resource specialists enter the risk of loss information in a person's profile manually, there is
no automated risk assessment process.

They evaluate the risk of workers changing jobs or leaving the enterprise and select the ratings.

What happens if I remove the comparison base?
The next item in the comparison is automatically designated as the comparison base and the differences from the new
base item are indicated. Note that the comparison must always include a base item.

130

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

What's the difference between performing a best-fit analysis and comparing profiles?

Perform a best-fit analysis to find matching profiles for a specified profile using a wide variety of criteria. For example,
use best-fit analysis to find the top five person profiles matching a job profile, based on competency requirements,
language skills, and certifications.

Compare profiles to evaluate the similarities and differences between known profiles and identify the most suitable
profiles. For example, compare the five person profiles identified by the best-fit analysis and identify the person most
suited to the job.

To compare or perform a best-fit analysis, use the Compare action in the smart navigation.

Can I delete a person record?
No, but you may be able to cancel work relationships.

If you cancel a person's only work relationship, and the person has no contact relationships, the person record:

•

Is identified as associated with a canceled work relationship.

• Doesn't appear in directory searches.

Can I add multiple national identifiers of the same type for a country?
Yes, you can provided the date of issue of the national identifier is after the expiration date of the existing national
identifier. This means that the validity period of the national identifiers must not overlap.

You can also specify which of these national identifiers you want to set as the primary national identifier. However, if
there is only one national identifier specified, then this is automatically set as primary.

Why can't I see my passport document in the Passports section?
Your passport is created using the Document Records task. Although you can enter passport details in the Passports
section you can't upload any documents. You need to use the Document Records task to upload any documents.

How can I designate a contact as a statutory dependent?
You can specify whether a contact is a statutory dependent when you do these actions

• Add or edit a contact

• Add a contingent worker

• Add a nonworker

• Add a pending worker

• Hire an employee

• Create a work relationship

The Statutory Dependent field is used in legislative processes and reports. This field isn't displayed by default unless
delivered by a specific Oracle localization.

What's a disability disclosure?
You can disclose any disability using the Personal Information work area. You can also specify if you have any
specialized equipment requirements and add supporting documents as attachments.

131

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 6
Person Information

Why can't a line manager who’s rehiring see the person's existing home address?
Person objects such as address, national IDs, phones, emails, visas and permits, and so on that are personal identifiable
information (PII) are secured with data security privileges.

Line managers, by default, don't have the data security privileges to view or manage a person’s personal addresses
because it's PII. A line manager who's rehiring a person with an existing personal address can't see the existing address
because of the data security policies. They must have the required data security privilege to view the data on a page or
in OTBI.

132

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

7  Employment Information

List of Values in Employment Processes

List of Values (LoVs) in employment processes can be filtered based on certain criteria and are formatted on certain
parameters.

This table lists the LoVs and the formatting (querying attributes) and the filtering criteria for each.

LoV

Action

Action Reason

Add Directs Action

Add Directs Action Reason

Assignment Status

Bargaining Unit

Business Unit

Format

• Name

• Code

• Name

• Code

• Name

• Code

• Name

• Code

• User Status

• Code

• Name

• Code

• Description

• Name

Filtering Criteria

• Assignment Transaction Effective Date

• Action Type

• Country (of the selected worker

assignment's legal entity)

• Role (of the logged in user)

• Used on Contract (only for Employment

Contracts standalone page)

• Assignment Transaction Effective Date

• Action

• Country (of the selected worker

assignment's legal entity)

• Role (of the logged in user)

• Assignment Transaction Effective Date

• Action

• Profile option -

PER_LOV_SEARCH_ACTIONS_STARTSWITH

• Assignment Transaction Effective Date

• Action Type

• Profile option -

PER_LOV_SEARCH_ACTIONREASONS_STARTSWITH

• Assignment Transaction Effective Date

• Profile option -

PER_LOV_SEARCH_ASSIGNMENTSTATUSTYPES_STARTSWITH

• Assignment Transaction Effective Date

• Country Tags

• Union

• Status (Active/Inactive)

133

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

LoV

Format

Collective Agreement

• Name

• Code

• Country

• Bargaining Unit

Filtering Criteria

• Legal Employer

• Profile option -

PER_LOV_SEARCH_BUSINESSUNITS_STARTSWITH

• Assignment Transaction Effective Date

• Status

• Legislation

• Legal Employer

• Union (only in Redwood)

• Union

• Bargaining Unit

• Profile option -

PER_LOV_SEARCH_COLLECTIVEAGREEMENTS_STARTSWITH

Department

• Name

• Location

• Assignment Transaction Effective Date

• Status

• Title (only in Redwood)

• Business Unit (Set ID)

Grade

• Name

• Code

Grade Ladder

• Name

• Grade Type

• Profile option -

ORA_PER_LOV_COMPACT_DEPARTMENT_SEARCH

• Profile option -

PER_LOV_SEARCH_DEPARTMENTS_STARTSWITH

• Assignment Transaction Effective Date

• Status

• Business Unit (Set ID)

• Grade Ladder

• Profile option -

PER_ENFORCE_VALID_GRADES

• Profile option -

PER_LOV_SEARCH_GRADES_STARTSWITH

• Assignment Transaction Effective Date

• Status

• Profile option -

PER_LOV_SEARCH_GRADELADDERS_STARTSWITH

Grade Step

• Name

• Grade

Job

• Name

• Code

•

Job Family

• Assignment Transaction Effective Date

• Assignment Transaction Effective Date

• Status

• Business Unit (Set ID)

• Profile option -

ORA_PER_LOV_COMPACT_JOB_SEARCH

• Profile option -

PER_LOV_SEARCH_JOBS_STARTSWITH

134

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

LoV

Legal Employer

Location

Position

Format

• Name

Filtering Criteria

• Assignment Transaction Effective Date

• Legislation Code

• Profile option -

PER_LOV_SEARCH_LEGALEMPLOYERS_STARTSWITH

• Name

• Code

• Town or City

• Country

• Name

• Code

•

Job

• Department

• Assignment Transaction Effective Date

• Status

• Business Unit (Set ID)

• Legal Employer

• Employee Location Flag

• Profile option -

ORA_PER_LOV_COMPACT_LOCATION_SEARCH

• Profile option -

PER_LOV_SEARCH_LOCATIONS_STARTSWITH

• Assignment Transaction Effective Date

• Status

• Business Unit

• Hiring Status (based on ORA_POS_

HIRING_STATUS_FILTER profile option
value)

• Profile option -

ORA_PER_LOV_COMPACT_POSITION_SEARCH

• Profile option -

PER_LOV_SEARCH_POSITIONS_STARTSWITH

Reporting Establishment

• Name

• Assignment Transaction Effective Date

• Status

• Profile option -

ORA_PER_LOV_SEARCH_REPORTINGESTABLISHMENTS_STARTSWITH

Union

Manager

Lookup-based LoVs

• Name

• Country

• Avatar (only in Redwood)

• HR Status (only in Redwood)

• Name

• Business Title

• Work Email

• Person Number

•

• Name

• Assignment Transaction Effective Date

• Status

• Legislation

• Profile option -

PER_LOV_SEARCH_UNIONS_STARTSWITH

• Can be a worker type of either employee,

 contingent worker, or nonworker

• Displays only incumbents of the parent

position when position synchronization is
enabled to use HCM Position Hierarchy

• Can search for managers without having
to enter at least 3 characters in the LoV

• Sort manager based on manager type and

manager name

• Assignment Transaction Effective Date

135

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

LoV

Format

Filtering Criteria

• Country Tags

Assignments

Work Relationships

A work relationship defines how a person and legal employer are related.

The work relationship is created when you use any of these processes:

• Hire

• Rehire

• Global Transfer

• Global Temporary Assignment

• Create Work Relationship

You select the worker type and legal employer values when you create the work relationship of a person.

Note:  You can't change the worker type or legal employer after you create the work relationship. To change either
of these values, you need to cancel the work relationship and repeat the process to create the work relationship. For
more information, search for these document IDs on My Oracle Support: 1595810.1 and 1633860.1

Worker Types
Each worker type is denoted by its alphabet value in the ASSIGNMENT_TYPE and PERIOD_TYPE columns of the
PER_ALL_ASSIGNMENTS_M and PER_PERIODS_OF_SERVICE tables respectively. For example, pending worker is
denoted by P, employee by E, contingent worker by C, nonworker by N, and offer by O.

Worker Type

Description

Pending Worker

A person who will be hired as an employee or contingent worker and for whom you create a person
record prior to the hire or start date. When the hire is finalized, you convert the pending worker to the
proposed worker type.

You can create a pending worker work relationship in these scenarios:

• For a new worker, as part of their hire.

• For an ex-worker, as part of their rehire or renew placement.

• For an existing worker, as part of their new job in a different legal employer or for a different

worker type in the same legal employer.

In Redwood pages, the Include for Automatic conversion attribute is moved from Correct Employment
Details process to the Work Relationship process.

136

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Worker Type

Description

Note:
A pending worker work relationship can't be created for an existing worker who has a job offer in
Oracle Recruiting Cloud.

Employee

A person who typically has a permanent relationship with the organization.

Contingent Worker

A nonemployee, for example, contract worker or temporary worker.

Nonworker

A person having a nonwork relationship with a legal employer, for example, a volunteer or retiree. The
work relationship defines the details of the association.

Note:

• Nonworkers can't be selected as Department Managers or Cost Center Managers on the

Manage Departments setup page.

• Nonworkers aren't displayed on the position hierarchy.

• Nonworkers aren’t considered as incumbents on a position. So, the validation for number of

incumbents in a position doesn’t include nonworkers.

Offer

A person having an offer assignment in the organization.

Note:  This worker type is available only if you're using Oracle Recruiting Cloud and an offer is
created for the candidate.

Nonworker Types
You can't create new nonworker types. You can only associate an existing system person type as a nonworker type. You
can do this by adding the system person type lookup code as a lookup code in the PER_NON_WORKER_TYPES lookup
type. You can view the list of predefined system person types and lookup codes using the SYSTEM_PERSON_TYPE
lookup type. However, you can't add new lookup codes to the SYSTEM_PERSON_TYPE lookup type.

Primary Work Relationship
The primary work relationship and assignment are the most significant for a person in terms of working hours,
assignment status, pay, benefits, and many other aspects. When you need information about a person from a single
work relationship, you look at the primary work relationship. For example, when you need a single worker type for a
person for reporting purposes, the primary work relationship provides it.

Here are some facts about primary work relationships:

• A person can have only one primary work relationship. All other work relationships are nonprimary.

137

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

• A person's first work relationship is the primary relationship by default. An exception is the pending worker

work relationship that's created as nonprimary by default. If you're using Oracle Recruiting Cloud and create job
offers for candidates, then the offer work relationship is also created as nonprimary by default.

• When a person has multiple work relationships, the overall primary assignment is the primary assignment in

the primary work relationship.

•

If a person has multiple work relationships, you can't terminate the primary work relationship until you select
a different primary relationship. This restriction exists because a person can't be without a primary work
relationship at any time.

If a person has two work relationships, you can make their nonprimary work relationship as primary by using the Work
Relationship quick action on the My Client Groups tab.

Rehires
When a person leaves the organization, you terminate their work relationship. The work relationship becomes inactive
but the person record remains active. So when you rehire the person, the application identifies the person and lets you
select the existing person and create a new work relationship (for example, pending worker, employee, or contingent
worker).

Related Topics

• Worker Types

• Worker Numbers

• Examples of Creating Multiple Work Relationships for a Person

Worker Numbers

A worker number is an optional identifier for employee and contingent worker work relationships. A person with more
than one such relationship may therefore have multiple worker numbers.

Human resource (HR) specialists can enable worker numbers at the enterprise and legal employer levels, using the
Manage Enterprise HCM Information and Manage Legal Entity HCM Information tasks.

When You Enable Worker Numbers
Worker numbers become mandatory in all employee and contingent worker work relationships. If you enable the worker
number at both the enterprise and legal employer levels, then the setting at the legal employer takes precedence.

Ways to Allocate Worker Numbers
You can allocate worker numbers in these ways:

• Manually

• Automatically from a global sequence

• Automatically from a legal-employer sequence

You can select different number allocation methods for different legal employers. If you use a legal employer sequence,
worker numbers may not be unique in the enterprise. You can't change an automatically allocated worker number.

138

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Worker Numbers for Rehires
If you use a global sequence, the worker number doesn't change when you do these actions.

• Rehire in the same legal employer.

• Rehire in a different legal employer.

• Globally transfer to a different legal employer.

If you use a legal employer sequence, the worker number doesn't change when you rehire in the same legal employer.
However, the worker number changes when you rehire in a different legal employer or globally transfer to a different
legal employer.

Cancel Work Relationships

You can use the cancel work relationship process if you want to completely remove an existing work relationship
because of a business requirement. For example, you may need to cancel a work relationship in these scenarios:

• You want to remove a pending worker or employment work relationship when the worker doesn't join the

organization (no show).

• You want to change the start date or legal employer of a global transfer or global temporary assignment. Since
the application doesn't allow this change directly on the work relationship page, you must first cancel the work
relationship that was created as part of the global transfer or global temporary assignment. You can then redo
the global transfer or create a global temporary assignment using the date and legal employer you want.

• You want to change the worker type or legal employer of an existing work relationship. Since the application
doesn't allow this change directly on the work relationship page, you must first cancel the work relationship
that was created as part of the hire flow (Hire an Employee, Add a Contingent Worker, Add a Pending Worker, or
Add a Nonworker) or Create Work Relationship flow. You can then select another worker type or legal employer
and redo the transaction.

What Happens When You Cancel a Work Relationship
The application automatically does these actions:

• Deletes the work relationship and any associated assignments, and payroll, salary, and compensation records.

• Deletes the assignment-based document records if the appropriate profile option is enabled.

• Reinstates the previous work relationship status if the canceled work relationship was created as part of a

global transfer or global temporary assignment.

If you cancel a worker's only work relationship, the assignment and work relationship data is erased for the worker.
Therefore, it's not possible to retrieve the canceled transaction details from the PER_ALL_ASSIGNMENTS_M and
PER_PERIODS_OF_SERVICE tables. However, the record of this action is stored in the PER_ACTION_OCCURENCES table.
You can search for a person whose work relationship was canceled by querying this table. The PARENT_ENTITY_KEY_ID
column in the table stores the person ID of the person whose work relationship was canceled. The ACTION_CODE
column in the table has the ORA_EMPL_CANCEL_WR value for the canceled work relationship.

If you cancel a person's only work relationship, the application still retains the person record. Such records are available
to be selected during a rehire, but are excluded from general person searches.

139

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Scenarios Where You Can't Cancel a Work Relationship

• You can't cancel a work relationship that has a current, past, or future-dated termination. If any assignments in
a work relationship are included in a payroll run, you can terminate the work relationship but you can't cancel it.

• You can't cancel a pending worker work relationship after you convert the pending worker to an employee or

contingent worker.

•

•

If an employee or contingent worker work relationship is canceled after being converted from a pending worker,
the corresponding pending worker work relationship won't be reverse terminated.

In case of multiple work relationships, you can't cancel the work relationship which was primary at any point of
time.

• You can't cancel the work relationship of a person from which they are transferred to another legal employer on

a permanent or temporary basis.

• You can't cancel the work relationship if the associated assignments have a manager relationship at any point

of time in the work relationship.

• You can't cancel the work relationship if a time card exists for any assignments in the work relationship.
If a time card exists, the application stops the cancel process and displays an error message. If you don't
want the application to prevent cancellation of the work relationship when a time card exists, set the
ORA_PER_EMPL_DISABLE_TIME_CARD_CHK_CANCEL_WR profile option value to Y.

Record Additional Info When Canceling a Work Relationship in Redwood Page

• You can now select the action and action reason for canceling the work relationship in the When and Why step.

You can now configure multiple actions as a part of the Cancel Work Relationship action type.

• Additionally, the action occurrence extensible flexfield (EFF) is added in the Additional info section so that you
can store extra information while canceling a work relationship. This section is only shown when the pages are
created for action occurrences EFF. The Info Group LOV displays all pages created for the action occurrence
extensible flexfield (EFF).

Note:  The When and Why step is a mandatory step in Redwood page which can’t be hidden.

Reverse Terminate Pending Worker Work relationship in Redwood Page
You can automatically reverse terminate the pending worker work relationship when canceling the work relationship of
an employee or contingent worker who was previously a pending worker. Use the Reverse Terminate Pending Worker
When Employee or Contingent work relationship is canceled (ORA_PER_EMPL_REV_TERM_PWK_WHEN_CANCEL_WR)
profile option to do this. The default value for the profile option is No.

Reassign Direct Reports When Canceling a Work Relationship
You can reassign a manager's direct reports to another manager during the cancel work relationship process. If you
are trying to cancel the work relationship of a manager with direct reports, the Cancel Work Relationship page displays
the list of direct reports and their relationship start date. All assignment information and associated direct reports are
displayed grouped by the business title of each assignment in the work relationship. You can view the direct reports
details of the manager for the entire history of the selected work relationship across multiple assignments. For example,
HR specialists can view the direct reports for the manager and their manager relationship start dates for the entire
history of the manager's work relationship.

140

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

On the Cancel Work Relationship page, you can see the manager's direct reports details. From this page, you can move
the direct reports individually by clicking Change Manager corresponding to each direct report. Alternatively, can also
move the direct reports together if the manager relationship start date of the reports is the same.

Here are some points to consider when you reassign a manager's direct reports during the cancel work relationship
process:

•

•

If the manager relationship start date is different for direct reports, then the Change Manager quick action is
recommended.

If the manager relationship start date is same for direct reports, then the Direct Reports quick action is
recommended because you can reassign the direct reports in a single transaction.

• All direct reports having a relationship with the manager (for all manager relationships, such as line manager,

project manager, matrix manager, and so on) will be displayed.

•

If you click Change Manager for an individual direct report, the manager relationship start date is defaulted as
the effective start date in the When and Why section of the Change Manager page. However, if you select the
Direct Reports quick action to move a set of direct reports, the manager relationship start date isn't defaulted in
the Direct Reports page. This is because each direct report may have different start dates.

In Redwood page,

•

•

•

If a manager has more than one direct report and all direct reports have the same relationship start date, then
the Reassign Direct Reports button is automatically displayed so that you can reassign all reports at the same
time.

If the direct reports have a different relationship start date, then you need to reassign the reports using the
Change Manager button.

If a direct report is a pending worker, then you need to reassign the worker using the Edit Pending Worker
button.

• The relationship start date isn't defaulted while changing the manager or reassigning direct reports. You need
to use the relationship start date displayed on the Cancel Work Relationship page during these transactions.

•

If the person is a line manager in the offer assignment, then the cancel can't be completed unless that
association is removed.

Canceling the Work Relationship for Managers Synchronized from Position
If you have selected the manager to be synchronized from the position without the option to override, you can't correct
or remove the manager. This restriction is enforced by the application to prevent data corruption. You need to correct or
remove the manager before you cancel the work relationship. To correct or remove the manager, do these steps:

1. Remove the position on the manager's assignment record that has direct reports.
2. Run the Synchronize Person Records from Assignment process so that the application automatically removes

the manager relationship created due to an earlier position synchronization.

3. Cancel the work relationship of the manager.

Assignments

An assignment provides information about a person's role such as job, position, pay, compensation, managers, working
hours, and location.

141

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

HR specialists can create and manage assignments using the employment-related quick actions on the My Client
Groups tab. Line managers can create and manage assignments for their team members using the employment-related
quick actions on the My Team tab. Let's take a look at these aspects of assignments.

Work Relationship
A work relationship must have at least one assignment. Your legal employer may allow multiple assignments in one
work relationship.

Worker assignments are secured by assignment-level security. An HR specialist or line manager can access a worker's
assignment only if they have access to the assignment. For example, a line manager will only see assignments
of workers reporting to them. Similarly, an HR Specialist can access worker assignments only within their area of
responsibility.

For more information, see the document Implementing Assignment-Level Security in HCM (Doc ID 2700661.1) on My
Oracle Support (https://support.oracle.com).

Primary Assignment
You can access a person's information from a single assignment which is their overall primary assignment. If you need
information from a single assignment, you use the overall primary assignment. For example, some government reports
are based on one assignment only.

You must identify one assignment as the primary assignment in each work relationship. When a person has multiple
work relationships, the overall primary assignment is the primary assignment in the primary work relationship.

All work relationships must have at least one primary assignment. The following work relationship types are created as
nonprimary, however, the assignments within these work relationship types are still created as primary.

• Pending Worker Work Relationship

• Offer Work Relationship (if you're using Oracle Recruiting Cloud)

In this example, assignment C is the overall primary assignment because it's the primary assignment in the primary

work relationship.

Assignment Number
You can assign assignment numbers either manually or automatically. Assignment numbers are automatically
generated by prefixing the person number with these characters: E (for employee), C (for contingent worker), N
(for nonworker), P (for pending worker). For example, if the person number is 45678 and you hire the person as an
employee, their assignment number would be E45678. Subsequent assignments of same type have suffix numbers, for

142

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

example E45678-2, E45678-3. The suffix-number sequence is global and ensures that assignment numbers are unique
in the enterprise. If you assign numbers manually, you must ensure they're unique in the enterprise.

Assignment Status
The status determines whether the assignment is active, inactive, or temporarily suspended. It also controls whether the
assignment is eligible for payroll processing.

Some assignment actions you take automatically change the assignment status. For example, when you create an
assignment, its status is set automatically to Active - payroll eligible. You can change this status if you want.

Contract and Collective Agreement
Assignments can include contract details for information purposes, which some legal employers require.

You can link a collective agreement with an assignment if the bargaining unit, country, and legal employer of the
collective agreement and assignment are same. If you created a collective agreement without a legal employer or
bargaining unit, you can link the collective agreement with any assignment within the same country.

Projected Dates
These are the two types of projected dates:

• Projected Termination Date: This date field is stored in the PROJECTED_TERMINATION_DATE column of
the PER_PERIODS_OF_SERVICE table. You can use the field to track the projected termination date of the
work relationship. For example, you can use the field to track the projected end date of the global temporary
assignment.

• Projected Assignment End Date: This date field is stored in the PROJECTED_ ASSIGNMENT_END column of
the PER_ALL_ASSIGNMENTS_M table (non-terms record). You can use the field to track the projected end
date of the assignment. For example, you can use the field to track the projected end date of the temporary
assignment.

Note:  The projected date details are for information purposes only and have no effect on application processing.

Employment Primary Status Attributes

You can set the primary status for work relationships, work terms, and assignments by setting their status in the
PER_PERIODS_OF_SERVICE and PER_ALL_ASSIGNMENTS_M tables.

This table describes the primary status attribute available on the PER_PERIODS_OF_SERVICE table.

Primary Status Attribute Name

Description

PRIMARY_FLAG

A worker can have multiple work relationships, but only one must be identified as primary. If you
want to make the work relationship as primary, then set this attribute to Y. If there's only one work
relationship, then it will be primary by default.

The PER_PERIODS_OF_SERVICE table is not effective dated. Therefore, when there is a primary status
change in the work relationship, the value of the PRIMARY_FLAG is updated to reflect the latest
primary status. If you want to track the history of the primary status change at the work relationship
level, see the PRIMARY_WORK_RELATION_FLAG in the PER_ALL_ASSIGNMENTS_M table.

143

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Primary Status Attribute Name

Description

This table describes the four primary status attributes available on the PER_ALL_ASSIGNMENTS_M table.

Primary Status Attribute Name

Description

PRIMARY_WORK_RELATION_FLAG

A worker can have multiple work relationships, but only one must be identified as primary. If you want
to make the work relationship as primary, then set this attribute to Y at the work relationship level. If
there's only one work relationship, then it will be primary by default and the primary status is set in the
work terms and assignment also.

PRIMARY_WORK_TERMS_FLAG

For two-tier employment models, you don't have to identify the primary set of work terms as long as
you can identify the primary assignment. In two-tier employment models, this attribute is set to Y in
the employment terms record for the corresponding primary assignment. This primary status is only
set in the work terms.

PRIMARY_ASSIGNMENT_FLAG

A worker can have multiple assignments, but only one must be identified as primary. If you want to
make the worker assignment as primary, then set this attribute to Y at the assignment level. If there's
only one assignment, then it will be primary by default and the primary status is set in the assignment
also.

PRIMARY_FLAG

This overall primary attribute is an application controlled attribute and is set to Y for the primary
assignment of the worker's primary work relationship. This primary status is set at the assignment.

Let's take a look at an example to understand how the primary status options work.

Vijay Singh is hired on 1-Jan-2010 and he has only one work relationship and assignment record. Therefore, all the
primary attributes are set to Y at the respective levels.

Note:  In the table, the prefix E denotes employee assignment and ET denotes employee work terms.

Start Date

Work Relationship Assignment

Number

Primary Work
Relationship

Primary Work
Terms

Primary
Assignment

Primary

1-Jan-2010

WR1

E100

1-Jan-2010

WR1

ET100

Y

Y

N

Y

Y

N

Y

N

An additional nonprimary assignment is added on 1-Jan-2011. The additional assignment is added to the same
work relationship, therefore, the work relationship will continue to be primary for the newly added assignment. The
PRIMARY_FLAG, PRIMARY_WORK_TERMS_FLAG, and PRIMARY_ASSIGNMENT_FLAG flags will be set to N because the
newly added assignment is nonprimary and the employment model is two-tier.

144

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Start Date

Work Relationship Assignment

Number

Primary Work
Relationship

Primary Work
Terms

Primary
Assignment

Primary

1-Jan-2010

WR1

E100

1-Jan-2010

WR1

ET100

1-Jan-2011

WR1

E100-2

1-Jan-2011

WR1

ET100-2

Y

Y

Y

Y

N

Y

N

N

Y

N

N

N

Y

N

N

N

A nonprimary work relationship is added on 1-Jan-2012. Therefore, the PRIMARY_WORK_RELATION_FLAG will
be set to N because of the newly added nonprimary work relationship. The PRIMARY_ASSIGNMENT_FLAG and
PRIMARY_WORK_TERMS_FLAG will be set to Y because there's only one assignment for the newly added work
relationship. The PRIMARY_FLAG will be set to N as the assignment is part of the nonprimary work relationship.

Start Date

Work Relationship Assignment

Number

Primary Work
Relationship

Primary Work
Terms

Primary
Assignment

Primary

1-Jan-2010

WR1

E100

1-Jan-2010

WR1

ET100

1-Jan-2011

WR1

E100-2

1-Jan-2011

WR1

ET100-2

1-Jan-2012

WR2

E100-3

1-Jan-2012

WR2

ET100-3

Y

Y

Y

Y

N

N

N

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

N

Y

N

N

N

N

N

Change Indicator for Primary Attributes in Employment

You can change the primary indicator to make a nonprimary work relationship or assignment as primary in the
responsive Change Assignment flow.

Primary Work Relationship
Here are some points to consider when you change the primary indicator for the work relationship:

• You can make a nonprimary work relationship as primary by changing the primary indicator value from No to

Yes. However, you can't change the primary indicator value from Yes to No to make a primary work relationship
as nonprimary.

145

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

• You can't change the primary indicator value when there is a future change in the primary work relationship

status for a person.

Primary Assignment

Note:  The Primary Assignment field is hidden out-of-the-box on the responsive Change Assignment page. You must
use the HCM Experience Design Studio to enable this field.

Here are some points to consider when you change the primary indicator for the assignment:

• You can't correct the primary indicator, you can only update the indicator with a date effective update.

• You can make a nonprimary assignment as primary by changing the primary indicator value from No to Yes.
However, you can't change the primary indicator value from Yes to No to make a primary assignment as
nonprimary.

• You can change the primary indicator value from No to Yes, but after having changed the value, you can't

revert back to the No value. If you want to revert to the earlier value, you need to cancel and restart the Change
Assignment flow.

• You can't change the primary indicator value when future employment changes exist for the selected

nonprimary assignment or the current primary assignment.

• You can't change the primary indicator value when you perform the End Assignment and End Temporary

Assignment actions.

• You can't change the primary indicator value of an inactive assignment.

Related Topics

• HCM Experience Design Studio

Examples of Creating Multiple Work Relationships for a Person

When you create a person record, you also create that person's first work relationship. Once a person record exists, you
can create additional work relationships with the same or different legal employers.

You manage work relationships using the Work Relationship quick action on the My Client Groups or My Team tab. Let's
look at some valid combinations of work relationships.

Multiple Work Relationships of Different Types with a Single Legal Employer
These work relationships can exist at the same time with the same legal employer because they're of different types.

Work Relationship Type

Legal Employer

Start Date

End Date

Employee

Corporation A

17 November, 2010

None

Contingent Worker

Corporation A

4 August, 2010

12 January, 2012

Nonworker

Corporation A

4 August, 2010

None

146

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Work Relationship Type

Legal Employer

Start Date

End Date

Multiple Work Relationships of the Same Type with Multiple Legal Employers
These work relationships can exist at the same time, even though they're all of the same type, because each is with a
different legal employer.

Work Relationship Type

Legal Employer

Start Date

End Date

Employee

Employee

Employee

Corporation A

1 January, 2011

Corporation B

3 April, 2011

Corporation C

17 June, 2012

None

None

None

Multiple Work Relationships of the Same Type with a Single Legal Employer
These work relationships can exist with the same legal employer, even though they're of the same type, because they're
sequential. If you create the second work relationship before the first is terminated, it will fail.

Work Relationship Type

Legal Employer

Start Date

End Date

Employee

Employee

Corporation C

11 October, 2010

17 March, 2011

Corporation C

19 July, 2011

None

Multiple Work Relationships of Different Types with Multiple Legal Employers
These work relationships can exist at the same time because relationships with a single legal employer are of different
types.

Work Relationship Type

Legal Employer

Start Date

End Date

Employee

Corporation A

12 December, 2010

None

Nonworker

Corporation A

12 December, 2010

31 December, 2011

Contingent Worker

Corporation B

14 September, 2010

Employee

Corporation C

10 May, 2011

Nonworker

Corporation C

15 February, 2011

None

None

None

147

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Work Measures

Full Time Equivalent (FTE)
Work measures are ways of accounting for a worker's time on an assignment. Work measures are of two types: FTE and
Headcount. In this topic, let's understand some concepts related to FTE.

Derived Standard Working Hours
Derived standard working hours are usually those of a full-time worker. You define them for the enterprise, the legal
employer, the department, the location, the job, or the position. For example, if the standard working hours derived
from any of the work structure objects is 40 weekly, and you specify the assignment standard working hours as 50
weekly, the assignment standard working hours are considered for calculation of adjusted FTE.

If you define the standard working hours for more than one work structure, the application uses this hierarchy to
derive the standard working hours: Position > Job > Location > Department > Legal Employer > Enterprise, if a value is
specified.

You can specify the working hours for an assignment in these ways:

• Fixed hours: Enter the total hours for a week in the Working Hours field.

• Variable hours: In the Assignment Hours Details window, enter the worker's availability for each day. For
example, you can specify the start and end time of the worker's shift or the number of hours in the shift.

Working Hours
Working hours is an editable attribute in the worker assignment and you can specify a different value for each
assignment. This value is used in calculation of the FTE.

You can specify the working hours and standard working hours for a position. If a value is specified for the working
hours in the position, it’s defaulted in the assignment. Else, when you change the position, the working hours are
defaulted from the standard working hours hierarchy: Job > Location > Department > Legal Employer > Enterprise in
that order.

Assignment Standard Working Hours
Assignment standard working hours is an assignment level attribute, when specified will override the standard working
hours derived from the work structures. If specified, this attribute is used in FTE calculation instead of the derived
standard working hours.

Standard Working Hours Override (GB)
This attribute is applicable only for the Great Britain (GB) legislation. If you enter a standard working hours override, this
hierarchy is used to derive the standard working hours: Standard Working Hours Override > Position > Job > Location >
Department > Legal Employer > Enterprise.

If you enter a standard working hours override, this attribute is used to derive the standard working hours. The standard
working hours override frequency is considered to be the same as the assignment working hours frequency. If you enter
both the standard working hours override and the assignment standard working hours, then the standard working
hours override takes precedence.

If you're not using both attributes, then it's recommended you use the assignment standard working hours instead of
the standard working hours override attribute.

148

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

FTE
The FTE for a worker is calculated by dividing the assignment working hours by derived standard working hours. For
example, if the assignment working hours are 20 and the derived standard working hours are 40, the FTE for the
assignment is 0.5. If there are no standard working hours defined for the enterprise, legal employer, department,
location, job, or position, then the FTE value is 0 on the Assignment page. If the transaction is done from HDL or REST,
then an FTE record isn’t created in the PER_ASSIGN_WORK_MEASURES_F table.

The FTE is rounded off to 10 decimal points in the responsive employment pages.

Note:  When you're editing the FTE value in the classic Manage Employment page, it's rounded off to 10 decimal
points, for example 0.1254677897. However, when you're viewing it as a read-only field, it appears rounded off to 2
decimal points, for example 0.13. Any customizations you make to the FTE field doesn't affect this behavior. The FTE
value stored in the database uses a rounded decimal precision of 10 decimals.

Adjusted FTE
Work measures are ways of accounting for a worker's time on an assignment. Work measures are of two types: FTE and
Headcount. In this topic, let's understand some concepts related to adjusted FTE.

Standard Annual Working Duration
You define the standard annual working duration for the enterprise, legal employer, department, location, job, and
position.

This is an editable attribute. If this value is changed in the work structure, it’s updated in the assignment as well.

If you define the standard annual working duration for more than one work structure, the hierarchy to derive the
standard annual working duration is same as derived standard working hours.

Annual Working Duration
Annual working duration is same as the standard annual working duration. The duration may differ but the duration
unit is the same as the duration defined for standard annual working duration. This is an editable attribute and is used
in the calculation of the annual working ratio.

The annual working duration is defaulted only when a new assignment is added as part of an employment transaction.
For example, Add Assignment and Hire an Employee. In the update flows, annual working duration is retained from the
earlier record.

If there's a difference between the frequency of the derived standard annual working duration and annual working
duration, the frequency specified for the standard annual working duration is taken into consideration for calculation
of adjusted FTE and the annual working duration are set to null. However, while loading data using HDL, an error
message is displayed to use the same unit for the annual working duration as the derived standard working hours. If
the standard annual working duration isn't specified in any of the work structures, then the adjusted FTE and annual
working duration are set to null

Annual Working Ratio
This is a ratio of the annual working duration and the standard annual working duration. This ratio multiplied by the FTE
is used to calculate the adjusted FTE for an assignment.

The annual working ratio accepts up to 5 decimals. The annual working ratio is recalculated whenever there's a change
in the standard annual working duration and annual working duration irrespective of the Calculate FTE and headcount
automatically option value.

149

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

The ratio and the adjusted FTE will be 0 when either the annual working duration or the standard annual working
duration is null.

Note:  Post 23B upgrade, even if you're not using Adjusted FTE and Annual Working Ratio, these fields will be
populated with 0 value and will be displayed in Summary of changes section along with any assignment changes.
Since the values for these fields in pre-upgrade assignment rows will be null as these fields were added only in release
23B. These fields wont be displayed again in the Summary of changes section for subsequent assignment changes
unless you change the values for these fields.

Adjusted FTE
The Adjusted FTE is calculated by multiplying the FTE value with the ratio of annual working duration and standard
annual working duration. For example, a teacher works only 36 weeks annually, while the standard annual working
duration is 52 weeks. The working hours and standard working hours are 20 and 40 weekly respectively, hence the FTE
is 0.5. The annual working ratio will be 36 / 52 and the adjusted FTE will be calculated as FTE * annual working ratio,
which is 0.5 * 36 / 52 = 0.346155.

The annual working duration and standard annual working duration are editable attributes and the application uses this
hierarchy to default these attribute values - position > job > location > department > legal entity > enterprise, in that
order, if a value is specified.

A key point to note is that the adjusted FTE is calculated when the Calculate FTE and headcount automatically option
is set to Yes and there's a change in any of these triggering attributes.

• Standard annual working duration

• Annual working duration units

• Annual working duration

• Annual working ratio

• Assignment standard working hours

• FTE

The adjusted FTE attribute accepts up to 10 decimals,

Example of Standard Annual Working Duration and Annual Working Duration
Defaulting in Assignment
You can default the standard annual working duration and annual working duration in the assignment from the position
> job > location > department > legal employer > enterprise in that order, if a value is specified.

In this example, we have 2 assignments – Assignment A1 and Assignment A2 that uses the work structures listed here.

This table lists the work structures and the respective standard annual working duration and annual working duration
values.

Work Structure

Standard Annual Working Duration

Annual Working Duration

POSITION- Application Engineer

JOB- Development

LOCATION-HYD

40 Weeks

50 Weeks

52 Weeks

20 Weeks

-

-

150

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Work Structure

Standard Annual Working Duration

Annual Working Duration

DEPARTMENT- Software Development

-

LEGAL EMPLOYER-IDC

ENTERPRISE-GBI

40 Weeks

35 Weeks

-

-

-

For example, if you're hiring an employee and adding an additional assignment, and you're using the following
information, the standard annual working duration and annual working duration will be defaulted as follows.

Assignment A1 - POSITION-Application Engineer, JOB-Development, LOCATION-HYD and DEPARTMENT- Software
Development

Assignment A2 - LOCATION-HYD and DEPARTMENT-Software Development

Attribute

Assignment A1

Assignment A2

Reason

Standard Annual Working Duration 40 Weeks

52 Weeks

Annual Working Duration

20 Weeks

52 Weeks

In assignment A1, a value exists in
position and job for this attribute
but the application defaults from
the position since it's higher in the
hierarchy.

In assignment A2, a value exists
in the location and legal employer
but the application defaults from
the location since it's higher in the
hierarchy.

In assignment A1, a value exists
in position and the application
defaults from the position since it's
higher in the hierarchy.

In assignment A2, there is no value
in the location or department.
Hence, the application defaults
from the standard annual working
duration.

Related Topics

• Workday Information Defaults

Headcount
The headcount value of a primary assignment in a work relationship is 1 and 0 for all other assignments within that work
relationship.

This is how it works.

151

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Number

Primary Work Relationship

Primary Assignment

Headcount

1

2

3

4

Yes

Yes

No

No

Yes

No

Yes

No

1

0

1

0

If you don’t provide the headcount value while creating a new assignment, then the application automatically sets the
value. This holds true for responsive employment UIs and the pending worker conversion process.

When You Edit Work Measures
In general, you don't need to edit work measures. However, you may want to enter a FTE value if no default value
appears.

Automatic Calculation of FTE and Headcount
Work measures are ways of accounting for a worker's time on an assignment. Work measures are of two types: FTE and
Headcount.

By default, work measures are calculated automatically for the worker when there's a change in the standard working
hours. The change in standard working hours can happen because of a change in position, job, location, department, or
legal employer.

In certain cases, you may not want the work measures to be automatically calculated. For example, you override the
FTE value of a contingent worker to zero. However, you don't want this manual override to be automatically recalculated
when there's a change in the worker's department. To retain the overridden value, you must clear the Calculate FTE
and headcount automatically check box on the worker's assignment.

This check box is hidden out-of-the-box for all flows except the Change Working Hours flow. By default, the value of
the Auto Calculate Work Measures attribute is Y. When the attribute value is Y or Null, the application automatically
calculates work measures. If you change this value to N by clearing the check box, the application doesn't automatically
calculate work measures and retains the user entered value.

If the Calculate FTE and headcount automatically check box is selected and you change a triggering attribute, the
application will populate the FTE value even if the calculated value is 0.

Note:  The value of the attribute is stored in the CALCULATE_WORKMEASURE_FLAG column of the
PER_ASSIGN_WORK_MEASURES_F table against the FTE row. For example, the table stores these values when the
value of FTE and Headcount is 1 and the Calculate FTE and headcount automatically check box is selected:

Assignment Number

Assignment 1

Unit

FTE

Assignment 1

Headcount

Value

1

1

CALCULATE_WORKMEASURE_
FLAG

Y

Null

152

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Conversion of Working Hours to Calculate FTE
If the frequency of standard working hours and assignment working hours are different, they're converted to the lowest
denominator frequency of hours in a day. This table shows you how the conversion is done to calculate FTE:

Frequency

Weekly

How working hours are converted

Assumption

Standard working hours * 0.2

40 working hours

Assignment working hours * 0.2

Biweekly

Standard working hours * 0.1

80 working hours

Assignment working hours * 0.1

Semi-monthly

Standard working hours * 0.093023256

88 working hours

Assignment working hours * 0.093023256

Monthly

Standard working hours * 0.046511628

176 working hours

Assignment working hours * 0.046511628

Yearly

Standard working hours * 0.003875969

2080 working hours

Assignment working hours * 0.003875969

Weekly Working Hours for Assignments

You can manage the weekly working hours for a worker's assignment from your employment flows. For example, you
can manage the weekly working hours in flows, such as Add Pending Worker, Transfer, and Change Working Hours.

Weekly Working Hours Section
You can use the Weekly Working Hours section to define the hours per day of the week for an employee according to
the requirements of their assignment. You can select the section along with other sections from the questionnaire page
of the flow you want to run.

The weekly working hours information is displayed in all relevant BIP and post approval notifications for each
employment flow. In case there are no weekly working hours defined, the notification won't display the weekly working
hours attributes.

Note:  The section is hidden out-of-the-box. You can enable the section in the responsive flow by using HCM
Experience Design Studio. For more information, see this Transaction Design Studio - What It Is and How It Works
(Document ID 2504404.1)

153

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Work Shift Type
There are two work shift types that you can select in the Weekly Working Hours section:

• Elapsed: When you select this type, you can record the hours for each working day.

• Time: When you select this type, you can record the start and end times for each working day.

The total working hours for each work shift type indicates if the working hours you entered is less or greater than the
designated assignment working hours for each week.

Points to Consider

• The Work Day Definition and Day Start Time fields are hidden out-of-the-box in the Weekly Working Hours

section. You can enable these fields using HCM Experience Design Studio.

• On the Employment Info page, the Weekly Working Hours section is collapsed by default, and will be displayed

only if the worker has weekly working hours data.

• When you delete the assignment, the weekly working hours data will also be deleted.

• When you delete the date effective assignment split, the corresponding date effective split of the weekly

working hours will also be deleted.

• The REST service doesn't support managing weekly working hours.

• The Weekly Working Hours section doesn't support flexfields.

• When you change the weekly working hours for any day in the responsive UI, the change doesn't affect the

Working Hours attribute. Therefore, the FTE doesn't change and remains the same.

• The Working Hours Type (Work Day or Frequency) field isn't available in the responsive UI. This field has been
removed from the Weekly Working Hours section in the responsive UI. This is because you can directly change
the Working Hours attribute in the Assignment section of the responsive UI for implementing working hours
type as frequency.

• The Weekly Working Hours section in approval notifications show the unit of time in hours only.

Related Topics

• Automatic Calculation of FTE and Headcount

• HCM Experience Design Studio

Assignment Attributes Based on Change Assignment Action

Some assignment attributes are displayed or hidden based on the action you select for the Change Assignment flow.
This table shows you the attributes:

Action

Displayed Attributes

Hidden Attributes

• SUSP_ASSIGN (Suspend Assignment)

Assignment Status

Job

• END_ASG (End Assignment)

• END_TEMP_ASG (End Temporary

Assignment)

Assignment Name

Department

Location

154

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Action

Displayed Attributes

Hidden Attributes

Business Unit

• PROBATION (Start Probation Period)

Probation Period

Job

• END_PROBATION (End Probation Period)

Probation End Date

Assignment Name

Department

Location

Business Unit

EXTEND_TEMP_ASG (Extend Temporary
Assignment)

Projected End Date

Job

DEMOTION (Demotion)

Job

Business Title

Grade

Assignment Name

Department

Location

Business Unit

Department

Location

Business Unit

These are some of the key points to note about the actions on the Redwood Change Assignment page:

• Suspend Assignment action isn't shown if the assignment status is suspended.

• End Probation Period action isn't shown if there's no earlier record of start probation period.

• Start Probation Period action isn't shown if there's already an earlier record with start probation period which

hasn't ended.

Business Title Defaulting for Assignment in Employment Flows

The assignment is identified with the business title and the title is defaulted from the job or position in responsive
employment flows using the ORA_PER_EMPL_DEFAULT_BUSINESS_TITLE_FROM profile option code.

Note:

• The business title for the Mass Legal Employer Change flow is defaulted from the source assignment

irrespective of the profile option.

• The business title for the Convert Pending Worker flows (Convert, Quick Convert, and ESS process) is defaulted

from the source pending worker assignment irrespective of the profile option.

This table shows how the business title is defaulted based on the profile option:

155

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Profile Option

Defaulting Behavior

Retain User Changes

This is the current application behavior where the business title is populated based on the worker's job
and the title changes automatically if there is a job change on the worker's assignment. However, if the
user manually updates the business title on the worker's assignment, the updated value is retained
even if there is a job change on the worker's assignment.

Automatically Update Based on Job
Change

The business title is populated based on the worker's job and the title changes automatically if there is
a job change on the worker's assignment. Even if the user manually updates the business title on the
worker's assignment, the changes are replaced with the new job value if there is a job change on the
worker's assignment.

Automatically Update Based on Position
Change

The business title is populated based on the position on the worker's assignment and the title changes
automatically if there is a position change on the worker's assignment. Even if the user manually
updates the business title on the worker's assignment, the changes are replaced with the new position
value if there is a position change on the worker's assignment.

This table shows the application behavior in the responsive employment flows based on the value configured for the
profile option:

Responsive Employment Flow

Behavior for Profile Option:
Automatically Update Based on
Position Change

Behavior for Profile Option:
Automatically Update Based on
Job Change

Behavior for Profile Option:
Retain User Changes

• The Business Title field is

• The Business Title field is

blank initially and defaults to
the job based on the value
selected in the Job field.

blank initially and defaults to
the job based on the value
selected in the Job field.

If no value is selected for the
Job field, the business title is
defaulted to the assignment
number at the time of submit.

•

If no value is selected for the
Job field, the business title is
defaulted to the assignment
number at the time of submit.

Add flows, such as Hire an
Employee.

Update flows, such as Promote and
Transfer.

• The Business Title field is
blank initially and defaults
to the position based on the
value selected in the Position
field.

•

•

•

If no value is selected for the
Position field, the business
title is defaulted to the
assignment number at the
time of submit.

If the position is changed, the
business title is defaulted to
the new position value.

If the position isn't changed,
 the previous business title
value is retained.

•

•

•

If the job is changed, the
business title is defaulted to
the new job value.

If the job isn't changed, the
previous business title value
is retained.

Correction flow, such as
Employment Details.

•

If the position is changed, the
business title is defaulted to
the new position value.

•

If the job is changed, the
business title is defaulted to
the new job value.

•

If the job is changed, these
things happen:

◦ The business title is defaulted
to the new job value if the
user hasn't overridden the
business title manually.
◦ If the user has manually
overridden the business title,
 the previous value of the
business title is retained.

•

•

If the job isn't changed, the
previous business title value
is retained.

If the job is changed, these
things happen:

◦ The business title is defaulted
to the new job value if the

156

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Responsive Employment Flow

Behavior for Profile Option:
Automatically Update Based on
Position Change

Behavior for Profile Option:
Automatically Update Based on
Job Change

Behavior for Profile Option:
Retain User Changes

Add Assignment (Permanent and
Temporary)

•

If the position isn't changed,
 the previous business title
value is retained.

•

If the job isn't changed, the
previous business title value
is retained.

• The business title is defaulted
from the source assignment.
If the position is changed, the
business title is defaulted to
the new position value.

• The business title is defaulted
from the source assignment.
If the job is changed, the
business title is defaulted to
the new job value.

•

If the user doesn't change
the defaulted business title,
 then -<number> will be
appended after the business
title at the time of submit.
For example, if the source
assignment business title is
Sales Manager, and the user
didn't make any changes
to the business title for the
new assignment, then the
new business title will be
Sales Manager -2 after the
user submits the transaction.
However, if the business title
already contains a hyphen (-),
for example, Sales - Manager,
then the number won't be
appended after the business
title.

•

If the user doesn't change
the defaulted business title,
 then -<number> will be
appended after the business
title at the time of submit.
For example, if the source
assignment business title is
Sales Manager, and the user
didn't make any changes
to the business title for the
new assignment, then the
new business title will be
Sales Manager -2 after the
user submits the transaction.
However, if the business title
already contains a hyphen (-),
for example, Sales - Manager,
then the number won't be
appended after the business
title.

•

If no value is selected for
the Position field, then the
business title will be defaulted
to the assignment number.

•

If no value is selected for the
Job field, the business title is
defaulted to the assignment
number.

user hasn't overridden the
business title manually.
◦ If the user has manually
overridden the business title,
 the previous value of the
business title is retained.

•

If the job isn't changed, the
previous business title value
is retained.

• The business title is defaulted
from the source assignment.

•

•

If job is changed on the new
assignment being added and
the business title value wasn't
overridden by the user in
the source assignment, the
business title is updated to
the new job value.

If the user doesn't change
the defaulted business title,
 then -<number> will be
appended after the business
title at the time of submit.
For example, if the source
assignment business title is
Sales Manager, and the user
didn't make any changes
to the business title for the
new assignment, then the
new business title will be
Sales Manager -2 after the
user submits the transaction.
However, if the business title
already contains a hyphen (-),
for example, Sales - Manager,
then the number won't be
appended after the business
title.

• The Business Title field is

blank initially and defaults to
the job based on the value
selected in the Job field.

•

If no value is selected for the
Job field, the business title is
defaulted to the assignment
number.

Local and Global Transfer (Global
Transfer and Global Temporary
Assignment)

• The business title is defaulted
from the source assignment.
If the position is changed, the
business title is defaulted to
the new position value.

•

If the position in the newly
added assignment and the
source assignment aren't the

• The business title is defaulted
from the source assignment.

• The business title is defaulted
from the source assignment.

•

•

If the job is different for the
newly added assignment, the
new job value is defaulted in
the business title.

If no value is selected for the
Job field, the business title is

•

If the job is changed on the
new assignment being added
and the business title value
wasn't overridden by the user
in the source assignment, the

157

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Responsive Employment Flow

Behavior for Profile Option:
Automatically Update Based on
Position Change

Behavior for Profile Option:
Automatically Update Based on
Job Change

Behavior for Profile Option:
Retain User Changes

same, the new assignment
position value is defaulted in
the business title.

•

If no value is selected for the
Position field, the business
title is defaulted to the
assignment number.

defaulted to the assignment
number.

business title will be updated
to the new job value.

•

If the job is different for the
newly added assignment,
 these things happen:

◦ The business title is defaulted
to the new job value if the
user hasn't overridden the
business title manually.
◦ If the user has manually
overridden the business title,
 the previous value of the
business title is retained.

•

If no value is selected for the
Job field, the business title is
defaulted to the assignment
number.

Display of Business Title for Multiple Assignments
You can identify and select the appropriate assignment by viewing assignment attributes in the Business Title list of
values (LOV) on the Employment Info page. Additionally, you can identify the required assignment in document records
by configuring additional assignment attributes to display in the Business Title LoV. This is the order of the attributes
available in the Business Title LOV:

• Business title

• Assignment number

• Legal employer

• Worker type

• Location (shows only if the value exists in the assignment)

• HR status (shows only if the assignment is suspended or inactive)

The attributes in the LOV are sorted first based on the HR status (in ascending order of Active, Inactive, or Suspended)
followed by the assignment creation date (in descending order of the latest date first).

For example, this is how the attributes look for a worker with an active assignment, suspended assignment, or inactive
assignment (with no location):

• For an active assignment: Manager Information Systems; E10101010; Vision Corporation; Employee; Alberta, CA

• For a suspended assignment: Management Consultant; E10101010-1; Vision Corporation; Employee; Alberta,

CA; Suspended - Payroll Eligible

• For an inactive assignment: Management Trainer; E10101010-2; Vision Corporation; Employee; Inactive - No

Payroll

Note:  The attributes are separated by a semicolon (;) in the LOV.

158

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

You can configure additional assignment attributes by using the REST LOV. These are the steps to enable the LOV:

• Set the ORA_PER_EMPL_ENABLE_WRK_ASG_REST_LOV profile option to Y.

• Use the Search Configuration in HCM Experience Design Studio to configure the Worker Assignment LoV.

This table shows the fields available for configuration and the fields that are displayed by default.

Field Name

Displayed by Default

Business Title

Yes (Search and Display)

Assignment Number

Yes (Search and Display)

Legal Employer

Yes (Search and Display)

Location

Yes (Search and Display)

Assignment Status

Yes (Display only)

Assignment Type

Business Unit

Position

Job

Grade

Department

Primary

Manager Name

No

No

No

No

No

No

No

No

Note:  If you enable the feature to configure additional assignment attributes, then the Business Title LoV will replace
the existing Business Title switcher on the Employment Info and Document Record pages. If you have personalized
the Business Title LoV using Page Composer, you need to redo the personalization.

These points summarize the behavior of the Business Title LoV:

• Displayed on the Employment Info page, only when the selected worker has more than 1 assignment.

• Lists assignments which are in any of these HR Statuses: Active, Suspended, Inactive.

• Lists all assignment types except the Offer assignment.

• Supports assignment-level security and lists only those assignments for the selected worker for which the

logged in user has access.

• The attributes in the Business Title LoV are sorted in this order:

◦ Active primary (Primary_Flag = Y, Primary_Assignment_Flag = Y)
◦ Active primary (Primary_Flag = N, Primary_Assignment_Flag = Y) Internal order by Assignment Creation

Date

159

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

◦ Active non-primary (Primary_Flag = N, Primary_Assignment_Flag = N) Internal order by Assignment

Creation Date

◦ Suspended primary (Primary_Flag = Y, Primary_Assignment_Flag = Y) Internal order by Assignment

Creation Date

◦ Suspended primary (Primary_Flag = N, Primary_Assignment_Flag = Y) Internal order by Assignment

Creation Date

◦ Suspended non-primary (Primary_Flag = N, Primary_Assignment_Flag = N) Internal order by Assignment

Creation Date

◦ Inactive - Internal order by Assignment Creation Date

Related Topics

• Employment Profile Options

Assignment Notes in Redwood Update Employment Processes

You can now record additional notes while making employment changes using the Redwood employment processes.

By default, the Notes field is hidden. You have to enable it using Business Rules. The Assignment Notes is a separate
fragment that's added under Assignment in Business Rules.

Here are some key points to note about this attribute

• Notes is a rich text field in which you can enter up to 4000 characters.

•

•

If you add an image to the rich text editor, it can use up the 4000 character limit if the image size is large.
Therefore, it's recommended to use only text or smaller size images.

In update processes, notes aren't copied from a prior date-effective record.

• You can delete notes using the Remove Person Information feature.

• Notes are stored in the per_assignment_notes table.

The Manager Hierarchy: How It's Maintained

In many situations, a person's manager hierarchy must be readily available. For example, a person's line manager
might be required during line manager security check, and business intelligence reports often retrieve data based on a
manager hierarchy.

How the Manager Hierarchy Is Maintained
A person's manager hierarchy could be derived from active data tables, but the impact of that approach on performance
is unpredictable. Therefore, the complete manager hierarchy for each person is extracted from data tables and stored
in a separate manager hierarchy table. This table is known as the denormalized manager hierarchy. The denormalized
manager hierarchy ensures that a person's manager hierarchy is both easily accessible and up to date.

160

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

These denormalized tables are populated during processing based on the source data in the
PER_ASSIGNMENT_SUPERVISORS_F table.

• PER_MANAGER_HRCHY_DN / CF – This table is required for evaluating line manager security, head counts, and

some flows in HCM are based on this table. It’s also used for the assignment list dimensions for OTBI.

• PER_MANAGER_HRCHY_REPORTEES_DN is specific to OTBI reporting only and for assignment manager

dimensions data.

When You Run the Refresh Manager Hierarchy Process
Whenever a change is made to a person's manager hierarchy through the application pages, the change is reflected
automatically in the denormalized manager hierarchy table. You use the Refresh Manager Hierarchy process to populate
the denormalized manager hierarchy table when person records are migrated from other applications.

How You Run the Refresh Manager Hierarchy Process
You run the Refresh Manager Hierarchy process in the Scheduled Processes work area. To run the process, you must
have the Human Resource Specialist job role. The process has no default schedule. You can run the process occasionally
to perform a complete refresh of the denormalized manager hierarchy. You can also specify a schedule to run the
process regularly. Refresh Manager Hierarchy processes all types of manager hierarchies.

You can run the process using these processing modes based on the parameter Updated Within the Last N Days value.

Updated Within the Last N Days

Mode

Details

No parameter value (Blank/NULL)

Normal - Full Run

+ve parameter value

Normal – Incremental Run

0 parameter value

OTBI – Full Run

Populates the denormalized tables PER_
MANAGER_HRCHY_DN and PER_MANAGER_
HRCHY_CF from the source of PER_
ASSIGNMENT_SUPERVISORS_F by executing
deletes and inserts of denormalized data for
ALL active assignment supervisor rows.
The minimum interval to run this process is 18
hours. If you schedule the process to run more
than once in 18 hours, it’ll be skipped.

Populates the denormalized tables PER_
MANAGER_HRCHY_DN and PER_MANAGER_
HRCHY_CF from the source of PER_
ASSIGNMENT_SUPERVISORS_F by executing
deletes and inserts of denormalized data for
assignment supervisor rows updated or created
in last N days (for example. if 5 is provided as
parameter value then data updated or created
in last 5 days will be processed).
The minimum interval to run this process is one
hour. If you schedule the process to run more
than once in one hour, it’ll be skipped.

Populates the denormalized table PER_
MANAGER_HRCHY_REPORTEES_DN from the
source of PER_ASSIGNMENT_SUPERVISORS_
F by executing deletes and inserts of
denormalized data for ALL the assignment
supervisor rows during processing and refers
to data of other denormalized tables PER_

161

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Updated Within the Last N Days

Mode

Details

-ve parameter value

OTBI – Incremental Run

MANAGER_HRCHY_DN and PER_MANAGER_
HRCHY_CF.

Populates the denormalized table
PER_MANAGER_HRCHY_REPORTEES_DN
from the source of
PER_ASSIGNMENT_SUPERVISORS_F by
executing deletes and inserts of denormalized
data for assignment supervisor rows updated
or created in last N days (for example, if -5 is
provided as parameter value then data updated
or created in last 5 days will be processed).

To improve performance, few additional parameters are introduced that are considered when running process with
NULL or 0 parameter value, that is, Normal – Full Run or OTBI – Full Run

Parameter

Values

Details

Ignore Inactive Assignments During Full
Refresh

Yes or No (Default Yes)

Ignore Historical Data During a Full Refresh

Yes or No (Default No)

If set to No, instead of processing only active
assignments supervisor data, it’ll process all
assignment supervisor data including inactive
assignments.

If set to Yes, instead of processing all
assignment supervisor data, will process only
current or future assignments supervisor data
and ignore historical (date effective) data of
assignment supervisor.

Normal denormalized tables (PER_MANAGER_HRCHY_DN and PER_MANAGER_HRCHY_CF) are automatically
synchronized when assignment supervisor data is created or updated from the application pages (New Hire,
Change Manager, and so on) or HDL. Automatic synchronization of denormalized data won't happen if Events
process is disabled, that is if, HRC: Disable HcmEvents Processing (HRC_DISABLE_HCM_EVENTS_PROCESSING)
profile is set to Y, or when assignment supervisor data being uploaded through HDL and in .dat file post
process task of RefreshManagerHierarchy is disabled using the setting SET DISABLE_POST_PROCESS_TASKS
RefreshManagerHierarchy, or due to SOA composite instances not getting triggered or infrastructure issues.

Guidelines for Running the Process
These are the guidelines to run the process.

• Normal Full Mode (parameter value of blank/NULL) can be run ad-hoc if denormalized data isn’t in

synchronization with source assignment supervisor data, or can be scheduled to run once every week (during
weekend) or daily once if more frequent full refresh is needed.

• Normal Incremental Mode (positive value) can be scheduled to run daily or multiple times (for example, 2-3

times) a day if needed, with parameter value, for example 1, all assignment supervisor data created or updated
in last 1 day will be considered for processing.

• OTBI Full Mode (parameter value of 0) and OTBI Incremental Mode (parameter value of -ve. For example,
-1 needed only if OTBI reports are based on assignment manager dimensions data. De-normalized table
PER_MANAGER_HRCHY_REPORTEES_DN doesn’t get synchronized automatically when assignment supervisor
data gets created or updated from the application pages or HDL. Process can be scheduled to run in OTBI Full
or Incremental mode once daily for populating data.

162

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

•

In addition to performing full refreshes of the manager hierarchy, you can perform incremental refreshes. With
this approach, you refresh the hierarchy based on manager changes occurring in the previous N days. Schedule
a full refresh every month or quarter and an incremental refresh every day or week, for example.

• You can select to run for a period of days since the last updated date, and you can exclude inactive assignment
and any historical data by selecting the Ignore Inactive Assignments and Ignore Historical Data options
when the process is run on Full mode.

Matrix Manager for an Assignment

An assignment can have a matrix manager or a dotted line manager in addition to a line manager. For example, an
employee may have an additional project or a separate compensation manager.

Matrix managers can use the matrix management functionality to view and track their employee's assignments similar
to a line manager.

How You Assign a Matrix Manager
To assign a matrix manager to an employee, do these steps:

In the Maintain Managers or Assign Managers section, click Add.

1. Navigate to any employment flow with the Manager section.
2.
3. Search and select the matrix manager in the Name field.
4. Select the manager type from the Type field, and then click OK.
◦ Note: You need to select a type other than line manager.

5. Repeat step 4 if you need to add another matrix manager.
6. Click Submit.

How You Can See the Employee in the Matrix Manager Hierarchy
Matrix managers don't see their matrix reports in the My Team work area because by default, only their direct reports
are displayed. To see their matrix reports, they need to use the search filters and filter by the manager type relationship
they have with the employee.

How You Can Add Custom Roles for Matrix Managers
You can use a custom role to only provide access to a specific type of matrix manager. For example, you can have
a custom role to restrict a manager's access to only those direct reports under the project manager hierarchy. By
having separate roles for each matrix manager, you can control how different matrix managers access employee
data. For example, a compensation manager should be able to see the salary of an employee, and not the project
manager. Similarly, a project manager should be able to transfer an employee from one location to another, and not the
compensation manager.

For more information about role-based security, see the Oracle Human Capital Management Cloud Securing HCM guide
on the Oracle Help Center (https://docs.oracle.com/en/cloud/saas/index.html)

Examples of Multiple Managers for an Assignment

You must define at least one line manager for an assignment. Optionally, you can add other manager types. Line
managers see the line-manager version of a person's spotlight and other restricted worker information.

163

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Other manager types can also see restricted worker information if their roles have the required security access.

Let's see some examples of assignments that need multiple managers.

Matrix Management in an Engineering Company
An engineering company uses a matrix management structure. An engineer reports to the lead engineer for everyday
functional guidance and to the operational manager for project assignment and tracking.

In this example, you define the lead engineer as the line manager and the operational manager as the project manager.
This is because the lead engineer interacts with the team members every day and evaluates their progress. The project
manager's role is restricted to assigning projects and tracking project completion.

Temporary Project Managers in a Service Company
A service company assigns workers to third parties to deliver contracted services. Each worker has a manager
whose primary task is to help the worker find their next assignment. The manager is common for all of the worker's
assignments. You define this manager as a line manager.

The worker also has a temporary project manager who manages a particular assignment but may not manage all of the
worker's assignments. You define the project manager as an additional manager (for example, as a project manager) in
relevant assignments.

Managers in a Global Company
A global company is organized functionally and workers report to a functional manager who may be in a different time
zone. You define the functional manager as the line manager for the assignment.

For day-to-day administrative purposes, such as approving leave or absence, each worker also has an administrative
manager. You define this administrative manager as an additional manager for the assignment.

How Line Managers Are Synchronized Using Position Hierarchy

You can enable position synchronization for the enterprise or legal entity, and synchronize the line manager value in the
assignment with the position.

You can synchronize using either the position tree or the HCM position hierarchy. Let's look at how line managers are
synchronized using the HCM position hierarchy.

Synchronize Line Manager for New Assignments
You create a new assignment and specify the position when you do any of these actions:

• Hire

• Add Assignment

• Temporary Assignment

• Create Work Relationship

• Global Transfer

• Global Temporary Assignment

• Local and Global Transfer

164

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

The line manager for the new assignment is synchronized based on the position hierarchy. Direct reports are also
assigned using synchronization, and displayed in the Add Direct Reports section. Here's how the synchronization
happens:

• The incumbent in the parent position is assigned as the line manager for the new assignment.

•

•

If there are any incumbents in the child positions, the incumbents are added as direct reports of the line
manager. If there is already an existing manager in the child position, this value is ignored and replaced with the
new manager.

If the new manager is hired for the same position as the existing manager, then the current manager will
remain.

Synchronize Line Manager for Existing Assignments
When you change the position in an existing assignment, the line manager is synchronized based on the position
hierarchy. Direct reports are reassigned based on the synchronization, and displayed in the Reassign Directs section.
Here's how the synchronization happens:

Note:  If a parent position doesn't exist or there are no incumbents in all the parent positions in the hierarchy, then
you can manually reassign the direct reports to other managers.

Related Topics

• Position Synchronization

• Synchronize Person Assignment from Position Process

Filter Locations Based on Legal Employers

The client-side Location list of values (LoV) is filtered based on the legal employer and displays only those locations
associated with the selected legal employer. The LoV is available in these responsive flows:

• Add a Pending Worker

• Edit Pending Worker

165

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

• Hire an Employee

• Add a Contingent Worker

• Add a Nonworker

• Create Work Relationship

• Local and Global Transfer

• Add Assignment

• Employment Details

• Change Assignment

• Promote

• Transfer

• Mass Legal Employer Change

• Change Location

Note:

• The locations are filtered first based on the business unit-set mapping and then by the legal employer.

• The Location LOV is filtered only by the legal employer you selected previously in the responsive employment

pages. The filtering is not a validation. Therefore, the filtering doesn't apply to REST API, HCM Data Loader, and
HCM Spreadsheet Data Loader.

Related Topics

• Associate Legal Employers with Locations

Filter Business Units Based on Legal Employers

The client-side Business Unit list of values (LOV) is filtered based on the legal employer and display only those business
units associated with the selected legal employer. The LOV is available in these responsive flows:

• Add a Pending Worker

• Edit Pending Worker

• Hire an Employee

• Add a Contingent Worker

• Add a Nonworker

• Create Work Relationship

• Local and Global Transfer

• Add Assignment

• Employment Details

• Change Assignment

166

Oracle Fusion Cloud Human Resources
Using Global Human Resources

• Promote

• Transfer

• Mass Legal Employer Change

Note:

Chapter 7
Employment Information

• The Business Unit LOV is filtered only by the legal employer you selected previously in the responsive

employment pages. The filtering is not a validation. Therefore, the filtering doesn't apply to REST API, HCM
Data Loader, and HCM Spreadsheet Data Loader.

Related Topics

• Associate Business Unit with Legal Employer

Filter Locations Based on Employee Location

The client-side Location list of values (LoV) is filtered based on the Employee Location attribute value set in the
Location Details page. When you create a location using the Location Details page, you can specify a location as an
employee location by selecting Yes in the Employee Location field. The Location LoV displays only those locations that
have the attribute value set to Yes, and doesn't display locations that have the attribute value No.

The Location LoV is available in these responsive employment flows:

• Add a Contingent Worker

• Add a Nonworker

• Add a Pending Worker

• Add Assignment

• Change Assignment

• Change Location

• Create Work Relationship

• Edit Pending Worker

• Employment Details

• Hire an Employee

• Local and Global Transfer

• Promote

• Transfer

• Mass Legal Employer Change

• Mass Legal Employer Change (Faceted Search)

• Pending Workers (Faceted Search)

Note:  The Location LoV is filtered based on the Employee Location field only in the responsive employment pages
listed in this topic. The filtering is not a validation. Therefore, the Location LoV filtering doesn’t apply to REST API,
HCM Data Loader, and HCM Spreadsheet Data Loader.

167

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Related Topics

• Locations

View and Manage Your Employment Information

Employees, line managers, HR specialists, and HR analysts can access a worker’s employment and salary details from
the Employment Info page.

The data on the Employment Info page is shown as of the date on which the worker is searched on the Employment Info
search page.

The Employment History section in the Employment Info page displays the worker's assignment history across legal
employer changes if their source and target assignments are linked. You can navigate to the employment details or view
employment details (based on profile option) page by clicking the action link in the Employment History section.

Correction and Deletion of Assignment Updates
You can only view and perform assignment corrections if you haven’t enabled the combined correction and deletion
feature. You can enable the feature by setting the ORA_PER_EMPL_COMBINED_CORRECTION_DELETION profile option
to Yes. Here’s the application behavior when the profile option is set to No:

Employment History and Future Actions Sections

You can view assignment update actions with dates in the Employment History and Future Actions sections. The
sections also display the worker's assignment history across legal employer changes if their source and target
assignments are linked. You can navigate to the employment details page by clicking the action link in the Employment
History section.

A user viewing their own data on the Employment Info page can’t navigate to the employment details from the
Employment History and Future Actions sections. The sections will display the fields related to the assignment update
based on your selection from HCM Experience Design Studio.

Employment Details

You can view, correct, and delete assignment updates by using the employment details page. If you access the
termination record, you can navigate to the termination page for correcting the termination.

Combined Correction and Deletion for Assignment, Salary, and Document Records
You can view and correct assignment updates by using a compact guided process and read-only view
employment details page instead of the employment details page. You can enable this feature by setting the
ORA_PER_EMPL_COMBINED_CORRECTION_DELETION profile option to Yes. When you enable the feature, the
application will navigate to the view employment details and correct employment details pages instead of the
employment details page. You can use these pages to correct or delete assignments along with its associated salary
changes and document records.

Employment History and Future Actions Sections

The Employment Info page displays the salary changes along with assignment changes for employment transactions in
the Employment History and Future Actions sections.

The salary change along with the assignment change is displayed in the Employment History section whereas only the
salary change is displayed in the Future Actions section.

168

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Here are some points to consider:

Chapter 7
Employment Information

•

If you completed an assignment change transaction without the salary change, then the salary value won’t be
displayed along with the assignment record.

• The salary records that are created along with assignment changes in employment pages will have the same
action occurrence details as the assignment. Only the salary records having the same action occurrence ID as
the assignment will be displayed along with the assignment record.

• The salary changes that were done outside the employment actions, such as the Change Salary, Salary History,

HCM Data Loader, and REST API will also be displayed on the Employment Info page. However, the salary
changes will be displayed as a separate record even if they were made on the same date as the assignment
changes. This is because the salary change will have a different action occurrence ID than the assignment
change.

View Employment Details

You can navigate to the view employment details page by clicking the action link in the Employment History or Future
Actions section of the Employment Info page.

When you click Delete from the view employment details page, the related salary change and document records
(records having the same action occurrence ID) will be deleted along with the date effective assignment record. If there
are future salary updates and the user deletes the assignment transaction, then only the assignment records will be
deleted. The salary record will be retained by the application. You can't delete an additional assignment completely from
the view employment details page if a time card exists for the assignment. If a time card exists, the application stops
the delete process and displays an error message. If you don't want the application to prevent deletion of the additional
assignment when a time card exists, set the ORA_PER_EMPL_DISABLE_TIME_CARD_CHK_CANCEL_WR profile option
value to Y. This check is not applied when only a date-effective assignment record is deleted.

The Summary of Salary Changes and Salary sections are displayed in these scenarios:

• The original transaction includes salary changes.

• You have the required data security access to view the salary.

When there are more than one assignment changes on the same day, the assignment attributes, such as Grade
displayed in the section will show the latest assignment change of the day. Similarly, the latest assignment details will be
used for calculations, such as differentials, salary ranges, or rate-based salary computations.

The Summary of Salary Changes section will display the changed attribute values by default. You can also see all
attribute values (changed or unchanged) by selecting the Show All check box.

This is how the application behaves when you select the standalone salary action in the Employment History or Future
Actions section of the Employment Info page:

• When you select an action that only includes salary change (for example, a transaction performed using

Change Salary, Salary HCM Data Loader, Salary HCM Spreadsheet Data Loader, or Salary REST API), the view
employment details page will only display the salary related details and it won’t have the assignment related
sections.

• The Edit button will be visible in the view employment details page instead of the Correct and Delete buttons.

• When you click the Edit button, the application will start the Change Salary compact guided process. It will

allow you to make changes to the salary including deletion.

• The module identifier for changes or deletions will be SalaryAdmin. So, the approval rules defined for the

SalaryAdmin module identifier or Administer Salary process will be used for approval routing.

169

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

The Document Records section isn't displayed if the original transaction didn't include document records. Additionally,
the section will display only those document records for which you have data security access.

You can enable the feature to delete document records associated with the deleted assignment record by setting the
ORA_PER_DOR_DELETE_ON_DELETE_ASG_DATE_EFFECTIVE_CHG profile option to Yes.

Note:  If document records are added as part of an employment transaction that involves two assignments (for
example, Add Assignment), the document records are displayed and can be managed from either of the assignments.

Delete Employment Details

If you want to add additional information while deleting an assignment record, you need to enable the
ORA_PER_EMPL_ADD_ASG_DEL_INFO profile option.

You can navigate to the delete employment details page by clicking the Delete button to delete the assignment record
on the view employment details page.

You can configure new actions and their action reasons using the Delete this change action type. You can select the
action and action reason for the assignment record deletion in the Details section of the delete employment details
page. The read-only action date in the section displays the effective date of the record being deleted.

The Additional Info section contains the action occurrence extensible flexfield (EFF) that you have enabled to store extra
information regarding the deletion of the assignment record.

If you have enabled the Additional Info section by using HCM Experience Design Studio and haven’t enabled any action
occurrence EFF, then the section won’t display any extra information.

The comments and attachments data is associated with the approval workflow. The attachments have a lifecycle after
which they are archived and purged and are no longer accessible.

Correct Employment Details

When you click Correct in the view employment details page, the compact guided process for correct employment
details starts. A questionnaire page is displayed where you can select the sections you want to correct. The header of
the Correct Employment Details page displays the action of the assignment record that you’re correcting.

The sections available for selection are based on your HCM Experience Design Studio configuration for this page. It’s
not based on the selected sections when the original transaction was submitted.

These conditions apply when you correct an assignment update:

• You can’t change the effective date of the employment transaction during correction.

• You can’t make salary changes for an inactive assignment.

• When you visit the Salary section or make a salary change, the details in the When and Why section, such
as action, action reason, and action occurrence identifier values of the salary will become the same as the
assignment.

• Salary and document records details can be viewed or edited only when you have the required data security

access.

• The data in the Salary and Document Records sections will be read-only when there is a Change Salary, Salary

History, or Document Record pending approval.

• The publish date can't be modified for existing document records. New document records added as part of the

correction will inherit the publish date as the transaction effective date can't be edited.

• After you correct and click Submit, you will be directed to the Employment Info page.

170

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Here are some points to consider:

Chapter 7
Employment Information

• You can correct and delete changes in the view employment details page only if assignment changes exist.

• The Additional Assignment Info section will be displayed only if the additional assignment record exists as of

the transaction date.

Related Topics

• Action Framework

• Employment Profile Options

FAQs for Assignments

What happens if I change a person's primary work relationship?
These are the changes that happen.

• The previous primary work relationship automatically becomes a nonprimary work relationship.

• The primary assignment in the new primary work relationship becomes the person's overall primary

assignment. If the new primary work relationship contains any future-dated assignments, the change in
primary status is propagated to the future records.

• The new primary work relationship and overall primary assignment is the main source of work-related and

analytic information and reporting.

• The person's worker type may change. For example, the person may become an employee from a contingent

worker if the new work relationship is an employee one.

Can I add matrix managers when I'm using position synchronization?
Yes, you can add matrix managers when you're using position synchronization. You can synchronize the line manager
from position and add a matrix manager.

Related Topics

• Matrix Manager for an Assignment

Where do person types come from?
Person types, can sometimes be referred to as user person types. They are subcategories of the predefined system
person types, such as employee and nonworker.

Each system person type has a single person type by default, which has the same name as the system person type. Your
enterprise can define additional person types for each system person type. For example, for the system person type
nonworker your enterprise could define the person types intern, retiree, volunteer, and counselor.

How can I create an assignment if the person type I need isn't in the list?
If the missing person type is valid for the worker type, you must update the list of person types.

For example, if the worker type is employee and you want to use the person type trainee, you must update the list of
employee person types.

171

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

If the missing person type isn't valid for the worker type, you must either create a new work relationship or update
an existing work relationship of the relevant type. For example, to use the person type volunteer, you create the
assignment in a nonworker work relationship if volunteers are classified as nonworkers.

Can I end the only assignment in a work relationship?
No, you must terminate the work relationship instead.

Can I end a primary assignment if there are other nonprimary assignments in the
same work relationship?
You can end the primary assignment, however, these conditions apply:

•

•

If there is only one nonprimary assignment in the work relationship, the application automatically makes the
nonprimary assignment as primary when ending the primary assignment.

If there are more than one nonprimary assignments, the application doesn't allow you to end the primary
assignment. You need to first make one of the nonprimary assignments as primary before ending the primary
assignment.

Note:  These conditions apply when you use the End Assignment and End Temporary Assignment actions.

Can I end an assignment one day before the second assignment starts?
No, you can end the assignment on the same day the second assignment starts.

What happens to the manager relationship when I end an assignment or terminate a
work relationship?
The manager relationship ends on the same date that you end the assignment or terminate the work relationship. If
you delete the end assignment row or reverse the termination later, you need to add the manager relationship again
because the application doesn't reinstate the manager relationship automatically.

What happens when I select a different line manager for an assignment?
The new line manager gets control of the assignment.

• The new line manager gains access to the assignment on the specified date. For example, the new manager

sees this assignment in management hierarchies and can see the line manager version of the person's
spotlight.

• From the specified date, the managed person sees the new manager's name in reporting hierarchies and other

information about this assignment.

•

If notifications are used at your enterprise, the new line manager, managed person, and you may be notified
automatically of this change.

172

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Why are some values completed automatically when I create assignments?
If you use positions, the selected position supplies the following values automatically: job, department, location, grade,
ceiling step, payroll, salary basis, probation period, manager, working hours, working-hours frequency, start time, and
end time.

If you don't use positions, these things happen:

• The location is inherited from the department.

• The standard working hours, working hours, and working-hours frequency are inherited from the department,

legal employer, or enterprise. Values specified for the department override those specified for the legal
employer, and values specified for the legal employer override those specified for the enterprise.

If you edit the source attributes of inherited values (for example, you update the salary basis of a position), the changes
don't copy automatically to the assignments. However, you can edit the inherited values to match the updated source
attributes.

If you change the business unit on assignments, the organization, job, position, grade, and job values are automatically
set to null.

How can I access inactive assignments?
Switch between active and inactive work relationships and assignments for a person using the Business Title drop-down
list on the Employment Info page.

Alternatively, find current inactive assignments for a person by searching for the person. The person search returns all
the person's current assignments, regardless of their status.

If the assignments are inactive because of a termination, you must select the option in the advanced search to include
terminated work relationships in the search results. Otherwise, inactive assignments in terminated work relationships
don't appear in the search results.

Can I use eligible jobs instead of adding an assignment?
Yes, you can but it's not a direct replacement.

Use eligible jobs in these scenarios.

• The worker is eligible to work on more than one job but may or may not be actually working on that job.

• There's no overlap of jobs or the overlap is for a short period.. For example, providing relief for someone who

didn't turn up for work.

Use additional assignment in these scenarios.

• Worker is working on multiple assignments at the same time

• Period of overlap of jobs is long enough to maintain multiple assignments

How can I update the location from the Change Location page when position
synchronization is enabled?
You need to first enable the Synchronize from Position field for the Change Location action using HCM Experience
Design Studio. Then you can update the location after you clear the Synchronize from Position check box on the Change
Location page.

173

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

How is the before and after assignment data displayed for transactions in the
employment details page?
In the employment details page, the Summary of Employment Changes section only compares the before and after
assignment data for the same assignment ID.

For the newly added assignment rows that are created as part of create flows, (for example, Add a Person, Rehire, Create
Work Relationship, Global Temporary Assignment, Add Assignment) only the After column will be populated.

Note:  The only exception is for a global transfer where the section compares the before and after assignment data
only for the two assignments that were part of the global transfer.

When you insert a new effective dated row for an existing assignment (for example, during a Transfer or Promotion), the
Summary of Employment Changes section displays the before and after assignment data because the update happens
in the same assignment.

Note:  The Summary of Employment Changes section doesn't show data for assignment key flexfields (KFF), such as
People Group and Default Expense Account and extensible flexfields (EFF).

Is the source work relationship impacted when you cancel the work relationship
created by a global transfer or global temporary assignment?
Global transfer: Yes, the cancel impacts the source work relationship from where the global transfer was initiated. The
assignment update in the source work relationship is removed and the source work relationship becomes active.

Global temporary assignment: No, the cancel doesn’t impact the source work relationship from where the global
temporary assignment was initiated. To reverse the transaction after cancellation of the destination work relationship,
you must delete the assignment update in the source assignment which was created as part of the global temporary
assignment.

Is the source work relationship impacted when you reverse terminate a work
relationship that was terminated using the End Global Temporary Assignment action?

No, the reverse termination of end global temporary assignment doesn’t impact the source work relationship from
where the global temporary assignment was initiated.

To reverse the End Global Temporary Assignment transaction, you can delete the assignment update in the source work
relationship after completing the reverse termination.

Is the source assignment impacted when you delete the End Temporary Assignment
record from the destination assignment?
No, the deletion doesn’t impact the source assignment from where the temporary assignment was initiated. You can
delete the source assignment update related to End Temporary Assignment.

174

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Can I initiate an assignment change when another employment transaction is
pending approval?
If the worker has an employment change that’s pending approval, you can’t change the employment data for the same
worker by using the following methods:

• Employment flows, such as Change Assignment or Promote.

• REST API

Employment Dates

Change Employment Start Dates

You can change the work relationship start date using the Employment Start Dates compact guided process. Using this
guided process, you can also change the hire date for terminated workers and proposed start date for pending workers.

You use this guided process if you only want to change the start date and not any other work relationship attributes,
such as the primary indicator and work relationship descriptive flexfield. If you want to change the start date along with
other work relationship attributes, you must use the work relationship process instead.

Here's how information is displayed in the Employment Start Dates page:

• Start Date Info section: Displays the read-only action name field where the action name is appended with

the date of the action. For a pending worker work relationship, the appended date is the proposed start date
of the pending worker. Additionally, this section displays error messages, if any, when you change the work
relationship start date.

• Assignments section: Displays the read-only assignment data as of the date the worker is searched in the

Employment Start Dates search page. If there are multiple assignments in the work relationship, only those
assignments which are active as of the searched date are displayed.

Note:  You can personalize the Employment Start Dates page by using HCM Experience Design Studio.

Start Date Change for Pending Workers
For pending workers, the application changes the proposed start date instead of the start date of the pending worker
work relationship. When you change the proposed start date for a pending worker, the work relationship start date is
automatically changed where applicable. This change only happens if the new proposed start date is earlier than the
original work relationship start date.

Points to Consider

• You can't change the work relationship start date when other employment transactions are pending approval.

• The contract and probation end dates won't be moved when you change the work relationship start date.

•

If assignment-level security is enabled, you can only change the work relationship start date if you have access
to the first assignment created when adding the work relationship.

175

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Change Start Dates for Employment Transactions

This table describes the methods used for changing the start date of employment transactions:

Use Case

Method

Hire, Create Work Relationship, Add

Use Employment Start Dates or the Work Relationship quick action.

Nonworker, Add Pending Worker, and Add

If the start date can’t be changed using these quick actions, then cancel and recreate the work

Contingent Worker.

relationship using the correct date.

Global Transfer and Global Temporary

Cancel the newly created work relationship and perform the global transfer and global temporary

Assignment.

assignment again with the correct date.

Termination, Resignation, and End Global

Use the Correct Termination page.

Temporary Assignment.

Promote and Transfer.

Delete the employment update by using the employment details page which can be accessed from the

Employment Info quick action.

Then, again perform the transaction using the correct date.

Add Assignment and Add Temporary

Delete the employment update by using the employment details page which can be accessed from the

Assignment.

Employment Info quick action.

Then, again perform the transaction using the correct date.

End Assignment and End Temporary

Delete the employment update by using the employment details page which can be accessed from the

Assignment.

Employment Info quick action.

Then, again perform the transaction using the correct date.

Examples of Start Date Changes When Assignment Changes Exist

Let's look at some examples of when you can change a person's start date when assignment changes exist and what's
the outcome of the change.

Future Assignment Changes Don't Exist
Vijay Singh is hired on 1-Jan-2010. He has no future assignment changes.

176

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Start Date

Changed Start Date

Changed Work
Relationship Start Date

Changed Assignment
Start Date

Outcome

1-Jan-2010

1-Jan-2009

1-Jan-2009

1-Jan-2009

1-Jan-2010

1-Jan-2011

1-Jan-2011

1-Jan-2011

When you change the start
date to an earlier date,
 the start date changes
for the employment
(work relationship and
assignment) and person
records.

When you change the
start date to a future date,
 the start date changes
for the employment
(work relationship and
assignment) and person
records.

Future Assignment Changes Exist
Vijay Singh is hired on 1-Jan-2010 and has a future assignment change on 1-Jan-2011. Assignment changes include
actions such as promotion, adding an assignment, and adding a temporary assignment.

Start Date

Assignment Change

Changed Start Date

Changed Work
Relationship Start
Date

Changed Assignment
Start Date

Outcome

1-Jan-2010

1-Jan-2011

1-Jan-2009

1-Jan-2009

1-Jan-2009

1-Jan-2010

1-Jan-2011

1-Jan-2012

Not applicable

Not applicable

Note:
This change isn't
possible.

Multiple Assignment Changes Exist on the Start Date
Vijay Singh is hired on 1-Jan-2010 and an assignment change was done for him on the same date.

When you change
the start date to
an earlier date, the
start date changes
for the employment
(work relationship
and assignment) and
person records.

You can't change
the start date to a
date that's later than
the date of the first
assignment change.
You need to delete the
assignment change
first.

177

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Start Date

Assignment Change Date Work Relationship Start

Assignment Start Date

Outcome

Date

1-Jan-2010

1-Jan-2010

1-Jan-2010

1-Jan-2010

If there are multiple
assignment changes on the
start date, you can't change
the start date. You need
to remove the assignment
change to change the start
date.

Invalid Supervisor or Direct Reports Exist on Start Date
If the supervisors, such as line manager, project manager, and so on or any of the direct reports is invalid as of the new
selected start date, then the start date change won't be allowed.

Additional Assignments Exist on the Start Date
Vijay Singh has an additional assignment added for him on 1-Feb-2010.

Start Date

Changed Start Date

Changed Work
Relationship Start Date

Changed Assignment
Start Date

Outcome

1-Jan-2010

1-Mar-2010

1-Mar-2010

Not applicable

(original assignment)

1-Feb-2010

(additional assignment)

1-Jan-2010

15-Jan-2010

15-Jan-2010

15-Jan-2010

(original assignment)

1-Jan-2010

1-Dec-2009

1-Dec-2009

(original assignment)

1-Feb-2010

(additional assignment)

1-Dec-2009

1-Feb-2010

(additional assignment)

You can't change the start
date to a date that's after
the date on which the
second assignment was
created.

When you change the start
date to a future date, the
start date changes for
the employment records
(work relationship and
assignment) that were
created during hire.

When you change the start
date to an earlier date,
 the start date changes
for the employment
(work relationship and
assignment) and person
records.

Vijay Singh has an additional assignment added for him on the same date as the start date.

Start Date

Changed Start Date

Changed Work
Relationship Start Date

Changed Assignment
Start Date

Outcome

1-Jan-2010

1-Mar-2010

1-Mar-2010

Not applicable

You can't change the start
date to a date that's after
the date on which the

178

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Start Date

Changed Start Date

Changed Work
Relationship Start Date

Changed Assignment
Start Date

Outcome

(original primary
assignment)

1-Jan-2010

(additional nonprimary
assignment)

1-Jan-2010

1-Dec-2009

1-Dec-2009

1-Dec-2009

(original primary
assignment)

1-Jan-2010

(additional nonprimary
assignment)

(original primary
assignment)

No change

(additional nonprimary
assignment)

second assignment was
created. In this case, since
the assignment was created
on the hire date, the start
date can't be moved in
future.

When you change the start
date to an earlier date, the
start date changes only for
the primary assignment
and the date of the newly
added assignment remains
the same. If the newly
added assignment is
added as primary, this
causes multiple assignment
changes on the same date
in the original assignment.
You can't change the hire
date if there are multiple
assignment changes on the
start date.

Related Topics

• How can I correct the global transfer and global temporary assignment start dates?

Examples of Start Date Changes When Work Relationship
Changes Exist

Let's look at some examples of when you can change a person's start date when work relationship changes exist and
what's the outcome of the change.

Note:  The enterprise start date can't be changed when you edit the work relationship because it's calculated based
on the first work relationship start date for a system person type. The work relationship start date may belong to a
person type, such as employee, pending worker, contingent worker, or nonworker. Therefore, when you change the
first work relationship start date for a person type, the enterprise start date is changed accordingly.

Work Relationship is Terminated
Vijay Singh is hired on 1-Jan-2010. He has a nonprimary work relationship that was created on 1-Jan-2011 and
terminated on 1-Jan-2012.

179

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Start Date

Work Relationship Start
Date

Termination Date

Page

Outcome

1-Jan-2010

1-Jan-2010

1-Jan-2012

Work Relationship

1-Jan-2010

1-Jan-2010

1-Jan-2012

Employment Start Dates

You can't change the
start date for this work
relationship because it's
terminated.

You can change the start
date as long as the date is
before the termination date
which in this example is any
date before 1-Jan-2012.

Terminated Work Relationship Exists in the Same Legal Employer
Vijay Singh is hired on 1-Jan-2010 and terminated on 31-Dec-2010. He is again rehired in the same legal employer on 1-
Jan-2012.

Start Date

1-Jan-2010

Work Relationship Start Date

Assignment Start Date

Outcome

1-Jan-2010 (original work
relationship)

1-Jan-2012 (rehired work
relationship )

1-Jan-2010 (original assignment)

1-Jan-2012 (rehired assignment)

You can move the start date for
the rehired work relationship to
a future date. However, you can't
move the start date earlier than
the end date of the original work
relationship. This is because the
person already has the same work
relationship type with the legal
employer. A person can have only
one active work relationship with
any legal employer for a given
person type.

Pending Worker Work Relationship Exists
Vijay Singh is added as a pending worker on 1-Jan-2010 and the proposed start date of the employee work relationship
is 01-Feb-2010.

Pending Worker
Work Relationship
Start Date

Proposed Start Date
of Work Relationship

New Proposed Start
Date

New Work
Relationship Start
Date

Page

Outcome

1-Jan-2010

1-Feb-2010

Not Applicable

15-Jan-2010

Work Relationship

You can change the
pending worker work
relationship start
date to earlier than
the proposed work
relationship start date,
 but not later than
the proposed work
relationship start date.

180

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Pending Worker
Work Relationship
Start Date

Proposed Start Date
of Work Relationship

New Proposed Start
Date

New Work
Relationship Start
Date

Page

Outcome

1-Jan-2010

1-Feb-2010

15-Feb-2010

1-Jan-2010

1-Feb-2010

1-Dec-2010

1-Jan-2010 (No
Change)

Employment Start
Dates

1-Dec-2010

The proposed start
date can't be changed
from the Work
Relationship page.

In case of pending
workers, the
application gives you
an option to change
the proposed start
date instead of the
work relationship
start date of the
pending worker
work relationship.
When you change
the proposed start
date for a pending
worker, the application
automatically changes
the work relationship
start date if applicable.
This change only
happens if the new
proposed start
date is earlier than
the original work
relationship start date.

You can't directly
change the pending
worker work
relationship date on
this page.

Vijay Singh is converted from pending worker to an employee on 1-Feb-2010.

Start Date

Changed Start Date

Changed Work
Relationship Start Date

Changed Assignment
Start Date

Outcome

1-Feb-2010

1-Jan-2010

1-Jan-2010

Not Applicable

1-Feb-2010

1-Mar-2010

1-Mar-2010

1-Mar-2010

You can't change the start
date to a date that's earlier
than the date on which
the pending worker was
converted to an employee.

When you change the
start date to a future date,
 the start date changes
for the employment
(work relationship and
assignment) records.

181

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Additional Work Relationships Exist in Future
Vijay Singh is hired on 1-Jan-2010 and he has a future dated work relationship on 1-Jan-2011.

Start Date

Work Relationship Start
Date

Assignment Start Date

Nonprimary Work
Relationship Termination
Date

Outcome

1-Jan-2010

1-Jan-2010 (primary)

1-Jan-2010

Not applicable

1-Jan-2011 (nonprimary)

1-Jan-2011

1-Jan-2012

You can change the start
date of the primary work
relationship to an earlier
date but not to a date later
than the nonprimary work
relationship start date. You
need to cancel the future
dated work relationship to
move the start date to the
future.

You can change the start
date of the nonprimary
work relationship to a
future date but not to
a date earlier than the
primary work relationship
start date.

Note:
A person must at least
have one active primary
work relationship.

Vijay Singh is hired on 1-Jan-2010 and a temporary legal employer change was done for him on 1-Feb-2010.

Start Date

Changed Start Date

Work Relationship Start
Date

Changed Assignment
Start Date

Outcome

1-Jan-2010

1-Mar-2010

(original work relationship)

1-Mar-2010

1-Feb-2010

(additional work
relationship)

Not applicable

You can't change the start
date to a date that's after
the date on which the legal
employer change was done.

1-Jan-2010

15-Jan-2010

15-Jan-2010

15-Jan-2010

(original work relationship)

1-Feb-2010

(additional work
relationship)

1-Jan-2010

1-Dec-2009

(original work relationship)

1-Dec-2009

1-Feb-2010

1-Dec-2009

When you change the start
date to a future date, the
start date changes for
the employment records
(work relationship and
assignment) that were
created during hire.

When you change the start
date to an earlier date,
 the start date changes

182

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Start Date

Changed Start Date

Work Relationship Start
Date

Changed Assignment
Start Date

Outcome

(additional work
relationship)

for the employment
(work relationship and
assignment) and person
records.

Vijay Singh is hired on 1-Jan-2010 and a permanent legal employer change was done for him on 1-Feb-2010.

Start Date

1-Jan-2010

Work Relationship Start Date

Outcome

1-Jan-2010

(original work relationship)

1-Feb-2010

(additional work relationship)

You can't change the start date of the
terminated work relationship. If the original
work relationship is terminated, the application
won't allow you to change the start date of the
additional work relationship.

Examples of Start Date Changes for Employment Work
Relationship Created from Pending Worker Work Relationship

Let's look at some examples of changing the start date of a person’s employment work relationship that’s created from
a pending worker work relationship.

Vijay Singh is added as a pending worker in on 1-Jan-2010 and converted from pending worker to an employee on 1-
Feb-2010.

Example 1
You want to change the start date of the employee work relationship to 25-Jan-2010. The application won’t allow you to
change the start date directly in the employee work relationship. Instead, you can change the start date by doing these
steps:

1. Do a correct termination on the pending worker work relationship and move the termination date to a day

before the intended start date of the employee work relationship. In this example, 24-Jan-2010.

2. Change the employee work relationship start date to 25-Jan-2010 using the Employment Start Dates UI.

If you want to change the start date to any date that’s before the pending worker conversion date, and after the pending
worker creation date, follow steps 1 and 2 in Example 1.

Example 2
You want to change the start date of the employee work relationship to 25-Dec-2009 or to any date which is before the
pending worker creation date. The application won’t allow you to change the start date directly in the employee work
relationship. Instead, you can change the start date by trying either of these options:

Option 1

1. Reverse terminate the pending worker relationship.

183

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

2. Use the Work Relationship quick action (instead of Employment Start Dates quick action) to correct the start
date of the pending worker to the required date. In this example, the date must be on or before 24-Dec-2009.

3. Terminate the pending worker on or before 24-Dec-2009.
4. Use the Work Relationship quick action to correct the start date of the employee to the required date. In this

example, 25-Dec-2009.

Option 2

1. Cancel the employee work relationship.
2. Reverse terminate the pending worker relationship.
3. Use the Work Relationship quick action (instead of Employment Start Dates quick action) to correct the start
date of the pending worker to the required date. In this example, on or before 24-Dec-2009. Also, correct the
proposed start date as the date from which you want the employee work relationship to start.

4. Reconvert the pending worker to an employee.

Examples of Start Date Changes for Converted Pending Worker
Work Relationship

Let's look at an example of changing the start date of a person’s converted pending worker work relationship.

Vijay Singh is added as a pending worker on 1-Jan-2010 and converted from pending worker to an employee on 1-
Feb-2010.

Example
You want to change the start date of the pending worker work relationship to 25-Dec-2009 or to any date which is
before the pending worker creation date. The application won’t allow you to change the start date directly in the
employee work relationship. Instead, you can change the start date by doing these steps:

1. Reverse terminate the pending worker relationship.
2. Use the Work Relationship quick action (instead of Employment Start Dates quick action) to correct the start

date of the pending worker to the required date. In this example, 25-Dec-2009.

3. Terminate the pending worker again on the required date.

Retain Your Employment Changes While Changing the Effective
Date

When you change the effective date of a transaction in employment flows, by default, all your employment-related
changes are reset as of the new effective date.

However, if you want to retain the changes even after you change the effective date, you need to enable the
ORA_PER_EMP_RETAIN_CHANGES profile option. The changes are retained when you use these flows:

• Local and Global Transfer

• Create Work Relationship

• Convert Pending Worker

• Add Assignment

184

Oracle Fusion Cloud Human Resources
Using Global Human Resources

• Change Location

• Promote

• Transfer

• Change Assignment

Chapter 7
Employment Information

Note:  Person changes will also be retained, but only in the Local and Global Transfer flow.

The changes are also retained when the transaction approver changes the transaction date in the employment flows as
part of Edit the Transaction feature.

Points to Consider

• Retaining your employment changes while changing the effective date is an opt-in feature that can be

controlled by using the ORA_PER_EMP_RETAIN_CHANGES profile option.

•

•

If you change the transaction date, and the date is earlier than the previous assignment record or later than the
future assignment record, your employment changes won't be retained. In this case, the current application
behavior of resetting your employment changes will continue.

If you are using the AutoComplete feature in responsive Employment flows where employment changes are
retained, you need to check your AutoComplete rules. The AutoComplete rules related to defaulting are not
impacted. However, the AutoComplete rules related to validation may be impacted and must be checked again.

Related Topics

• Employment Profile Options

Examples of Retaining Your Employment Changes While
Changing the Effective Date

Here's an example of how your employment changes are retained in employment flows when you change the effective
date.

New Effective Date Needs to be Between the Previous and Next Record's Effective
Date
If you added the assignment row having effective date of 01-Mar-2019, the changes will be retained only when the date
is changed between 01-Feb-2019 and 01-Jun-2019.

Date

Action

Business Unit

Location

Job

Department

Grade

Additional
Information

01-Jan-2019

Hire

Business Unit 1

Location 1

Job 1

Department 1

Grade 1

Historical record

01-Feb-2019

Transfer

Business Unit 1

Location 1

Job 1

Department 2

Grade 1

Historical record

185

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Date

Action

Business Unit

Location

Job

Department

Grade

01-Mar-2019

Change
Location

Business Unit 1

Location 2

Job 1

Department 2

Grade 1

Additional
Information

Newly added
record

01-Jun-2019

Promotion

Business Unit 1

Location 1

Job 1

Department 2

Grade 1

Future record

Value Becomes Invalid When You Change Effective Date
If you enter a value that's not valid as of the newly changed date, the value will be reverted to the old value. Let's have a
look at how this works by using this example:

Grade 1 is active from 01-Jan-1951 and Grade 11 is active from 01-Jun-2019.

Date

Action

Business Unit

Location

Job

Department

Grade

Additional
Information

01-Jan-2019

Hire

Business Unit 1

Location 1

Job 1

Department 1

Grade 1

N/A

01-Jun-2019

Promotion

Business Unit 1

Location 1

Job 1

Department 2

Grade 11

Newly added
record

If you change the date of the newly added record from 1-Jun-2019 to 1-May-2019, the grade value will be reverted back
to Grade1 as Grade11 isn't valid as of the new date.

Dependent Field Defaulting While Retaining Your Employment Changes
Consider the application setup where location is defaulted from the department. In the following example, the user
changes the department from Sales to Finance and the location is defaulted to Delhi which is then cleared by the user.

Action

Effective Date

Department
Attribute

Location Attribute
(Dependent
Attribute)

User Change

Application Behavior

01-JAN-2010

Sales

Hyderabad

Not applicable

Not applicable

Hire

Transfer

01-MAR-2010

Finance

Transfer

15-MAR-2010

Finance

Null

Null

Clear Delhi location

Delhi location is
cleared

Change effective date

Displays Finance
department and blank
location

The application will ignore the user input for the dependent attribute if the following conditions are true:

• The initial value of the dependent attribute is null and you have manually cleared the defaulted value in the

dependent attribute during the transaction.

• You changed the effective date of an employment transaction.

186

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Consider the following example of an employee whose department and location are not populated during hire and the
user populates the department value as Human Resources during transfer.

Action

Effective Date

Department
Attribute

Location Attribute
(Dependent
Attribute)

User Change

Application Behavior

Hire

Transfer

01-JAN-2010

No value

No value

Not applicable

Not applicable

10-JAN-2010

Human Resources

Null

• Select Human
Resources

Bangalore location is
cleared

• Clear Bangalore

location

Transfer

01-FEB-2010

Human Resources

Bangalore

• Change effective

date

• Visit the

Assignment
section

Bangalore location is
defaulted

In this example while transferring a worker, the user selects the Human Resources department and the Bangalore
location is defaulted. The user then clears the Bangalore location to make it blank. Now when the user changes the
effective date of the transfer transaction, Bangalore will be again defaulted even though the user had cleared the
Bangalore location. The user needs to manually clear the Bangalore location again. This behavior occurs because
initially there was no location and later the user clears the defaulted location. In this scenario, since there was no change
between the initial value and the value after the user change for the Location attribute, the application doesn’t consider
it as a user change and doesn’t retain the value.

Control Default of Effective Start Date in Employment Flows

You can control the defaulting of the effective start date in these responsive employment flows using the
ORA_PER_EMPL_DEFAULT_EFFECTIVE_DATE profile option:

• Add Assignment

• Add Contingent Worker

• Add Nonworker

• Add Pending Worker

• Change Assignment

• Change Location

• Change Manager

• Change Working Hours

• Create Work Relationship

• Direct Reports

• Hire an Employee

• Local and Global Transfer

• Promote

187

Oracle Fusion Cloud Human Resources
Using Global Human Resources

• Termination

• Transfer

Here are some points to consider when you use the profile option:

Chapter 7
Employment Information

•

If you have selected not to default the effective start date in the responsive employment flow, you need to first
enter the effective start date in the flow. The other fields in the flow will be enabled for changes only after you
enter the effective start date.

• You must not use Page Composer or HCM Experience Design Studio to hide the effective start date field

when the profile option is set to N. This is because the effective start date is a required field for responsive
employment flows.

• You must not use Page Composer or HCM Experience Design Studio to hide the termination notification date
when the profile option is set to N. This is because the termination notification date is a required field for the
responsive termination flow.

• There will be no change to the behavior of the offer conversion flows even if you set the profile option value to

N. The effective start date will display the date entered during the job offer creation.

• There will be no change to the behavior of the Convert Pending Worker flow even if you set the profile option
value to N. The effective start date will display the proposed start date entered during the pending worker
creation.

Related Topics

• Employment Profile Options

How You Validate a Worker’s Salary when the Hire Date is Changed

You can validate the salary when you change the hire date for a worker.

When the hire date is changed, the application checks for salary related validations and displays them on the page as an
error or warning message based on the user configuration.

You can configure the validation result as an error or warning message using the Salary Validations Behavior When
Changing Start Date (ORA_CMP_SALARY_CHECKS_BEHAVIOR_IN_CHANGE_START_DATE) profile option.

When you change the hire date using actions, such as Change Hire Date or Work Relationship, the application validates
the salary on these bases:

• A salary change proposal is pending for approval

• There’s more than one salary existing for the assignment

• The salary basis is no longer active

• The salary amount violates the salary range on the proposed hire date

When a validation fails and the profile option is set to error, you won’t be allowed to submit the transaction. However, if
the profile option is set to warning, a warning message is displayed and you can submit the transaction if you choose to
ignore the warning.

188

Oracle Fusion Cloud Human Resources
Using Global Human Resources

These are some key points to note:

Chapter 7
Employment Information

• Salary range validation is performed when you set the salary range violation behavior in salary basis to Error
and the profile option is also set to Error. When the profile option is set to Warning, validation will not be
performed even though the setting in salary basis is set to Error.

• The salary validations are performed when you submit the hire date change by using the Change Hire Date and
Work Relationship responsive pages, HCM Data Loader, or REST API. However, warning messages won’t be
displayed when uploading changes using HCM Data Loader or REST API.

• When the salary validation fails, the warning or error message is displayed based on how the profile option is

configured. You can’t set separate error or warning messages for individual validations.

FAQs for Employment Dates

How can I correct the start date of an assignment or temporary assignment that I
added?
You can't change this date directly on the assignment page. You need to delete the newly created assignment and add
the assignment or temporary assignment again on the date you want.

How can I correct or delete a date-effective assignment record using the responsive
UI?
Use the Employment Info quick action under My Client Groups to search for the employee. Select the relevant
assignment record from the Employment History section to open the employment details page.

You can then correct or delete the selected assignment record from the employment details page.

How can I correct the start dates of assignment-related transactions?
You can't change these dates directly on the Employment Info or Employment Details page. You must first delete the
assignment record that was created as part of the transaction (for example, Promote or Transfer).

This removes the assignment record. You can then do the transaction again on the date you want.

How can I correct the global transfer and global temporary assignment start dates?
You can't change these dates directly on the assignment or Work Relationship page. You must first cancel the work
relationship that was created as part of the global transfer or global temporary assignment.

This removes the global transfer and global temporary assignment records from the original assignment. You can then
do the global transfer or create a global temporary assignment on the date you want.

189

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Eligible Jobs

Overview of Eligible Jobs

An eligible job is an additional job for which the worker is eligible in addition to the worker's current job.

You can use this feature to track the additional jobs. The additional jobs can also be used to report time on the time
sheet. Use the value set ORA_PER_EMPL_ELIG_JOBS when configuring the time sheet to display eligible jobs.

Relief Type
The relief type governs the job filtering and rate override options for the additional jobs. By default, when you add a new
eligible job, the relief type is Derived.

• Derived - You need to set the start date, end date and select a job that's mapped to the job family of the

assignment job.

• Manual - You can attach any job even outside the job family of the assignment job. If you add a job under this

relief type then you need to enter the rate and frequency along with start date and end date. If you want to use
this relief type you need to un-hide these fields- Relief Type, Manual Rate, Currency, and Frequency.

However, a point to note is that when you enter the eligible job, an element entry or time card entry isn't automatically
created. You need to refer the overridden rate and frequency in your payroll fast formula to calculate the pay difference
for a worker if you're using the Manual relief type.

Eligible Jobs Example
Let's see how you can track additional jobs based on the relief type from these scenarios.

Scenario

Action

Bob Price is Supervisor at Acme Inc. He is
being given an additional responsibility
of Manager, a position in the same job
family for a period of two months till a new
person is hired.

• Select relief type as Derived.

• Enter the start and end dates for the additional job

Jenna Markum is the Vice President of
the Sales division. She is asked to head
the Marketing division for a period of one
year. Since there is no fixed job rate for the
Sales division, her payroll for the additional
job must be calculated based on what's
defined at the eligible job level.

• Select relief type as Manual

• Enter the start and end dates for the additional job

• Enter the manual rate as per the industry standards

• Select the frequency as Weekly

Related Topics

• Considerations for Adding Eligible Jobs

190

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

Considerations for Adding Eligible Jobs

You can add additional jobs for which a worker is eligible. Consider these points when adding eligible jobs for a worker.

Job
You can't add an eligible job same as the one in the worker's current assignment. You can't add the same eligible
jobs twice for the same period. The start date of an eligible job must be after the start date of the worker's current
assignment.

Job Set and Job Family
The jobs that you see are dependent on the job family and the relief type selected. For example, when you select the
relief type as Derived for a worker whose current assignment is Consultant, then the jobs displayed are based on the job
family and job set to which this job belongs.

Relief Type
The relief type mode can be either Manual or Derived. You need to map jobs to the appropriate job families if you want
to use the Derived relief type mode. This is because the application will only display jobs that are from the same job
family as the assignment job. You must specify the manual rate and frequency when the relief type model is Manual.
You can add a job from the same job set as the worker's current assignment when the relief type is Manual. You can't
select the frequency as Periodically.

191

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 7
Employment Information

192

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 8
Areas of Responsibility

8  Areas of Responsibility

How You Assign Areas of Responsibility

You can assign a worker a responsibility and identify the scope of the responsibility.

For example, you can assign a worker the Human Resources (HR) Representative responsibility and define the scope
as people in a specific organization or department hierarchy. Select the Include in work contacts option for the worker
to appear as a HR representative in the Work Contacts list of those people. To assign responsibilities, use the Areas of
Responsibility quick action on the My Client Groups tab.

Assigning an area of responsibility doesn't affect the person records the representative can see. Access to records is
controlled through security. Your security administrator can set up security profiles using areas of responsibility.

What Happens if Scope Overlaps
If you assign the same responsibility to multiple people, overlap between scopes may occur. For example, you define the
scope of the HR Representative responsibility for person A using an organization hierarchy. You define the scope of the
HR Representative responsibility for person B using a supervisor hierarchy. The scopes overlap because some workers
appear in both hierarchies. These workers then have both A and B as their HR representatives. If this isn't the desired
result, you may redefine the scope by specifying a different combination of information.

Including a Representative in Work Contacts
You can define areas of responsibility to identify representatives for a worker population, identify approvers in an
approval flow, or secure access to person and position records.

You may not want certain representative types to appear under Work Contacts, for example, if you're securing access
to person and position records. It's recommended that you create a custom representative type starting with "ZZ_" for
easy identification in case performance measures need to be taken. You can also use responsibility templates to ensure
that your security-only representatives are consistently assigned this representative type. Select the Exclude from work
contacts option to not display the representative under Work Contacts.

Note:  If you use Responsibility Templates, the Work Contacts value defaults from the template when creating the
responsibility.

In addition, you may want to edit all instances to set the value for Work Contacts to Exclude from work contacts. Use
HCM Data Loader to change the work contacts setting for multiple records at once. Set the WorkContactsFlag attribute
of the Areas of Responsibility object to N; These responsibilities will be excluded from work contacts.

Integrating with Checklists
You can create and assign responsibilities for use in checklists. You identify the task performers' responsibilities when
you create a checklist template. During checklist allocation, the persons with the selected responsibilities are derived
and designated as task performers automatically.

193

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 8
Areas of Responsibility

Integrating with Sensitive Transactions
Certain future-dated terminations may be identified as sensitive and hidden from everyone until an appropriate time.
You can use responsibilities for such terminations to identify who should receive notifications involving the termination.
Any conflicts involving sensitive terminations are handled by routing the actions to a person with an HR Representative
responsibility.

Note:  A nonworker can't be a work contact or representative so you can't assign areas of responsibility to a
nonworker.

Related Topics

• Examples of Setting Scope of Responsibility

• How do I add or change a responsibility type?

Autoprovision Areas of Responsibilities

You can now automatically mass assign or inactivate and end-date representatives' areas of responsibilities (AOR)
based on user-defined template criteria.

The Responsibility Template’s Criteria section decides the AOR scope for each individual. You must identify your
organizational needs and then specify the appropriate criteria to match against your workforce assignments. When the
template criteria are matched against a representative’s assignment, a responsibility is created or updated. In case an
assignment no longer matches the template criteria, the assigned responsibility is end-dated, and the Status is set to
Inactive. For example, in case of a local or global transfer.

The responsibility autoprovisioning process flow varies when Bypass Preview is enabled and when it’s disabled. The
Bypass Preview option is disabled by default. Enable this option only if you're certain that you're getting the desired
results.

How to Autoprovision Responsibility
Step 1: Define Responsibility Template criteria.

When autoprovisioning is enabled and you copy a responsibility template, the criteria are also copied. You can also
modify the criteria if the section is enabled on the questionnaire page. The Assign by Criteria section enables you to
add criteria and values that identify the representatives who must receive the responsibility with the Basic Info and
Scope you defined in the prior sections of this page. You can enable or disable the Bypass Preview option directly at the
template-level. After thorough testing, it's no longer necessary to preview each template and apply the results every
time autoprovisioning is run.

This process uses the AND operand if you specify multiple criteria and the OR operand when using multiple values
of the same criteria. For example, using the criteria defined in the above screenshot, the process will search for
assignments where these conditions are satisfied.

• Legal Employer = ARS US Legal Entity AND

• Job = HRM-Human Resources Manager OR HRM-Human Resources Specialist 1

Step 2: Schedule Autoprovisioning.

194

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 8
Areas of Responsibility

You can Autoprovision Responsibilities using either of these 2 options:

• Responsibility template row-level actions

• Autoprovision Responsibilities scheduled process from the Scheduled Processes work area.

This action is useful while you're testing the expected results of your responsibility template and helps ascertain that
the Autoprovision Responsibilities process will only process this specific template. You’ll receive a confirmation message
that the job has been submitted with the job ID returned. You can check the progress from the Scheduled Processes
work area or refresh your page. The process is complete when the Apply Autoprovisioning option is active.

Step 3: Apply Autoprovisioning.

The Apply Autoprovisioning action enables you to see the results in the context of that individual responsibility
template.

Note:  The Inactivated count is calculated based on worker assignments that no longer match the criteria for the
template such as promotion, local or global transfer or, termination. When inactivating these responsibilities, 2 things
happen:

• The status becomes Inactive.

• The end date is updated to the Autoprovision Responsibilities process system date.

Step 4: Restore Autoprovisioning.

You can restore the responsibilities to their last state after applying Autoprovision Responsibilities, in case you want to
revert the data changes.

Step 5: Bypassing the preview and apply step.

You can skip the preview and apply step of the Autoprovisioning Responsibilities process after you’ve tested the results
and behavior of your responsibility template.

After you’ve enabled the Bypass preview option on the responsibility template, new responsibilities and updates to
existing responsibilities are reflected directly against the people matching the criteria. You’ll no longer see a list of the
impacted people when applying autoprovisioning. The same applies if a representative no longer matches the criteria.
This means the respective AOR will be end-dated and inactivated automatically, and you’ll not see the person listed on
Autoprovision Responsibilities.

You can view and confirm changes directly in the representative’s area of responsibility.

For more information, see 24B What's New Autoprovision Areas of Responsibilities.

Dynamic Representative Scope
Dynamic representative scope enables you to reduce the number of overall responsibility templates. This is useful,
especially for organizations with several locations, business units, or departments.

Dynamic Representative Scope settings allow you to automatically assign these atrributes:

• Location

• Business Unit

• Department Scope

• Legal Employer

195

Oracle Fusion Cloud Human Resources
Using Global Human Resources

• Department Hierarchy

Chapter 8
Areas of Responsibility

For example, this resolves these scenarios where they need access only to the data where they work:

• The line manager or store administrator is responsible for their department.

• The retail or hotel manager is responsible for their location.

• The University department head is responsible for their business unit.

For more information, see Dynamic Representative Scope section, 24B What's New Autoprovision Areas of
Responsibilities.

Areas of Responsibility Integration with Work Contacts

You can specify how you want to display the representative name in the Representatives or Contact Us sections using
the Work Contacts option.

If you select Include in work contacts, the representative's name appears as a work contact along with the
representative type (Human Representative, Benefits Representative, for example). The representative’s name appears
in the Contacts section in the Directory and the Contact Us section. If the option is deselected the person doesn’t
appear in these pages.

Other representative types are also available, out of the box, or can be configured based on your requirements.

Examples of Setting Scope of Responsibility

Let's look at some examples of how you can define the scope of a responsibility.

Based on Assignment Information
Gail Williams is a Human Resources (HR) representative in Vision Corporation, UK. You assign her the HR representative
responsibility and set the scope of her responsibility to application developers based in Reading in the UK.

Field

Value

Business Unit

Vision Applications Development

Legal Employer

Vision UK

Country

Location

Job

UK

Reading

Applications Developer

196

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 8
Areas of Responsibility

Based on Name
Terry Smith is a benefits representative in Vision Corporation, UK. You assign him the benefits representative
responsibility and set the scope of his responsibility to workers whose names are within an alphabetic range (A to L).

Field

Legal Employer

From Last Name

To Last Name

Value

Vision UK

A

L

Based on Payroll Information
Grace Miller is a payroll representative in Vision Corporation, US. You assign her the payroll representative responsibility
and set the scope as external training staff in Vision Corporation, US.

Field

Value

Statutory Unit

Vision Training US

Legislative Data Group

External Training

Related Topics

• What's the recruiting responsibility type?

Areas of Responsibility Templates

Templates allow you to create a simple, less-cluttered responsibility description and scope just once, and reuse that
same definition multiple times. You can define templates separately from representatives, and can support different
scope patterns as your organization requires.

Responsibility templates are intended to create areas of responsibility with predefined scope for your representatives.
With a responsibility template, you can control and lessen the number of responsibility visible scope items displayed
on a worker's responsibility, so you choose only the scope that applies to your organization without any customization.
Templates will also default values on the worker responsibility but you can also specify required values for the worker
responsibility.

How You Create a Responsibility Template
You can create an area of responsibility template for responsibilities that you frequently need to assign to people. For
example, you may have a shared service center with 3 HR representatives covering workers in the same Legal Employer;

197

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 8
Areas of Responsibility

define a single responsibility template and assign to all 3 HR representatives. You can create areas of responsibility
templates from the Workforce Structure quick actions.

You can create a worker's responsibility from active, current, or future-dated templates. Whichever template you choose,
the basic responsibility information and the scope are displayed, by default. However, you can change the name, from
and to dates, and status. You need to specify a code for area of responsibility template, and can update any of the fields,
which are optional in the template. Scope fields will appear as read-only if default value for that field is specified in the
template. If a default value isn't provided, then you can choose or specify a value.

How You Delete a Template
Although, you can copy a responsibility template, you can't delete one if there are people associated to it. If
you want to display a warning confirmation message to users before deleting a template, you must enable the
HCM_SAVE_CHANGES_WARNING_ENABLED profile option.

Note:  Details in the template are currently independent of any changes in the worker level area of responsibility.
There isn't any synchronization of the start date, end date or status fields between the worker area of responsibility
and the template.

How You Assign a Template
You can either create a template and directly assign it to people or select people and associate them to a template.
When you associate workers to a template, their area of responsibility is listed in the Directly Assigned section. You can
also create different responsibilities from a template and assign it to the same person multiple times. For example, if
you configure Country in the template as not required, at the person-level responsibility, you can update each area of
responsibility to have different country values unique to the representative's service areas.

FAQs for Areas of Responsibility

What happens if I don't record a person's areas of responsibility?

The person doesn't appear in the Work Contacts lists of people for whom the person holds an area of responsibility.

What happens if I reassign a responsibility?

The responsibility you reassign is immediately visible in the assignment record of the person to whom it's reassigned.
The From Date of the responsibility is the current date, and there's no To Date.

The scope of the responsibility remains the same. The change is visible in the Work Contacts list of affected people
when the records are next viewed.

The assigned responsibility of the person from whom the responsibility is being removed, will be end dated effective
immediately. So, the existing To Date becomes the current system date.

198

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 8
Areas of Responsibility

If you are reassigning a responsibility that was created from a Responsibility Template with an end date (same as
template or modified), then after it's reassigned from one person to another, the end date will take on the end date of
the associated Responsibility Template. It'll not necessarily be the end date from the person-level responsibility.

If you're reassigning an autoprovisioned responsibility that was created and assigned because the original person
matches the template criteria, then after the responsibility is reassigned to someone else (that doesn't match criteria),
it's no longer considered autoprovisioned. So, you'll see the reassigned responsibility appear as a directly-assigned
responsibility. You'll then have to manually remove this assignment from the Responsibility Template, when the time
comes.

Can I reassign an inactive responsibility?
You can reassign future-dated, inactive responsibilities, but you won't be able to reassign past-dated, inactive
responsibilities.

What's the recruiting responsibility type?

You can assign the recruiting responsibility to a person and define the scope of responsibility to secure job requisitions
based on specific recruiting attributes.

The recruiting responsibility type controls the list of recruiters available in the Recruiter Selector field of the job
requisition and job offer.

Note:  If representative's scope is based on recruiting attributes including recruiting location hierarchy, recruiting
organization hierarchy, and recruiting type, these representatives won't appear in approvals, or in the Contact Us
section in the UI.

What is the naming convention I see in the responsibility name
when I create and assign a responsibility from a template?

In order to maintain a unique responsibility name for a person, the new responsibility name is created with the following
structure:

→ Template name + Assignment + system counter

You can rename the responsibility to a name of your choice from the Areas of Responsibility page.

How do I add or change a responsibility type?

You can add, change, or inactivate existing representative types using the PER_RESPONSIBILITY_TYPES lookup code on
the Manage Common Lookups page in the Setup and Maintenance work area.

199

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 8
Areas of Responsibility

Is there a limitation on the number of responsibility types I can define?
Yes, the fewer the better, but in general you want to stay stay well under 500 values. For more information, see Areas of
Responsibility Lookups.

200

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

9  Hire and Manage Workers

Overview of the Workforce Lifecycle

The workforce lifecycle is a series of stages starting with hiring, managing promotion, transfer, direct reports, contracts,
seniority, termination, and enabling HCM worker notifications. Human Resource (HR) specialists and line managers
perform various tasks in this workforce lifecycle.

Let's see what are the key tasks in a person's workforce lifecycle.

Task

Hire people

Description

Hire employees, contingent workers, nonworkers, and pending workers. As a part of this task, you also
create the person's first work relationship with the enterprise.

Promote and transfer workers

Promote workers. Transfer workers within the same legal employer or to a different legal employer.

Manage worker contracts

Manage contract information in worker assignments.

Calculate seniority dates

Calculate a person's seniority in the enterprise using seniority dates.

Terminate workers

Terminate an employee's work relationship.

Manage direct reports

Add and reassign line reports and reports of other types such as project reports and mentees.

Employment Processes

This table lists the employment processes based on the type of operation.

Type of Operation

Process Name

Changes in Application

Add Person

• Add Contingent Worker

• New person record is created

• Add Nonworker

• Add Pending Worker

• Hire an Employee

• New work relationship is created

• New assignment is created

Add Work Relationship

• Create Work Relationship

• New work relationship is created

• New assignment is created

201

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Type of Operation

Process Name

Changes in Application

• Convert Pending Worker

• New work relationship is created

• New assignment is created

• Source pending worker work relationship

is terminated

• Re-Hire

• New work relationship is created

• New assignment is created

• Global Temporary Assignment

• New work relationship is created

• New assignment is created

• Source assignment can be suspended

based on user input

• Global Transfer

• New work relationship is created

• New assignment is created

• Source work relationship is terminated

• Change Worker Type

• New work relationship is created

• New assignment is created

• Source work relationship is terminated

Add Assignment

• Add Assignment

• New assignment is created

• Add Temporary Assignment

• New assignment is created

• Source assignment can be made non-

primary based on user input

• Source assignment can be made non-

primary based on user input

• Source assignment can be suspended

based on user input

New date-effective update is inserted in the
assignment

Update Assignment

• Change Assignment

• Change Location

• Change Manager

• Change Working Hours

• Direct Reports

• Promote

• Promote and Change Position

• Request My Assignment Change

• Transfer

Correct Assignment / Work Relationship

• Correct Employment Details

Existing assignment row is corrected

• Edit Pending Worker

202

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Type of Operation

Process Name

Changes in Application

Remove Assignment/ Work Relationship
Changes

• Work Relationship

• Work relationship level attributes are

• Employment Start Dates

corrected

•

If you change the primary status of a
work relationship, then a date-effective
row is also inserted in the assignment
corresponding to the work relationship
change

• Delete Employment Details

• Date-effective update is removed from an

assignment

•

In case of multiple assignments, if
you delete the initial row for the newly
added nonprimary assignment, then the
secondary assignment is deleted

• Cancel Work Relationship

• Work relationship is removed from the

application

• All assignments that are under the
canceled work relationship are also
removed

Terminate Work Relationship

• Resign from Employment

• Work relationship is terminated

• Terminate Employment

• New date-effective update is inserted in

the assignment

Hire People

When to Create Person Records

You can create a person record when a worker is hired for employment in an organization. In this topic you will learn
when to create person records.

You create a person record when you:

• Hire an employee

• Add a contingent worker

• Add a nonworker

• Add a pending worker

• Add a contact to the record of another person

Person records continue to exist even when people leave a company. If a person gets rehired, you simply create a new
work relationship with the new legal employer on that same person record.

Here are some examples of when and how to create person records:

• You're hiring Alex as a contingent worker. Alex has never worked in your company before. He hasn't been an
emergency contact, dependent, or beneficiary of another employee in your company. So his person record
doesn't exist.

203

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

You must create a person record for Alex and a work relationship with his legal employer.

• You're hiring Sonia who was previously employed by your company. Sonia's person record already exists. When
you hire her the application pulls out her person record and asks you to confirm that she's the same person.

To rehire Sonia, you create a new work relationship with the new legal employer on the existing person record.

• You're hiring Arturo who has been a volunteer mentor in your company for some time. Arturo will continue

working as a volunteer after he's hired.

Arturo already has a person record. To hire him you just need to create a new work relationship. Arturo now has
two work relationships with the same legal employer.

• You're hiring Mary who's an emergency contact of another employee. Although Mary has never worked in the

company before, she has a person record because she's a contact of another employee.

If there's enough detail in her person record to identify her, you only need to create her a new work relationship
with the legal employer. If not, you create a new person record too.

Rehire a Worker

You create a person record and a work relationship in Oracle HCM Cloud when you hire an employee. When you rehire
an ex-worker, you create a new work relationship because the person record already exists in the application.

This procedure explains how to rehire a worker. You rehire a worker using the Hire an Employee quick action under My
Client Groups tab on the Home page.

Prerequisites
The worker record already exists in the application.

Specify Basic and Personal Information

1. On the Home page, click the Hire an Employee quick action under the My Client Groups tab.
2. Select Hire in the Hire Reason field.
3. Select US 1 Legal Entity in the Legal Employer field.
4. Enter the last and first name.
5. Enter the national identifier details.
6. Click Next.

Note:  The application displays a list of person records, including contacts, contract employees, and previous
employees, that match the information provided in the new person record.

7. Select the person record from the Matching Person Records list and click Continue
8. Verify the home address and email address.
9. Click Continue.

Specify Employment Information

1. Select the I-9 Status. This determines the new person's work relationship.
2. Select the business unit and the job for which you're hiring.
3. Select if the person is paid a fixed salary or on an hourly basis in the Hourly Paid or Salaried field.

204

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

4. Select the person's manager in the Manager Details section.
5. Click Continue.

Provide Compensation and Other Information

1. Enter the Salary Basis and the Salary Amount.
2. Add the required roles for the new person. By default, the employee role is assigned.
3. Review the information provided
4. Click Submit to complete the rehiring. You can add any missing information by searching for the person and

adding the information using the relevant quick action.

Hiring an Employee

Hire an Employee
You create a person record and a work relationship in Oracle HCM Cloud when you hire an employee. In this example,
you will hire an employee, Jennifer Grace to the US1 Legal Entity.

Watch video

The following table summarizes the key decisions for this scenario:

Decisions to Consider

In this Example

What should be Jennifer's salary range?

Jennifer's salary range must be between 40000 to 70000 dollars annually.

Will Jennifer be working from home?

Yes. Although Jennifer's work location is Chicago, but Jennifer will be working from home in Dallas.
This information is crucial in processing her payroll.

What roles should be assigned to her?

Employee

Do the following tasks to create Jennifer's person record:

1. On the Home page, click the Hire an Employee quick action under the My Client Groups tab.

2. Complete the fields as shown in this table.

Field

Hire Date

Hire Action

Hire Reason

Legal Employer

Last Name

First Name

Gender

Value

4/10/20

Hire

Hire to fill vacant position

US1 Legal Entity

Grace

Female

205

Chapter 9
Hire and Manage Workers

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Field

Date of Birth

3. Click the Add Row icon in the National Identifiers section.

4. Complete the fields as shown in this table.

Field

National ID Type

National ID

5. Click Continue.

6. Complete the fields as shown in this table.

Field

Address Line 1

City

State

Zip Code

Country

Value

3/12/69

Value

Social Security Number

471-51-8091

Value

113 Hopper

Dallas

TX

75206

Dallas

If you enter the ZIP code, the application automatically populates the city, state, and county. If there is more than one
valid address, all the addresses that are valid for the selected ZIP code are displayed.

7. Click the Add Row icon in the Phone Details section.

8. Complete the fields as shown in this table.

Field

Type

Country Code

Area Code

Number

9. Click the Add Row icon in the Email Details section .

10. Complete the fields as shown in this table.

Field

Type

Email

Value

Home Mobile Phone

United States 1

214

755-1975

Value

Home E-mail

jennifer@wfh.com

11. In the Legislative Information section, complete the fields as shown in this table.

Field

Marital Status

Value

Single

206

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Field

Highest Education Level

Citizenship

Status

12. Click Continue.

13. Select Not Started from the I-9 Status list.

14.Complete the assignment fields as shown in this table.

Field

Business Unit

Person Type

Job

Grade

Department

Working at Home

Worker Category

Assignment Category

Regular

Full Time or Part Time

Hourly Paid or Salaried

Value

Bachelor Degree

American

Active

Value

US1 Business Unit

Employee

Buyer

Prof03

Procurement US

Yes

White Collar

Full time regular

Regular

Full time

Salaried

15. In the Manager Details section, select Roth, Calvin from the Name list.

16. In the Payroll Details section, complete the fields as shown in this table.

Field

Tax Reporting Unit

Salary Basis

Salary Amount

Value

US1 Legal Entity

US1 Annual Salary

55000

Note that the legal entity must be associated with a legislative data group to enable payroll processing for the
employee. When you enter the salary, the salary range and compensation ratio are automatically displayed based on
the selected grade, if this information is defined when creating the grade.

17. By default, the employee role is assigned to the user.

18. Click Continue to review the information.

19. Review the new hire information and approvers for Jennifer's person record, and click Submit. Jennifer's person

record will be created when all required approvals are received.

20.In the Warning dialog, click Yes.

21. In the Confirmation dialog, click OK.

207

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

How You Create a Work Email

In the person record, you can add up to two work email addresses or add none at all. The work email address is stored in
the Oracle Identity Store but you can manage it using the security console.

Things to Remember

•

If you have the required access, you can change the primary work email address in the security console. If not,
you need to contact your administrator for the change. However, you can't change or delete the primary work
email address if it's already saved in the Oracle Identity Store.

• Any changes made in the security console reflect back in the HCM pages

• To add a secondary work email address, you must add a lookup value to the EMAIL_TYPE lookup type.

• You can change the secondary work email addresses in the HCM pages but you can't change the primary work

email address.

How You Specify Work Phones

A person can have only one primary phone. Typically, employees see others' phone details only if it's work related and
primary. If you specify a nonwork phone as primary then workers can't see the phone details.

Who can see which phone number is controlled by Oracle's virtual private database policy, which can't be changed

Access Security and Privileges
You can see a coworker's work and nonwork phone numbers if your role has these privileges

• Manage person phones data

• View person phones data

• Report person phones data

It's important to understand these phone lookup codes since the virtual private database policy relies on the lookup
codes:

Lookup Code

W1

W2

W3

WF

WM

Meaning

Work Phone

Second Work Phone

Third Work Phone

Work Fax

Work Mobile Phone

208

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

If you want to change the phone type, keep in mind the lookup code and how the VPD policy works with that lookup
code. Lookup codes starting with W indicate the phone number is public and can be viewed by all. Lookup codes not
starting with W indicate the phone number is private and can be seen only by people with the required privileges.

Contact Relationship Start Date Changes

Let's look at different scenarios and the outcome when a worker's hire date is changed. Vijay Singh's original hire date
was 15-Jun-2020 and he has a contact, Rahul.

Start Date

Changed Start Date

Contact Relationship Start Date

Outcome

15-Jun-2020

1-Jun-2020

15-Jun-2020

(original start date)

15-Jun-2020

1-Jun-2020

18-Jun-2020

15-Jun-2020

1-Jul-2020

15-Jun-2020

Contact relationship start date
changes to 1-Jun-2020

These are the changes in Rahul's
personal info:

• Start date of non-effective--
dated objects such as phone,
email, and other common
accounts, changes to 1-
Jun-2020.

• Start date of effected-dated
objects (address, visa, and
name) that don't have a split
change to 1-Jun-2020.

Contact relationship start date
and start date of non-effective-
dated and effective-dated objects
without split won't change because
the relationship start date is after
the original hire date.

If Rahul's person record has date-
effective objects (address, name,
visa) starting from 15-Jun-2020
with splits (15-Jun-2020 to 20-
Jun-2020 and 21-Jun-2020 to
end of time), then these can't be
synchronized to the new hire date
because of conflicts. As a result,
the entire transaction will be rolled
back.

How You Convert Pending Workers

You can convert pending workers to employees or contingent workers either manually or automatically.

209

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Manually: Use the Pending Workers quick action on the My Client Groups tab to convert pending workers. The hire
details are populated using the details from the person's pending worker record. You can edit these details and add
any additional information before converting. When you convert a pending worker, the work schedule is also copied on
conversion.

If you're a human resources specialist, you can use the Quick Convert option in the Actions menu to convert pending
workers. You can directly convert a pending worker to the proposed worker type without reviewing the hire details or
going through an approval process.

When adding, changing, or converting the pending worker if you can't see the Proposed Person Type attribute, then you
need to enable the Proposed Worker Type attribute. You can enable this attribute for the Employment Info region for the
Add Pending Worker, Edit Pending Worker and Create Work Relationship actions respectively in the HCM Experience
Design Studio.

If you cancel the conversion, or the pending worker record is rejected, the record remains in the application. You need to
resume the transaction from your Worklist notification

Automatically: Use the scheduled process, Convert Pending Workers Automatically in the Scheduled Processes work
area. The process includes all those pending worker records that have the Include for Automatic Conversion option set
to Yes. You specify whether to include a pending worker record in automatic conversion or not when you create the
pending worker. You can change this setting later by editing the pending worker record. You can also change the setting
for multiple pending workers at one time. On the New Workers to Process page, select the relevant pending worker
records and select either of these options:

•

Include in Automatic Conversion

• Exclude from Automatic Conversion

Candidates from Oracle Taleo Recruiting Cloud Service aren't included in the automatic conversion if there were errors
during import.

Note:  You can configure the Convert Pending Worker flow using the Create Work Relationship action in the HCM
Experience Design Studio.

Conversion Actions
When a pending worker is hired as an employee or a contingent worker and converted, you can specify an action from
one of these: Rehire an Employee, Add Employee Work Relationship, or Hire an Employee in case of the pending worker
being converted to an employee. In case of a pending worker being converted to a contingent worker, you can specify
the action as Renew Contingent Worker, Add Contingent Work Relationship, or Add Contingent Worker.

If a terminated contingent worker is rehired as a pending worker and converted the action is Hire. But, if you're adding
a work relationship for the same pending worker, then the action can be any one of these - Add Contingent Work
Relationship, Add Employee Work Relationship, Add Non-Worker Work Relationship, Add Pending Work Relationship,
and Renew Placement.

Note:  A point to note is that when you create, delete, or cancel a person type work relationship record, then the
person type usages record is deleted and recreated for that worker. As a result, a new person type usage ID is
generated for the worker.

210

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Automatic Conversion of Pending Workers

When you want to automatically convert pending workers, you can run the Convert Pending Workers Automatically
process using available conversion criteria. HR specialists can run this process from the Scheduled Processes work area.

If you don't select any criteria, then all conversion criteria will be selected by default.

Criteria

Action

Conversion Date

Enter the conversion date. The conversion date can be the same as the proposed start date of the
pending worker, or number of days before or after this date.

Proposed Worker Type

Select if the conversion is to contingent worker or employee. If you have both then run separate
instances for each type.

Country

Select the country for automatically converting pending workers.

Legal Employer

Select the legal employer for automatically converting pending workers.

Business Unit

Select the business unit for automatically converting pending workers.

Department

Select the department for automatically converting pending workers.

Location

Select the location for automatically converting pending workers.

Let's look at how you can use the conversion criteria in the process.

Scenario

Action

InFusion enterprise has pending workers
spread across legal employers in different
time zones. The pending workers must
be converted at the beginning of the
proposed start date.

InFusion has many pending workers of the
type Employee and rarely pending workers
of the type Contingent Worker.

• Schedule the process separately for each legal employer that’s in a different time zone.

• Schedule two instances of the process, one for the employee worker type, and the other for the

contingent worker type.

InFusion has many pending workers in
some locations, business units, or legal
employers, and very few in others.

• Schedule two instances of the process: one that runs daily for the selected location, business

unit and legal employer with many pending worker; another that runs on a periodic basis for the
selected location, business unit, and legal employer with few pending workers.

211

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Related Topics

• Employment Configuration Options

Examples of Creating Multiple Work Relationships for a Person

When you create a person record, you also create that person's first work relationship. Once a person record exists, you
can create additional work relationships with the same or different legal employers.

You manage work relationships using the Work Relationship quick action on the My Client Groups or My Team tab. Let's
look at some valid combinations of work relationships.

Multiple Work Relationships of Different Types with a Single Legal Employer
These work relationships can exist at the same time with the same legal employer because they're of different types.

Work Relationship Type

Legal Employer

Start Date

End Date

Employee

Corporation A

17 November, 2010

None

Contingent Worker

Corporation A

4 August, 2010

12 January, 2012

Nonworker

Corporation A

4 August, 2010

None

Multiple Work Relationships of the Same Type with Multiple Legal Employers
These work relationships can exist at the same time, even though they're all of the same type, because each is with a
different legal employer.

Work Relationship Type

Legal Employer

Start Date

End Date

Employee

Employee

Employee

Corporation A

1 January, 2011

Corporation B

3 April, 2011

Corporation C

17 June, 2012

None

None

None

Multiple Work Relationships of the Same Type with a Single Legal Employer
These work relationships can exist with the same legal employer, even though they're of the same type, because they're
sequential. If you create the second work relationship before the first is terminated, it will fail.

212

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Work Relationship Type

Legal Employer

Start Date

End Date

Employee

Employee

Corporation C

11 October, 2010

17 March, 2011

Corporation C

19 July, 2011

None

Multiple Work Relationships of Different Types with Multiple Legal Employers
These work relationships can exist at the same time because relationships with a single legal employer are of different
types.

Work Relationship Type

Legal Employer

Start Date

End Date

Employee

Corporation A

12 December, 2010

None

Nonworker

Corporation A

12 December, 2010

31 December, 2011

Contingent Worker

Corporation B

14 September, 2010

Employee

Corporation C

10 May, 2011

Nonworker

Corporation C

15 February, 2011

None

None

None

How You Default the Manager in Hire and Create Work
Relationship Flows

The line manager value is typically defaulted to the person doing the transaction in the Add Person and Create Work
Relationship responsive flows. You can change this value at any time.

However, if you don't want to default the manager value in an assignment, then you need to disable the Default Logged
in User as Line Manager Enabled (ORA_PER_EMPL_DFLT_LOGGED_USER_AS_LINE_MGR_ENABLED ) profile option.
The manager can also be defaulted from the position hierarchy if position synchronization is enabled or from the parent
department if the value of the profile option PER_DEPARTMENT_TREE_FOR_MANAGER is Yes.

The value in the Default Logged in User as Line Manager Enabled profile option doesn't impact these - HCM Data
Loader (HDL), REST, classic Add Person and Create Work Relationship flows, Manage Users, and Offer or Convert Offer
flows.

Worker Types

You select a worker type when you create a new person record or work relationship. Because a person can have multiple
work relationships of multiple types simultaneously, a person can have multiple worker types at once.

213

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

You manage work relationships using the Work Relationship quick action on the My Client Groups or My Team tab.

Which worker types apply at any time depends on the legal employer context. For example, consider this summary of a
single person's work relationships with the enterprise.

Work Relationship Type

Legal Employer

Start Date

End Date

Contingent worker

Corporation A

13 March, 2010

None

Employee

Corporation B

11 June, 2010

20 February, 2011

Nonworker

Corporation C

10 July, 2010

Employee

Corporation D

21 February, 2011

None

None

Contingent worker

Corporation D

21 February, 2010

31 December, 2010

On 1st March, 2011 this person is:

• A contingent worker in Corporation A

• An ex-employee in Corporation B

• A nonworker in Corporation C

• An employee and an ex-contingent worker in Corporation D

Identifying a Single Worker Type
When a single worker type is needed for a person, the worker type from the person's primary work relationship applies.

Related Topics

• What's a pending worker?

• What’s the Not Managed by HR system person type?

How Person Records Are Matched

When you create a person record, the application searches if a record already exists with the same details.

How Matching Records Are Identified
The application searches all person records (with the exception of Oracle Recruiting candidates) to find potential
matches, based on the enterprise setting in the Person Creation Duplicate Check option.

These are the Person Creation Duplicate Check option settings.

214

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Serial Number

1

2

3

4

5

6

7

Setting

None

National ID Country-Type-ID

Last Name, First Initial, DOB Or NID Country-
Type-ID

Last Name, First Initial, DOB, Gender Or NID
Country-Type-ID

Last Name, First Name, DOB, Gender Or NID
Country-Type-ID

NID

Last Name, First Initial, Date of Birth or National
ID

Chapter 9
Hire and Manage Workers

Will Find Duplicates

There are no potential matches identified for
the new person record.

If a person's national identifier matches the
national identifier value, country, and type of
ID. Note that if the person's national identifier
value is null, no duplicates are found.

If the new person's national identifier matches
a person's national identifier within the same
country and type, irrespective of whether the
names and birth dates match.

Alternately, if the last name and the initial of
the first name match, and if the new person's
birth date matches or either person's birth date
is null, irrespective of whether the NID matches
or doesn't match or is null.

If the new person's national identifier matches
a person's national identifier within the same
country and type, irrespective of whether the
names, gender, and birth dates match.

Alternately, if the last name and the initial of the
first name do match, and if the new person's
birth date and gender match or either person's
birth date or gender are null, irrespective of
whether the NID matches or doesn't match or is
null.

If the new person's national identifier matches
an existing person's national identifier within
the same country and type, irrespective of
whether the names, gender, and birth dates
match.

Alternately, if the last name and the first name
do match, and if the new person's birth date
and gender match or either person's birth date
or gender are null, irrespective of whether the
NID matches or doesn't match or is null

Similar behavior as setting 2 above, except if
national identifiers from different countries
have matching numbers then additional
duplicates may be found.

Similar behavior as setting 3 above, except if
national identifiers from different countries
have matching numbers then additional
duplicates may be found. Note that this is the
default behavior when no option has been
explicitly selected for the check.

215

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Serial Number

Setting

Will Find Duplicates

8

9

Last Name, First Initial, Date of Birth, Gender or
National ID

Last Name, Full First Name, Date of Birth,
 Gender or National ID

Similar behavior as setting 4 above, except if
national identifiers from different countries
have matching numbers then additional
duplicates may be found.

Similar behavior as setting 5 above, except if
national identifiers from different countries
have matching numbers then additional
duplicates may be found.

Examples of Matching Person records
You're an HR specialist creating this person record:

First Name

Last Name

Date of Birth

National Identifier
Country

National Identifier
Type

National Identifier
Number

John

Ward

25 March 1963

US

Social Security
Number

390-89-8128

The application compares these details with those in existing person records and displays these 4 potentially matching
person records. By default, the enterprise option is null, which is equivalent to selecting the option which matches last
name, first initial, and date of birth, or national ID and its country and its type.

First Name

Last Name

Date of Birth

National Identifier Country-Type-
Number

Jennifer

Juana

Josie

Tyler

Ward

Ward

19 June 1969

US-SSN-390-89-8128

25 March 1963

FR-DL-558743776318

25 March 1963

US-SSN-872-19-9398

Let's see which options would find each of these people as potential duplicates, and why:

First Name

Jennifer Tyler

Person Creation Duplicate Check Setting

Reason for Match

Any option except None

Though the first name, last name, and date of
birth don't match, still Jennifer's person record
qualifies as a potential match with John due to
the match of the national ID and its country and
its type

Juana Ward

Either of the above options that check first
name initial but not full first name.

Though the national identifiers don't match,
 still Juana's person record qualifies as a

216

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

First Name

Person Creation Duplicate Check Setting

Reason for Match

potential match with John due to the following
reasons:

• Same last name as John Ward

• Same date of birth as John Ward

• First name starts with same character

Josie Ward

Either of the options that check first name
initial but not full first name.

Though the national identifiers don't match,
still Josie's person record qualifies as a potential
match with John due to the following reasons:

• Same last name as John Ward

• First name starts with the same character

• Same date of birth as John Ward

Related Topics

• How National Identifiers are Validated

• Candidate Duplicate Check and Merge After Job Offers

Examples of Employment Information for Nonworkers

Some employment information is marked as required for all workers and nonworkers. The amount of additional
information that you must provide in nonworker assignments depends on the nonworker type.

You add employment information for nonworkers using the Add a Nonworker task in the New Person work area.

Nonworker Who Receives No Payments
Ellen Woods is a volunteer in your organization; a government body meets her expenses. She receives no payments
from the legal employer, but does report to a manager there. All other information is optional.

Nonworker Who Receives Payments
Todd Granger is a retiree. When Todd retired, you terminated his employee work relationship with the legal employer
and created a new, nonworker work relationship with the same legal employer. As a retiree, Todd receives payments
from the legal employer. Therefore, Todd's assignment must contain payroll information. The assignment status and
person type values on the assignment must also allow payments to be made. All other information is optional.

Nonworker Who Has Other Work Relationships
A person can have multiple work relationships at once, but each relationship is always independent of the others. For
the nonworker work relationship, you enter only the information required for that relationship. For example, if the
person receives no payments in the nonworker assignments, then you don't provide payroll information for those
assignments, even if the person receives payments in assignments of other types.

217

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

FAQs for Hire People

How can I create a user account for a new worker?
When you create a person record, a user account is created automatically if automatic creation of accounts is enabled. If
a user account isn't created automatically, then an authorized user can create it on the Security Console or using SCIM
(REST) APIs.

You can link the account to the person record using the Manage User Account or Create User page.

What's a pending worker?
A person who will be hired or start a contingent worker placement and for whom you create a person record that's
effective before the hire or start date.

A pending worker is a person who's yet to start employment and doesn't have a person record in the application. You
create a pending worker record with a date that's effective before the hire date.

You convert a pending worker to the proposed worker type when the new hire is confirmed. For example, when a new
employee's hire is completed, you convert the pending worker record to an employee record. The pending-worker
functions provide greater control of the hiring process than hiring an employee or adding a contingent worker with a
future start date.

Can I enter more information about an emergency contact?
Yes, you can. You need to update the contact's person record to enter additional information such as an address or a
national ID. A person record is created automatically when you submit the associated employee or nonworker record.

Employees and nonworkers can also maintain information about their own contacts.

How can I create other types of contacts for a person?
When you create a person's record, you can identify an emergency contact for the person.

When you edit a person's record, you can add more contacts, any of which can be an emergency contact. If you want to
identify a person's contact as a beneficiary or dependent, you need to edit the person's benefits information.

How can I create multiple nonworker roles for a person?
You can create separate assignments for each nonworker role in the same nonworker work relationship. You can select a
nonworker person type for each assignment.

For example, a nonworker could have three assignments with a single legal employer, two as a paid volunteer, and one
as a retiree.

Why can't I see the person number for this new person record?
Based on your enterprise settings, the person number is generated after the Add Person transaction is approved. For
example, once the transaction is approved, you can see the person number on the Person page.

218

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Why can't I see the current manager when I am adding a person as a direct report?
This is because the person doesn't have a manager currently.

Promote and Transfer People

Promoting People

Example of a Worker Promotion
You're a human resources (HR) specialist promoting Stacey from a senior consultant to director of learning in the
Learning US department. Her manager will remain the same.

The promotion involves these changes for Stacey:

• New job and grade

•

Increased salary

Let's look at the steps to update the key values for this promotion. For other fields, you can use the default values.

Select Stacey and the Promotion Action

1. On your home page, click the My Client Groups tab, and then select the Promote quick action in the

Employment area.

2. Search for Stacey Kaufman and select her record.
In the When and Why section, enter these values.
3.

Field

Value

When does the promotion start?

Select the date the promotion takes effect.

What's the way to promote?

Promotion

Why are you promoting Stacey

Performance

Kaufman?

4. Click Continue to proceed.

Change Promotion Information

1.

In the Promotion section, enter these values.

Field

Job

Value

Director of Learning

219

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Field

Grade

Value

Prof04

2. Click Continue to proceed.

Change Salary Information

1.

In the Salary section, enter these values.

Field

Value

Salary Basis

Desired salary basis

Salary Amount

Changed salary value

2. Click Submit to complete the transaction.

Example of a Worker Promotion with Position Change in Redwood
You're a line manager promoting Vijay Singh from a senior software developer to a manager of software development
in the Hyderabad department of InFusion Corporation. In his new role he will report to Ed Kelly. This will require making
job and department changes to his existing position.

The promotion involves these changes for Vijay:

• Modifying his existing position

• Making assignment changes

• Changing his existing manager

•

Increasing his salary

• Adding 2 new direct reports

Let's look at the steps to update the key values for this promotion. For other fields, you can use the default values.

Select Vijay and the Promotion Action

1. On your home page, click the My Client Groups tab, and then select the Promote and Change Position quick

action in the Employment area.

In the Info to include step, select Managers, Salary, and Direct Reports.

2. Search for Vijay Singh and select his record.
3.
4. Click Continue to proceed.
5.

In the When and why step, enter these values.

Field

Value

When does the promotion start?

Select the date the promotion takes effect.

220

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Field

Value

What's the way to promote?

Promotion

How do you want to do this action?

Modify existing position

Why do you want to promote?

Performance

Business Unit

India Development Centre

Position

Manager - Software Development

6. Click Continue to proceed.

Change Position Information

1.

In the Position Details step, enter this value.

Field

Grade

Job

Value

M1

Software Development Manager

Department

InFusion-Hyderabad

In Position override step, accept the position override values.

2. Click Continue to proceed.
3.
4. Click Continue to proceed.
5.
6. Select Yes from the Working as Manager list.
7. Click Continue to proceed.

In the Assignment step, verify the values defaulted from position.

Change Manager

1. Click Edit beside the line manager row in the Managers step.
2. Enter these values.

Field

Select Person

Manager Type

Value

Ed Kelly

Line Manager

3. Click Continue to proceed.

221

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Change Salary

1.

In the Salary step, enter these values.

Field

Value

Salary Basis

Desired salary basis

Salary Amount

Changed salary value

2. Click Continue to proceed.

Add Direct Reports

1.

In the Direct Reports step, click Add and enter these values.

Field

Person

Value

Emily Thorn

Reporting Relationship

Line Manager

2. Repeat the above step by searching for Lucy Hall.
3. Click Submit to complete the transaction.

Related Topics

• Position Override in Redwood Employment Processes

Promote Actions

You can use these actions to promote people.

Action

Promote

How it works

Updates the current assignment. Along with that user has the option to manage salary, compensation,
 payroll, and document records.

Use this process if you want to update the above mentioned areas while promoting the worker.

Promote and Change Position

Updates the position while promoting the worker. So, if you're looking to update the position and
promote in the same process then only you should use this.

Use this if you would like to manage position, salary, compensation, payroll, and document records
while promoting a worker.

Position change and promote are now part of the same approval process. Earlier, since these were two
different processes two approval process used to trigger and promote could only be initiated once the
position changes were approved.

222

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Transfer Actions

You can use these actions to move people within the same assignment.

Action

Transfer

How it works

Updates the current assignment and leaves the work relationship and any other assignments
unchanged.

Local and Global Transfer

If you don't change the current legal employer, the transfer is local and within the same assignment.
Local transfer updates the current assignment and leaves the work relationship and any other
assignments unchanged.

The assignment number and ID remain the same. The local transfer does the same update as the
standalone Transfer guided process. Based on the data that you change, the application automatically
determines if it’s a local or global transfer or a global temporary assignment.

You can use these actions to move people within the same legal employer.

Action

How it works

Add Assignment

Creates an additional assignment leaving the work relationship, primary assignment, and any other
assignments unchanged. By default, the additional assignment is nonprimary.

You end the assignment by selecting the End Assignment action.

Temporary Assignment

Creates an additional assignment and suspends the existing assignments. The work relationship
remains unchanged.

The status of the existing assignments changes to Suspended- Payroll Eligible by default. You can
change this status to any other value or revert to the original status using the Change Assignment flow.

This action is recommended when the organization has clear guidelines about temporary assignments
and the person is expected to return back after the temporary assignment ends. If you have a
requirement to add an additional assignment for the person and end the source assignment in future,
 then you must use add assignment instead of temporary assignment.

It's recommended to not create a new temporary assignment by using an existing temporary
assignment as the source.

End Temporary Assignment

Ends the temporary assignment and reinstates the original assignments by the specified return date.

You can use these actions to move people to a different legal employer.

Action

How it works

Create Work Relationship

Creates an additional work relationship and associated assignment leaving the existing work
relationship, primary assignment, and any other assignments unchanged.

223

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Action

How it works

Local and Global Transfer - Global Transfer

Local and Global Transfer - Global
Temporary Assignment

If you create an additional work relationship in another legal employer, you have two concurrent work
relationships in different legal employers.

You end a work relationship by using the Terminate action.

If you change the current legal employer and select the transfer type as permanent, then it results in
a global transfer. Permanent global transfer ends the current assignment and any other assignments,
 and ends the current work relationship. Additionally, it creates a new work relationship in the newly
selected legal employer.

Note:  The global transfer won’t delete future dated assignments if a time card exists
for any assignments in the source work relationship. If a time card exists, the application
stops the global transfer and displays an error message. If you don't want the application
to prevent deletion of a future dated assignment when a time card exists, set the
ORA_PER_EMPL_DISABLE_TIME_CARD_CHK_CANCEL_WR profile option value to Y. This check isn’t
applied when only a date-effective assignment record is deleted.

The new primary assignment has all the data from the old one by default, but you can change it.

If you change the current legal employer and select the transfer type as temporary, then it results in
a global temporary assignment. Global temporary assignment suspends only the current assignment
and doesn't end the current work relationship. You create a new work relationship and a primary
assignment within the new legal employer. The new primary assignment has all the data from the old
one by default, but you can change it.

You create a primary assignment for the new work relationship in the new legal employer. The status
of the existing assignments in the source work relationship changes to Suspended-Payroll Eligible by
default. You can change the status of the existing assignments from Suspended-Payroll Eligible to any
other value. You can reverse this change in status to the original status using the Change Assignment
flow.

This action is recommended when the organization has clear guidelines about global temporary
assignments and the person is expected to return back after the global temporary assignment ends.
If you have a requirement to add an additional work relationship for the person and end the source
work relationship in future, then you must use create work relationship instead of global temporary
assignment.

It’s recommended to not create a new global temporary assignment by using an existing global
temporary assignment as the source.

End Global Temporary Assignment

Ends the temporary assignment and work relationship and reinstates the assignments with the original
legal employer.

Mass Legal Employer Change (For HR
specialists)

Transfers multiple employees from different legal employers to the same destination legal employer.

Ends the current work relationships for the employees and creates new ones within the destination
legal employer.

Creates new primary assignments and ends the old ones. The new primary assignments have all the
data from the old records by default, but you can change it.

What Happens to Source Assignment Status
You can override the default status of the source assignment by manually selecting it in the Local and Global Transfer
(Global Transfer and Global Temporary Assignment only) and Add Assignment (Temporary Assignment only) flows.

224

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

This table shows the properties of the source assignment status:

Field Property

Local and Global
Transfer (Transfer)

Local and Global
Transfer (Global
Transfer)

Local and Global
Transfer (Global
Temporary
Assignment)

Add Assignment
(Permanent)

Add Assignment
(Temporary)

Visibility

No

Yes

Yes

No

Yes

Values

Not applicable

All inactive HR
statuses

All active and
suspended HR
statuses

Not applicable

All active and
suspended HR
statuses

Selected Value
Applicability

Not applicable

All assignments of
the source work
relationship

Only the assignment
which was used to
start the flow

Not applicable

Only the assignment
which was used to
start the flow

Here are some points to keep in mind regarding the source assignment status:

• The status is controlled by the application and it's automatically available in the applicable flows.

• The status value must be valid as of the effective date of the corresponding flow.

• The default status of the source assignment is displayed.

• The default sort order of the status is displayed first, followed by descending order of system status (in the

order Suspended to Active) for Global Temporary Assignment and Temporary Assignment flows.

• The status isn't supported in the HCM Data Loader, REST, and HCM Spreadsheet Data Loader tools.

Related Topics

• How You Reassign or Add Direct Reports During Local and Global Transfer

• Employment Profile Options

Local and Global Transfer

You can transfer the worker within the same legal employer or to a different legal employer using the Local and Global
Transfer flow. This flow can be used to do these types of transactions:

Transaction

Does the legal employer change?

Local transfer within the assignment

No

Global transfer

Yes, within the same legislation and outside the legislation.

Global temporary assignment

Yes, within the same legislation and outside the legislation

225

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

During a permanent global transfer, the worker data is defaulted from the assignment where the transfer is initiated.

If you have configured the application to view assignment history during a global transfer, and assignment-level
security is enabled, then you can only see those assignments for which you have access. For example, if you have
access to only the newly created assignment in global transfer, then you can’t view the complete assignment history.
The person who has access to both the source and target assignment can view both the assignments in the Business
Title field and employment history. For more information, see the document Implementing Assignment-Level Security
in HCM (Doc ID 2700661.1) on My Oracle Support (https://support.oracle.com).

Related Topics

• Why isn't the Create Primary Work Relationship field visible for a global transfer even though it's set to Visible in

the Transaction Design Studio?

Data Copy and Display Options for Local and Global Transfer

You can select data that you want to copy from the source to the target assignment during a permanent legal employer
change (global transfer). The worker data is defaulted from the source assignment where the transfer is initiated.

These tables describe the visibility of the various sections in the Local and Global Transfer flow and what data gets
copied from the source to destination for a global transfer and global temporary assignment.

Personal Details and Other Info

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

Personal Details

No

Only when
global transfer or
global temporary
assignment is
to a different
legislation.

Not applicable

Not applicable

Not applicable

This section
isn’t available in
HCM Experience
Design Studio
and its visibility is
controlled by the
application.
The section is
displayed only if
there is a change
in the legislation
of the person’s
work relationship.
The reason is that
a new name and
legislation record
are automatically
created based on
the destination
legislation. The
Biographical Info
and National
Identifier regions
are included
because some

226

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

Contact Info

No

Needs to be
enabled using
HCM Experience
Design Studio.

Not applicable

Not applicable

Not applicable

Legislative Info

No

Only when
global transfer or
global temporary
assignment is
to a different
legislation.

Not applicable

Not applicable

Yes

Other Info

No

Needs to be
enabled using
HCM Experience
Design Studio.

Yes

Yes

Yes

applications
such as Payroll
or Benefits may
require this
information and
including the
regions during the
transfer process
reduces additional
navigation.

This section is
displayed when
you select Contact
Info from the
questionnaire
page. If there is
existing data,
 the data will be
displayed. If no
data exists, you
can enter the data
as part of the
transfer process.

This section
isn’t available in
HCM Experience
Design Studio
and its visibility is
controlled by the
application.
Legislative
information, such
as a person’s
marital status,
 ethnicity, religion,
 or gender will
be copied to
the destination
legislation if the
lookup codes are
the same as the
source legislation.
If they are not the
same, the field will
be blank, and you
can select from
the destination
country’s valid list
of values.

This section is
displayed when
you select Other
Info from the

227

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

questionnaire
page. If there is
existing data,
 the data will be
displayed. If no
data exists, you
can enter the data
as part of the
transfer process.

Assignments and Work Relationships

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

Yes

Always

Yes

Yes

Yes

Assignment and
Work Relationship
(nonflexfield
attributes and
descriptive
flexfields)

By default, all
assignment and
work relationship
information
including
descriptive
flexfields (DFF)
are copied.
However, you
can change the
assignment and
work relationship
values. The
information that
exists as of the
global transfer date
is copied if the
Future Assignment
Changes Copy
Enabled profile
option is set to Y.
You can select the
source assignment
status during a
global transfer or
global temporary
assignment.

You can also
override the
default source
assignment status
by selecting
the status from
the page in
the responsive

228

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

Yes

Always

Yes

Yes

No

Assignment and
Work Relationship
(developer
descriptive
flexfields)

Assignment
(extensible flexfield
contexts)

No

Needs to be
enabled using
HCM Experience
Design Studio.

Yes

Yes

Yes

Work Relationship
(V1 Seniority Dates)

No

Only if you use
version 1 (V1)
seniority dates.

Yes

Yes

Yes

Local and Global
Transfer flow.

By default,
 developer
descriptive
flexfields (DDF) are
copied.

By default, all
assignment
extensible flexfield
(EFF) contexts are
copied. However,
 you can select
the contexts that
you don't want to
copy. The smart
list of values only
provides the list
of contexts which
has data populated
in the source
assignment.
This feature is
available only
when you perform
a global transfer.

During the
global transfer
transaction, you
can select to
copy the list of
extensible contexts
in the When and
Why section.
However, the list of
extensible contexts
isn’t refreshed
even if you change
the legal employer
or change the
global transfer to
global temporary
assignment.

Only the V1
enterprise seniority
date is copied.

229

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Payroll and Salary

Section or
Component

Visible by Default Visibility
Condition

Chapter 9
Hire and Manage Workers

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

Payroll Details
(Payroll)

Yes

Always

Yes (only for global
transfer)

No

No

Payroll Details (Tax
Reporting Unit)

Depends on
legislation

Payroll Details
(person costing
overrides)

No

Needs to be
enabled using
HCM Experience
Design Studio.

Needs to be
enabled using
HCM Experience
Design Studio.

Yes (only for global
transfer)

No

No

No

No

No

By default, all
payroll information
is copied only
if the source
and destination
legal employers
belong to the
same legislative
data group. The
information that
exists as of the
global transfer
date is copied
but changes
effective after the
global transfer
date aren’t. If the
transfer results
in a new payroll
relationship, the
information that
exists at a payroll
relationship level is
also copied.
This feature is
available only
when you perform
the global transfer.

The Payroll
attribute defaults
to the value from
the source. You
have the option to
override the value
if required.

The Tax Reporting
Unit attribute
defaults to the
value from the
source. You have
the option to
override the value
if required.

By default, costing
overrides aren't
copied. If you
choose to copy,
 then the copy
occurs across the
four levels at which

230

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

Person Costing

No

Needs to be
enabled using
HCM Experience
Design Studio.

Yes (only for
permanent global
transfer)

No

No

Payroll Details
(calculation cards)

No

Always

Yes (only for global
transfer)

No

Payroll Details
(recurring element
entries)

No

Needs to be
enabled using
HCM Experience
Design Studio.

Yes (only for global
transfer)

No

Payroll Details
(nonrecurring
element entries)

Payroll Details
(Time Card

No

Not applicable

No

No

Conditional

Needs to be
enabled using

Yes (only for global
transfer)

No

No

No

No

No

the person costing
setup is held.

The Person
Costing section
allows you to
update the costing
information before
it’s copied to
the destination
assignment,
whereas the Payroll
Details (person
costing overrides)
section doesn’t.
The other major
difference between
the two sections
is that the Person
Costing section
doesn’t support all
four costing levels,
 it only supports
the Assignment
costing level.
Additionally, the
two sections are
mutually exclusive;
you must only
enable one section,
 but not both.

Each country’s
legislation
determines the
calculation cards
and components
that are copied.

Copy for element
entries are subject
to eligibility. If you
want to exclude
certain elements
from the copy, you
have to define an
element (object)
group with the
usage type of
Global Transfer.

Data not copied.

Visibility depends
on legislation.

231

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

Required and
Overtime Period)

HCM Experience
Design Studio.

Payroll Details
(balances)

No

Needs to be
enabled using
HCM Experience
Design Studio.

No

No

No

Salary (Type 1, Type
3, and Type 4)

Yes

Always

Yes

No

No

The Time Card
Required and
Overtime Period
attributes default
to the values from
the source. You
have the option to
override the values
if required.

You carry forward
assignment and
relationship
level balances
using balance
adjustments from
the source to
the target legal
employer during
the global transfer
of employees.
The overall balance
that's copied
includes:

• The balance
calculated
within the
source payroll
relationship.

• The balances
copied to the
source payroll
relationship
for prior
global
transfers.

The salary
information is
defaulted from the
source assignment
when the legal
employers involved
in the transfer
have the same
legislative data
group. For Type 1
salary basis, the
salary amount is
determined by the
user. For Type 3
salary basis, the
salary amount is
determined by
rates. And for type

232

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

Salary (Type 2)

Yes

Always

Only in certain
scenarios.

No

No

4 salary basis, the
salary amount
is determined
by simple
components.

For Type 2
salary basis, the
salary amount
is determined
by incremental
components.
The salary basis
setting should be:
Enable component
selection during
allocation.

Compensation and Benefits

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

Compensation
(Individual
Compensation
Plan)

Yes

Always

Yes (only for global
transfer)

No

No

Compensation
(Compensation
Plan)

Yes

Always

Benefits

No

Needs to be
enabled using
HCM Experience
Design Studio.

No

No

No

No

No

No

When you transfer
people globally,
 the process now
automatically
copies individual
compensation
awards and any
document record
attachments from
the source legal
employer to the
destination legal
employer.

None

You can select to
transfer balance
for a life event
within the same
legislative data
group.
You can choose
the life event for
global transfer
and transfer the

233

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

benefits balance to
the worker's new
assignment.

Performance Goals and Documents

Section or

Component

Visible by Default Visibility

Is Data Copied

Is Data Copied

Is Data Copied

Description

Condition

During Transfer

During Transfer

During Transfer

Within Same

to Different

to Different

Legislative Data

Legislative Data

Legislation

Group

Group Within

Same Legislation

Performance Goals

No

Only when there is

No

No

No

The performance

and Documents

(Performance

Documents and

Performance

Goals)

a global transfer.

goals and

documents

information is not

copied. However,

 you can move

performance goals

and documents to

the workers’ new

assignments within

a legal employer

when using the

Local and Global

Transfer guided

process.

You can select to

move performance

goals and

documents based

on review periods.

You can move

all the workers'

performance goals

and documents

associated with all

review periods. Or,

 you can choose

only current and

future review

periods and

234

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Section or

Component

Visible by Default Visibility

Is Data Copied

Is Data Copied

Is Data Copied

Description

Condition

During Transfer

During Transfer

During Transfer

Within Same

to Different

to Different

Legislative Data

Legislative Data

Legislation

Group

Group Within

Same Legislation

leave historic

performance goals

and documents

associated with

the inactive

assignments.

Managers and Direct Reports

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

Managers

Yes

Always

Yes

Yes

Yes

Add Direct Reports Yes

Always

Not applicable

Not applicable

Not applicable

Reassign Existing
Reports

No

Only when the
selected worker
has direct reports.

Yes

Yes

Yes

By default,
 manager
information
is copied that
includes all
manager types,
 such as line
manager and
project manager.
However, you
can change the
manager values.
The information
that exists as of the
global transfer date
is copied if the
Future Assignment
Changes Copy
Enabled profile
option is set to Y.

You can add new
direct reports
during a global
transfer.

This section is
displayed on the
questionnaire page
only if the user
has direct reports
assigned.

235

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

When the
reporting manager
of a pending
worker is globally
transferred, the
worker continues
to report to the
source assignment
of the manager
even though
the assignment
becomes inactive
after the global
transfer.

Other Sections

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

Employment
Contracts

No

Weekly Working
Hours

No

Absences

Yes

No

No

No

Yes

Yes

Yes

Yes

No

No

Only if the
destination legal
employer is
contract enabled.

Needs to be
enabled using
HCM Experience
Design Studio.

Needs to be
enabled using
HCM Experience
Design Studio.

No data is copied
because contracts
are defined within
a legal employer
context.

By default, all
working hours
information is
copied, however,
 you can change
this information.

All accrual plans
are supported.
The Local and
Global Transfer
process automates
the accrual plan
enrollment and
copying of plan
balances. When
an employee is
transferred, all
active plans are
end-dated in the
old organization.
If the employee
is eligible for the
same plans in the

236

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

Work Schedule
Assignments

Not applicable

Not applicable

Yes

Yes

Yes

new organization,
the application
automatically
enrolls the
employee to the
same plans.

Only if the
schedule and
exceptions are
available.
Local and
global transfers
also automate
work schedule
enrollment
and copy
work schedule
exceptions. When
you globally
transfer someone,
 all active and
future work
schedules and
work schedule
exceptions are
automatically
end dated in
the old Legal
Employer. The
transfer process
automatically
links them with
the same work
schedule and
work schedule
exceptions in
the new Legal
Employer, if the
schedule and
exceptions are
available.

Additionally, as a
manager or HR
specialist, you
can review all
work schedule
assignments
affected by the
transfer. You
can see relevant
messages about
end-dating and
copying schedules
and exceptions
using the Change

237

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Section or
Component

Visible by Default Visibility
Condition

Is Data Copied
During Transfer
Within Same
Legislative Data
Group

Is Data Copied
During Transfer
to Different
Legislative Data
Group Within
Same Legislation

Is Data Copied
During Transfer
to Different
Legislation

Description

Seniority Dates

Yes

Not applicable

Not applicable

Not applicable

Not applicable

Legal Employer
dashboard.

This is a read-
only section. Only
the person-level
seniority date rules
that are configured
to be displayed in
guided flows are
visible.
This table shows
the seniority dates
that are displayed
for different
seniority date
versions:

• V1 seniority

dates:
Enterprise
and legal
employer
seniority
dates.

• V3 seniority
dates: Only
person-level
seniority date
rules that are
configured to
be displayed
in guided
flows.

The document records will be moved from the source to the destination assignment during the global transfer only if
the ORA_PER_DOR_ASG_LVL_MOVE_ON_CHANGE_LE profile option is set to Y. In case of multiple assignments in the
source work relationship, only document records from the assignment used to start the global transfer will be moved.

These features aren’t specific to a worker's assignment and aren’t directly impacted due to a change in legal employer.
Hence, there is no data copy option for these features.

• Person Extensible Flexfields

• Talent Profiles

• Development Goals

• Career Development Plans

• Talent Review Meetings

• Succession Management Plans

• Learning Information

• Workforce Reputation Information

238

Oracle Fusion Cloud Human Resources
Using Global Human Resources

• Employee Wellness Information

Chapter 9
Hire and Manage Workers

Related Topics

• How You Reassign or Add Direct Reports During Local and Global Transfer

• How Global Transfers Impact Performance Goals

• Automatic Plan Enrollment and Balance Copy During Local and Global Transfer

• Can I copy individual compensation allocations as part of a global transfer?

• Can I copy salary as part of a global transfer?

Mass Legal Employer Change

When you need to transfer multiple employees to the same legal employer, use the Mass Legal Employer Change task.
This accomplishes the transfers in a single batch.

It uses the Local and Global Transfer process to copy the selected employees' assignment and work relationship data
from the source to the destination work relationship. The data is copied as of the global transfer date along with any
future-dated changes.

Some things to consider when performing this kind of transfer.

• Use this task to transfer people from different legal employers into the same target legal employer.

• Use this task when changing legal employers within the same country or legislation. If you use this task to mass
change legal employers across legislations, it doesn't copy the data for salary and payroll. Additionally, there
may be issues with certain personal data elements that aren't copied across legislations.

For example, a person is transferring from the Netherlands to the United States. In the Netherlands, their
marital status is Living Together. Because the US doesn't have this status, their marital status would be null.
However, if the marital status is Married, both legislations support that status, and it would be copied during
the transfer.

• You can override certain assignment attributes from the source assignment that are common and apply to the

set of workers transferring to new legal employers.

For example, these attributes can include the business unit, department, and location. However, you can't
override assignment attributes like job, grade, and position because they are unique and may differ for each
worker in the destination assignment.

For further info, see HCM Experience Design Studio in the Help Center.

• All types of direct reports are copied to the assignment, which gets newly created during the Mass Legal

Employer Change process.

• Pending and draft performance goals aren't transferred to the new assignment when you do a mass legal

employer change. Therefore, you must make sure approvals for such performance goals are complete before
you perform the transfer.

• You can't do a mass legal employer change for an employee that has:

◦ Future-dated global transfer or global temporary assignment change
◦ Pending transaction awaiting approval that involves an assignment change
◦ Work relationship start date with the same as the effective date of the transfer

239

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Data Transferred
This task copies the following data items.

Chapter 9
Hire and Manage Workers

Data Item

What This Includes

Override Assignment Values

You can provide specific values for certain assignment attributes. These values:

1. Apply to all people being transferred
2. Override the corresponding values on their source assignment

Additional Changes

By default, the task copies all assignment extensible flexfield (EFF) contexts. However, you can choose
which contexts you don’t want to copy to the worker's new assignment.

Salary Changes

You can copy the salary from the primary assignment of the previous work relationship. However:

1. The legal employers involved in the transfer must have the same LDG.
2. The salary basis must be one of the following.
◦ Type 1: Salary amount is determined by the user.
◦ Type 2: Salary amount is determined by components and the salary basis setting is Enable
component selection during allocation.
◦ Type 3: Salary amount is determined by rates.

Performance Goals and Documents
Related Changes

You can move performance goals and documents to the worker’s new assignments. You can move:

All workers' performance goals and documents associated with all review periods

Only current and future review periods, excluding historic performance goals and documents
associated with inactive assignments.

When you perform a mass employee transfer:

1. For workers whose performance data is the same across all assignments within their work

relationship, the task copies only the performance goals and documents associated with the
primary assignment to the new assignment.

This performance data includes:

◦ Performance goals
◦ Goal plans
◦ Performance documents

The performance goals and documents associated with the secondary assignments remain
unchanged on the source relationship. You can edit, cancel, or delete them as needed.

2. The task doesn't change eligibility profiles. If the eligibility profiles used for performance goals
and documents include inactive assignments, after the transfer, the inactive assignments
continue to be eligible for the same performance goals and documents.

You must update the eligibility profiles to exclude the inactive assignments to prevent them being
recreated.

Payroll Details

You can copy payroll details from the source to the target assignment and payroll relationship during a
mass legal employer change within the LDG.

For further info, see Payroll Data Transferred below.

240

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Data Item

Benefits

What This Includes

You can choose the life event for global transfer and transfer benefits balance to the worker's new
assignment.

Select People

You can choose the workers for whom you would like to perform the transaction.

Review Selected People

You can review the people you selected before submitting the Mass Legal Employer process.

Payroll Data Transferred
For Payroll implementation , the process copies the data from the original assignments and work relationships to the
new one, depending on your selections.

Note:  You can use the Change Legal Employer Dashboard to view the results of transfer. It lists a consolidated
summary related to the global transfer for each employee. For further info, see "Dashboard for Legal Employer
Change" in the Help Center.

Here's the payroll items the process can copy. For details on all data the process copies, see "Data Copy and Display
Options for Global Transfers for the US" in the Help Center.

Payroll Item

What This Includes

Payroll Relationship and Assignment
attributes (Payroll Details)

Personal Payment Methods

Payroll, Tax Reporting Unit, Overtime Period, and Time Card Required.

Payment methods are copied subject to the availability of a valid organization payment method (OPM)
for the same payment type.

Third-Party Payment Methods

The flow links payment methods for third-party person payees to the new payroll relationship.

For further info, see "What Happens to Payment Methods During Person Transfers" in the Help Center.

Person Costing Overrides

By default, the flow doesn't copy costing overrides . If you choose to copy, then the flow copies data
across four levels at which the person costing setup is held.

For further info, see "What Happens to Costing Overrides During Person Transfers" in the Help Center.

Recurring Element Entries

The flow copies element entries subject to eligibility. To exclude certain elements from being copied,
 define an element (object) group with the Global Transfer usage type.

For further info, see "What Happens to Element Entries During Person Transfers" in the Help Center.

Calculation Cards and Components

The flow copies the cards and components at the payroll relationship level based on each country's
legislation.

For further info, see "What Happens to Calculation Cards During Person Transfers" in the Help Center.

Balances

The flow copies the source assignment and relationship-level balances to the target assignment and
payroll relationship respectively.

241

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Payroll Item

What This Includes

Note:  The Mass Legal Employer Change flow interprets a blank entry to imply the value on the
source assignment and payroll relationship. Unless you override this value, the application copies
the source value to the target assignment and payroll relationship.

For further info, see "What Happens to Balances During Person Transfers" in the Help Center.

Dashboard for Legal Employer Change

HR specialists and line managers can view global transfer details for workers using the Change Legal Employer
Dashboard quick action on the My Client Groups and My Team tabs respectively.

The details include information related to functional areas, such as Employment, Payroll, and Performance Documents
and Goals.

The Change Legal Employer Dashboard page lists a consolidated summary related to the global transfer for each
worker. When you select a worker to view their transfer details, you can see status messages and links to the functional
areas.

Points to Consider

• Only global transfers initiated using the Local and Global Transfer flow are displayed on this dashboard.

• The dashboard doesn’t display data for global transfers done using these methods:

◦ Classic pages
◦ HCM Data Loader
◦ REST service

• The dashboard doesn’t display data for global transfers which are still pending approval. Only approved global

transfer details are displayed on the dashboard.

• Users can view the workers on the dashboard based on their assigned data security.

Process to Link Source and Destination Assignments for Global
Transfer

Use the Migrate Employment Data process to link the source and destination assignments during a global transfer.
By linking the assignments, you can view the complete assignment history of the source and destination work
relationships.

Here's what the process does:

• Selects all active workers (employee, contingent worker, and nonworker) who don't have their termination dates

populated in the work relationship and for whom the source assignment ID isn't populated.

242

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

•

Identifies the source and destination assignment IDs for the selected workers based on these items:

◦ Action occurrence ID.
◦ Comparison of the assignment start date of the destination assignment and assignment end date of the

source assignment.

Once identified, the process stores the assignment ID of the primary assignment as the source assignment in
the destination assignment.

Note:

• The Migrate Employment Data process will populate the SOURCE_ASSIGNMENT_ID field in the

PER_ALL_ASSIGNMENTS_M table only for global transfer.

• During a global temporary assignment, the assignment ID isn't stored as the source assignment ID.

Points to Consider

• You can run this process to only link your existing global transfer transactions. Change legal employer

transactions initiated from the UI after release 20B will be linked by the application.

• You can rerun the process, but the process will only select data where the source assignment ID isn't populated

for a global transfer action.

• When you run the process, it includes all active workers and processes their historical records including those

from their earlier work relationship. For example, the process will also include the historical records of a
currently active rehired worker.

Process Parameter
The Migrate Employment Data process uses the Link Global Transfer assignments parameter. This parameter links the
source and destination assignments related to global transfer by updating the PER_ALL_ASSIGNMENTS_M table.

View History of Assignment Updates
After you have linked the source and destination assignments, you need to set the
ORA_PER_EMPL_DISPLAY_GT_HISTORY profile option to view a continuous history of assignment updates across legal
employer changes. For more information about this profile option, see the Employment Profile Options topic in the
Related Topics section.

Related Topics

• What are scheduled processes?

• Submit Scheduled Processes and Process Sets

• Employment Profile Options

243

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Transferring People

Example of a Worker Transfer
You're a human resources (HR) specialist transferring Ralph Amber, working as a sales representative in the Sales West
US department. You're transferring him within the same legal employer to the Sales East US department in New York.

Let's look at the steps to update the key values for this transfer. For other fields, you can use the default values.

Selecting Ralph and the Transfer Action

1. On your home page, click the My Client Groups tab, and then select the Transfer quick action in the

Employment area.

2. Search for Ralph Amber and select his record.
3.

In the When and Why section, enter these values.

Field

Value

When does the transfer start?

Select the date the transfer takes effect.

What's the way to transfer?

Transfer

Why are you transferring Ralph Amber?

Reorganization

4. Click Continue to proceed.

Enter Transfer Information

1.

In the Transfer section, enter these values.

Field

Value

Department

Sales East US

Location

New York

2. Click Submit to complete the transaction.

244

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

FAQs for Transfers

Can I transfer people if I don't have access to all of their assignments?
No. You can transfer people only if you have access to all of their assignments.

Does a person automatically move to another payroll during a global transfer?
If the global transfer happens within the same legislative data group, then the payroll attributes are defaulted or copied
depending on the transaction done by the user.

If you use the Local and Global Transfer flow, the payroll attributes are defaulted from the source assignment. If you
use the Mass Legal Employer Change flow, the payroll attributes are copied from the source assignment to the new
assignment, provided the user hasn't entered any override values.

If the global transfer doesn't happen within the same legislative data group, then the payroll attributes are not defaulted
or copied.

Can I use the Global Transfer action for a person with a future termination date?
Yes, the global transfer ignores the future termination date and ends the existing work relationship a day before the
start date of the new work relationship.

Can I do a global transfer for a suspended assignment?
Yes, as long as the assignment isn't suspended because of a global temporary assignment.

Can I use the Global Transfer action for a person having a future global transfer or
global temporary assignment?
No, you can't globally transfer such a person.

Can I do a global transfer for an assignment from where the global temporary
assignment was initiated or which was created as part of the global temporary
assignment?
No, you need to end the global temporary assignment first before you do the global transfer.

Can I terminate a work relationship with an active global temporary assignment?
No, you must first end the global temporary assignment before you terminate the work relationship.

How can I correct the global transfer and global temporary assignment start dates?
You can't change these dates directly on the assignment or Work Relationship page. You must first cancel the work
relationship that was created as part of the global transfer or global temporary assignment.

245

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

This removes the global transfer and global temporary assignment records from the original assignment. You can then
do the global transfer or create a global temporary assignment on the date you want.

Employment Contracts

Overview of Contracts

The worker's assignment can include contract information which is required by some legal employers. The contract
details are for information only; they have no effect on processing.

Legal employers can use contracts only if it's enabled at the legal employer level and use any of these employment
models:

• 2 Tier Multiple Contract - Single Assignment

• 2 Tier Single Contract - Single Assignment

You can associate a contract with an assignment by creating a new contract or selecting from existing contracts. You can
use the same contract across assignments only within the same work relationship.

If you create a new assignment for a worker in a legal employer that supports contracts and don't enter contract details,
a default contract record is still created in the application.

You can extend the contract period and manage other contract details using the Employment Contracts task. HR
Specialists can access this task from the My Client Groups tab under Quick Actions. Line managers can access the task
from the My Team tab under Quick Actions. Employees can view their contract information on their Employment Info
page.

You can configure approvals for the Manage Contracts business process by using the Manage Contracts approval rule.
You can select the type of contract whether its fixed-term, full-time, or seasonal. The values for the contract type field
are populated by the user lookup CONTRACT_TYPE.

You can migrate contract data from the assignment to the contract by running the Migrate Employment Data scheduled
process. You must run this process only once before you manage contracts using the Employment Contracts task.

How You Manage Contracts

You can associate a contract with an assignment and specify key information such as contract type, duration, and start
and end dates.

You can extend a contract and manage other details, such as adding, deleting, or editing contract extensions using the
Employment Contracts task under Quick Actions.

Note:  When you extend a contract, the Employment Contracts task updates the contract end date in the
PER_CONTRACTS_F table. The task doesn't update the projected assignment end date in the work terms record.

246

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Associate a Contract With an Assignment
You can associate a new contract with an assignment when doing any of these actions:

• Hire a person

• Change the legal employer

• Transfer a person globally

• Create a global temporary assignment

• Create a work relationship

Note:  You can create a contract only when you do any of these actions. There's no separate task available for creating
a contract.

You can associate a new contract or an existing contract with an assignment under the same work relationship when
doing any of these actions:

• Add an assignment to a work relationship

• Add a temporary assignment

Extend a Contract
You can extend a contract from the Employment Contracts page by specifying the contract end date or the contract
duration. However, you can't extend a contract which doesn't have a contract end date.

•

•

If you enter the contract end date, the application automatically calculates the duration.

If you enter the contract duration, the application automatically calculates the contract end date. This is done by
adding the duration to the previous contract end date.

Correct Contract Extension History
You can view the history of extensions made to a contract in the contract details. This table shows the fields in the
contract extension history.

Contract
Number

Extension
Number

Initial Contract
Start Date

Contract Start
Date

Contract End
Date

Contract
Duration

Contract Type

Description

CONT100010

0

01-Jan-2018

01-Jan-2018

31-Mar-2018

3 months

Fixed

Initial contract
record

CONT100010

CONT100010

1

2

01-Jan-2018

01-Apr-2018

31-May-2018

2 months

Fixed

First extension

01-Jan-2018

01-Jun-2018

31-Jul-2018

2 months

Fixed

Second
extension

The contract start date isn't a stored value. The application calculates the contract start date by adding one day to the
contract end date of the previous extension. For the initial contract record, the contract start date is the same as the
initial contract start date.

247

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

You can correct records in the contract extension history, but with a few conditions.

You can only correct the contract end date and contract duration fields for the latest contract record (second extension
record in the table). This is because any changes that you make to these fields in the initial records aren't propagated
to the subsequent future records. This condition ensures that there are no gaps in the contract duration. For example,
in the table if you reduce the contract duration to 1 month for the first extension, the contract end date becomes 30-
Apr-2018. However, the contract end date for the second extension doesn't automatically change to 30-Jun-2018. You
can't delete the initial contract record.

Update a Contract
You can update a contract from the Employment Contracts page by adding an effective dated update to the existing
contract record. To add a new effective dated record, you need to first edit the record above which you want to add
the new effective dated record. When you edit the record, you need to enter the date when you want to insert the new
effective dated record. If you leave the date unchanged, the application will consider it as a correction. You can also
update the contract duration while updating a contract, when you add an effective dated record which is the latest
record for a contract. However, you can't change the duration of contract while adding an effective dated record, if a
future record exists.

Note:  Except for the contract duration and contract end date, you can update all the other fields even if the newly
added record is the latest effective dated record or not.

Updating of the contract can also be used for tracking contract deduction.

For example, an employee is hired for a 1.5 year contract on 01-Jan-2018 and 5 months later on 01-Jun-2018, his
contract needs to be reduced to 1 year. You can create an effective dated update on Employment Contracts page to track
this transaction.

Contract
Number

Extension
Number

Effective Start
Date

Effective End
Date

Contract Start
Date

Contract End
Date

Contract
Duration

Description

CONT100010

CONT100010

0

0

01-Jan-2018

31-May-2018

01-Jan-2018

30-Jun-2019

1.5 years

01-Jun-2018

31-Dec-4712

01-Jan-2018

31-Dec-2018

1 year

Initial contract
record

Effective dated
update

Note:  Date effective contract changes aren't supported when you are updating contracts using REST API.

How You Update or Extend a Contract with Assignment Updates in
Redwood

You can either correct a contract, extend it, or add a date-effective update when updating a worker assignment if you
have the Manage Worker Contract aggregate security privilege.

However, you can extend a contract only when the date selected in the When and Why step is contract end date + 1 day.

248

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Only those contract records that share the same effective date with the assignment updates are available for correction
on the Correct Employment Details page. Contract records that don’t share any effective dated rows with the
assignment can be managed from the standalone Redwood Employment Contracts page. If a contract is pending
approval, then you won't be able to update the contract. Including the contract info in approval notifications will be
added in a future release.

Process to Migrate Contract Data

You must use the Migrate Employment Data process to migrate contract data from the assignment to the contract. You
must run this process once before you manage contracts using the Employment Contracts task under Quick Actions.

Note:

• You must run this process to enable assignment-level security for the employment contract. For more

information about assignment-level security in HCM Common, refer to the HCM 20D Release Readiness What's
New: Secure Access for Workers with Multiple Assignments

•

If you run the process more than once, only records having the period of service ID as null in the
PER_CONTRACTS_F table are processed.

Here's what the process actually does:

• Updates the period of service ID for workers having contracts and for whom the ID isn't populated in the

PER_CONTRACTS_F table.

• Copies the contract end date from the projected assignment end date in the work terms record to the

PER_CONTRACTS_F table.

• Updates the contract ID for workers having contracts and for whom the ID isn't populated in the

PER_ALL_ASSIGNMENTS_M table.

• Copies the assignment action to the PER_CONTRACTS_F table if the action code is null in the
PER_CONTRACTS_F table and there's a corresponding assignment split on the same date.

• Updates the action as contract extension if the action code is null in the PER_CONTRACTS_F table and there's a

contract extension record with no corresponding assignment split on the same date.

After the process is run, you can check the contract end date in the worker's employment information. The contract end
date will be populated for all the rows for which the projected end date is populated in the work terms record.

The process won't create any default contract records for existing assignments even though the assignments are part of
a legal employer that supports contracts.

The update of historical records for the action will happen only once. Therefore, even if you run the process again, the
contract updates you did after running the process for the first time in release 21A won't be synchronized back in the
responsive user interface.

Process Parameter
The Migrate Employment Data process uses the Enhance contract data to enable it's use in the responsive UI
parameter. This parameter enhances the contract data by updating the UPDATE_PER_CONTRACTS_F table.

249

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Related Topics

• What are scheduled processes?

• Submit Scheduled Processes and Process Sets

FAQs for Employment Contracts

How are contract numbers generated?
Contract numbers are automatically generated by prefixing the person number with 'CONT'. For example, if the person
number is 17040, the contract number would be CONT17040. Subsequent contracts of the assignment would have
suffix numbers, for example CONT17040-2, CONT17040-3.

You can override these generated numbers and assign contract numbers manually.

Note:  If you don't enter the contract number manually in add person flows (Hire an Employee, Add a Contingent
Worker, Add a Pending Worker, or Add a Nonworker), then the contract number is generated at the time of submit.
Therefore, you can't view the auto generated contract number while performing the transaction. This behavior occurs
irrespective of the person number generation method.

Can I add contracts information for contingent workers and pending workers?
Yes, if the employment model that you configured supports contracts.

Related Topics

• Employment Model

• When to Select the Employment Model

How can I convert a fixed-employment contract to an open-ended one?
You must set a blank value for the contract end date and the contract duration for the most recent contract extension
record. If there is no contract extension, you can make these changes in the initial contract record.

What does the table in the Contract Extensions region show?
The table shows the initial contract and the contract extension records that are used to change the contract duration.

250

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Add and Reassign Direct Reports

How You Reassign Direct Reports

You add or reassign a manager's direct line reports and other report types such as project reports, resource reports,
or mentees when you do the change location, change manager, create work relationship, hire, promote, transfer, or
termination actions.

You reassign direct reports using the Direct Reports task in the My Team work area.

You can add all or reassign selected reports. When you reassign reports, there are changes at the assignment level for
each report.

For example, this is how you can reassign John Smith's reports and mentees on his transfer:

• Three of his reports to the same new line manager

• Fourth report to a different line manager

• Two of his mentees to a different mentor

Some of John's existing reports may continue to report to him in his new department.

You can reassign reports as of the same effective date or different effective dates. For example, John Smith's date
of transfer is 1st October, 2018 and you want to reassign his direct reports on 15th September, 2018. You reassign his
existing direct reports with an effective date of 15th September, 2018. The new direct reports you add are approved
when the parent transaction is approved.

Note:  Pending workers aren’t displayed in the Reassign Directs section in all responsive employment flows.

How You Select the Manager
You can select the same new manager for all the reports or a different new manager for each report. If most directs
are being reassigned to the same new manager, you can select this person as the new manager by default for all the
reports, and later reassign selected directs to different managers.

But remember, when you reassign reports you can't change the manager type. For example, if the direct is a line report
for the current manager, you can reassign the direct only as a line report to a new manager, but not as a direct of other
type, such as a project report or mentee.

When you change the position in an existing line manager assignment, you must ensure that the direct reports
assigned to the new position aren't reporting to the line manager already. If there's a conflict, check and remove the
same directs listed in Add Direct Reports from Reassign Line Manager as well.

Areas of Responsibility
Areas of responsibility associated with the manager's role aren't affected by the Direct Reports task. For example, if a
line manager also has an area of responsibility as an HR representative, the HR reports can't be managed from this task.

251

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Note:  You can't use the Direct Reports task to assign new roles to managers during the reassign process. Instead, use
the Manage Role Provisioning Rules or Manage HCM Role Provisioning Rules task in the Setup and Maintenance work
area to manage the assignment of roles. You must assign manager roles for people who didn't have reports before the
reassign process.

Related Topics

• What's the difference between the Change Manager and Direct Reports functionality?

• Can I reassign indirect reports of the manager from the same Direct Reports task?

• How You Assign Areas of Responsibility

• How You Reassign Pending Approvals and Invalid Supervisor Assignments

• How many direct reports can I reassign at a time using the responsive or Redwood pages?

How You Reassign Direct Reports for Terminations and
Resignations

If a line manager resigns or is terminated then depending on the configuration, you can reassign their direct line report
types to new managers before you approve the resignation request or terminate the work relationship.

When you reassign direct reports, the reassignment is effective after the termination date plus one day with changes at
the assignment level for each report.

Whether it's termination, correction of termination, or resignation you can reassign only direct line reports in these
transactions. Here's what happens if the manager has line reports:

• The Reassign Existing Reports area displays, otherwise it doesn't.

• The direct line reports are displayed as of the termination date and not the current date.

If the manager has multiple assignments, each assignment is listed separately with the direct line reports to be
reassigned.

If the manager has other types of reports such as project reports, resource reports, or mentees, you must reassign those
reports before the termination effective date using the Direct Reports task.

Related Topics

• How You Reassign Pending Approvals and Invalid Supervisor Assignments

• Employment Configuration Options

• How many direct reports can I reassign at a time using the responsive or Redwood pages?

252

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

How You Reassign or Add Direct Reports During Local and Global
Transfer

When you transfer managers, they automatically keep their direct reports, even when moving to a new legal employer.
But you can change that. As part of the transfer, you can reassign direct reports to other managers. You can also add
new reports.

Here's where you make these changes:

• You can add new direct reports in the Add Direct Reports section.

• You can reassign direct reports in the Reassign Direct Reports section. This section displays only if the manager

has direct reports assigned. By default, all manager relationships be it line manager or project manager
are available for the direct report. You can reassign or retain existing direct reports. If you retain the direct
reports during global transfer, their assignments are updated with the newly created assignment record of the
manager. When you add or reassign direct reports, changes occur at the assignment level for each report. You
can select the same new manager for all direct reports or a different new manager for each report.

• However, in case of a global temporary assignment, you can move the manager's direct reports
to the destination assignment or retain them in the source assignment. You can configure the
ORA_PER_EMPL_GTA_POP_DIRECTS profile option code to do either of these actions in the Local and Global
Transfer flow:

◦ Default the manager's existing direct reports in the Reassign Direct Reports section when you perform a

global temporary assignment.

◦ Default the manager's existing direct reports in the Add Direct Reports section when you perform a

global temporary assignment. You can then remove the direct reports from the section that you don't
want to move to the destination assignment.

For more information about the profile option, see the Employment Profile Options topic in Chapter 11,
Employment in the Implementing Global Human Resources guide.

Related Topics

• Examples of Direct Reports Reassignment During Global Transfer

• How many direct reports can I reassign at a time using the responsive or Redwood pages?

How You Add Direct Reports During Add Assignment

You can add direct reports of a manager's assignment in the Add Assignment flow.

Here's where you make these changes:

• You can add new direct reports in the Add Direct Reports section.

• The direct reports which were assigned to the source assignment are also copied by default in the Add Direct

Reports section. Only the line manager relationships are copied in the Add Direct Reports section. If you retain
the direct reports, their assignments are updated with the newly created assignment record of the manager. If

253

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

you don't want to move the direct reports to the newly created assignment, then you can remove the directs
from the Add Direct Reports section before submitting the transaction.

Examples of Direct Reports Reassignment During Global Transfer

Let's look at some examples of how you can reassign direct reports during global transfer.

Reassign Direct Reports to the Transferring Manager
When you reassign direct reports to the transferring manager, you must deselect all reports who continue to report to
the same manager in the new assignment. Use the Reassign Existing Reports section on the Local and Global Transfer
page to reassign the direct reports.

Reassign Direct Reports to the Transferring Manager's Manager
You can reassign direct reports to the transferring manager's manager using either of these methods:

• Automatically reassign the direct line reports using the Reassign Pending Approvals for Terminations and

Correct Invalid Supervisor Assignments scheduled process. All direct reports are reassigned to the transferring
manager's manager as of the date following the transfer.

• Manually reassign the line reports to the transferring manager's manager during the global transfer

transaction.

Reassign Direct Reports to the Transferring Manager, Other Managers, and
Manager's Manager on Different Dates
Here's how you can reassign directs in the primary assignment:

• Reassign any direct reports before transferring the worker using the Direct Reports page

• Deselect any direct reports continuing to report to the transferring manager

• Reassign the remaining direct reports to the same or different new managers

• Reassign any direct reports on specific dates using the Change Manager page

And here's how you can reassign direct reports in the secondary assignment:

• Reassign any direct reports to new managers using the Direct Reports page

• Schedule the Reassign Pending Approvals for Terminations and Correct Invalid Supervisor Assignments

process to automatically reassign any remaining direct reports to the manager's manager. The direct reports
are reassigned as of the date following the transfer.

• Reassign any direct reports on specific dates using the Change Manager page.

Related Topics

• How You Reassign Pending Approvals and Invalid Supervisor Assignments

• How many direct reports can I reassign at a time using the responsive or Redwood pages?

254

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

How You Reassign Pending Approvals and Invalid Supervisor
Assignments

A manager assignment can become inactive due to the end of an assignment or work term, termination, or global
transfer. So you need to reassign direct reports and correct any invalid supervisory assignments that result due to an
inactive assignment.

If the manager has any pending approval notifications, you must reassign those too.

You can run the Reassign Pending Approvals for Terminations and Correct Invalid Supervisor Assignments process
in the Scheduled Processes work area to reassign the direct reports and pending approval notifications of a manager
who's either terminated or globally transferred. You can skip the step of reassigning pending notifications if you want to.
Here's what the process does:

•

•

It reassigns the direct reports of a terminated manager to that person's line manager and also assigns any
pending notifications to the line manager.

It reassigns pending approval notifications based on the number of days you specify. For example, if you
specify 30 days, the process reassigns pending approvals of workers or managers terminated in the past 30
days.

FAQs for Add and Reassign Direct Reports

What's the difference between the Change Manager and Direct Reports functionality?

You use the Change Manager flow to change the manager for a worker and the Direct Reports flow to reassign existing
reports or add direct reports for a manager.

For example, Rahul is the line manager for Jennifer and Vijay, and project manager for Stacey. At the same time, Terry is
the project manager for Vijay. You use the Change Manager flow if you want to change Vijay's line manager and project
manager, based on requirements. This flow will be launched for Vijay (employee) and the change in supervisors will
result in a change in Vijay's assignment data.

On the other hand, if you want to reassign Rahul's direct reports (Jennifer, Vijay, and Stacey) to another manager, you
would use the Direct Reports flow. This flow will be launched for Rahul (supervisor) and the changes in supervisors (line
manager or project manager) will result in change of assignment data for his directs (Jennifer, Vijay, and Stacey).

Can I reassign indirect reports of the manager from the same Direct Reports task?
No, you can't. You can reassign only direct reports of the manager.

255

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Why can't I see the direct reports action and action reason fields in the When and
Why section of the Resignation flow even though they're enabled in the Transaction
Design Studio?
You can't see the action and action reason fields for the direct reports in the Resignation page because the person
resigning can't reassign their own direct reports. The fields are visible to the approver of the resignation when the
resignation transaction goes for approval.

Terminate Work Relationships

Resignations

Employees can use either the Resignation (version 2) or Resign from Employment (version 3) quick action on the Me tab
to submit their resignation from an assignment.

Alternatively, employees can use the Employment Info quick action on the Me tab to submit their resignation (Actions
> Resignation or Resign from Employment). Human resources (HR) specialists can submit employee resignations either
by using the Termination or Terminate Employment quick action on the My Client Groups tab. Line managers can
submit their directs' resignation using either the Termination or Terminate Employment quick action on the My Team
tab.

This table shows the application behavior when an employee uses the Resignation and Resign from Employment quick
actions:

Condition

Version 2 Resignation

Version 3 Resignation

The employee hasn't submitted their
resignation and neither has the HR specialist or
line manager submitted their resignation.

The Submit Resignation page is displayed.

The Resign from Employment page is
displayed.

The employee has submitted their resignation
dated in the future.

The View Resignation page is displayed and the
employee can withdraw their resignation.

The View Resignation page is displayed and the
employee can withdraw their resignation.

The HR specialist or line manager has
submitted the employee's resignation on a
future date.

The View Resignation page is displayed and the
employee can withdraw their resignation.

The View Resignation page is displayed and the
employee can withdraw their resignation.

This table shows the application behavior when a HR specialist or line manager uses the Termination and Terminate
Employment quick actions:

Condition

Version 2 Termination

Version 3 Termination

The HR specialist or line manager hasn't
submitted the employee's resignation.

The Submit Termination page is displayed.

The Terminate Employment page is displayed.

256

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Condition

Version 2 Termination

Version 3 Termination

The HR specialist or line manager has
submitted the employee's resignation on a
future date.

The View Termination page is displayed and
you can correct or reverse the termination
based on your user privilege.

The View Termination page is displayed and
you can correct or reverse the termination
based on your user privilege.

The HR specialist or line manager has
submitted the employee's resignation on a past
date.

The manager can't search for the employee in
the application because they can access the
employee's record only up to the resignation
date. However, the HR specialist can view the
termination and correct or reverse it.

The manager can’t search for the employee in
the application because they can access the
employee's record only up to the resignation
date. However, the HR specialist can view the
termination and correct or reverse it.

For more information about version 3 resignation, see the following document on My Oracle Support (https://
support.oracle.com): Version 3 Termination and Resignation (Doc ID 2821906.1)

Resignation Dates
An employee needs to first notify the company when they decide to resign and also specify their actual resignation
date.

• Resignation notification date is the date the initiator notifies the other party of the resignation. This date

defaults to the current date. For example, a worker notifies an employer of their resignation.

• Resignation date is the worker's last working date with the employer. This date defaults to the notification

date plus the notice period specified in the assignment. Employee can override this default when entering the
resignation.

Withdrawing a Resignation
When you withdraw a resignation, the assignments ended because of the resignation are restored with the status prior
to the resignation.

An employee can use either the Resignation or Resign from Employment quick action on the Me tab and click Withdraw
on the View Resignation page to withdraw their resignation. HR specialists and line managers can use either the
Termination or Terminate Employment quick action on the My Client Groups and My Team tabs respectively to reverse
a resignation. HR Specialists can search for the resigned worker and click Reverse on the View Termination page. Line
managers can reverse the termination, provided it's in the future and they have the privilege to do so.

Related Topics

• Process to Migrate to Version 3 Termination or Redwood Experience

Terminations

When you terminate a person's work relationship, you end all of the person's assignments in the work relationship.

Human resources (HR) specialists can terminate people by using the existing Termination quick action (version 2) or the
new Terminate Employment quick action (version 3) on the My Client Groups tab. Line managers can terminate their
workers by selecting either the Termination or Terminate Employment quick action on the My Team tab.

This table shows the application behavior when you use the Termination or Terminate Employment quick action:

257

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Condition

Version 2 Termination

Version 3 Termination

The person's assignment isn't terminated.

The Submit Termination page is displayed.

The Terminate Employment page is displayed.

The assignment is terminated in the future.

The View Termination page is displayed and
you can correct or reverse the termination
based on your user privilege.

The View Termination page is displayed and
you can correct or reverse the termination
based on your user privilege.

The person's assignment is terminated in the
past.

The manager can't search for the person in
the application because they can access the
person's record only up to the termination
date. However, the HR specialist can view the
termination and correct or reverse it.

The manager can’t search for the person in
the application because they can access the
person's record only up to the termination
date. However, the HR specialist can view the
termination and correct or reverse it.

Here's what happens when you terminate a work relationship:

• The work relationship and its associated assignments become inactive the next day after the termination.

• User access and roles are revoked after the termination date. You can revoke the person's access

immediately after termination or the next day after the termination date, by passing a suitable value to the
ReviewUserAccess attribute for termination through HDL or HSDL. If no value is passed to the attribute, then
the user account becomes inactive after termination.

• The enterprise and legal employer service periods end on the termination date. The person becomes an ex-

worker for the legal employer.

•

If you use Oracle Payroll, the payroll administrator gets a notification about the termination, which is the
administrator's cue to terminate the person's payroll

Note:  If the person has many work relationships and you want to terminate all of them, you must terminate the
primary one last.

For more information about version 3 termination, see the following document on My Oracle Support (https://
support.oracle.com): Version 3 Termination and Resignation (Doc ID 2821906.1)

Termination Dates

• Termination notification date is the date the initiator notifies the other party of the termination. For example, a

worker notifies an employer of his resignation or an employer notifies a worker of a layoff.

• Termination date is the worker's last date of employment, unless you have enabled the last working date which
is different than the termination date. This defaults to the notification date plus the notice period specified in
the assignment. You can override this default when entering the termination.

Ending a Single Assignment

Version 2 Termination

Version 3 Termination

If the work relationship has many
assignments and you want to end one of
them, you end the specific assignment and
don't terminate the work relationship.

If the work relationship has many assignments and you want to terminate one of them, you only
terminate the specific assignment and not the entire work relationship.

258

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Version 2 Termination

Version 3 Termination

If the work relationship has a single
assignment and you want to end it, you
terminate the work relationship itself.

If the work relationship has a single assignment and you want to terminate it, you terminate the work
relationship itself.

Ending a Temporary Assignment
You can end a temporary assignment by using the Terminate Employment quick action in Version 3 Termination. The
original assignment is activated when you terminate the temporary assignment.

Note:  Correct termination and reverse termination actions are not supported for temporary assignments.Here are
some points to consider when you end a temporary assignment in Version 3 Termination:

•

•

•

You can correct the End Temporary Assignment action by selecting the record from the Employment Info
page. However, you can't correct the termination date of the temporary assignment.

You can reverse the End Temporary Assignment action by selecting the record from the Employment Info
page and deleting the record.

The correction or deletion of the record from the Employment Info page only impacts the selected
assignment. If you need to make changes for more than one assignment, you must perform the action for
each assignment.

Change Assignment Versus Terminate Employment
This table describes when you can use the Change Assignment > End Assignment and Terminate Employment quick
actions:

Change Assignment > End Assignment

Terminate Employment

• Update assignment fields except
assignment termination fields

• Update assignment flexfields

• End permanent or temporary

assignments

• Enter these assignment termination fields:
◦ Notification Date
◦ Termination Date
◦ Last Work Day (hidden out-of-the-box for resignation and displayed for termination)
◦ Recommended for Rehire
◦ Review User Access
• Update assignment flexfields

• End temporary assignments

Correcting a Termination
You can correct the earlier termination data for a worker by editing their data.

HR specialists and line managers can use the Termination quick action (version 2) or the Terminate Employment quick
action (version 3) on the My Client Groups and My Team tabs respectively to correct a termination. You can search for
the terminated worker and on the View Termination page, click Edit for the sections where you want to correct the

259

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

termination data. Then you can submit your changes on the Correct Termination page. Line managers can correct the
termination, provided it's in the future and they have the privilege to do so.

Note:  You can't view or correct earlier termination comments and information related to reassigning of existing
reports. If you need to correct information related to reassigning of existing reports, use the Manage Direct Reports
process.

If you change the termination date for a second time on the Correct Termination page, a warning message is displayed
that your changes will be lost. If you click Continue on the message, your data changes in all sections after the first date
change will be reverted except for the second changed date. The data reverted changes will be retained except for the
second changed date even if you click Cancel on the page.

If you prepone the assignment termination date on the Correct Termination page, these things happen:

• All changes in the Termination Info section are lost and the termination fields are populated with default values.

The value in the Last Working Day field is reset to the termination date only if the existing value is invalid
according to the new termination date.

•

If there are future dated changes for the assignment, the changes are deleted when you click Submit.

What Happens to Payroll in a Termination
When you terminate employees with eligible earnings, such as bonuses or vacation payouts after their termination date,
you must associate them with a nonrecurring element.

Related Topics

• What Happens to Direct Reports in a Termination

• Process to Migrate to Version 3 Termination or Redwood Experience

• Employment Model

• Example of a Worker Termination

Termination and Resignation Version 2 versus Version 3

This table shows a comparison between the existing version 2 termination and resignation UI and the new version 3
termination and resignation UI:

Version 2

Version 3

• You can use either person-level

• You can use either person-level security or assignment-level security.

•

If you use assignment-level security, you can't terminate the work relationship unless you have
access to all assignments in the work relationship.

security or assignment-level security.

•

If you enable assignment-level
security, the user can't search
for assignments that they don't
have access to. However, if the
worker has access to one of the
assignments in the work relationship,
they will be able to terminate the
work relationship. During work
relationship termination, you
terminate assignments in the work

260

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Version 2

Version 3

relationship even though you don't
have access to those assignments.

• You can only terminate or resign from

• You can terminate or resign from the work relationship or a single assignment.

the work relationship.

• Workers can’t resign on their own
if they have more than one work
relationship and they need to contact
the HR specialist.

• Workers can choose the assignment or work relationship they want to resign from.

• Only work relationship flexfields are

• Work relationship (DDF and DFF) and assignment (DDF, DFF, and EFF) flexfields are available.

available (DDF and DFF).

• You can perform assignment-level
termination (End Assignment)
using the Change Assignment >
End Assignment action. However,
managers usually won't have access
to the Change Assignment action.
In this case, managers will need to
contact the HR specialist to perform
assignment-level termination for
their reports.

• Managers can perform assignment-level termination using the termination UI.

• Managers or HR specialists can continue to terminate an assignment using the Change

Assignment page (End Assignment action).

• You can view termination details

• You can view termination details at assignment level or work relationship level depending on the

termination level you select.

• The termination fields (Review User Access, Recommended for Rehire field group, and Last

Working Day) are now also displayed at the assignment level.

• Workers can resign if they have more than one work relationship.

• Workers can resign from the whole work relationship or from a single assignment.

at the work relationship level. The
termination fields include Review
User Access, Recommended for
Rehire field group, and Last Working
Day.

• Workers can’t resign if they have
more than one work relationship.

• Workers who have multiple

assignments in a work relationship
can’t resign from a single
assignment. They have no choice
but to resign from the whole work
relationship.

• Termination is a privileged

• Termination is not a privileged transaction.

transaction.

• Termination will take precedence
over any pending transaction for
the same assignment and the other
transaction will be rejected.

• Termination will display along with any pending transaction for the same assignment.

Note:  If you're implementing Fusion Terminations or Resignations functionality for the first time, implement V3
Terminations to simplify the uptake of Redwood Terminations in the future. Otherwise, you'll need to configure the
Approvals twice.

For more information about version 3 termination and the steps to enable for it, see this document on My Oracle
Support (https://support.oracle.com): Version 3 Resignation and Termination (Doc ID 2821906.1)

261

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Related Topics

• Process to Migrate to Version 3 Termination or Redwood Experience

Terminating or Resigning from Assignments and Work
Relationships in Version 3

Let's say you're a human resources (HR) specialist terminating one of the work relationships or assignments of Zak
Tyler, who’s an employee. Or maybe Zak wants to resign due to personal reasons.

Let's look at the steps to update the key values for terminating or resigning from a work relationship or assignment. For
other fields, you can use the default values.

Watch video

Terminate a Work Relationship or Assignment
Let’s look at how you terminate a work relationship or assignment in V3, as a human resources (HR) specialist. In this
example, you will terminate a work relationship or assignment of an employee, Zak Tyler.

1. On your Home page, click the Terminate Employment quick action on the My Team tab.

In v3, managers can only view and terminate the work relationships and assignments they have access to.

2. Search for and select Zak Tyler.
3. Click Termination Info.
4. Click Continue.
5.

In the What are you terminating? section, click Director H.

Note:  By default, the entire work relationship is selected. Once you select what you’re terminating and
continue to the next section, you can’t change the selection.

If the termination type is voluntary, the employee will be able to see the details. Managers will only see the
employee’s assignments that they have access to. Managers will see the Work Relationship termination option
only if they have termination access to all the assignments belonging to that work relationship.

6. Click Continue.

If needed, you can also see more details for the selected assignment.
Whether you’re terminating an assignment or a work relationship, the termination info and any additional
assignment, legislative, or data fields defined by the company are the same.

7. Once you enter all the information, click Submit.

Resign from a Work Relationship or Assignment
In V3, if you have multiple assignments and multiple work relationships, you can opt to resign from an entire work
relationship or only from a single assignment in a work relationship.

Let’s look at how you resign from a work relationship or assignment in V3.

1. On your Home page, click the Resign from Employment quick action on the Me tab.
2. Click to expand the Director H section.

262

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Here, you can see all your work relationships, assignments, and the assignment details. You can select the
specific assignment you want to resign from.

3. Click the Director H link.
4. Click Continue.
5. Add any comments or attachments, if needed.
6.

In the What are you resigning from? section, click Director H.

Note:  The entire work relationship is selected by default. Once you select what you’re resigning from and
continue to the next section, you can’t change the selection.

7. Verify whether you’ve selected the correct assignment or work relationship.

You can also view more details for the selected assignment if needed.

8. Once you enter all the information, click Submit.

Note:  If you're implementing Fusion Terminations or Resignations functionality for the first time, implement V3
Terminations to simplify the uptake of Redwood Terminations in the future. Otherwise, you'll need to configure the
Approvals twice.

What Happens to Direct Reports in a Termination

When you terminate managers, the direct reports are automatically reassigned to the terminated manager's manager if
one of these conditions is true:

• Position synchronization is enabled.

• The direct reports still report to the manager the day after the manager's termination, and the Reassign

Pending Approvals for Terminations and Correct Invalid Supervisor Assignments process is scheduled to
be run regularly.

You can also reassign the direct reports by using the Termination UI when you terminate the manager. We recommend
that you do this in these scenarios:

• The time between the termination notification date and the actual termination date is relatively short.

• You know the new manager of the direct reports.

You can terminate a manager even if they have pending workers as direct reports who aren't yet converted to
employees.

263

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

This flow chart shows how direct reports are reassigned if position synchronization is enabled:

Any direct report changes are reverted in these scenarios, and you get a warning message informing of the same:

• You manually reassign one or more direct reports during the termination, and then change the termination or

the termination notification date.

• You submit the termination for approval after manually reassigning one or more direct reports. The approver

edits the termination and changes the termination or the termination notification date.

Note:  The warning message isn't displayed if you submit the termination without manually reassigning any direct
reports.

264

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Related Topics

• Terminations

• Example of a Worker Termination

About Reversing Terminations

When reversing a termination, any work relationships and assignments previously ended are restored with the statuses
prior to the termination. If a primary work relationship or assignment became non-primary during the termination, it's
changed back to primary when the termination is reversed.

HR specialists and line managers can use either the Termination (version 2 (V2)) or Terminate Employment (version 3
(V3)) quick action on the My Client Groups and My Team tabs respectively for reversing a termination. You can search
for the terminated worker, and click Reverse on the View Termination page. Line managers can reverse the termination,
provided it's in the future and they have the privilege to do so.

What Happens to Roles and User Access

• Any roles automatically provisioned to the person at termination (Beneficiary, for example) are automatically

deprovisioned.

• Any roles deprovisioned either manually or automatically at termination are provisioned again.

•

If the person's user account was disabled at termination, it's re-enabled.

Changes Before and After Termination
If any employment-related actions or changes took place before the termination, they're applied back when you
reverse the termination. But any future-dated changes taking place after the termination aren't restored. Let's say the
employee's department was end-dated after his termination and all employees were relocated to another department.
The reversal of the termination restores the end-dated department and not the new department. An employee's line
manager isn't automatically restored when you reverse the termination. You must manually add the employee back
under the line manager hierarchy by running the Refresh Manager hierarchy process with parameter 0. It's important to
manually verify the employment data after reversing a termination and make the required changes.

Restriction for Reversing a Termination
You can't reverse the termination if the same legal employer has rehired the worker at the same time. Let's say you
terminated an employee on April 15 and rehired the employee with the same legal employer on May 1. You try to reverse
the termination on May 15. You can't do so because this causes the person to have two concurrent employee work
relationships with the same legal employer.

You can perform the reverse termination for an End Global Temporary Assignment transaction only when the
transaction is performed on a nonprimary work relationship.

Note:  You can only use HCM Data Loader and REST API to perform the reverse termination for an End Global
Temporary Assignment transaction if you are using V3 Termination.

265

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

Terminating a Work Relationship

Example of a Worker Termination
You're a human resources (HR) specialist terminating Jack Smith's work relationship. Jack wants to resign from his part
time job of Analyst at the Data Center due to personal reasons.

Let's look at the steps to update the key values for this termination. For other fields, you can use the default values.

Selecting Jack and the Terminate Action

1. On your home page, select either the Termination or Terminate Employment quick action on the My Client

Groups tab.

Note:  The Termination quick action is for version 2 termination and Terminate Employment quick action is
for version 3 termination.

2. Search for Jack Smith and select his work relationship record with the Analyst job.

Enter Termination Information

1.

In the When and Why section, select these values.

Field

Value

When is the termination notification

Select the date Jack first notified you about his plans to resign.

date?

When does the termination take effect?

Select the actual date when you want to terminate Jack's work relationship.

What's the way to terminate the

Resignation

employee?

Why are you terminating Jack Smith?

Personal Reasons

2. Click Continue.
3.

In the Enter Termination Info section, select these field values:

Field

Value

Recommended for Rehire

Yes

Revoke User Access

After termination

266

Oracle Fusion Cloud Human Resources
Using Global Human Resources

4. Click Continue.

Chapter 9
Hire and Manage Workers

Before terminating the work relationship, check whether Jack has direct reports. If yes, reassign the reports by
using the Reassign Existing Reports section. We recommend that you reassign in these scenarios:

◦ The time between the termination notification date and the actual termination date is relatively short.
◦ You know the new manager of the direct reports.

Complete the Termination

1. Click Submit when you're done with the changes.

How Line Manager Synchronization Happens During Termination
When Position Hierarchy Is Used

When the application reassigns direct reports of a terminated manager, the manager is updated for all direct reports,
including active and suspended assignments. This topic explains how the line manger value is synchronized during
termination if you enable synchronization using HCM position hierarchy.

How Line Manager Is Synchronized
When you terminate a manager with direct reports, they’re reassigned when the Synchronize Person Assignment from
Position process is run. However, you can still update the new line manager from the Reassign Directs section but if
the new line manager is different from the manager derived from the position hierarchy, then the line manager will be
corrected when the above process is run.

The line manager is synchronized based on the following conditions:

•

•

•

•

If the position has multiple incumbents, the other incumbent is the new manager.

If no other incumbent exists in the position, the incumbent in the parent position is the new manager. If the
parent position doesn't have an incumbent either, the application checks for an incumbent one level up in the
hierarchy or until it finds an incumbent.

If the parent position has multiple incumbents, the incumbent with the longest tenure is the new manager.

If a parent position doesn't exist or there are no incumbents in all the parent positions in the hierarchy, you can
manually reassign the direct reports to other managers.

Related Topics

• Synchronize Person Assignment from Position Process

FAQs for Terminate Work Relationships

Can I terminate a work relationship if there are future-dated employment changes?
Yes, provided the future changes aren't related to global temporary assignments. If the changes are related to global
temporary assignments, you must delete them and cancel any new work relationship before terminating the current
work relationship.

267

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 9
Hire and Manage Workers

In general, all future-dated changes are lost when you terminate the work relationship or resign from a work
relationship.

Can I terminate the source work relationship from which a global temporary
assignment is created?
No. You must first end the global temporary assignment before terminating the source work relationship.

Can I terminate a person's work relationship when they have a resignation pending
approval from the same work relationship?
Yes, you can because an involuntary work relationship termination is a privileged transaction and takes precedence over
the voluntary work relationship termination (resignation).

Why don't I see all termination actions and reasons when terminating a work
relationship with a global temporary assignment?
Only actions related to ending a global temporary assignment are available when terminating such a work relationship.

How are data conflicts arising from a termination handled?
The application may not identify and resolve all data conflicts arising from a termination. You must verify the data and
manually resolve any pending conflicts.

For example, you must manually reassign any checklist tasks assigned to the terminated person or cancel any training
scheduled for the person.

What happens if I revoke user access from a person with multiple active work
relationships?
The person loses roles provisioned automatically for assignments in this work relationship only. The person keeps roles
that were:

• Provisioned manually

• Acquired automatically for other active work relationships

If the person has roles at termination, then the user account remains active. Otherwise, it's suspended automatically.

What happens when you select worker death in a termination?
If you select death as the termination action for a worker, the termination date, notification date, and the death date
default to today's date. You can edit any of these dates.

However, if you enter a death date that's earlier than the termination date, you get a warning about the date. You may
ignore the warning, in which case the death date defaults to the termination date. Alternatively, you can accept the
changed date and continue, and the new death date is retained.

What's the impact of entering a rehire recommendation during a termination?
The rehire recommendation is for information purposes only and doesn't determine whether a person can be rehired.

268

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

10  Seniority Dates

Overview of Seniority Dates

You can define, manage and use the seniority of workers using version 3 or version 1 of the seniority dates functionality.

You can configure V3 seniority dates using the Configure Seniority Dates task and a fast formula. You can manage them
using the Seniority Dates task under Quick Actions.

This table describes the differences based on the decision points:

Decision

Available from

V1 Version of Seniority Dates

V3 Version of Seniority Dates

Release 1

Release 13.17.11 (17D)

Steps required to enable seniority dates

None

Which seniority dates can be managed?

Only the following seniority dates:

• Enterprise Seniority Date

• Legal Employer Seniority Date

Run the Enterprise Scheduler Service (ESS) job:
Migrate to Version 3 of Seniority Dates

Customers can configure the seniority dates
at different levels, such as Person, Work
Relationship, and Assignment for the following
attributes:

• Business Unit

• Bargaining Unit

• Collective Agreement

• Country

• Department

• Enterprise

• Grade

• Grade Step

•

Job

• Legal Employer

• Location

• Position

• Union

From where are the seniority dates managed?

Work Relationship UI

Seniority Dates UI

Can the seniority dates be entered during Hire
flows?

Yes

No. However, refer to this MOS document for an
alternate solution:

How are seniority dates calculated?

Manually entered or Manually updated

Automatically calculated when the following
ESS job is run: Calculate Seniority Dates

269

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Decision

V1 Version of Seniority Dates

V3 Version of Seniority Dates

Is the seniority calculated in real time?

N/A

No, the following ESS job must be run regularly
to recalculate the seniority dates: Calculate
Seniority Dates

How are the seniority dates updated or
adjusted?

Manually on the Work Relationship UI

Automatically based on Employment actions.

The Legal Employer Seniority Date is 1-
May-2018 and needs to be updated to 1-
Apr-2018. How is the seniority date updated in
this case?

The Legal Employer Seniority Date is corrected
to 1-Apr-2018.

Do you need to configure seniority dates?

No configuration is required.

Note: If you want to default the enterprise
seniority date as the first hire date, you must
set the Default Enterprise Seniority Date
employment configuration option to Yes at the
enterprise level.

Can Fast Formula be used to calculate seniority
dates?

No

Additionally, manual adjustments can be
entered for the seniority dates on the Seniority
Dates UI.

Provide an adjustment of 30 days for the
configured Legal Employer Seniority Date. This
will update the seniority date to 1-Apr-2018
when the ESS job is run.

Seniority rules configuration is required. Use
the Configure Seniority Dates task.

Yes

These formula types are supported:

• Employment Seniority Date Adjustment

• Employment Seniority Hours to Days

Conversion

Do you need to update any worker assignment
before the data migration?

No

Yes

Do you need to run any process post data
migration?

No

Update the seniority basis for all worker
assignment records to the appropriate values in
days or hours. You can do this using HCM Data
Loader.

Run the following ESS job to calculate the
seniority dates for workers: Calculate Seniority
Dates

This ESS job needs to be run regularly or
scheduled to recalculate the seniority dates for
workers.

What are the considerations when uploading
worker assignments?

None

You must provide a value of ORA_PER_SNDT_
DAYS for the Seniority Basis attribute.

File Name: worker.dat

File Discriminator: Assignment

Attribute: SeniorityBasis

270

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Decision

V1 Version of Seniority Dates

V3 Version of Seniority Dates

How can I update seniority dates using HCM
Data Loader?

The Enterprise and Legal Employer seniority
dates can be updated using the following
parameters:

Not Supported

File Name: worker.dat

File Discriminator: WorkRelationship

Attributes: EnterpriseSeniorityDate,
 LegalEmployerSeniorityDate

How can I load seniority date adjustments using
HCM Data Loader?

N/A

Are Database Items (DBIs) available for seniority
dates?

Yes

Which is the table storing the seniority dates
configuration?

N/A

Adjustment for each configured seniority
rule can be uploaded using the following
parameters:

File Name: worker.dat

File Discriminator: SeniorityDate

Attributes: ManualAdjustmentDays,
 ManualAdjustmentComments

Yes

PER_SENIORITY_DATES_SETUP

Which is the table storing the seniority dates of
workers?

Can seniority dates be reported using Oracle
Transactional Business Intelligence (OTBI)?

Can seniority dates be used in Eligibility
Profiles?

PER_PERIODS_OF_SERVICE

PER_SENIORITY_DATES_F

Yes

Yes

Yes

Yes

For more information, see these documents on Customer Connect:

• Seniority Dates - Troubleshooting Seniority Dates - Frequently Asked Questions (https://

community.oracle.com/customerconnect/discussion/631046)

• Seniority Dates V3 - Calculating Seniority Dates Using Fast Formula (https://community.oracle.com/

customerconnect/discussion/631033)

• Seniority Dates V3 - Common Use Cases Configured Using V3 Seniority Dates (https://community.oracle.com/

customerconnect/discussion/631036)

• Seniority Dates V3 - Enabling Enterprise and LE Seniority During Hire (https://community.oracle.com/

customerconnect/discussion/631039)

Note:  If you're using V3 seniority dates, you can't view and manage V1 seniority dates of the legal employer and
enterprise on the Work Relationship page.

271

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Related Topics

• Seniority Dates

• Examples of Calculating Seniority Dates

• Examples of Calculating Cumulative and Noncumulative Seniority Dates

Chapter 10
Seniority Dates

Seniority Dates

Seniority date is the basis of calculation of a person's seniority with the enterprise, department, grade, or other entity.
You can see the seniority dates on the Employment Info page. In most cases, seniority dates are the same as start dates.

On the Seniority Dates page, you can do these things:

• View the length of service, history, and other details for each seniority date rule.

•

If the seniority date rule is configured to allow edits, you can update or correct the manual adjustment units.

Note:  Any adjustments made to the seniority dates don't go through an approval since there is no approval
configuration available for the Manage Seniority Dates process.

• After making any adjustments, you can recalculate a person's seniority using the Recalculate Seniority feature.

You can populate seniority dates for all workers by running the Calculate Seniority Dates process.

You may find that a worker's seniority rule isn't displaying on the Seniority Dates page even though the rule is active.
This may be due to these reasons:

• The rule has a filter and the worker doesn't meet the filter criterion.

• The total length of service for the worker is zero. This could happen for example if the rule is hours-based and

you haven't loaded the seniority hours for the worker.

Related Topics

• How You Configure Seniority Dates

Adjust a Seniority Date

To adjust a seniority date, you can update or correct the seniority date.

When you update a person's seniority date, you add an effective dated record for the person's seniority rule. An
effective dated split is created in the seniority record. For example, here's the seniority record having an effective date of
1-Jan-2005, and it's seniority calculation as of 31-Dec-2007:

Seniority Date Level

Job

Seniority

Seniority Date

Seniority Change
Start Date

Seniority Change End
Date

Job - Person Level

Sales Consultant

3 Years

1-Jan-2005

01-Jan-2005

31-Dec-4712 (Ongoing)

272

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

To do an effective dated update as of 31-Jan-2008, you need you change the date from 1-Jan-2008 to 31-Jan-2008 by
editing the record. To do a correction, leave the date of the record unchanged. In this case, we have added the effective
dated split by changing the date to 31-Jan-2008 and adding the adjustment of 1 year.

Here's the seniority calculation as of 31-Jan-2008:

Seniority Date
Level

Job

Seniority

Seniority Date

Adjustment

Seniority Change
Start Date

Seniority Change
End Date

Job - Person Level

Sales Consultant

4 Years 1 Months

1-Jan-2004

1 Years

31-Jan-2008

31-Dec-4712
(Ongoing)

Job - Person Level

Sales Consultant

3 Years

1-Jan-2005

Null

01-Jan-2005

30-Jan-2008

Note:  The seniority change end date for a particular seniority rule is shown as Ongoing in the latest effective-dated
row, instead of the actual date 31-Dec-4712.

You can manually adjust a seniority rule by clicking the edit icon (pencil icon) on a seniority record. By default, the
seniority record displays the same effective date as the row from which the transaction was initiated.

Here's how you can adjust a person's seniority by updating the manual adjustment units:

1. Click the Seniority Dates task under Quick Actions on the home page.
2. Search and select the person for whom you want to adjust the seniority date.
3.
In the Seniority Dates section, click Edit.
4. Select the date for the seniority change.

Note:  Don't change the existing date if you're correcting the seniority.

5. Enter the manual value for the seniority adjustment.

Note:  If the seniority basis on the worker's assignment is days, enter the adjustment in days. If it's in hours,
enter the adjustment in hours. Enter a positive number to increase seniority by moving the date back. Enter a
negative number to reduce seniority by moving the date forward.

6. Add any comments.
7. Click OK.
8. Click Save.

Examples of Calculating Seniority Dates

Let's look at some examples of calculating seniority dates based on assignment and work relationship changes.

In these examples, the job seniority date is configured at these levels:

• Person

• Work Relationship

• Assignment

273

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Calculation Based on Assignment Changes
Vijay Singh is hired in Vision IND legal employer on 1-Jan-2005. He has multiple assignments and work relationships in
the enterprise. This table shows a summary of his default seniority dates.

Date

Action

Legal Employer

Assignment

Job

Department

1-Jan-2005

Hire

Vision IND

Assignment 1

Sales Consultant

ERP

Here's the seniority calculation as of 1-Jan-2006:

Seniority Date Level

Job

Seniority

Seniority Date

Exit Date

Job - Person Level

Sales Consultant

1 Year

1-Jan-2005

Job - Work Relationship
Level

Sales Consultant

1 Year

1-Jan-2005

Job - Assignment Level

Sales Consultant

1 Year

1-Jan-2005

N/A

N/A

N/A

Starting 1-Jan-2007, Vijay has a new assignment in the HCM department, but continues to perform the same job. His
current assignment is end dated.

Date

Action

Legal Employer

Assignment

Job

Department

1-Jan-2005

Hire

Vision IND

Assignment 1

Sales Consultant

ERP

1-Jan-2007

End Assignment

Vision IND

Assignment 1

Sales Consultant

ERP

1-Jan-2007

Add Assignment

Vision IND

Assignment 2

Sales Consultant

HCM

Here's the seniority calculation as of 1-Jan-2008:

Seniority Date Level

Job

Seniority

Seniority Date

Exit Date

Job - Person Level

Sales Consultant

3 Years

1-Jan-2005

Job - Work Relationship
Level

Sales Consultant

3 Years

1-Jan-2005

N/A

N/A

Job - Assignment Level

Sales Consultant
(Assignment 1)

2 Years

1-Jan-2005

31-Dec-2006

274

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Seniority Date Level

Job

Seniority

Seniority Date

Exit Date

Job - Assignment Level

Sales Consultant
(Assignment 2)

1 Year

1-Jan-2007

N/A

Calculation Based on Work Relationship Changes
On 1-Jan-2010, Vijay is transferred globally to a new legal employer but in the same department.

Date

Action

Legal Employer

Assignment

Job

Department

1-Jan-2005

Hire

Vision IND

Assignment 1

Sales Consultant

ERP

1-Jan-2007

End Assignment

Vision IND

Assignment 1

Sales Consultant

ERP

1-Jan-2007

Add Assignment

Vision IND

Assignment 2

Sales Consultant

HCM

1-Jan-2010

Global Transfer

InFusion US

Assignment 3

Sales Consultant

HCM

Here's the seniority calculation as of 1-Jan-2011:

Seniority Date Level

Job

Seniority

Seniority Date

Exit Date

Job - Person Level

Sales Consultant

6 Years

1-Jan-2005

N/A

Job - Work Relationship
Level

Sales Consultant (Vision
IND)

5 Years

1-Jan-2005

31-Dec-2009

Job - Work Relationship
Level

Sales Consultant (InFusion
US)

1 Year

1-Jan-2010

N/A

Job - Assignment Level

Sales Consultant
(Assignment 1)

2 Years

1-Jan-2005

31-Dec-2006

Job - Assignment Level

Sales Consultant
(Assignment 2)

3 Years

1-Jan-2007

31-Dec-2009

Job - Assignment Level

Sales Consultant
(Assignment 3)

1 Year

1-Jan-2010

N/A

Related Topics

• Examples of Calculating Cumulative and Noncumulative Seniority Dates

275

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

How Cumulative Seniority Dates Are Calculated

You can configure the seniority dates rules to calculate seniority on a cumulative basis. Let's look at an example that
explains how the application calculates cumulative seniority.

In this example, the enterprise seniority date is configured at the Person Level.

Calculation Based on Cumulative Seniority
Vijay Singh is hired in Vision IND legal employer on 1-Jan-2005.

Date

Action

Legal Employer

Assignment

Job

Department

1-Jan-2005

Hire

Vision IND

Assignment 1

Sales Consultant

ERP

Here's the seniority calculation as of 31-Dec-2005:

Seniority Date Rule

Seniority

Seniority Date

Seniority Change Start
Date

Seniority Change End
Date

Enterprise- Person Level

1 Year

1-Jan-2005

1-Jan-2005

31-Dec-4712 (Ongoing)

On 31-Dec-2006, Vijay Singh resigns from the organization.

Date

Action

Legal Employer

Assignment

Job

Department

1-Jan-2005

Hire

Vision IND

Assignment 1

Sales Consultant

ERP

31-Dec-2006

Resignation

Vision IND

Assignment 1

Business Analyst

ERP

Here's the seniority calculation as of 31-Dec-2006:

Seniority Date Rule

Seniority

Seniority Date

Exit Date (Enterprise
End Date)

Seniority Change
Start Date

Seniority Change End
Date

Enterprise- Person
Level

2 Years

1-Jan-2005

31-Dec-2006

1-Jan-2005

31-Dec-4712 (Ongoing)

The exit date will be populated because the person is no longer active.

276

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Note:  The seniority dates UI displays the label for the exit date as <Seniority Rule Attribute> End Date. In this case, it
will be Enterprise End Date because the seniority rule is configured by using the Enterprise attribute.

On 1-Jan-2008, Vijay Singh is rehired in the organization.

Date

Action

Legal Employer

Assignment

Job

Department

1-Jan-2005

Hire

Vision IND

Assignment 1

Sales Consultant

ERP

31-Dec-2006

Resignation

Vision IND

Assignment 1

Business Analyst

ERP

1-Jan-2008

Rehire

Vision IND

Assignment 2

Program Manager

ERP

Here's the seniority calculation as of 31-Dec-2008:

Seniority Date
Rule

Enterprise- Person
Level

Enterprise- Person
Level

Seniority

Seniority Date

Exit Date

Seniority Change
Start Date

Seniority Change
End Date

Auto Adjustment
Days

3 Years

1-Jan-2006

Null

1-Jan-2008

31-Dec-4712
(Ongoing)

-365 days

2 Years

1-Jan-2005

31-Dec-2006

1-Jan-2005

31-Dec-2007

null

The new seniority split will be created on the rehire date.

Here's how the application calculates the seniority for Vijay:

1. The length of service is calculated between the seniority process run date and the hire date (the period

between 1-Jan-2005 and 31-Dec-2008 = 4 years).

2. The duration for which the person wasn't active for the seniority rule is calculated. In this case, it's 1 year or 365

days (the period between 1-Jan-2007 and 31-Dec-2007).

3. The period for which the person wasn't active in a seniority rule is subtracted from the duration that's

calculated in step 1 (4 years - 365 days = 3 years). Since this period needs to be reduced, the -365 days is added
as an auto adjustment in the latest seniority record. Therefore, the total cumulative seniority period will be 4
years - 1 year (365 days) = 3 years.

4. Finally, the seniority date is calculated by reducing the seniority period (3 years) calculated in step 3 from the

process run date (31-Dec-2008). Therefore, in this case, the seniority date will be 1-Jan-2006 (31-Dec-2008 - 3
years).

277

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Examples of Calculating Cumulative and Noncumulative
Seniority Dates

You can configure the seniority dates rules to calculate seniority on a cumulative basis. Let's look at some examples of
calculating seniority dates based on cumulative and noncumulative seniority.

In these examples, the job seniority date is configured at these levels:

• Person

• Work Relationship

• Assignment

Calculation Based on Cumulative Seniority
Priya Krishnan has multiple assignments and work relationships in the enterprise, and the cumulative option has been
turned on for all the 3 job seniority dates.

Priya Krishnan is hired in Vision IND legal employer on 1-Jan-2005. This table shows a summary of her default seniority
dates.

Date

Action

Legal Employer

Assignment

Job

Department

1-Jan-2005

Hire

Vision IND

Assignment 1

Sales Consultant

ERP

Here's the seniority calculation as of 1-Jan-2006:

Seniority Date Level

Job

Seniority

Seniority Date

Exit Date

Job - Person Level

Sales Consultant

1 Year

1-Jan-2005

Job - Work Relationship
Level

Sales Consultant

1 Year

1-Jan-2005

Job - Assignment Level

Sales Consultant

1 Year

1-Jan-2005

N/A

N/A

N/A

On 1-Jan-2007, Priya Krishnan has a job transfer in the current assignment.

Date

Action

Legal Employer

Assignment

Job

Department

1-Jan-2005

Hire

Vision IND

Assignment 1

Sales Consultant

ERP

1-Jan-2007

Job Change

Vision IND

Assignment 1

Business Analyst

ERP

278

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Date

Action

Legal Employer

Assignment

Job

Department

Here's the seniority calculation as of 1-Jan-2008:

Seniority Date Level

Job

Seniority

Seniority Date

Exit Date

Job - Person Level

Sales Consultant

2 Years

1-Jan-2005

31-Dec-2006

Job - Work Relationship
Level

Sales Consultant

2 Years

1-Jan-2005

31-Dec-2006

Job - Assignment Level

Sales Consultant

2 Years

1-Jan-2005

31-Dec-2006

Job - Person Level

Business Analyst

1 Year

1-Jan-2007

Job - Work Relationship
Level

Business Analyst

1 Year

1-Jan-2007

Job - Assignment Level

Business Analyst

1 Year

1-Jan-2007

N/A

N/A

N/A

Note:  Two seniority date records are generated at each seniority date level. This is because there's a change in the job
attribute that's used for calculating the seniority dates.

On 1-Jan-2008, Priya Krishnan has a new assignment in a different department. However, her job changes back to her
earlier job of Sales Consultant. Her current assignment is end dated.

Date

Action

Legal Employer

Assignment

Job

Department

1-Jan-2005

Hire

Vision IND

Assignment 1

Sales Consultant

ERP

1-Jan-2007

Job Change

Vision IND

Assignment 1

Business Analyst

ERP

1-Jan-2008

End Assignment

Vision IND

Assignment 1

Business Analyst

ERP

1-Jan-2008

Add Assignment

Vision IND

Assignment 2

Sales Consultant

HCM

Here's the seniority calculation as of 1-Jan-2009:

Seniority Date Level

Job

Seniority

Seniority Date

Exit Date

Job - Person Level

Sales Consultant

2 Years

1-Jan-2005

31-Dec-2006

279

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Seniority Date Level

Job

Seniority

Seniority Date

Exit Date

Job - Work Relationship
Level

Sales Consultant

2 Years

1-Jan-2005

31-Dec-2006

Job - Assignment Level

Sales Consultant
(Assignment 1)

2 Years

1-Jan-2005

31-Dec-2006

Job - Person Level

Business Analyst

1 Year

1-Jan-2007

31-Dec-2007

Job - Work Relationship
Level

Business Analyst

1 Year

1-Jan-2007

31-Dec-2007

Job - Assignment Level

Business Analyst
(Assignment 1)

1 Year

1-Jan-2007

31-Dec-2007

Job - Person Level

Sales Consultant

3 Years

1-Jan-2008

Job - Work Relationship
Level

Sales Consultant

3 Years

1-Jan-2008

Job - Assignment Level

Sales Consultant
(Assignment 2)

1 Year

1-Jan-2008

N/A

N/A

N/A

Note:  Job seniority dates are configured to be cumulative, therefore, the job seniority equals 1 year in the current
assignment plus 2 years in the previous assignment.

Calculation Based on Noncumulative Seniority
Priya Krishnan has multiple assignments and work relationships in the enterprise, and the cumulative option has been
turned off for all the 3 job seniority dates.

Priya Krishnan is hired in Vision IND legal employer on 1-Jan-2005. This table shows a summary of her default seniority
dates.

Date

Action

Legal Employer

Assignment

Job

Department

1-Jan-2005

Hire

Vision IND

Assignment 1

Sales Consultant

ERP

Here's the seniority calculation as of 1-Jan-2006:

Seniority Date Level

Job

Seniority

Seniority Date

Exit Date

Job - Person Level

Sales Consultant

1 Year

1-Jan-2005

N/A

280

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Seniority Date Level

Job

Seniority

Seniority Date

Exit Date

Job - Work Relationship
Level

Sales Consultant

1 Year

1-Jan-2005

Job - Assignment Level

Sales Consultant

1 Year

1-Jan-2005

N/A

N/A

On 1-Jan-2007, Priya Krishnan has a job transfer in the current assignment.

Date

Action

Legal Employer

Assignment

Job

Department

1-Jan-2005

Hire

Vision IND

Assignment 1

Sales Consultant

ERP

1-Jan-2007

Job Change

Vision IND

Assignment 1

Business Analyst

ERP

Here's the seniority calculation as of 1-Jan-2008:

Seniority Date Level

Job

Seniority

Seniority Date

Exit Date

Job - Person Level

Sales Consultant

2 Years

1-Jan-2005

31-Dec-2006

Job - Work Relationship
Level

Sales Consultant

2 Years

1-Jan-2005

31-Dec-2006

Job - Assignment Level

Sales Consultant

2 Years

1-Jan-2005

31-Dec-2006

Job - Person Level

Business Analyst

1 Year

1-Jan-2007

Job - Work Relationship
Level

Business Analyst

1 Year

1-Jan-2007

Job - Assignment Level

Business Analyst

1 Year

1-Jan-2007

N/A

N/A

N/A

Note:  Two seniority date records are generated at each seniority date level. This is because there's a change in the job
attribute that's used for calculating the seniority dates.

On 1-Jan-2008, Priya Krishnan has a new assignment in a different department. However, her job changes back to her
earlier job of Sales Consultant. Her current assignment is end dated.

Date

Action

Legal Employer

Assignment

Job

Department

1-Jan-2005

Hire

Vision IND

Assignment 1

Sales Consultant

ERP

281

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Date

Action

Legal Employer

Assignment

Job

Department

1-Jan-2007

Job Change

Vision IND

Assignment 1

Business Analyst

ERP

1-Jan-2008

End Assignment

Vision IND

Assignment 1

Business Analyst

ERP

1-Jan-2008

Add Assignment

Vision IND

Assignment 2

Sales Consultant

HCM

Here's the seniority calculation as of 1-Jan-2009:

Seniority Date Level

Job

Seniority

Seniority Date

Exit Date

Job - Person Level

Sales Consultant

2 Years

1-Jan-2005

31-Dec-2006

Job - Work Relationship
Level

Sales Consultant

2 Years

1-Jan-2005

31-Dec-2006

Job - Assignment Level

Sales Consultant
(Assignment 1)

2 Years

1-Jan-2005

31-Dec-2006

Job - Person Level

Business Analyst

1 Year

1-Jan-2007

31-Dec-2007

Job - Work Relationship
Level

Business Analyst

1 Year

1-Jan-2007

31-Dec-2007

Job - Assignment Level

Business Analyst
(Assignment 1)

1 Year

1-Jan-2007

31-Dec-2007

Job - Person Level

Sales Consultant

1 Year

1-Jan-2008

Job - Work Relationship
Level

Sales Consultant

1 Year

1-Jan-2008

Job - Assignment Level

Sales Consultant
(Assignment 2)

1 Year

1-Jan-2008

N/A

N/A

N/A

Note:  Job seniority dates are configured to be noncumulative, therefore, the job seniority considers the length of
service in the current assignment only.

Related Topics

• Examples of Calculating Seniority Dates

282

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Hours-Based Seniority Calculation

These dates impact the seniority calculation for an hours-based rule:

• Seniority process run date

• Attribute end date

• Seniority end date

Seniority Process Run Date
The date on which the Calculate Seniority Dates process was run is used in the seniority-hours calculation. The process
calculates the seniority dates for workers based on the seniority rules configured in the application.

Attribute End Date
If there's a change in the attribute or level at which the seniority rule is configured, the attribute end date is used in the
calculation. For example, let's say the rule is configured for job attribute and assignment level, and a worker has a job
change. The job end date of the first job will be used in the seniority date calculation.

Seniority End Date
This date is used in the calculation if there's an effective-dated update on the seniority rule. For example let's say
an effected-dated adjustment resulted in a new row being added for a seniority rule. The seniority end date of the
previously existing row is calculated as: Start date of the newly added row - 1 day.

Note:  The calculations are valid when the attribute end date or the seniority end date isn't set to a null or to the end
of time (12-31-4712).

Seniority Date Calculation
Here's how the seniority date for the hours-based rule is calculated.

1. Get the minimum date from these dates: Calculate Seniority Dates process run date, attribute end date, and

seniority end date.

2. Reduce the length of service from the minimum date.
3. Add one day to the resulting date value in step 2.

Examples of Calculating Hours-Based Seniority

In this example, you're an HR specialist configuring the enterprise seniority date at the person level. You are defining an
hours-based seniority rule to calculate a worker's length of service. Here's how the hour conversion is defined:

• 8 hours in a day and 40 hours in a week

•

173.33 hours in a month (hours in a year divided by 12)

• 2080 hours in a year and 52 weeks in a year

283

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Let's see how to calculate the length of service for a worker Maya Singh using the hours-based seniority rule. Maya is an
hourly employee and her work hours are entered in the seniority hours table (PER_SENIORITY_HOURS) every week.

Maya is hired in the Vision IND legal employer on 1-Jan-2007.

Date

Action

Legal Employer

Assignment

Job

Department

1-Jan-2007

Hire

Vision IND

Assignment 1

Sales Consultant

ERP

Seniority at the End of a Week
Applying the rule, Maya has a seniority of 40 hours for the week ending 7-Jan-2007.

Start Date

1-Jan-2007

End Date

7-Jan-2007

Seniority Hours

40

Here's how the seniority is calculated:

Length Of Service

Total Seniority Hours

How length of service is calculated

0 Years 0 Months 5 Days

40

Total seniority hours are less than the hours
defined for a month (173.33). Therefore, total
seniority hours are converted into days when
calculating the length of service. The length of
service calculation in days is 40 divided by 8
(hours in a day).

Seniority at the End of 6 Months
Maya has a seniority of 1080 hours after 6 months as of 7-Jul-2007.

Here's how the seniority is calculated:

Length Of Service

Total Seniority Hours

How length of service is calculated

0 Years 6 Months 5 Days

1080

Total seniority hours are less than the hours
defined for a year (2080), but more than the
hours defined for a month (173.33).

The number of months are calculated first
so that the total number of seniority hours -
(number of months * hours defined for the
month) < hours defined for the month.

Therefore, the number of months in this
scenario are 6. Using values in the equation:
1080 - (6 * 173.33) = 40 (this is less than 173.33).
For the remaining 40 hours, a day conversion

284

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Length Of Service

Total Seniority Hours

How length of service is calculated

is done, which amounts to 5 days (40 divided
by 8). Therefore, the final length of service is 0
years 6 months 5 days.

Seniority at the End of 1 Year 6 Months
Maya has a seniority of 3160 hours after 1 year and 6 months as of 7-Jul-2008.

Here's how the seniority is calculated:

Length Of Service

Total Seniority Hours

How length of service is calculated

1 Years 6 Months 5 Days

3160

Total seniority hours are more than the hours
defined for a year (2080).

The number of years are first calculated so
that total number of seniority hours - (number
of years * hours defined for the year) < hours
defined for the year.

Therefore, the number of years in this scenario
is 1. Using values in the equation: 3160 - (1 *
2080) = 1080 (this is less than 2080). For the
remaining 1080 hours, a month conversion is
done, which amounts to 6 months. Then, a day
conversion is done that amounts to 5 days.

Note:  For hours-based seniority rules, the seniority date is calculated by reducing the total length of service from the
seniority calculation process run date.

Process to Calculate Seniority Dates

Use the Calculate Seniority Dates process to calculate the seniority dates for workers based on the seniority rules
configured in the application. Use the Scheduled Processes work area to schedule and run the process.

Note:

•

•

Even if you have enabled audit for seniority dates, the dates aren't audited when they are updated by the
Calculate Seniority Dates process.

Seniority dates aren't calculated for work relationships and assignments that start in the future.

Process Parameters

• Person Number: This parameter filters the person numbers which are to be included in the ESS process for
processing. You can run this process for more than one person by entering the person numbers separated

285

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

by commas. For example, use this format: Person Number 1,Person Number 2,Person Number 3. Don't enter
leading or trailing space, or special characters. If you want to run this process for all persons, don't enter any
value.

• Past Period in Days: This parameter indicates the last period in days in which the data is changed for the

person. The parameter scans these tables to find any data changes:

◦ PER_ALL_ASSIGNMENTS_M
◦ PER_ASSIGN_GRADE_STEPS_F
◦ PER_SENIORITY_HOURS

The parameter analyzes the LAST_UPDATE_DATE column of these tables and compares it with the days passed
in the parameter for processing.

Note:  Workers who have no changes to their assignment, grade step, or seniority hours in the past period
in days are excluded from the calculation. But you can recalculate seniority for a specific worker using the
Recalculate Seniority option on the Manage Seniority Dates page.

•

•

Include Terminated Work Relationships: This parameter checks the status of the work relationship. If you
pass the value Y as the parameter, the process will include terminated work relationships for calculating
seniority dates. When you modify the data in an inactive work relationship and pass the value N, the application
won't process the assignments in this work relationship. You notice this behavior even though the assignment
records are modified in the past N days.

Include Complete Assignment History: This parameter completely refreshes the version 3 (V3) seniority dates
for the persons selected based on the values passed for other parameters. When you select this parameter, the
application checks the complete assignment history of persons and recalculates their V3 seniority dates. For
example, this parameter can be used to calculate the cumulative seniority dates for rehires.

• Legal Employer: This parameter filters the person records based on the legal employer specified.

• Union: his parameter filters the person records based on the union specified.

• Available Seniority Date Rules: This parameter filters the seniority dates rules for which the ESS process
needs to be run. If we pass the parameter as null, the ESS process will run for all the active rules in the
application.

Process Frequency
It’s recommended that you run the Calculate Seniority Dates process regularly. Here’s the recommended schedule:

• Daily: Schedule the process to run daily by setting the value of the Past Period in Days parameter as 1 day.
• Weekly: Schedule the process to run weekly by setting the value of the Past Period in Days parameter as 7 days.
• Quarterly: Schedule the process to run quarterly by setting the value of the Past Period in Days parameter as

1500 days.

• Ad hoc: Run the process before important events in the organization, such as Promotion Cycle, Performance

Cycle, and Annual Compensation Cycle.

Note:  The recommended guidelines are generic. You must determine the process schedule based on the business
process and worker population in your organization.

286

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Related Topics

• What are scheduled processes?

• Submit Scheduled Processes and Process Sets

V1 Seniority Dates

You can manage the following two seniority dates while using V1 version of the Seniority Dates.

Enterprise Seniority Date
A person has a single enterprise seniority date, which is the date on which calculation of a person's enterprise seniority
is based. The enterprise seniority date is the start date of a person's primary work relationship by default. You can
update a person's enterprise seniority date only when you create or edit the person's primary work relationship.

You can update the enterprise seniority date for any reason; for example, you may want to adjust the date to include
previous service. Consider the following employee work relationships, where a break exists between the end of the first
work relationship and the start of the second.

Type

Legal Employer

Start Date

Enterprise Seniority Date

Termination Date

Employee

Employee

A

B

5 January, 2004

5 January, 2004

31 December, 2004

1 May, 2005

5 May, 2004

In this example, the person's enterprise seniority date, until the start of the work relationship with legal employer B, is 5
January, 2004. When you create the second work relationship, you can enter a new enterprise seniority date that takes
account of the person's previous employee seniority. To calculate the person's new enterprise seniority date, you would
add 120 days (the period from 1 January, 2005, to 30 April, 2005, when this person was not employed) to the previous
enterprise seniority date, 5 January, 2004, to give a revised enterprise seniority date of 5 May, 2004. If you didn't enter
the new date, the enterprise seniority date is 1 May, 2005.

Note:  If you select a different primary work relationship for a person, the existing enterprise seniority date copies
automatically to the new primary work relationship and is removed from the previous primary work relationship.

Legal Employer Seniority Date
A person can have three work relationships simultaneously with a single legal employer:

• Employee

• Contingent worker

• Nonworker

Legal employer seniority dates are maintained for all three types of work relationships; therefore, a person can have up
to three legal employer seniority dates for a single legal employer.

287

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

If you leave the legal-employer seniority date in a work relationship blank, it's assumed to be the same as the start or
hire date of the work relationship.

You can adjust legal-employer seniority dates for any reason. For example, if a person takes an absence of one month
that can't be included in seniority calculations, you can adjust the dates of the person's work relationship as shown in
this table.

Type

Employee

Start Date

1 March, 2010

Legal Employer Seniority Date

1 April, 2010

This adjustment has the effect of reducing the person's employee legal-employer seniority by one month, which may
affect the person's entitlement to seniority-related benefits.

When a person has multiple sequential relationships of the same type with a single legal employer, you can adjust the
legal employer seniority date of the latest work relationship manually to include the previous seniority.

These are the frequently asked questions (FAQs) for V1 version of the Seniority Dates functionality.

What's the difference between legal employer seniority dates and
enterprise seniority dates?
Legal employer seniority dates relate to work relationships with a legal employer. The legal employer:

• Start or hire date is the start date of the work relationship.

• Seniority date is the date on which a person's legal employer service of a particular type (employee, contingent
worker, or nonworker) is based. A person can have up to three legal employer seniority dates for a single legal
employer. If you enter no date, the legal employer seniority date is assumed to be the start date of the work
relationship.

Enterprise seniority dates relates to a person's service with the enterprise rather than with individual legal employers.

The enterprise start or hire date is the start date of a person's first work relationship of this type (employee, contingent
worker, or nonworker) in the enterprise. For example, a person's nonworker enterprise start date is the start date of the
person's first nonworker work relationship with any legal employer in the enterprise. Therefore, a person can have up to
three enterprise start dates.

The enterprise seniority date is the date on which a person's enterprise service is based. By default, the enterprise
seniority date is the start date of the person's current primary work relationship.

How can I configure the enterprise seniority date as default?
You can configure employment-related options at the enterprise level using the Manage Enterprise HCM Information
task in the

Setup and Maintenance work area. The following table explains the Default Enterprise Seniority Date.

Option

Description

Default Value

Default Enterprise Seniority Date

You can use this option to control whether
the enterprise seniority date is automatically
populated when you create a new work

Yes

288

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

Option

Description

Default Value

relationship. You can select from the following
values:

Yes: The enterprise seniority date is
automatically populated.

No: The enterprise seniority date is not
automatically populated.

What happens to the enterprise seniority date if I change a person's
primary work relationship?
If there's no break in service between the previous and new primary work relationships, the enterprise seniority date is
copied automatically to the new primary work relationship. Otherwise, you may need to enter the date manually.

What happens if I change a person's hire or start date?
The start dates of any assignments that had the same start date as the work relationship change automatically to the
new date.

In addition:

• The enterprise start date changes automatically to the new date if you change the start date of a person's first

work relationship of a particular type in the enterprise. Otherwise, the enterprise start date is unaffected.

• The legal-employer seniority date is assumed to be the same as the new hire or start date if the dates were the
same before the change was made. Otherwise, the date is unaffected by the change. You may have to adjust
the legal-employer seniority date manually if you had previously entered a date.

• The enterprise seniority date adjusts automatically to match the new hire or start date if you change the start
date of the primary work relationship and the dates were the same before you made the change. Otherwise,
you may have to adjust the enterprise seniority date manually.

What happens if I change a person's seniority date?
Changes to a person's legal-employer or enterprise seniority dates affect the calculation of the person's length of
service. Therefore, the changes may affect the person's entitlement to seniority-based benefits.

In addition:

•

•

If you update the enterprise seniority date on a person's primary work relationship, that change applies
automatically to all of the person's work relationships that had the same enterprise seniority date before the
update. You can't update the enterprise seniority date on a nonprimary work relationship.

If you leave a legal-employer seniority date blank, it's assumed to be the same as the start or hire date of the
work relationship. If you enter a value for the legal-employer seniority date, you may be required to maintain it
subsequently.

289

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 10
Seniority Dates

290

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 11
Document Records

11  Document Records

Overview of Document Records

Document Records is a generic and extensible transaction within HCM. It can be used in various ways as it supports
granular levels of security, approvals, auditing, custom fields, attachments and so on.

The basic usage of Document Records is to capture documents records related to an employee's personnel file that are
required by the various business processes of the organization. For example, birth and marriage certificates required for
benefits processing, passport and visa documents required for business travel arrangements.

There's a difference between Document Records and attachments. Document Records is a combination of metadata
and attachments. It enables you to capture key metadata information about the attachment that they upload. For
example, Issue Date, Expiry Date, and Document Number.

Differences between Document Records and Person Identification Info

Document Records

Person Identification Info

Built after the initial release of HCM Cloud

Built to support easy migration from PeopleSoft to HCM Cloud. Also, these objects have some specific

and designed to be a generic solution for

fields and potential localization validations applied to them and are intended for HR professionals and

capturing details of various document

employees, not Line Managers.

types across various roles.

There's no limit on the number of

Only these types are available: Citizenship, Driver's Licenses, Passports, Visa and Permits.

document types that can be configured.

Additional document types can be added

Can't add additional types.

using the Document Types setup task.

Stores all information in a single HR

Separate tables to store specific information such as passports, visas, and so on.

document records table.

Supports Attachments.

Attachments aren’t supported.

Follows approval rule of Manage

Follows approval rule of Change Personal Information: Citizenship, Change Personal Information:

Document Records.

Driver's Licenses, Change Personal Information: Passports, Change Personal Information: Visa and

Permits.

Access to document records can be

Access to objects in person identification info can be managed through specific aggregate privileges.

managed through document type security

For more information, see Securing HCM guide.

profiles.

291

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 11
Document Records

How You Scan Attachment to Prefill Document Record
Attributes

You can prefill document record attributes including flexfield attributes without having to manually enter them in the
Document Details page. You can scan and prefill these attributes from an attachment:

• Number

• From Date

• To Date

•

•

•

•

Issuing Country

Issuing Location

Issued On

Issuing Authority

You can scan and prefill flexfield attributes which have value sets of validation type FORMAT ONLY, TABLE,
INDEPENDENT and SUBSET.

You can control the manual entry of attribute values by making the fields as read-only. This will ensure that users only
use the scanning feature to prefill the attribute values.

This example explains how you can scan an attachment for the Passport document type and prefill attributes (Number,
From Date, To Date, and Issuing Location) in the Document Details page.

1. On the home page, click the My Client Groups tab.
2. Click the Document Records quick action in the Employment area.
3.

In the Document Records page, search and select the person for whom you want to prefill document record
attributes.

4. Click the Add drop-down list, and then select Add from Attachment.
5. Select the Passport document type for which you want to prefill document record attributes.
6.
In the Attachments section, click the link to add the passport attachment.
7. After the attachment has been successfully uploaded, click Extract Data.
8.

In the Select Field list, select the following attributes and scan the corresponding values from the attachment:
◦ Number: Select the area in the attachment which displays the passport number, and then click OK.
◦ From Date (Select the appropriate date format): Select the area in the attachment which displays the

issue date, and then click OK.

◦ To Date (Select the appropriate date format): Select the area in the attachment which displays the expiry

date, and then click OK.

◦ Issuing Location: Select the area in the attachment which displays the place of issue, and then click OK.

9. Click Done. The document record attributes will be prefilled in the Document Details page.

This example explains how you can scan an attachment for the Drivers License document type and prefill flexfield
attributes (Name, Driver License Type, Reference Number, and Country Code) in the Document Details page.

1. Repeat steps 1 through 4 in the previous example.
2. Select the Drivers License document type for which you want to prefill document record flexfield attributes.
3.

In the Attachments section, click the link to add the driver license attachment.

292

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 11
Document Records

4. After the attachment has been successfully uploaded, click Extract Data.
5.

In the Select Field list, select the following flexfield attributes and scan the corresponding values from the
attachment:

a. Name: Select the area in the attachment which displays the name of the person, and then click OK.
b. Driver License Type: Select the area in the attachment which displays the license type, and then click

OK.

c. Reference Number: Select the area in the attachment which displays the reference number, and then

click OK.

d. Country Code: Select the area in the attachment which displays the country code, and then click OK.

6. Click Done. The document record flexfield attributes will be prefilled in the Document Details page.

Points to Consider

• You can’t scan and prefill while editing a document record.

• You can upload attachments for scanning. These file formats are supported for scanning of attributes: PDF, PPT

or PPTX, DOC or DOCX, TXT, and XLS or XLSX

Note:  Image file formats, such as PNG, JPG, TIF, and GIF are not supported for scanning of attributes. This
includes images converted to PDF or added to word processing documents, such as DOC or DOCX.

•

If you add more than one attachment for scanning, then the extract data process will only consider the most
recent attachment.

• You can’t upload or parse password-protected documents.

• You can scan and prefill a read-only attribute in the Document Details page.

• The Select Field list includes attributes configured for the document type, such as Name, Number, and Issuing

Country. Additionally, the list includes these segments:

◦ Global segments of the document record descriptive flexfield (DFF).
◦ Context-specific segments of the document type. These segments default the context based on the

system document type for document record DFF and developer descriptive flexfield (DDF).

Note:  If the document type and context code don't match, then the context defaulting doesn't happen
and the context segment won’t be displayed in the list.

•

If you select the Issuing Country attribute from the Select Field list while scanning, you need to select the
corresponding country name (for example, United States), and not the country code (for example, US) from the
attachment.

Mass Download Document Records

You can mass download all document records and its attachments for a document type or person, or both. For example,
you can download all document records for a particular document type, such as passports for all persons.

You can use the Mass Download of Document Records quick action in the My Client Groups tab on the Home page. Or,
you can use the download option on the Document Records list page to download all document records for a person
based on the filter criteria used.

• You can't download document records for all document types and people at once because of performance

reasons. You must specify either a document type or a person.

293

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 11
Document Records

• You can't download document records that are pending approval.

• You might receive an intermittent error message when you download large attachment files; however, the files

are downloaded. Click OK to bypass the error message.

Submit Request to Mass Download Document Records
You can submit a request to mass download document records by using the Add button on the Submitted Mass
Download Processes page. On the New Mass Download of Document Records page, you can select these values:

• Process Name: Enter the process name for the new request.

• Group by: Group document records using any of these options:

◦ None: This is the default option.
◦ Document Type: Group by each document type.
◦ Person: Group by individual person.

• List of Persons

• Person

• Document type

• Category of the document record. For example, Absence, Benefits, and Compensation.

• Subcategory

• Document Type

Note:  If you select a person, then the application populates only those document types of the person for
which the logged in user has access. If you don’t select a person, all document types are populated based on
the logged in user’s access and roles.

• Created From: Source of the document record creation. For example, Absence cases, Allocated checklist tasks,

and Employment actions.

• Document records updated in a specific date range (optional).

The application creates download folders based on the grouping criteria. This is how folders are created for each criteria:

• None: No folders are created and all downloaded files are saved in a single folder.

• Document Type: A folder is created for each downloaded document type. The folder is named after the

document type and contains individual downloaded files for each person.

• Person: A folder is created for each person. The folder is named after the person number and contains

individual downloaded files for each system document type.

The download folder uses this file name format: PersonNumber_SystemDocumentType_UCMID_PhysicalFileName. For
example, 955160008186124_GLB_PASSPORT_UCMFA00027817_My India Passport.pdf

Note:  You can't change the file name format.

Here are some points to consider:

• You can select multiple values in the List of Persons field from the respective List of Values (LoV) when you’re

selecting users for whom you want to download document records.

• You can also select multiple categories, subcategories, document types, created from, and tags.

294

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 11
Document Records

Status of Submitted Mass Download Requests
After you submit the request to mass download document records, a scheduled process or job is submitted and its
status is displayed on the Submitted Mass Download Processes page. The status of the submitted process is displayed
as Running, Succeeded, or Error. Also, the page displays a progress bar to indicate the progress of each submitted
process. The page is auto refreshed every 30 seconds to display the latest progress of the submitted process. You can
cancel an incomplete scheduled job and resubmit the job using the same set of parameters.

When a submitted scheduled process job succeeds, the attachments can be downloaded as compressed files. For
security reasons, the compressed files are available only on the Mass Download of Document Records page and not on
the scheduled process page. This is how the application creates the file:

• The zipped file name contains the scheduled process job ID.

• The ESS_Z file contains attachments, ESS_O the output, and ESS_L the log files. All the three files are available

on the Mass Download of Documents Record page and on the scheduled process page, only the output and log
files are available.

• The ESS_Z file extracts the document record details into a DocumentsOfRecord.dat file. The document record
and attachment related columns are separated with | delimiter and can be opened in a spreadsheet with the
delimiter set as | to view data in .xls format. You can use the .dat file to create document records in another
environment.

• The ESS_O file contains the consolidated output and won’t be split even if the file size exceeds 2 GB.

• The ESS_L file only contains details of document records that had errors during creation. The file doesn’t

include details about document records that were created successfully.

Note:

• For security reasons, the attachment link is only valid for 10 minutes. If you try to click the URL link after 10

minutes, you'll receive a 404 error. You need to restart the UI to regenerate the secured hyperlinks.

• The individual files within the zipped file have a default size limit of 5 MB. Attachments which

are larger than 5 MB aren't included in the download. This size limit is controlled by the
ORA_PER_DOR_FILE_DOWNLOAD_MAX_SIZE profile option which has a default value of 5 MB. You can modify
the value of this profile option to enable larger files to be included in the download.

You can also audit your mass download of document records by accessing the log data generated during the mass
download process and stored in database tables. This log data contains information such as which document records
were downloaded, which workers they were downloaded for, and which user downloaded them. Additionally, this log
data contains the following information:

• Total number of document records

• Maximum file download size

• Number of processed document records

• Name of the Zip file

• Attachment status (successful or unsuccessful)

• Error log if the mass download process fails

• Time taken to download the document records

295

Oracle Fusion Cloud Human Resources
Using Global Human Resources

The audit data is available in the following tables:

• hr_dor_mass_requests

• hr_dor_mass_request_params

• hr_dor_mass_request_lines

Chapter 11
Document Records

The data for the submitted mass download processes is available until the scheduled processes aren't purged.

Mass Download of Document Records using Filtered Lists
You can download document records for multiple people using Filtered Lists. These lists can be configured from
My Client Groups or using the Manage List of Persons link on the Mass Download of Document Records page. The
configured filtered lists can be selected in the List of Persons field on the Mass Download of Document Records page.

You can preview of the list of workers who satisfy the conditions in the Filtered List configuration on the Filtered Lists
page. Ensure that the preview displays results for workers who are to be selected on the Mass Download of Document
Records. For more information, see Create Filtered Lists in HCM Applications.

Note:

• This feature is available only on the Redwood Mass Download of Document Records page.

• You must create a Filtered List for it to be available on the Mass Download of Document Records page. Use the
Manage List of Persons link to create a list. While creating the list, make sure that you select Mass Download
Document of Records in the Subscriber field.

Related Topics

• Document Records Profile Options

• Restrict Document Types During Mass Download of Document Records

Archive and Purge Document Records

You can archive and purge document records that are no longer required for regular access.

The archiving process involves moving the document records from the HR_DOCUMENTS_OF_RECORD table to the
HR_DOCUMENTS_OF_RECORD_ARCHIVE table. After the document records are archived, they will be removed from the
HR_DOCUMENTS_OF_RECORD_ARCHIVE table based on the purge settings enabled for the document type.

Here's how the archive process works:

• For each document record, the process gets the Archive After Days and Archive Criteria Basis based on the

document type.

• For each document record, add the Archive After Days to the appropriate document record attribute selected
for the Archive Criteria Basis (Creation Date, From Date, To Date, or Issue On). If the resultant value is greater
than the system date, then the document record will be archived.

296

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 11
Document Records

• Copy all the archived document records data to the HR_DOCUMENTS_OF_RECORD_ARCHIVE table.

• The archived document records in the HR_DOCUMENTS_OF_RECORD_ARCHIVE table is marked with the

archive date.

• Delete all the copied document records data from the HR_DOCUMENTS_OF_RECORD table.

Here's how the purge process works:

• For each archived document record, the process gets the Purge After Days based on the document type.

• For each archived document record, add the Purge After Days to the archive date. If the resultant value is

greater than the system date, then the document record will be purged.

• Remove all the purged document records along with their attachments from the
HR_DOCUMENTS_OF_RECORD_ARCHIVE table and the attachment repository.

You can control access to archived document records data in OTBI reports by using the
HR_DOR_ARCH_REPORTING_LIST_V view. This view is implemented in the Workforce Management - Documents of
Record Archive Real Time subject area.

Related Topics

• Move Deleted Document Records to Archive Table

• How You Configure Archiving and Purging for Document Records

Change Publish Date for Document Records

You can modify the publish date for existing document records from the Document Records page.

Here are some points to consider when you modify the publish date:

• When you add a document record, the Publish Date field is displayed as a required field only when the Publish

Required option is set to Yes on the Create Document Type setup page.

• When you view a document record, the Publish Date field is displayed as a read-only field only if the field has a

non-null value.

• When you edit a document record, the following conditions apply:

◦ You can change the publish date only when the Publish Required option is set to Yes.
◦ You can select any date.
◦ If you change the publish date to later than the current date (including a current null value), then a

warning message is displayed which states that the document record won’t be displayed on the UI until
the changed publish date is reached. If you click OK in the message, the application will use the modified
date. However, if you click Cancel, the application reverts the modified publish date to the existing date.

•

If the publish date is in the future, the document record won't display on the user interface until that date.
However, you can view document records with a future publish date if you have the required privilege.

• You can update the publish date using REST or HCM Data Loader.

• By default, the application will not validate if the publish date is after the current date. You can enable the

seeded Validate Document Record Publish Date is After Current Date autocomplete rule if you need this
validation.

297

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 11
Document Records

Related Topics

• Delivered Rules for Document Records

Sources of Creating Document Records

You can create document records from product flows, application pages, or processes. The product sources are
integrated internally with the Document Records feature.

This table shows the products that document records are created from:

Product

Description

Absence cases

Document records created from absence cases.

Allocated checklist tasks

Document records created from allocated checklist tasks.

Employment actions

Document records created from employment actions.

Payroll object actions

Document records created from payroll object actions.

Payroll relationship actions

Document records created from payroll relationship actions.

Recruiting job submissions

Document records created from recruiting job submissions.

Recruiting offers

Document records created from recruiting offers.

Note:  Document records created using the Document Records quick action is not listed in the table. This is because
creating document records from the Document Records page is not considered as an integration.

Preview Document Records

You can preview various attachment file formats for document records without having to download them to a local
folder. This includes preview of Reference Info attachments and document record attachments.

Points to Consider

• You can preview Reference Info attachments of a document type when creating or editing document records.

• You can preview document record attachments when viewing the document record.

• An initiator can't preview a document record's recent attachments when it's pending approval.

• An approver can't preview attached files in the notification. However, they can download the attachments from

the notification.

• These file types are supported for preview: PDF, DOC, DOCX, DOCM, DOT, RTF, TXT, ODT, ODS, ODP, XLS,

XLSX, XLSM, XLSB, CSV, DAT, PNG, JPG, JPEG, BMP, TIFF, TIF, PPT, PPTX, PPTM.

298

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 11
Document Records

• Preview of attached files is supported only for the desktop application.

• Adjust your browser settings appropriately to use this feature.

Note:  You can configure most of the browsers to open PDF documents. If you don’t set this configuration
option for your browser, then the PDF document will be automatically downloaded to the local device.

Audit Access to Document Records Pages

You can monitor users who have accessed data on the Document Records and Mass Download of Document Records
pages by using the Sensitive Data Access Audit page.

Here’s how you navigate to the page on the application home page: My Client Groups > Transaction Configuration and
Audit > Sensitive Data Access Audit.

This table shows the data logged by the application in the PER_SENSITIVE_DATA_AUDIT table when the user accesses
data:

Action

Page Title

Type of Data Accessed

Start Document Records page

Document Records list page

List of all document records

View a document record

Document Records details page

Document record ID

Delete a document record

Document Records details page

Document code of system document type and
document record ID

Start Mass Download of Document Records
page

Submit request to mass download document
records

Mass Download of Document Records page

Downloaded document records

Submitted Mass Download Processes page

Submitted request ID

Start document records in plugin section

Document Records plugin section

List of all document records

View a document record in plugin section

Document Records details plugin section

Document record ID

Here are some points to consider for auditing the read access to document records:

• You can build a custom report to view the audit data by using the Workforce Management - Sensitive Data

Access Audit Real Time OTBI subject area.

• You can track the following data:

◦ Users who accessed the Document Records pages and not users who created or edited the document

record.

◦ Users who visited a page from where the attachment can be previewed or downloaded and not users

who previewed or downloaded the document record attachment.

299

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 11
Document Records

FAQs for Document Records

Why is my document type LOV blank?

Either you don't have access to any document type, or your roles do not include the following aggregate privilege: Use
REST Service - HR Document Types List of Values

What is the significance of the From and To dates of a document
record?

These are information only dates. Customers can create custom reports to identify documents which are expiring based
on the To Date and send notifications and alerts.

What is the significance of the document code for document
records?

The document code was introduced to provide a user-friendly unique identifier when multiple document records of the
same document type exist for the person.

The document code is used as one of the user keys when updating a specific document record for a person using HCM
Data Loader.

On what basis is the document code generated for a document
record?

System document type is internally stored as a concatenation of the following:

• Prefix of GLB if the document type is global, or prefix of the legislation code if the document type is specific to a

legislation.

• Document type name in upper case, with spaces replaced with an underscore ( _ ).

Document code is defaulted as a concatenation of the following:

• System Document Type.

• Time stamp in yyyy-mm-dd-hh24-mi-ss format. The time stamp includes the database date and time (24-hour

format, minutes and seconds).

For example, GLB_BIRTH_2019-06-13-09-25-10 is the document code defaulted for the Birth global document type.

300

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 11
Document Records

Is there a limit to the number of document records per worker?

There's no such limit imposed.

Is there a limit to the number of attachments or size of an
attachment for a document record?

There's no such limit imposed for number of attachments. File upload size is limited to the value specified by the
protected profile option FND_FILE_UPLOAD_MAX_SIZE. The default value is 2 GB.

What types of attachments can be uploaded using document
records?

All the regular file types can be uploaded. However, the application won’t allow uploading of executable files. It's
recommended that you enter unique file names when you upload multiple attachments.

Is there a tool for mass uploading document records and its
associated attachments?

Yes, you can use the HCM Data Loader (HDL) tool to do so. For details about loading document records using HDL, refer
to the Oracle Human Capital Management Cloud Integrating with HCM guide on Oracle Help Center.

Additionally, there is REST API support for document records. Therefore, users can build a simple extension to
programmatically load document records using APIs. For details about REST services for document records, refer to the
REST API for Oracle HCM Cloud guide on Oracle Help Center.

Which file format should I use when uploading an attachment for
document records using REST API?

Use the Base64 format to upload the attachment file.

301

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 11
Document Records

If an assignment transaction that created a document record is
deleted, what happens to the document record?

The document record is not automatically deleted when its related assignment transaction is deleted. You have to
manually delete the document record if required.

Why do I get an error when I enter the URL in upper case as an
attachment in a document record?

While creating and managing document records using Redwood pages, if you enter a URL in the Attachments section,
URL field, you must use only lower case. Upper case isn't supported for URLs.

302

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

12  Workforce Records

Overview of Workforce Records

As a part of managing workforce records, you can access the worker directory, do mass updates, and create and
manage work schedules. Let's look at the key tasks:

• Worker Directory

All workers access public information about a person in the person spotlight.

Line managers access information about their workers in the person spotlight, including person, employment,
compensation and skills and qualification details. They can also initiate manager self-service actions from here.

Workers access their own information in the Personal Information work area and perform employee self-service
actions.

• Mass Updates

Human resource (HR) specialists can update multiple employment records in a single request, using the
mass update functionality. Examples of mass update transactions include assignment change, transfer, legal
employer change, and others.

• Work Schedules

You can create work schedules, include exceptions such as public holidays, and assign different work schedules
to different workers. You can designate a work schedule as primary, which determines the worker's availability.

Directory and Person Spotlight

Person Spotlight Search

As a professional user, you can use the Person Spotlight Search that uses Oracle Search for an enhanced search
experience.

Here's what you can do with the person spotlight search:

• Use Oracle Search to search for people quickly and easily.

• Use the display name, person number, or assignment number to search for people.

• Filter the results using various assignment filters, for example, Effective as-of Date and Include Terminated

Work Relationships.

• View workers' active assignments when you open their person spotlight page.

• View the search results in a grid pattern and manage the grid columns to suit your search requirements.

• Navigate to a person's spotlight page from the search results where you can perform tasks depending on your

role.

303

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

As you type your search criteria, you can see a list of suggested results with names and assignment numbers. From the
list, you can select a person to open their person spotlight page. If you don't select from the list and press Enter, the
application performs a search.

Oracle Search performs a fuzzy search and your search results include names that closely match your search criteria.
For example, if you search for Anderson, you can see results that include similar names like Andersen. You can scroll on
the page to load more results and find more people that match your search criteria.

For a filter category, the top 10 values are displayed in the LOV. If you don’t see the value that you need, you can start
typing the value in the LOV to find it. After you apply relevant filters, click the See Results button to view the filtered
data.

The fields listed in Hide aren't shown in the results. To view a field from this list as a column, you can drag it in the
column configurator or select the checkbox next to the field.

You can use filters across categories to refine your search results. Apart from the filters displayed on the page, you can
click the filter icon to view the full list of filters. The filters also display the aggregation counts of results having the same
value.

Person Spotlight

You can view public information about a person in the person spotlight. The information that you see in a worker's
person spotlight depends on your security privileges.

You can access the person spotlight when you click the person's name on these pages:

• Directory Search Results

• My Team

• Team Talent

• Team Compensation

• Person Smart Navigation

What Line Managers Can Do
Line managers can see their workers' information in the person spotlight, and take certain actions depending on the
security configuration of their role. For example, they can do these actions:

• Promote, transfer, or terminate workers

• Manage workers' salary and compensation

• Share worker information with third parties

• Plan workers' careers

• Specify goals for their workers

• Enter feedback for workers.

What Workers Can Do
Workers can see and change their public information in the person spotlight. For example, they can do these things:

• Change their photo

304

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

• Maintain their contact information such as phone number and email address.

• Add social networks they're subscribed to

• Add their areas of interest and expertise

• Send messages to people

• Manage their document records such as visas, licenses, and awards

• Share information with others

For all other self-service actions such as changing the address, and viewing benefits, payslips, and compensation,
workers must use the Personal Information work area.

In the new My Spotlight page, you can view your employment, compensation, payslips, benefits and so on and also
navigate to the relevant pages from the Spotlight page. You can access this page from the My Spotlight quick action in
the Me tab.

What HR Specialists Can Do
HR Specialists can see their workers' information in the person spotlight, and take certain actions depending on the
security configuration of their role. For example, they can do these actions:

• Promote, transfer, or terminate workers

• Manage workers' salary and compensation

• Share worker information with third parties

• Plan workers' careers

• Specify goals for their workers

• Enter feedback for workers

What Other Users Can Do
Users such as payroll managers, payroll administrators, and matrix managers can manage their workers' information
in the person spotlight. The tasks and actions available to them depend on the security configuration of their role. For
example, they can do these actions:

• Payroll administrators can enter element entries for a worker and submit a QuickPay calculation.

• Managers including matrix managers can manage performance and development goals of the person whose

spotlight page they’re viewing. They can also create succession plans for them.

Related Topics

• People Directory

• How You Manage Your Team

• Payroll Tasks in Person Spotlight

• How You Use Matrix Management with Performance Evaluations

How You Manage Your Team

As a line manager, you can see your workers' information on the My Team Overview page of the My Team tab. You can
do certain actions for your workers depending on the security configuration of your role.

305

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Worker Information

Chapter 12
Workforce Records

• You can see worker details in the My Team area.

• You can do any action on your team as permitted by your security setting.

Positions, Requisitions, Offers, and Vacancies
You can view positions in the HCM position hierarchy along with the existing assignment manager hierarchy if position
hierarchy is enabled (in the Manage Enterprise HCM Information page). You can drill down the hierarchy and see the
incumbents for each position, which can be either assignments or requisitions.

You can also see all offers, vacancies and requisitions for the line manager hierarchy when you select the All Reports
filter.

Here's a list of what you see in the Workers, Positions, With Offer, Requisitions, and Vacancies sections.

Section

Positions

Workers

With Offers

Requisitions

Vacancies

Assignment View

Position View

N/A

Shows current workers and current and future
pending workers reporting to the manager in
focus. It doesn't show future dated workers.

Shows offers for whom the manager in focus
is the hiring manager with all proposed start
dates in Draft, Pending Approval, Extended,
 Approved, Approval Rejected, Pending Manual
Processing and Processing in Progress statuses.
It doesn't show offers in Withdrawn or Rejected
status.

Lists all positions under the position or worker
in focus. Shows incumbent workers and certain
incumbent offers. It doesn't show Future offers.

Shows current workers and current and future
pending workers reporting to any of the
incumbents of the position in focus and aren't
part of the position hierarchy. It doesn't show
future dated workers.

Shows offers for which the hiring manager can
be any of the incumbents of the position and
the offer isn't part of the position hierarchy.
Statuses shown are same as in assignment
view.

Shows requisitions with the manager in focus
as the hiring manager.

Shows requisitions with any of the incumbents
of the position as the hiring manager.

Shows vacancies with the manager in focus as
the hiring manager.

Shows vacancies under any of the incumbents
of the position.

Profile Option to Default Position View
The Position or Assignment switcher will persist automatically within a session between Overview, Talent, and
Compensation tabs. To default this to position for all users, you need to create and enable the profile option
PER_MY_TEAM_POSITION_DEFAULT.

You can change the profile value settings on the Manage Administrator Profile Values page after selecting Global
Human Resources as the Application and Workforce Directory as the User Module Name.

306

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

Team Activity Center
If you enable the Team Activity Center page, you can view all the information listed above and also perform these
actions:

• View the Team Activity Center pages of managers in your org.

• View the employment, compensation, and talent related details of all the members in your org.

• Navigate to the Spotlight pages of all employees in your org.

• Create and send short surveys to your org.

• Navigate to all the pages or applications in the My Team tab.

• Share information that's been shared with you.

People Directory

You can access the directory from your home page. You can search for and select people to view their public
information. You can see a person's organization chart, which is based on the line manager hierarchy defined in the
assignment.

What the Directory Shows
The people you see in the search results and the details you see for those people depend on your security privileges.
Anyone in the organization can access public information about people who are designated as public during security
implementation. Line managers and human resource specialists can access more detailed information about their
workers and people for whom they're responsible respectively.

You can see more information about yourself in the directory and take actions for yourself. For example, you can
maintain your talent profile, update your contacts, share your information, and participate in social connections.
If you're a manager, you can do actions for your workers such as promoting them, sharing their information, and
providing them with roles.

Directory Search
Directory search is based on keyword attributes of a person record. The priority for areas of expertise, areas of interest,
and talent skills is lower compared to the other fields in the person record. This ensures that the accurate person
records are displayed at the top of the search results.

For example, if you search for a person by keyword "Simpson," the search results first display person records containing
the word "Simpson" in the name, department, job, and so on. The person records containing the word "Simpson" in
areas of expertise, areas of interest, and talent skills are displayed lower in the order.

Related Topics

• Why do some people appear more than once in the search results?

• Why didn't my keyword search return the expected results?

• How You Share Data Access With Another Person

307

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

How You Print the Organization Chart

You can print the organization chart from the Directory in the Home page.

The organization chart shows the managerial hierarchy for the selected worker. For example, if you're an employee
without any direct reports, the organization chart shows your manager and peers and if you're a line manager, the
organization chart shows your direct reports.

When you print the organization chart, you can select the hierarchy levels you want to display and the visual orientation.
You can select which information you want to display in the printed organization chart. These settings apply to all the
employee cards in the organization chart.

You can display the following information in the organization chart:

• Job Name

• Work Email

• Work Phone Number

•

Image

• Assignment Name

• Position Name

• Location Country and Code

Finding Colleagues Using the Directory

Find Colleagues Using the Directory
Oracle HCM Cloud enables you to access information about any employee from your organization using the Directory.
The information that you see depends on your security access.

Watch video

Use the following procedure to find your colleagues using the Directory and view their information.

Search for Colleagues
Use the directory to search for colleagues

In the Search Results, click Eric Ross.

1. On the Home page, click the Directory link.
2. Click in the Search field and enter eric ross.
3.
4. Click the Back icon.
5. Click the Search field.
6. Click the Advanced Search link.
7. Click Show Filters.
8. Click the Department field and enter Sales West US.
9.

In the Search Results, click Sales West US (Supremo).

308

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

In the Name field, enter aaron.
In the Search Results, scroll down and highlight Aaron Moore.

10.
11.
12. Click the Back icon

Print Organization Chart
Use the organization chart to see your peers

1. Click My Organization Chart to print your organization chart for quick reference.
2. Click the Mitch Bloom link
3. Click Print.
4. Click the Levels to Display list and select 2 to print organization chart up to 2 levels.
5. Click the File Format list and select or leave the selection as SVG.
6. Click the Fields to Display list and select Photo to print..
7. Click the Group Last Level list and select or leave the selection as Group Last Level.
8. Click Preview to see a preview of the chart before printing it.
9.
10. Click the Back icon.
11. Click the Show Filters link. You can also use the filters to see your manager's extended organization, including

In the Orientation section, select Vertical.

12.

the various managers, dotted line reports, and contingent workers.
In the Manager Type section, click to select Line Manager, Project Manager, Regional Manager, Mentor/
Mentee , and Resource Manager.
In the Worker Type section, select Contingent Worker and Employee.

13.
14. Scroll down and highlight the dotted-line report Kristine Doyle and the contingent workers, James Gardner.

View Public Info
Use the Public Info page to view your own details.

1. Click the Curtis Ferry link to look at your Public Info page
2.
3.
4.

In the Public Message section, click Add.
In the Start Date field, click the Calendar icon, select today, and click OK.
In the Notification field, enter In the office M/W/F, working from home T/Th. If you need immediate
assistance and you're unable to reach me contact my manager, Jack Taylor.

5. Scroll down and highlight Favorite Links.
6. Click to expand Representatives.
7. Click the Gloria Daze link
8. Click the Actions list and select Provide Feedback.
9. Click Add.
10. Click the Who can see my feedback list and select Everyone.
11.

In the What do you want to say? field, enter Gloria has been amazing and endlessly patient, thanks so
much!

12. Click Save and then click the Back icon.
13. Click My Public Info.
14. Click the Authors list to see feedback given to you from specific people.
15. Click to close the Authors list.
16. Click the Time period list to see feedback for a specific time period
17. Click to close the Time period list.

Related Topics

• Person-Record Keyword Searches

309

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

How You Create and Display Vacancies

You create and display vacancies either from the My Team page or the Vacancies quick action on My Client Groups tab.
You can access the organization chart from the quick actions on the Me tab.

To Create a Vacancy

• Select the employee card in the organization chart or the employee name on the My Team page under whom

you want to create the vacancy.

• Click the More Information icon in the employee card in the organization chart or the row actions menu for the

selected employee on the My Team page, and select Vacancies..
As an HR specialist, you can click the Vacancies quick action on the My Client Groups tab.

• Click Add to create a vacancy.

On the Vacancies page, select the position. The position-related fields (Job, Department, and Location) automatically
inherit the values from the selected position. The number of openings isn't automatically updated against a hire; you
must manually update it whenever the vacancy is filled. You typically use the Requisition field if you're using a third-
party recruiting application and want to enter a requisition number for the vacancy; This is an optional field and is used
for information purposes only.

You can update and remove any vacancies You can associate an existing vacancy with yourself by editing the vacancy
and changing the manager name to yourself.

To Associate a Vacancy With a Requisition

You can either add requisition details for a vacancy if you've already created a requisition or create it at the time of
creating a vacancy. You can also choose to add the requisition details later.

• Click the vacancy that you want to convert and click the Edit button.

• Add the requisition details.

You can enter these details for a job requisition: Primary Location, Openings, Hiring Manager, and Recruiter. When you
create a job requisition for a vacancy, the job requisition appears in the organization chart and the vacancy is removed.
The position information in the vacancy is lost. However, you can update the job requisition in Oracle Recruiting Cloud
to make any further changes.

Person-Record Keyword Searches

The application searches for keywords in these attributes: department, person number, job name and code, position
name and code, person name, primary email, primary phone, work location, competencies, language skills, licenses and
certifications, school education, awards and honors, memberships, interest areas, and areas of expertise.

Access to Restricted Information
Line managers can access their workers' restricted information such as competencies, language skills, licenses and
certifications, school education, awards and honors, and affiliations. Restricted information is included in search results
when the searcher is a line manager. For example, if a line manager searches for a language skill and a match is found

310

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

in any direct or indirect reports, that information appears in the search results. However, if the match is found in public
information such as areas of expertise, it appears in the search results for any user.

Keyword Indexing
Keywords are indexed values, which means that they're copied from person records and organized in a keywords table
for fast retrieval. Most changes to person records are copied to ensure that the source and indexed values don't differ.
Your enterprise can also run a keyword-refresh process to update all keywords and fix any discrepancies. Depending on
when this process was last run, some recent changes to person records may not appear in search results.

Name and Keyword Search
The person search uses a person's full name instead of the first name or last name. The full name definition may vary
for each country. For example, the full name definition for India may be First Name Middle Name Last Name, while the
full name definition for Canada may be First Name Known As Last Name Suffix. You control the definition of the full
name using the Manage Person Name Formats task in the Setup and Maintenance work area.

There's an implied OR condition between the search criteria when you use keyword search. When you use the name
search, there's an implied AND condition between the search criteria For example, when you enter Chris Harper in the
Name field, all person records that have both Chris and Harper in the full name are shown in the search results. Here are
some examples:

You enter...

Harper Chris

Chris Harper

Chris%

Search Results

•

Jenner, Chris

• Harper, Smith

• Chris, Ray

• Harper, Liam

• Harper, Chris

• Harper, Christopher

•

Jenner, Chris

• Harper, Smith

• Chris, Ray

• Harper, Liam

• Harper, Chris

• Harper, Christopher

•

Jenner, Chris

• Black, Chris

• Blake, Christopher

• Simpson, Christy

• Harper, Chris

• Harper, Christopher

• Christ Johnson

Chris

•

Jenner, Chris

311

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

You enter...

Search Results

"Chris Harper"

• Black, Chris

• Harper, Chris

• Harper, Chris

Chris and Harper

• Harper, Chris

"Chris" "Harper"

• Harper, Chris

Date-Effective Search
In the person search UI, you can enter an effective as-of date. When date-effective values such as work location are
copied to the keywords table, their history isn't copied: only the latest change is stored in the keywords table. Therefore,
if you enter both a keyword value and an effective as-of date, the search results may not be as expected. Here's an
example:

• You change the work location of assignment 12345 from Headquarters to Regional Office on 27 January, 2011.

• The changed work location is copied automatically to the keywords table on 27 January, 2011.

• You search for a person on 1 February, 2011 using the keyword Headquarters and the effective as-of date 10

January, 2011.

Although the work location on 10 January, 2011 was Headquarters, assignment 12345 doesn't appear in the search
results because the work location stored in the keywords table at the time of the search is Regional Office.

How You Optimize Person Search Keywords

The Oracle Text index in the PER_KEYWORDS table is utilized for person searches in My Client Groups, and the
Directory. This index may become fragmented over a period of time and may cause a delay in displaying search results.

Why You Run the Process
You run the Optimize Person Search Keywords Index process to identify the fragmented indexes and help improve the
overall search performance. To launch this process, use the Navigator > Tools > Scheduled Processes > Schedule New
Process button in the search results table.

Note:  You must run the Update Person Search Keywords process first and then the Optimize Person Search Keywords
process. You cant schedule both processes simultaneously. If you schedule them at the same time, the second
process will wait for the first process to complete before it starts.

When to Run the Process
You must run the Optimize Person Search Keywords Index process daily at times of low activity with the options, Full
mode and the appropriate maximum time. The default time is 180 minutes. Although, if the process is run consistently
over time it may take about 10 to 30 minutes only. You can decide the frequency of running the process based on the

312

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

size of your customer base, system usage, database usage, data loaders used, index fragmentation, and schedule of the
Update Person Search Keywords process.

Best Practices for Optimizing Person Search Keywords
Here are some best practices for optimizing person search keywords.

Do's

• Schedule the Optimize Person Search Keywords Index process to run at least once a week during off peak

hours with all parameters null, to prevent the keywords index from being fragmented.

•

It’s recommended that you don’t schedule both these processes to run simultaneously:

◦ Update Person Search Keywords
◦ Optimize Person Search Keywords Index

Even if you do, the second process waits for the first process to complete before it starts.

• Let’s say a large volume of person records are updated every day, and the Update Person Search Keywords
process is scheduled to run daily. Then you need to schedule the Optimize Person Search Keywords Index
process with all parameters as null to run immediately after the Update Person Search Keywords process.

Don'ts
Don’t schedule the Optimize Person Search Keywords Index process to run more frequently than once daily. That’s
because the keywords index isn’t expected to be fragmented heavily in such a short period of time.

How You Update Person Search Keywords

Several attributes of person, employment, and profile records are used as person-search keywords. Keyword values
are copied automatically from the originating records to the PER_KEYWORDS table, where they're indexed to improve
search performance.

Process to Update Person Keywords
An event is raised when the value of a keyword attribute changes, for example, if a person acquires a language skill or
a different phone number. In response, services run a process to update the relevant attributes for the person in the
PER_KEYWORDS table. Therefore most changes are made in PER_KEYWORDS immediately and automatically. When
you create a new person record, keyword values for that person are copied automatically to the PER_KEYWORDS table.

Why You Run the Process
Although most changes to the PER_KEYWORDS table are automatic, you need to run the Update Person Search
Keywords process regularly because of these reasons:

• The automatic process doesn't apply future-dated changes to the PER_KEYWORDS table.

• The process ensures that all changes are copied to the PER_KEYWORDS table, despite any temporary failures of

the automatic process.

313

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

When You Don’t Need to Run the Process
Let's say a person’s data is modified from anywhere in the Fusion Apps UI, except from Work Structures or CRM
Resource Information. Then the keywords are updated directly and this job isn’t required.

When You Run the Process
Here are some of the scenarios where you run the Update Person Search Keywords process:

• For a specific Batch ID

◦ If post-processing is disabled during HDL load of Workers data, then run the “HCM Data Loader Worker

Post processing” job using the specific UCM content ID.

• For a specific Person

◦ Select person name in the Name parameter.
◦ For a specific person, the job can be executed as and when required.
◦ Estimated Execution Time: approximately 30 seconds to 1 minute.

• For only Delta population

◦ To update keywords for the changed workers and to create keywords for new workers loaded, submit the

job with only After Batch Load = Y.

◦ Use this option only if the number of person records changed is less than 20,000.
◦ Estimated Execution Time: approximately 20 minutes for every 20,000 records.

• For all the Persons in the system

◦ Submit a request with all parameters as null to recreate keywords for all persons in the system.
◦ Use this option only if a new language is installed or if the number of person records changed is more

than 20,000.

How to Schedule the Process
You can run the Update Person Search Keywords process manually or schedule it to run at regular intervals (for
example, weekly at a specified time).

The likely volume and frequency of changes to person records in your enterprise will determine how often you run the
process:

•

•

If the volume and frequency are high, you need to schedule the process to run frequently.

If the volume and frequency are low, running the process once a month is recommended.

Running the Update Person Search Keywords process refreshes the whole PER_KEYWORDS table. Therefore, you must
run the process at times of low activity to avoid performance issues.

Best Practices for Updating Person Search Keywords
Here are some best practices for updating person search keywords.

Do’s

• Schedule the process at least once a day during off peak hours to run with parameter After Batch Load = Y to

process any changed worker data (delta population) and keep keywords up-to-date.

314

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

• When loading workers by using HDL, enable post-processing to process keywords for the workers that were just

loaded.

If the number of worker records loaded exceeds 20,000, then disable post-processing and manually run the job
with all parameters as null, which will process the entire worker population.

•

If you’re running 'Refresh Manager Hierarchy' daily, then set the 'Updated Within the Last N Days' parameter
value as 1 for incremental updates. This prevents the delta population size from getting larger than 20,000,
which would require the job to be run for the entire person population.

Don’ts

• Don’t schedule the process to run at frequent intervals with all parameters as null.

◦ Running the job with all parameters as null processes all person records in the system, which is

unnecessary and can potentially leave the index in an inconsistent state.

◦ You must run the job manually with all parameters as null only if the number of worker records for whom

keywords should be updated exceeds 20,000.

• Don’t run or schedule the process with Batch ID values as -100 and -200. These are unsupported values and

can cause issues with keyword search.

Related Topics

• Person-Record Keyword Searches

Worklist Transactions

Transactions may undergo an approval process before being applied to the database. A transaction typically passes
through a chain of approvers, and remains in pending status until the final approver approves it. You can access all your
transactions in the Worklist.

Pending Transactions
In your worklist, you can see transactions having these statuses:

•

Initiated by you

• Approved but pending because one or more approvers in the approval chain haven't approved yet

• Returned to the previous approver

• Reviewed by you as a notification recipient

This list also includes transactions routed to any approval groups that you belong to, even though you may not have
approved the transactions. You can edit a pending transaction and do the same actions as those available in your
worklist or notification summary. You can approve, reject, or return a transaction to the previous approver. You can also
withdraw a transaction after initiating it. For example, you may want to withdraw a new hire transaction after initiating it,
because of budget constraints.

Other Transactions
You can view transactions that you saved for later, and those that aren't pending with you anymore, such as your
approved and rejected transactions. You can suspend transactions that you have initiated or approved. A suspended

315

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

transaction remains inactive until you resume the transaction. However, the suspend and resume actions are only
available to users having the role BPMWorkflowSuspend.

FAQs for Directory

Why can't I see the roles that I want to request for myself?
Before you can request a role:

• The role must appear in a role mapping where it's Self-requestable.

• At least one of your assignments must match all conditions, such as job and location, in the role mapping.

Typically, an application administrator or IT security manager creates and maintains role mappings.

Why didn't my keyword search return the expected results?
Your keyword search didn't return the expected results because of any of these reasons.

• Keywords are copied to the keywords table only when the keyword-refresh process is run in some cases.

Depending on how frequently you run this process, some recent changes to person records may not appear in
keyword-search results.

• Keyword searches return a result only if you have access to the information in which the keyword is found. For
example, if your keyword search is procurement and a match occurs in a person's competencies, the person
appears in the search results only if you have security access to the person's competencies.

• When you enter both a keyword and an effective as-of date, the search results include only those assignments

for which the keyword value in the keywords table matches the keyword value on the effective as-of date.

Why do some people appear more than once in the search results?
Each search result relates to an assignment. Any person who has multiple assignments can appear more than once in
the search results.

If the search criteria include assignment attributes, such as department or job, only those assignments that satisfy all
the search criteria appear in the search results.

What's a matrix chart?
A matrix chart displays dotted line relationships. The chart displays employees by manager type (for example, project
manager, line manager, and functional manager) in a tabular format. It lists the employees as rows and manager types
as columns.

What's the difference between rejecting and withdrawing an approval transaction?
The effect of these actions is the same: the transaction is not applied to the database.

The difference is in who can do which action. Only the initiator of a transaction can withdraw the transaction. Only the
current approver in the approval chain can reject the transaction.

316

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

Why was my saved transaction deleted?
This maybe because an identical transaction initiated for the person by another user was applied to the database.

What's a calendar event message?
A message that appears on the calendars of people covered by a calendar event.

For example, a message about a Spanish public holiday could appear on the calendars of people working in Spain. It
lets people working in other countries know why people in Spain are unavailable on that date. You create calendar event
messages using the Planned Schedule task in the Time Management work area.

Why didn't a calendar event message appear on the calendars of everyone in an
organization or location?
If you use work schedules and a calendar event covers a person, you need to include the calendar event as a schedule
exception.

Otherwise, even though the person belongs to the organization or location covered by the calendar event, no calendar
event message appears on their calendar. You add the calendar event exception to their primary work schedule or
schedule assignment.

Connections

Overview of Connections

Use Connections to search for colleagues across functions and departments and find information about them. The
application enables you to build work relationships, engage, and collaborate better with your coworkers.

With Connections, you can:

• Search and find coworkers quickly. Browse and filter search results easily using Oracle Search.

• View a coworker’s profile for information like work location and time zone to schedule meetings.

• Add information about yourself in your profile for your coworkers to know and collaborate better with you.

• Use Favorites to mark people that you interact with often, or to build a network of people to help achieve your

career objectives.

• See people’s assignments, interests, and expertise to discover what you have in common with them. If a person
has multiple assignments, you’ll see multiple search results and view the assignment details in their profile.

• View a coworker’s organization chart to understand their role and how they relate within their organization

structure.

• Provide feedback to your coworkers and view feedback given to them by others depending on your role.

317

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

Search for People in Connections

You can access the Connections application from a quick action in the Me tab. On the Connections page, use a person’s
name or email to search.

As you type your search criteria, you see an autosuggested list of results that you can select from to open a person's
profile. If you don't see the person you’re searching for in this list, you can press Enter and see another list of profiles
that match your search criteria.

You can search using various person-related fields, but Connections uses people’s names for a primary search and
other fields are secondary.

You can also click the Advanced Search icon on the page to view filters across categories. You can select multiple values
to refine your search. When you click a filter, a list of values available for that filter along with the number of people
that match that filter are displayed in a list. For a filter, the top 10 values with more number of results are displayed, but
you can search for other values. Select a value from the list and apply it to your search for more targeted results. The
available filters include Country, City, Tags, Title, Location, Job, Department, and Position.

After you search for a person and press Enter, you’ll see some results that match your search criteria. To see more
results, click Show All Employees and you can see all results that match your search criteria.

Connections performs a fuzzy search so that people whose names closely match your search criteria are also displayed.
For example, if you search for person named ‘Anderson’, you can see results with names like ‘Andersen’. This means
you can still find the person you’re looking for if you don’t know how their name is spelled or if you type a name
incorrectly.

After you visit a person’s profile from the main page, you can search for other people from that profile. You need not go
back to the Connections page to search for other people.

What's a Connections Profile

Your Connections profile includes information about yourself in different sections. Some information is initially
available, and you can add more details about yourself. Here’s what your profile includes and the details you can add to
it.

• Header: Header contains your name, contact information, business title, work location, work phone number,

your Slack and Zoom details. You can add a display picture and links to your social media profiles like LinkedIn,
Twitter, and Facebook. You can use the use the icon next to the phone numbers and email addresses to copy
and then paste them elsewhere easily.

• Organization: Organization displays your reporting hierarchy, your reports if you have any, number of reports,

job, department, business unit, and Areas of Responsibility representatives.

• About Me: You can describe yourself and your work here. You can add your areas of interest, expertise,

and work experience. You can also add tags that indicate your work, interests, expertise, and anything that
represents you. Your colleagues can use tags to search for people in Connections. You can also use artificial
intelligence to generate content about yourself using keywords that describe your job and any other details.

• Favorites: If you're using Oracle Grow, you can mark connections as favorites from their profiles to create a

network of people. On the Oracle Grow page, you’ll see them all in the Connections region. You can also find
others who are considered Popular in your role. You need to have the Access Career Growth by Worker privilege
added to your role to add favorite connections.

318

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

• Skills and Development: You can see this panel on your profile if you’ve purchased and implemented Dynamic

Skills. For more information, see the Dynamic Skills documentation.

• Experience: This section contains your tenure with the company and your enterprise service history.

• Links: You can add links of your interest in this section.

• What Others Think: You can view the feedback you've received, thank the person that sent you feedback,

and provide feedback for your colleagues. The person who sent you feedback can select who can view their
feedback to you.

All information displayed on the profile is considered public information, except for the What Others Think section,
which is displayed based on the visibility option the feedback provider has selected.

Related Topics

• Understanding Skills Center

• Resources and Actions for Your Career Growth

Organization Chart

The organization chart provides a dynamic view depending on whose assignment you select.

Navigation up and down the organization chart is achieved by selecting the manager above or direct report below the
selected person assignment. The selected assignment either up or down the org chart becomes the new focus and is
displayed as the largest box. Then, select the focused assignment to access that worker’s profile.

The Organization chart is available from the profile and it is comprised of a number of views:

• Directs: lists the direct reports of the selected person's assignment and it includes direct reports and dotted
line reports. You can select a direct report to move down the hierarchy, or click the manager to move up the
hierarchy.

• All Reports: lists all the workers, contingent workers and non-workers who report up through the selected

person either in a line manager relationship or a dotted line or matrix relationship. You can view the groups of
persons by their worker type (employee, contingent or non-worker). Select anyone’s assignment to make them
the new focus of the organization chart.

• Departments: lists all the departments that everyone in All Reports belong to. Selecting a department lists
the workers in that department who report to the selected person. You can return to the selected person
assignment by selecting their name above the department.

• Locations: lists all the work locations that everyone in All Reports belong to. You can view workers at that
location who report to the selected person by clicking the location and then return to that selected person
assignment by clicking their name above the location.

While viewing the Manager hierarchy, you can search for the next person by using the search box on the top of the page
above the hierarchy diagram.

When to Use Connections or Directory

Connections is intended for use by every worker, but doesn't replace the actions available in the current Directory for
HR personnel. For example, HR personnel need to use the Directory to create a public message or initiate employment
actions.

319

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

Personal data entered in Connections is shown and editable in Directory as well; users can maintain shared data in both
places.

Find Colleagues Using Connections

Use Connections to find and view your coworkers’ profiles and update your own profile. You can view their work
location, organization chart, contact information, and their assignments. Depending on the information they added to
their profile, you can view their interests, work experience, and areas of expertise. On their profile, you can also add your
feedback for them.

Watch video

Search for a Colleague and Add your Feedback
In this example, you’re an employee using Connections to search for a coworker and add your feedback for them.

1. On the Home page, click Connections.
In the search field, enter Elizabeth.
2.

You can see autosuggestions as you’re typing.
3. You can select one of the results or press Enter.

You can see a list of all the people that are named Elizabeth.

4. Refine your search further by adding filters.

a. Click the Advanced Search icon.
b. Click the Location filter.

When you click in the Location search field, you can see all the locations that has employees named
Elizabeth and how many worker assignments each location has.

c. Select the location that you want.
d. For more filters, click More.
e. Click the Title filter.
f. Click in the Title search field and select Directory of HR Service Desk.
g. From the search results, select Elizabeth Mavery.

On her profile, you can see Elizabeth’s title, contact info, location, organizational and personal
information. If she has added tags, interests, skills to her profile, you can see that information. Depending
on the feedback settings, you can also see the feedback others have given Elizabeth.

5. Add your feedback for Elizabeth.

In the What Others Think section, click the Provide Feedback icon.

a.
b. Click the Who can see this field and select Visible to managers and Elizabeth Mavery.
c.
d. Click Save.

In the What do you want to say field, enter your feedback. For example, Great job closing the quarter!

320

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

Get Familiar with Your Organization
You can search for anyone from any profile page or any org chart in Connections. You can use org charts to explore the
organization and find the people reporting to a manager including dotted line reports. In this example, you’re exploring
your organization using org charts.

In Connections, search for an employee, for example, Elizabeth Mavery.

1.
2. Click the chevron icon next to her manager, Robert Jackman.

You can see all the people that report to Robert Jackman.

3. Click Robert Jackman's profile.
4. On his profile page, in the Reports section, click the Org Chart button.

You can see Robert Jackman’s manager, Robert Jackman’s direct reports, and the people who report to Robert
Jackman’s direct reports, if there are any.

5. Optionally, you can search for anyone using the search icon on the org chart page.
6. On the org chart, click Elizabeth Mavery’s profile.

You can to see the people she reports to, including dotted line managers.

7. On the org chart, click the Directs tab to see the people that report to Elizabeth directly.
8. Click the All Reports tab to see all the people that report to Elizabeth through her direct reports.
9. Click the Departments tab to view the different departments Elizabeth’s reports are in.
10. Click a department to view all the people that report to Elizabeth in that department.
11. Click the Locations tab to view the different locations all her reports are in.
12. Click a location to view all the people that report to Elizabeth in that location.

Update Your Profile
On your profile, you can add or edit your picture, contact information, links to your social networking profiles, Linkedin,
Slack, and Zoom. You can add information about yourself that your coworkers in your organization can see when they
search for you.

1.
2.

In Connections, search for your profile.
In the About Me section, click the Edit icon to update your profile.

You can add information about yourself, your interests, expertise, and tags using which people can search for
you.

3. Click Save.

Activity Centers

Overview of Activity Centers

Activity Centers provide employees and managers with a landing page that that can use to perform their daily
tasks easily with minimum navigation to other areas of the application. They provide a personalized view that helps
employees and managers prioritize the tasks in their roles. There are two activity centers:

• My Activity Center: Employees can use My Activity Center to easily access and manage their tasks related to
employment, compensation, skills, learning and so on. Recent updates that require employees’ attention are
displayed as cards on the page. For example, if your passport is expiring soon, a card is displayed with the

321

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

relevant details. You can use the card to navigate to the page where you can enter your renewed passport
details.

• Team Activity Center: Managers can use Team Activity Center to access all the information related to their
employees. You can create surveys, communicate messages to the whole team, and perform any team or
individual actions in one go. Depending on the setup, you can view organization and position hierarchies. You
can also view the Team Activity Center pages of other managers if they delegate their teams to you.

My Activity Center

Implement My Activity Center to enable employees stay on top their daily tasks, skills, and learning needs. To navigate
to your My Activity Center page, click Me > My Activity Center quick action or the app.

Here’s what you can do using My Activity Center:

• Use the analytic cards that highlight tasks pending or information that needs your attention to navigate to

the relevant pages where you can complete the tasks. You can hide the cards that you don’t need using Visual
Builder Studio.

• Personalize the quick actions available on the page to access applications that you use the most. You can pin
the quick actions that you want to see on the page and access the rest from the Quick actions pane. You can
remove and control access of the quick actions using the Structure tool. However, doing this will change the
access throughout the application..

• Use the timeline or list view to view important events that occurred in the last one year and events that are

going to happen in the coming 6 months. You can also navigate to the respective applications areas using these
clickable events.

Your manager can also view your My Activity Center page which is the Person Activity Center page. This is the Person
Activity Center page for them.

Team Activity Center

Implement Team Activity Center to enable line managers view, access, and manage all their employee-related
information. To navigate to your Team Activity Center page, click My Team > Team Activity Center quick action or the
app.

Here’s what you can do as a manager using Team Activity Center:

•

If you have multiple assignments, manage all your teams at one place by selecting the relevant assignment.

• View team-related numbers using the analytics cards. The Workers and Retention cards show the numbers of
your entire org and the Achieve and Dynamic skills cards show the numbers of the team directly reporting to
you. You can personalize the cards that are displayed on your page using Visual Builder Studio.

• View Team Activity Center pages of managers reporting to you using the Switch Team option. Team Activity

Center pages are available only for managers and not workers.

• View and manage Employment, Compensation, and talent related tasks of your employees using different tabs

on the page.

• Use the Workers, Positions, Requisitions, and Offers views to manage different team-related tasks based on
your organizational setup. For example, you need to implement Oracle Recruiting to view information in the
Requisitions view. The default view is Workers that you can change using Visual Builder Studio.

322

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

• Announce news or important information to your team using HCM Communicate or Journeys. You need to

implement Journeys and HCM Communicate to use the Communication section.

• Access the apps in the My Team tab from the Applications pane.

You can view the following analytic cards in the Team Activity Center.

Analytic Card

Workers

View

Description

N Directs, N Total

Retention

X%

Achieve

X of Y goals completed

Dynamic Skills

X of Y core skills achieved

Count of the number of line manager worker
assignments directly reporting to the manager,
 and the total number reporting to the manager
in the hierarchy.

This is 100% minus the annualized headcount
turnover (termination headcount for the year /
average of headcount a year ago and current
headcount).

Count of completed performance goals among
the manager's direct reports (including matrix)
for the "current review period" out of the total
assigned

Y=Count of the distinct core skills assigned to
line manager directs

X=Count of the distinct core skills assigned to
line manager directs that are achieved

Mass Updates

Mass Updates

You can update multiple employment records at the same time. For example, you can transfer all workers in a
department to another department as part of a company reorganization. You go to My Client Groups > Mass Updates to
do a mass update.

Assignment Changes
You can do a mass assignment change to update multiple assignments at once. The type of assignment changes
include transfer, promotion, location change, position change, and others.

Assignments with Future Changes
Assignments you select in the mass update process can include future dated changes or changes that are effective
on the same date as the mass update. You can include or exclude assignments with such future dated changes in the
mass update. If you include assignments with future changes, you need to manually modify those records that have an
effective date of change later than the mass update date to resolve any conflicts. For those assignments with changes
that coincide with the date of the mass assignment change, the previous assignment changes are retained and the
mass update is applied as the last change.

323

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Related Topics

• Create a Mass Transfer

• Guidelines for Using Desktop Integrated Excel Workbooks

Chapter 12
Workforce Records

How You Make Mass Assignment Changes Using a Spreadsheet

If you need to update many assignments at once, you can download the data from the Verification page into a
spreadsheet and make the changes offline.

You need to do these things before downloading the data to a spreadsheet:

•

Install the Oracle ADF 11g Desktop Integration desktop client

• Enable the Trust access to the VBA project object setting in Microsoft Excel

If you added any attributes on the Changes page using personalization, they will be hidden when you download the
data into a spreadsheet. You can display these attributes using Unhide feature in Microsoft Excel. You can check in and
verify the data in the spreadsheet multiple times while making revisions. After the final check in, you need to go to the
Review page to submit the changes.

Note:  The mass update transaction gets automatically saved when you go to the Verification page. The current
changes overwrite the earlier mass update in this process and you can't restore the earlier changes even if you cancel
the current transaction

Related Topics

• Guidelines for Using Desktop Integrated Excel Workbooks

Mass Update Statuses

After you do a mass update you can monitor the status of the update on the Manage Mass Updates page. Let's see
what each status means:

Status

Initiated

What it Means

Mass update process has started. The status is automatically set to Initiated when you create a mass
update.

Awaiting user verification

Mass update changes are awaiting verification.

Awaiting user verification - exported

You exported the mass update rows to a spreadsheet.

Awaiting user verification - imported

You made changes to the spreadsheet and checked it in, it's awaiting verification.

Completed

Mass update is complete.

324

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

Status

What it Means

Create a Mass Transfer

You want to transfer all workers from the Applications Support department to the Global Support department, within
the same legal employer. Since there are many workers, you want to do a mass transfer.

Let's look at the steps to update the key values for this mass transfer.

Create a Mass Transfer

1. On the Manage Mass Updates page, click Create to open the Create Mass Assignment Change: Basic Details

page and complete these details.

Field

Name

Action

Value

Reorganization September 2011

Transfer

Assignments with Future Changes

Show errors and exclude assignments

2. Click Next.

Select the Population

1. On the Create Mass Assignment Change: Population page, click Select and Add to open the Select and Add:

Persons page.

2. Click Advanced to open the Advanced Search page.
3. Select the Applications Support department and click Search.
4. Select all the rows in the search results.
5. Click OK to display the search results in the Selected Persons region.
6. Click Next.

Enter the Changes

1. On the Create Mass Assignment Change: Changes page, enter these values.

Field

Value

Business Unit

Global Support

Department

Global Applications Support

325

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

Field

Value

Building

New Pleasanton Campus

2. Click Next.

Verify the Changes

1. On the Create Mass Assignment Change: Verification page, in the Proposed Changes column, delete the

Building value New Pleasanton Campus for those workers who work from home.

2. Click Verify Changes and review any errors and warnings.
3. Click Next.
4. On the Create Mass Assignment Change: Review page, review the current and proposed values.
5. Click Submit.

FAQs for Mass Updates

Can I make changes in the mass update after submitting it?
No, but you can save the mass update for later, and edit or delete the mass update any time before submitting it. You
can manage mass updates in the Mass Updates work area.

What are the worker and assignment category tags in a mass update?
When you select a worker or assignment category in the Job Details section of the Create Mass Assignment Change
page, you can see tags displayed next to the fields. These tags specify the legislations associated with the selected
category and have the following meaning:

• Tags with + prefixes: Indicate that the selected category only applies to the legislations with the + prefix.

For example, Tags +FR,+IE,+NZ indicate that the selected category only applies to France, Ireland, and New
Zealand.

• Tags with - prefixes: Indicate that the selected category applies to all legislations except the legislations with

the - prefix. For example, Tags -FR,-IE,-BR indicate that the selected category applies to all legislations except
France, Ireland, and Brazil.

• Tags with + and - prefixes: If the tags contain a combination of + and - prefixes, the first prefix is considered

and the rest is ignored. For example, Tags +FR,-IE,-BR indicate that the selected category only applies to France,
Ireland, and Brazil.

326

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

Work Schedules

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

327

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

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

328

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

Departments 1 and 3 don't have primary schedules, so the primary schedule at the enterprise level applies to everyone,
with one exception. A person in department 3 has a schedule for their primary assignment. That primary assignment
schedule applies instead of the enterprise-level schedule. Department 2 has a primary schedule, and it applies to
everyone in that department.

The calendar events and resource exceptions that exist in the primary work schedule affect everyone's schedules,
regardless of level. Any absences they report during the selected time period also affect the individual's schedule.

Standard Working Hours
The person's primary assignment includes their standard working hours. Schedules built with these hours also show
applicable calendar events and absences.

Exception Options in Work Schedules

When you create a work schedule, you can include exceptions, such as public holidays or training sessions. You then use
these exceptions to identify people's availability to work.

329

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 12
Workforce Records

Calendar Event
A calendar event is an exception for a single event on 1 or more consecutive days, such as a public holiday or training
event.

Calendar Event Category
A calendar event category is an exception for all calendar events that make up the event category. For example, the
events New Year's Day, Good Friday, and Easter Monday make up the category UK Public Holidays.

Resource Exception
A resource exception is an exception for everyone assigned the work schedule. For example, everyone assigned the
Night Shift schedule get scheduled to attend a training event, so they aren't available to do their regular work.

People can see the Work period exceptions for themselves and their team on the Time and Absences work area
calendar. They need to select either or both of the Employment schedule and My schedule display options. They can't
see any off period, or nonwork, exceptions.

Related Topics

• How do I change exceptions in individuals' work schedules?

FAQs for Work Schedules

What's a primary work schedule?
The schedule used to identify an individual's work availability.

For example, you assign two schedules for different time periods to someone's primary work assignment. So that those
schedules identify the person's work availability for those time periods, you need to set both schedules to Primary. If
you assign only a single work schedule, that schedule automatically identifies the person's work availability.

You manage work schedules using the Work Schedule Assignment task in the Person Management work area.

How do I change exceptions in individuals' work schedules?
You can change how the exceptions affect that person's work availability when you assign a schedule to someone using
the Work Schedule Assignment page.

For example, you added a calendar event as an exception that affects everyone. But, a designated person needs to
remain available to handle critical customer queries. So, you change the person's work availability for that exception.

330

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 13
Workforce Deployment Analysis

13  Workforce Deployment Analysis

Generate Workforce Deployment Intelligence

Workforce Modeling

Workforce Modeling provides managers and human resource (HR) specialists with the ability to plan, model, and
execute workforce changes using a graphical tool. You base your model on either the manager hierarchy or the position
hierarchy.

The hierarchy starts with the top manager or position and includes assignments, positions, vacancies and requisitions.
They report to the top manager or position, either directly or indirectly.

You can perform the following actions in the model:

• Promote

• Transfer

• Terminate

• Change manager

• Change location

• Add, change, inactivate, or delete positions

• Change position incumbents

• Create, change, or delete vacancies

• Create and edit Oracle Recruiting Cloud requisitions (dependent on security settings)

You can move people with or without direct reports either by dragging and dropping or using the table view and
selecting a new manager. You can create vacancies in the model, and on final approval they're added to the database.
Review the impact of your planned changes using the analytics. The application uses the modeled changes to create
effective dated transactions when the model is approved. Vacancies are not effective dated, therefore vacancy changes
or new vacancies appear when the model is approved.

Perform position changes by dragging and dropping on the graphical hierarchy. For example, drag and drop a position
including its incumbents on the hierarchy and then move an incumbent to a different position. Use the position
synchronization and position defaulting features.

For the position hierarchy, you can perform the following actions for positions:

• Create

• Edit

•

Inactivate or delete

• Undo inactivate

• Undo delete

• Move positions in the model

331

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 13
Workforce Deployment Analysis

• Convert a vacancy into an open position

• Create and edit requisitions

Security and Access
Line managers and HR specialists have access to Workforce Modeling. You can access all the Workforce Modeling
features if you are either an author or the top manager of a model. To access the model as the top manager, the author
of the model can give you access in the model properties. HR representatives can edit the model, and other approvers
can open and view the model.

The following rules define who the default approvers are:

•

•

•

If all the modeled changes occur within the top manager os position's organization, then the approvers are the
author's HR Representative, the top manager's manager and one level of manager approval above.

In addition to the above rule, the manager who has authority to approve all the changes and one level above,
are the approvers. These approvers are in addition to the author's HR Representative and two levels above the
top manager.

If there are any changes outside the top manager or position's hierarchy, then a further rule requires the
manager who has authority to approve all the changes and the manager one level above to approve the model.

Any role with position related privileges, for example, create, edit, or delete positions, can perform position related
actions in Workforce Modeling. For HR specialists, this feature is ready to use automatically.

Statuses
The following table describes the Workforce Modeling statuses.

Status

Draft

Pending

Rejected

Returned

Completed

Description

A model is in the Draft status:

• Until it's submitted

• Once it's edited

•

•

If an approver edits a model during approval

If the author withdraws a pending model

A model is in the Pending status after it's submitted from the Draft, Rejected, or Returned modes.

A model is in the Rejected status if an approver rejects it.

A model is in the Returned status if an approver requests more information.

A model is in the Completed status after it's approved by all approvers. At that point, transactions are
created and assignments are updated with effective dated changes.

Effects of Reorganizing
Once the newly created workforce model is approved, the relevant assignments are updated using the model effective
date. Currently, notifications aren't issued for this. Role provisioning security occurs automatically if it's set up

332

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 13
Workforce Deployment Analysis

accordingly. For example, if the line manager role is enabled for autoprovisioning, then a user who becomes a manager
is given the line manager role automatically.

Note:  Vacancy changes appear on the date the model is approved, irrespective of the model effective date because
vacancies are not effective dated in HCM Cloud.

Related Topics

• Workforce Modeling Analytics

• Considerations for Terminating Workers in Workforce Modeling

Security, Access, and Approvals in Workforce Modeling

Line managers and HR specialists have access to Workforce Modeling. You can access all the Workforce Modeling
features if you're either an author or the top manager of a model.

To access the model as a top manager, the author of the model can give you access in the model properties.HR
representatives can edit the model, and other approvers can open and view the model.

You need to assign the Workforce Model Plan HR Specialist Duty to any predefined HR specialist roles you've copied and
edited if you want them to see Workforce Modeling under My Client Groups.

Approvals
The HR specialist configures the approval rules relevant to Workforce Modeling.

The following rules define who the default approvers are:

•

•

If all the modeled changes occur within the top manager or position's organization, then the approvers are the
author's HR representative, the top manager's manager and one level of manager approval above.

If there are any changes outside the top manager or position's hierarchy, then a further rule requires the
manager who has authority to approve all the changes and the manager one level above to approve the model.
This rule is only used when at least one change is outside the top manager's or top position's hierarchy.

Any role with position related privileges, for example, create, edit, or delete positions, can perform position related
actions in Workforce Modeling. For HR specialists, this feature is ready to use automatically.

If you'd prefer not to go through an approval process, then the HR specialist can enable the Bypass Approvals option in
the Transaction Console. With this option, any model you create won't go through the approval process and submitting
the model automatically commits the planned changes to the application.

Workforce Modeling Analytics

The Workforce Modeling analytics appear on the Workforce Models and Model pages for the modeled changes as of
the model effective date. Use the analytics to view the impact of proposed changes to headcount, salary costs, count of
alerts and changes.

333

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 13
Workforce Deployment Analysis

Once a model is complete, the analytics are frozen as of the date of the final approval. The Projected Worker Cost and
Projected Headcount analytics don't include information for any worker assignments that the model doesn't have the
security to see.

The following table describes the Workforce Modeling analytics.

Analytic

Changes

Description

Shows the number of worker assignments with changes.

For example, if you move an assignment to a new manager and then to another manager and then
make a job change, then all these actions count as one change.

Projected Worker Cost

Displays the change in the total cost for the top manager as a result of modeling. The analytic on the
Workforce Models page only displays the cost change due to modeling. The analytic on the Model
page displays the cost due to modeling and the change due to modeling.

Cost is based on the annualized salary and changes are only included if you have security access to the
assignment.

For example, you can move a worker to report to you and update their salary. However, if you don't
have security access to view the worker's salary, then any change you make to that worker's pay in the
workforce model isn't included in the analytic.

Projected Headcount

Displays the change in the headcount for the top manager as a result of modeling based on the
workforce measurement value of headcount.

Alerts

Displays the number of outstanding alerts for the model.

The two types of alerts are:

• Validation Error: occurs when the Oracle Fusion assignments are updated on final approval and

issues exist

• Assignment Change: occurs if an assignment has changed in the live application since modeling

started and that change has not yet been resolved using the synchronization dialog

Workforce Modeling Actions

You can access Workforce Modeling actions from various locations, including the Model page and the Holding area.

Here's a list of where you can access the actions:

• Model page

• Worker assignment node

• Vacancy node

• Workers region in the table view

• Terminated workers region in the table view

• Vacancies region in the table view

• Holding area

334

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 13
Workforce Deployment Analysis

• Position node

• Positions region in the table view

• Requisitions node

• Requisitions region in the table view

This table lists and describes the actions available on the Model page:

Action

Where Available

Description

Edit Worker Assignment

Worker Assignment Node, Chart and Holding
area

Move or edit the modeled attributes for a
worker assignment. If you change a worker's
manager, then the worker moves to that
manager's hierarchy.

Create Vacancy

Worker Assignment Node, Chart and Holding
area

Create a vacancy node as a placeholder for an
open headcount.

Edit Vacancy

Vacancy Node, Chart and Holding area

Edit the vacancy.

Delete Vacancy

Vacancy Node, Chart and Holding area

Edit Assignment

Model page

Delete the selected vacancy node. You must
confirm the deletion to remove the node from
modeling.

Note:
You cannot delete vacancies imported from
Oracle Taleo Recruiting Cloud Service.

Select a worker assignment node in the
chart, holding area, or the table and edit the
assignment.

Undo and Redo

Model page

Select this option to undo and redo a change.

Edit Model Properties

Model page

Edit the model details.

Synchronize

Model page

Terminate

Worker Assignment Node

Cancel Termination

Terminated Worker Assignment Node

Run the synchronization process to update
any information that has changed in the live
application.

Select a termination action, reason and
notification date.

Select this option to cancel the termination
within the model.

Export to Excel

Terminated Workers, Workers, and Vacancies, in
the table view

Select this option to open and save the
information in a spreadsheet.

335

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 13
Workforce Deployment Analysis

This table lists and describes the actions available on the Model page for positions:

Action

Where Available

Description

Create Child Position

Model page, Position node

Edit Position

Model page, Position node

Inactivate Position

Model page, Position node

Undo Inactivate Position

Model page, Position node

Delete Position

Model page, Position node

Undo Delete Position

Model page, Position node

Convert to Position

Model page, Vacancy node

Available for existing positions only. Enter basic
position information. The application creates
the new position in the position hierarchy and
that position reports to the position from which
the action initiated.

Edit the position and if required, the parent
position details. If you edit a parent position,
 then you also have the option to move or leave
the children with the parent position.

Available for positions that do not have active
or suspended incumbents as of the effective
date or a date in the future.

For positions that have been inactivated in the
model.

You can delete a position if it does not have
incumbents in the past, present, or in the
future.

Select this option to reverse the deletion and all
the associated changes. Available for positions
that have been deleted in the model only.

Edit the vacancy and review the default values
for the position. This option is available only if
the parent of the vacancy is an incumbent of a
position in the hierarchy.

Related Topics

• Workforce Modeling

• Considerations for Terminating Workers in Workforce Modeling

Considerations for Terminating Workers in Workforce Modeling

You can use workforce modeling to create or edit a model to terminate workers. You can use existing models to
terminate workers, and these models can also include other planned updates, such as promotions and transfers.

Any workers you terminate will display as grey in the model. The terminations affect the analytics which you can use to
review the impact of your planned terminations. The termination changes are only applied to the transactional system
when the model is approved.

336

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 13
Workforce Deployment Analysis

Canceling Terminations
Cancel a termination, if, for example, you realize that the planned termination could harm the business or you
terminated a worker as part of a planned restructure, which has been canceled. Canceling a termination also affects the
analytics.

Analyzing Terminations
The impact of the termination or canceled termination in terms of headcount and salary cost is calculated and
displayed, providing you with immediate feedback on your modeled changes.

Terminating Managers with Subordinates
If you terminate a manager with subordinates, then you can decide to terminate them also. If you cancel this
termination, then you must cancel the termination of each subordinate separately. If you decide not to terminate the
subordinates, then the subordinates are assigned to the terminated manager's manager. If you cancel the termination,
then you must manually move each reassigned subordinate back to their original manager.

Related Topics

• Workforce Modeling

How Synchronization Works in Workforce Modeling

Workforce Modeling runs a synchronization process that checks the attributes in the live transactional application
against the attributes in the model, and makes some automatic updates, and other recommendations.

The synchronization process ensures the assignment and vacancy information in Workforce Modeling are up to date
with any changes made in the live transactional application.

The synchronization process runs automatically when you:

• Open the model for editing.

• Open the Review page.

• Open the Approval page.

You can also run the process manually from the Actions menu on the Model page.

Synchronization Rules
When you open a saved model, the synchronization process runs automatically to review all application changes that
occur after the date the model was last updated, and on or before the model effective date. If there are any changes in
the live application, for example, one of the workers in the model has been transferred and another worker has been
terminated, then the application synchronizes each attribute using the following rules:

•

•

If the live application has changed but the model hasn't, then automatically update the model.

If the same attribute has changed in the model and in the live application, and if the live application changes
are irreversible, then automatically update the model with the live application change. Irreversible changes
include any moves in or out of the hierarchy, such as, hires, transfers, and terminations.

337

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 13
Workforce Deployment Analysis

•

If the same attribute has changed in the model and in the live application, and you can update the live
application change, then the application recommends the modeled value. If this scenario occurs, then the
application recommends the model changes for all attribute updates.

Synchronization Alerts
When you reopen a saved model, and the synchronization process finds changes in the live transactional application
and in the model, then you can review the automatic updates and recommendations in the Alerts page. If you confirm
the changes, the application updates the analytics and the information in the hierarchy.

Related Topics

• Workforce Modeling

FAQs for Generate Workforce Deployment Intelligence

What happens if I move or edit a worker assignment in Workforce Modeling?
If you move a worker assignment in the organization chart, the Manager and Department fields in the Edit Assignment
dialog box default to the new manager and the new manager's department.

All the other fields show their most recent values as of the model effective date. The current values are secured to
ensure that people with no access to a worker's grade and salary can't view them.

Why can't I inactivate a position in Workforce Modeling?
Because the position you want to inactivate either has an active or suspended incumbent as of the effective date or in
the future.

To inactivate a position with incumbents, you can either move incumbents out of the position or terminate the
incumbents and then inactivate the position. If you implement a model with inactivated positions, then this position will
not appear in the HCM position hierarchy.

How can I convert a vacancy into a position?
Open the vacancy to edit, and review the default values for the position. The option to convert a vacancy into a position
is available only if the parent of the vacancy is an incumbent of a position hierarchy.

The position headcount defaults from the number of openings, therefore, if the vacancy has unlimited openings, then
the position headcount defaults to 1. You create the new position and it reports to the parent position.

FAQs for Evaluate Workforce Deployment Performance

When do changes to my organization hierarchy appear?

The hierarchy is based on completed transactions. Incomplete transactions, such as transfers or new hires awaiting
approval, don't appear.

338

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 13
Workforce Deployment Analysis

However, terminations that are withheld from publication until a specified date are evident in your organization
hierarchy from the termination date rather than the publication date.

Where do promotion-readiness values come from?

A person's readiness for promotion is based on the time since the person's last promotion relative to the average time
between promotions for people in the same job or position and grade.

For example, if the average time between promotions for people in the same job and grade is 5 years, a promotion
appears due if the time since a person's last promotion is within range of 5 years. If the gap is outside this range,
the promotion appears as either not due or overdue. Additional factors, such as performance and length of service,
determine whether you decide to promote a person whose promotion appears due or overdue.

Why do some people appear more than once in my organization
hierarchy?

Each entry in the hierarchy is an assignment. If a person has more than one assignment, and each assignment reports
to a manager in the hierarchy, then the hierarchy contains an entry for each of the person's assignments.

Can I terminate a manager's whole organization in Workforce
Modeling?

Yes, when terminating a manager you can select an option to also terminate his or her subordinates. The default
behavior is not to terminate a manager's subordinates, but to automatically reassign them to the terminated manager's
manager.

Related Topics

• Considerations for Terminating Workers in Workforce Modeling

Can I update a worker's salary in Workforce Modeling?

Yes. Edit the assignment and select the Promotion or Location Change action.

You can update a worker's salary information if the worker has a current salary record, their assignment does not have a
grade ladder and if their salary basis does not use components or payroll rates.

339

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 13
Workforce Deployment Analysis

Can I terminate a worker outside the top manager's hierarchy in
Workforce Modeling?

You can search for workers, place them in the holding area, and then terminate them. Predefined approval rules ensure
that the appropriate manager approves such changes.

For example, if you terminate a worker who does not directly report to you, then the first manager in the hierarchy who
you both report to, must approve the termination. The approver's manager must also approve the change.

Related Topics

• Considerations for Terminating Workers in Workforce Modeling

Can I cancel a termination in Workforce Modeling?

Yes you can cancel a termination. For example, if you terminate a worker in the model and then cancel that termination,
there is no change in the model.

You can select to cancel the termination within the model without affecting the live transactional system.

Related Topics

• Workforce Modeling

• Considerations for Terminating Workers in Workforce Modeling

340

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 14
HR Help Desk Service Requests Classic

14  HR Help Desk Service Requests Classic

HR Help Desk Classic Documentation

The classic HR Help Desk application is used to create and submit HR Help Desk service requests (HRHD SRs). Oracle
introduced Redwood Help Desk in release R13.22.07 (21C).

If you are implementing or using the classic version of HR Help Desk, the documentation is located in the appendixes of
the new Redwood Help Desk guides.

Related Topics
•

Implementing Redwood Help Desk

• Using Redwood Help Desk

341

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 14
HR Help Desk Service Requests Classic

342

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 15
Troubleshooting

15  Troubleshooting

Reverse a Termination

To reverse a termination, follow these steps:

1. On the Home page, click the My Client Groups tab (if you're an HR specialist).

Note:  Click the My Team tab if you're a line manager.

2. Click Show More under Quick Actions.
3. Click either the Termination or Terminate Employment quick action in the Employment area.

Note:  The Termination quick action is for version 2 termination and Terminate Employment quick action is
for version 3 termination.

4. Search and select the person for whom you want to reverse the termination.
5. On the View Termination page, click Reverse.
6. Select Reverse Termination for the action name.
7. Select the reason for reversing the termination.
8. Click Submit.

Things to Keep in Mind

•

If approvals are enabled, the line manager will need to approve the termination reversal.

• After the termination is reversed:

◦ Work relationships and assignments are restored to their previous statuses and the person is listed back

as a worker on the line manager's My Team page.

◦ Previous employee roles are provisioned again.
◦ User accounts are restored.

Note:  If the person isn't listed as a worker, you need to run the Refresh Manager Hierarchy process
from the Scheduled Processes area. For more information, refer to The Manager Hierarchy: How It's
Maintained topic in Chapter 10 in the Implementing Global Human Resources guide on the Oracle Help
Center.

How do I unlock a worker’s employment record?

A worker’s employment record is locked when there are transactions pending approval. In this example, you unlock a
worker's employment record to update his manager information.

Watch video

343

Chapter 15
Troubleshooting

Oracle Fusion Cloud Human Resources
Using Global Human Resources

This process involves these changes:

• Finding the transaction ID using Conflicting Transaction Details diagnostic.

• Searching for the pending transaction in the Transaction Console.

• Completing the transaction.

Let's look at the steps to unlock a worker's employment record.

Find Pending Approval Transaction ID

1. On your home page, click the Settings and Actions icon.
2. Click Run Diagnostics Tests in the Troubleshooting area.
3. Enter Conflicting Transaction Details in the Test Name field and click Search.
4.
5. Click the Click to Supply or Edit Input Parameters icon under the Input Status column in the Choose Tests to

In the search results section, select the test name check box and click Add to Run.

Run and Supply Inputs section.
6.
In the Input Parameters dialog box, enter the person number in the Person Number field and click OK.
7. Provide a unique run name in the Run Name box in the Choose Tests to Run and Supply Inputs section.
8. Click Run.
9. Click OK in the Test Run Submitted dialog box.
10. Click the Display Latest Test Run Status Information icon in the Diagnostic Test Run Status section and

expand the folder.

11. Click the View Test Results icon.
12. On the Conflicting Transaction Details page, click the hyperlink.
13. Click the report name in the Recent Downloads dialog box.
14. Open the report and make a note of the Transaction ID and Submitted On date.

Search Pending Transaction in Transaction Console

1. On your home page, click the Navigator> Tools > Transaction Console.
2. On the Transaction Manager: Transactions page, click the Settings icon.
3. Select Configure for Self.
4. On the Personalize Saved Search: Default Criteria menu, scroll down and select the Transaction ID check box.
5. Click Save.
6.
7. Click the Search icon.
8. Click the Transactions From drop down list.

In the Transaction ID field, enter the transaction ID you noted earlier.

By default, the summary page is set to search for and display the last 3 months’ transactions. If the submitted date of
the transaction you are searching for is more than 3 months, then use the Transactions From drop down menu and
select the appropriate value.

Complete the Transaction
Transactions in Failed, Draft, or In Progress status can be terminated. If a transaction is pending for approval, you can
get it approved. In this example, the transaction is in a failed state, hence, we will terminate it.

1. Select the check box in the transaction row.

344

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 15
Troubleshooting

2. Click the Actions menu and select Terminate Process.
3. Click Done in the Status of Terminate Process Action dialog box.

The pending transaction will be terminated and the employment record of the worker is released for further
employment related updates. You can now update the manager information for the worker.

345

Oracle Fusion Cloud Human Resources
Using Global Human Resources

Chapter 15
Troubleshooting

346

