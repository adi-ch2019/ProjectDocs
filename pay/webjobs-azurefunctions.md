 ### Background and Preqs

Azure WebJobs to run scripts or programs as background processes in the context of an App Service.

At present we are going for the supported format i.e .ps

WebJobs can be to be run on a schedule via CRON expressions.

#### Role of Azure Functions
Pricing calculator for Azure Functions indicate we have 400,000 GB/s of execution and 1,000,000 executions are free as well.

This is all on F1 App Service Plan.

### Workflow to be sort out

* From Azure
WEBHOOK URL
USERNAME
PASSWORD 
to be set in Azure with approciate RG and Service accounts for Dev 

* Create Function App
Choose timer

* (Either choose Powershell/Batch or C# - TBD)

for run.csx code to be replaced follow the template

```
using System;

public static void Run(TimerInfo myTimer, TraceWriter log)
{
    string userName = "$yourWebJobUserName";
    string password = "vepyr4Jk8*******************";
    string webJobName = "yourWebJobName";
    string webhookURL = "https://yourUrl.scm.azurewebsites.net/api/triggeredwebjobs/blogWebJob01/run";
    
    var unEncodedString = String.Format($"{userName}:{password}");
    var encodedString = Convert.ToBase64String(System.Text.Encoding.ASCII.GetBytes(unEncodedString));

    System.Net.WebRequest request = System.Net.WebRequest.Create(webhookURL);
    request.Method = "POST";
    request.ContentLength = 0;     
    request.Headers["Authorization"] = "Basic " + encodedString;
    System.Net.WebResponse response = request.GetResponse();  

    log.Info($"timer trigger function executed at: {DateTime.Now}");  // To Be replaced for 20:30 to 3:30 
}
```

Replacing the userName, password, webJobName and webHookURL respectively.

Schedule Job using CRON expression.