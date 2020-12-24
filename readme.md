Changing the human task status to failed and seeting the error path
===================================================================

This exmaple provides inforamtion about, how to make human task status as failed and diverting the process flow to error path.

In this example we are using signal to set the process variables which will be used to decide the error path of process flow.

Post deploying the kJar follow the the below steps.

  * Step 1: Create a process instance for [human-signal](src/main/resources/com/temenos/human_signal/human-signal.bpmn)
  * Step 2: Claim and work on human task. 
  * Step 3: Start button will make the human task status to 'inprogress'
  * Step 4: Signal process case instance with signal name (i.e. errorSignal) and "failed" as data to signal. 
   ![project modules1](images/Signal.png)
  * Step 5: Observe the process varables. Now we can observe the process varaible status value as failed.
   ![project modules1](images/pv.png)
  * Step 6: Use the below REST Api to change the status of the human task to "failed"
   ![project modules1](images/rest.png)
  * Step 7: Observe the process diagram.
   ![project modules1](images/pd.png)
