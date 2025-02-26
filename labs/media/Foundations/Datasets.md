Lab 2.1 - Construct a Dataset from Schema
==========
<table style="border-collapse: collapse; border: none;" class="tab" cellspacing="0" cellpadding="0">

<tr style="border: none;">

<div align="left">
<td width="600" style="border: none;">
<table>
<tbody valign="top">
      <tr width="500">
            <td valign="top"><h3>Objective:</h3></td>
            <td valign="top"><br>This lab will show you the how to convert a schema into a dataset
            </td>
     </tr>
     <tr width="500">
           <td valign="top"><h3>Prerequisites:</h3></td>
           <td valign="top"><br>
                            <li>schema in place
           </td>
     </tr>
</tbody>
</table>
</td>
</div>

<div align="right">
<td style="border: none;" valign="top">

<table>
<tbody valign="top">
      <tr>
            <td valign="middle" height="70"><b>section</b></td>
            <td valign="middle" height="70"><img src="https://github.com/adobe/AEP-Hands-on-Labs/blob/master/assets/images/left_hand_nav_menu_schemas.png?raw=true" alt="Schemas"></td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>version</b></td>
            <td valign="middle" height="70">1.0.1</td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>date</b></td>
            <td valign="middle" height="70">2020-01-06</td>
      </tr>
</tbody>
</table>
</td>
</div>

</tr>
</table>

Before be begin go to [https://platform.adobe.com/home](https://platform.adobe.com/home). Follow the instructions detailed below.

Instructions:
-----------------

We will be creating a dataset for the schema we created in the previous exercise. Please follow the steps below
1. In the left-hand menu, navigate to "Datasets":

      <!--
      ![Demo](./images/datasetshome.png)
      -->
      <kbd><img src="./images/datasetshome.png"  /></kbd>
      
2. Click "+Create Dataset": 

      <!--
      ![Demo](./images/datasetcreate.png)
      -->
      <kbd><img src="./images/datasetcreate.png"  /></kbd>
      
3. Since we will be creating the dataset from a schema definition, please select "Create dataset from schema":

      <!--
      ![Demo](./images/datasetcreate2.png)
      -->
      <kbd><img src="./images/datasetcreate2.png"  /></kbd>
 
4. On the Select Schema page search for "Subscription Schema [your-assigned-number]" then select the schema and click "Next":
      
      <!--
      ![Demo](./images/datasetschema.png)
      -->
      <kbd><img src="./images/datasetschema.png"  /></kbd>
      
5. Next, to configure the dataset we need to give it a name. Please name your dataset "Subscription Dataset [your-assigned-number]" and give it the same description: 
      
      <!--
      ![Demo](./images/datasetname.png) 
      -->
      <kbd><img src="./images/datasetname.png"  /></kbd>
 
6. Click "Finish" to save the dataset:
      
      <!--
      ![Demo](./images/datasetfinish.png) 
      -->
      <kbd><img src="./images/datasetfinish.png"  /></kbd> 

7. We have successfully created the dataset, but this dataset has not ingested data. We will now import a file into this dataset. This time we will import a JSON file and it will simply need to be dragged and dropped into the dataset. 

    On the right panel scroll down until you see the "ADD DATA" section:
    <!--  
    ![Demo](./images/datasetadddata.png) 
    -->
    <kbd><img src="./images/datasetadddata.png"  /></kbd> 

8. From the lab files you downloaded, drag and drop the "subscription_data_001.json" file into the "ADD DATA" section:

      ![Demo](./images/datasetbatchdragdrop.png)

      You will now see a batch with a "Processing" status:
    <!---
    ![Demo](./images/datasetbatch.png)
    --->
    <kbd><img src="./images/datasetbatch.png"  /></kdb>

9. Adobe Experience Platform will perform the XDM mapping and conversion for JSON format to parquet and make this data available on the data lake and the profile store. Refresh the screen This process only takes afew seconds.

    Once your batch status is 'Success', you can preview the data by hitting the 'Preview Dataset' button on the top right corner.

    <!--  
    ![Demo](./images/datasetpreview.png)
     -->
     
    <kbd><img src="./images/datasetpreview.png"  /></kdb>

10. Congratulations!!! You created a dataset and ingested a JSON file.


<br>
<br>
<br>

Return to [Lab Agenda Directory](https://github.com/adobe/AEP-Hands-on-Labs/blob/master/labs/media/README.md#lab-agenda)


