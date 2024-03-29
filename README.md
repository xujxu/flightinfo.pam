# flightinfo.pam
The power automate package to generate the flight info


## Step to import this zip file to create your own power automate flow

1. Download this zip file from this git repo: 
2. login in https://make.powerautomate.com/ with your Power BI account
3. Navigate to "My flow" in the left navigating pane
   ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/e07aecec-386d-4cc0-9926-2980424b957a)
4. Select the "Import Package (Legacy)" after clicking the "Import" button
   ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/74a6fc0d-c005-4acd-9605-95b26ddec41e)
5. Select the zip file you downloaded from step#1, and upload it
   ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/78c32a63-47cc-4c84-bc9f-d52f9cb61ba9)
6. Update it as "Create New"
   ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/e457ab0f-2cf9-4d2d-955d-8f7058882483)
   ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/439e8e6b-8e07-4978-b901-507e90004835)
8. And then you can import it to your own flow
   ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/d7d733ba-93bf-478c-8225-76a95f6f8464)
9. Navigate back to your "My flow", and select the new flow to Turn on it
   ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/367b52da-8c6a-48ec-86d7-d6e7a254043d)
10. Click your flow and open it. And select Edit button to modify your flow for adding the Event Hub action so that the data can flow into our Eventstream.
   ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/fcf8a889-6475-45b8-9576-aacd0fc884c9)
11. Click the "+ New step" to add the Event Hub action step
    ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/567820c1-d989-4fb1-b772-8f6f7a8db413)
12. Type 'event hub' and select the Event hub
    ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/8b01482e-b172-42cc-a293-aef19c3e14b2)
13. Select 'Send event'
    ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/0ce63a7f-ca30-4b94-ac96-9e70cfa3580f)
14. Configure the Event Hub with connection string which can be obtained from Eventstream Custom App EH tab
    ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/8553f27c-3f66-4de5-89a3-b2edb040781c)
    ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/d3912137-fbc2-4a53-ad75-0858f4501230)
15. After the connection is set up, complete the full configuration below
    ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/b4ba05ea-0b5e-4a46-b1aa-f5f57b407d22)
    Event hub name can be copied from below place in your Eventstream:
    ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/535d1c4b-26bc-43ee-b6b7-8badebf0375c)
    Configure the content as the output from previous step
    ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/43b916d3-a0d8-4200-9e9c-90de8b59abe4)
16. Save it and do the test. It should run well.
17. If everything runs well, go to the first step of "Recurrence" to configure it as long-running. If it runs into error, call for help from us.
    ![image](https://github.com/xujxu/flightinfo.pam/assets/68268054/a82712da-dc42-4d64-bd54-30822b714476)




 
