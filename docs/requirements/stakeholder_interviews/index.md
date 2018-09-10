# Stakeholder Interviews

## Database Requirements Interview

### Current System

1. Can you describe the current system?
    1. Version of Access (Can we create a mock)
2. How is the data entered?
3. How do you interact with the data?
4. Who else interacts with the data?
    1. Is anyone else directly accessing the database?
5. How much data is stored?
6. How long is data persisted? (Does this contain everything?)
7. What is the schema of the current database? (Tables)

### Reports Generated

1. What kinds of reports do you generate?
    1. Are these SQL queries? Can we see them?
2. How are reports presented after generation? (Are you just sending out numbers?)
3. How are reports generated?
4. How long does a report take to generate?

### New System

1. If you could have any other report(s) generated what would they look like?
2. How do you see yourself interacting with the new system?

### Final Questions

1. Is there anything else that we should have covered that we missed?
2. Is there anyone else we should be talking to?

## Database Requirements Interview Notes

Date: 10/09/2018

### Current System

#### Data

- LCStats
  - Takes the raw LCData table and replaces numeric representations with human readable values
  - This table is used for most of the queries
  - Refer to the Access Database for details
- Subjects should not change frequently (just added ENGD or engineering design)
  - If this does occur currently a new number designation would be added
- A few non-obvious Subject Types
  - 16 is a catch all Misc. mainly used to record entries where the information is mostly unreadable (18 is basically the same)
  - 17 is for workshops
    - Percopo perspectives
    - Car maintenance
- James maintains the Access Database currently on his own
- Databases are separated by years and go back as far as 2006
- 1 hour corresponds to 1 visit (i.e. 3 hours is 3 visits)

#### Forms

- Data Entry
  - Kelly uses this to input the data from the sign in sheets
  - Note that names of students and professors use auto-fill
- Professor Info
  - Adds new professors to the system
  - Used infrequently
- Student Info 
  - Adds new students manually to the system, mostly for transfer students
  - At the beginning of each year James gets a spreadsheet from the Registrar's office of all the student information which he reformats and imports into Access


#### Reports

- Service Report
  - gives the number of visits for each service by subject
  - this is used by both James and Susan
  - most used report of the 3
- Student Report
  - Shows the same information as Service Report but for a specified student
  - Used infrequently to check if a certain student has been using the Learning Center
- NTP (Notes to Professors)
  - Kelly uses this report
  - At the end of each week (Friday) professors are sent a list of their students who used the learning center that week
- Review Session Sheet
  - uses the data from the Registrar Dump to create the fancy sign in sheets

### New System

#### Querying

- Query across years?
  - Not frequent
  - The current solution is to copy multiple years into a single spread sheet and deal with it there
  - Recently checked multiple years to look for a trend in what week students typically use the Learning Center most
  - maybe in the spreadsheet export we can select a range of years
- Custom Queries
  - James occasionally makes queries that he forgets to delete
  - To support these ad-hoc queries we'll need to be able to export the data to csv's
- New queries/reports
  - frequency queries
- problem description
  - Mainly useful for tutors to possibly determine what they need to review before helping students
  - Possible querying would include key-word search (Need to talk to some returning tutors)
  - Might require some adjustment of our original access plan for the role "tutor"

#### Dashboards

- Public
  - Visits per classroom/study room by subject
- Private
  - Breakdowns for each tutor
    - evaluation data
    - number and duration of visits
    - shortest and longest visit per tutor
    - student that has the most visits for that tutor
  - Maybe even a tutor leader-board

#### Miscellaneous

- should add location in data collection