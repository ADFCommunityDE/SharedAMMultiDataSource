# SharedAMMultiDataSource
Demo-Application showing shared-application usage for lov's when working with different data sources

### How-To start
* pull whole repo
* activate the HR schema on your oracle db and create a second schema (for example salary)
* create a salary_steps table for the second schema and fill some data for it (you might want to use the files in the DatabaseModel project)
* Run HRService Application Module
* After querying data from Employees, you should get a table or view not found exception
* To fix, change scope for SharedModule instance in Model.jpx to application
* retry run, now you should see a working select lookup
