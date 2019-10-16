# IATI XML Dataset
**IATI** is an open data sharing standard and technical framework created by the humanitarian community to make aid activity information transparent and accessible to machine applications, including new artificial intelligent applications and popular digital assistants like Alexa, Siri and Cortana. IATI is managed by the [International Aid Transparency Initiative](http://reference.iatistandard.org/).
### How IATI Works
Organizations report activities in compliance with IATI by converting detailed information about their activities, transactions and results into machine readable XML code using an assortment of over 200 standardized fields ([elements and attributes](http://reference.iatistandard.org/203/activity-standard/summary-table/)) to structure the information. Then organizations publish the XML files on their own web servers (or via third party applications like [AidStream](https://aidstream.org/) and send file metadata, including the URL addresses of the files, to the IATI Registry which makes the entire body of information easily accessible, comparable and aggregatable

Here's an example [IATI XML file](http://iati.oxfam.org.uk/xml/oxfamgb-jo.xml) published by Oxfam GB. The single file contains information on twelve separate activities that the organization either has, is or is planning to carry out in Jordan.
## Dataset Download
![Organization Data Folders](https://github.com/Humanitarian-AI/IATI-XML-Dataset/blob/master/Media/IATI_Org_Folders.png)

IATI’s entire corpus can be downloaded via this [tool](https://github.com/andylolz/iati-data-dump) developed by the IATI community. However, the data will arrive organized/packaged into folders listed by publishing organization.

## Micro-project

This group micro-project will create one single XML file containing all the information found in organization folders. Organization by organization, the goal is to append files to the end of preceding files, keeping the XML structured and valid. See below:

```
<iati-activities>       (org A)
    <iati-activity>     (activity one)
    </iati-activity>    
    <iati-activity>     (activity two)
    </iati-activity>
</iati-activities>
<iati-activities>       (org B)
    <iati-activity>     (activity one)
    </iati-activity>
    <iati-activity>     (activity two)
    </iati-activity>
</iati-activities>
```
According to IATI's [website](https://iatistandard.org/en/), IATI's entire corpus currently contains 1,149,491 activities published by 1,058 organizations.

## Connected Micro-projects

The initial master XML file will enable the group to generate a JSON version and carry out other projects.
