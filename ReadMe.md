# camunda-common
This project is used for all the framework components that is specific to camunda.

#### Retry with Configurable Interval
The configurable retry interval configuration is shown in below diagram,
![1](retry-decisions.png)

With the above retry interval "5,10,15,20,25", the job will be retried for 5 times with specified delay interval (comma separated values).
#### Note:-
1) Number of retries is equal to number of comma separated values.( e.g if interval 5,10,15,20,25 then number of retries will be 5, For 1st retry the delay interval will be 5, then for 2nd retry the delay interval will 	be 10 and so on etc)<br/>
2) No need to make entry in the num_of_retries column, when configure the interval column with comma separated values. 

# camunda-camel
This project is the bridge between camunda and camel

 
