# discourse_script
Given a date range, returns the reports of those days in a JSON format. 

The reports are accessed by reverse engineering the undocumented Discourse API methods. 

It requries three parameters in the header: "Accept", "Api-key", "Api-username". 

The request should be sent to {HOST}/admin/reports/bulk?reports%5B{REPORT_NAME}%5D%5Bfacets%5D%5B%5D=prev_period&reports%5B{REPORT_NAME}%5D%5Bstart_date%5D={START_DATE}&reports%5B{REPORT_NAME}%5D%5Bend_date%5D={END_DATE}. 

The report name can be found by clicking on the report and looking in the URL.

# How to run
* Clone to repository.
* Navigate to main directory.
* Run main.py with "python3 main.py" or "python main.py".
