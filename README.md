# cs455-project-1-solved
**TO GET THIS SOLUTION VISIT:** [CS455 Project 1 Solved](https://www.ankitcodinghub.com/product/cs455-project-1-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;96326&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS455 Project 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
The objectives of Project 1 are:

<ul>
<li>Continue practicing using AWS services. In this project you will combine many of the concepts we have looked at to do a simple cloud application (S3, Lambda, RDS, XML, and JSON).</li>
<li>Learn how S3 Event Notifications work. S3 can publish events to many destinations (including a Lambda function). Read this article about S3 Event Notifications. We also did a module where we configured a Lambda with an S3 trigger (see Module 12).</li>
<li>Learn how to interact with a relational database running in the cloud.</li>
<li>Learn how several cloud services can be used together.
Scenario

In the spirit of current events, we will do a scenario related to COVID vaccination. You will devise a system where a central authority (e.g., the Center for Disease Control and Prevention (CDC)) is tasked with keeping track of the vaccination drive taking place across the US. The collected information is useful to monitor areas of the country that are making progress vs. others that are not, adjust policies accordingly, and keep the public informed about the vaccination progress (e.g., by publishing daily numbers in major newspapers).

Let’s start with a few assumptions:
</li>
</ul>
<ol>
<li>The CDC is the central authority that aggregates and keeps track of vaccination data. It does
that by collecting daily information that covers the following:

<ol>
<li>Total number of people who have received their first shot.</li>
<li>Total number of people who have received their second shot and are considered fully
vaccinated.
</li>
</ol>
</li>
<li>There are thousands of sites across the US administering vaccines (pharmacies, clinics, hospitals, etc.). These sites do not have systems in place to directly communicate with the CDC computer systems. All sites, however, have Internet connections and can upload data to the cloud.</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
3. The CDC created an AWS S3 bucket and requested all sites to upload at the end of each day a summary of the vaccines administered in each site. The CDC gave sites the option of uploading their data in XML or JSON format. Examples of the expected format are shown in Figure 1.

XML:

JSON:

Figure 1: XML and JSON data examples the CDC is expecting from vaccination sites.

<ul>
<li>day, month, year: date of vaccination.</li>
<li>id: a unique ID the CDC gives each participating site.</li>
<li>name, zipCode: site name and its location zip code.</li>
<li>brand: vaccine brand name (assume only two allowed: Pfizer and Moderna).</li>
<li>total, firstShot, secondShot: total number of people who got a shot at the site in a
given day, number that it is their first shot, number that it is their second shot (firstShot + secondShot should be equal to total).
</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
4. Note that not every site administer both vaccine brands. Some sites offer Pfizer only, some offer Moderna only, and some offer both. Therefore, the XML does not necessarily have to have two &lt;brand&gt; elements under &lt;vaccines&gt;. Same applies to the JSON equivalent: the vaccines array may contain only one item.

System Design

Your task is to implement a cloud application for the CDC that works like this:

<ul>
<li>At the end of each day, vaccination sites upload their daily summary (in XML or JSON format) to an S3 bucket that the CDC created. Each site uses a simple program (UploadData.exe) to upload the XML or JSON file. The UploadData.exe executable is called from the command line of any computer connected to the Internet. It takes two arguments: The first argument is the path of the file to upload. The second argument is a string (xml or json) that indicates whether the file is XML or JSON. Here are two examples of how UploadData.exe may be called (text in blue is the first argument, and text in red is the second argument):
prompt&gt; UploadData.exe C:\Temp\daily.xml xml

prompt&gt; UploadData.exe C:\vaccination\data\today.json json

UploadData.exe uploads the file passed in the first argument to the S3 bucket and sets with the uploaded object a tag named “type” with a value that indicates if the file is XML or JSON (“xml” or “json”).
</li>
<li>An AWS Lambda function is listening on file arrival to the S3 bucket (using an S3 event notification mechanism). When a file is uploaded to the bucket, S3 triggers the invocation of the Lambda function. Lambda can then read the file content and the “type” tag, parse the file content, extract vaccination data, and enter the data into a PostgreSQL relational database.</li>
<li>The PostgreSQL relational database schema should have two tables: Sites and Data. Since a given site uploads daily data, you should have a one-to-many relationship between the “Sites” and “Data” tables (use a primary-foreign key combination).</li>
</ul>
o TheSitestableshouldhavethefollowingfields:

</div>
</div>
<div class="layoutArea">
<div class="column">
SiteID: Name: ZipCode:

</div>
<div class="column">
The site ID (an integer – can be used as the primary key of this table). A string that represents the site name.

A string that represents the site zip code.

</div>
</div>
<div class="layoutArea">
<div class="column">
o TheDatatableshouldhavethefollowingfields:

SiteID: A foreign key (also of type integer) to the Sites’ table SiteID primary key.

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
Date: FirstShot: SecondShot:

</div>
<div class="column">
The data of vaccination

An integer that represents the first shot. An integer that represents the second shot.

</div>
</div>
<div class="layoutArea">
<div class="column">
Note that the SiteID and Date (together) form the primary key of the Data table. That is, the combination of SiteID/Date should be unique.

No need to keep track of vaccine brand. So there is no field for it.

• On any given day, it is possible that a site makes mistakes and need to upload a corrected XML or JSON file. Your system should allow this; in this case a row in the Data table should get UPDATED (not INSERTED since you already have a row for the SiteID/Date combination).

Figure 2 is a diagram that summarizes the workflow of this system.

</div>
</div>
<div class="layoutArea">
<div class="column">
Figure 2: System workflow

Files to Use for Testing

8 files were provided to you for testing. See folder TestFiles.

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
Implementation Hints

<ol>
<li>In order to query the S3 objects tags you need privileges beyond what the AWSLambdaExecute policy gives you. To do that, create a custom role and use that role for your Lambda function.
<ol>
<li>Go to the IAM service. Click on Roles. Then click the Create role button.</li>
<li>Under Choose a use case, select Lambda then click the Next: Permissions button.</li>
<li>Search for the following two policies and check each:
i. AWSLambdaExecute ii. AmazonS3FullAccess
</li>
<li>Click the Next:Tags button, then the Next:Review button.</li>
<li>Give your role a name (e.g., CDCVaccinationSystemRole).</li>
<li>Click the Create role button.
This creates a role named CDCVaccinationSystemRole with two policies attached to it: AWSLambdaExecute and AmazonS3FullAccess.
</li>
</ol>
Now when you use the publish Lambda function wizard in Visual Studio, choose role CDCVaccinationSystemRole for your function (you do this in the second screen – this new role that you created in your account should appear in the dropdown):
</li>
<li>You need to read the tag “type” associated with the S3 file that was uploaded to S3. Its value will tell you whether the file is of type XML or JSON. You can read the tags associated with an S3 object using a combination of the following classes/methods:
<pre>      GetObjectTaggingRequest
      GetObjectTaggingResponse
      GetObjectTaggingAsync
</pre>
This documentation article shows you an example how it is done (expand “Uso dos AWS SDKs” then click the .NET tab). Sorry, I wasn’t able to find the English version of this doc page.
</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
3. To query the PostgreSQL database from the Lambda function, use the Npgsql library. You need to add this package to your Lambda function in Visual Studio.

Cheating Policy

This is an individual project and you should present your own code and work. If I notice unusual resemblance between the codes of two students, both students will get a 0 (the student who gave help and the student who received help).

What to Submit?

There are no files to submit.

I will grade your project by having you give me a quick demo that shows your system is working start to end. I will also observe your UploadData and AWS Lambda code and ask you questions about the overall system. I can do that one-on-one via a 5-minutes Teams meeting that I will do with each student.

<ol>
<li>&nbsp;</li>
</ol>
</div>
</div>
</div>
