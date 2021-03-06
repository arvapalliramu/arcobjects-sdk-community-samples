## Time Series Graph tool add-in

  <div xmlns="http://www.w3.org/1999/xhtml" xmlns:my="http://schemas.microsoft.com/office/infopath/2003/myXSD/2006-02-10T23:25:53">The Time Series Graph tool builds a line graph from a point feature layer according to different time values. The layer contains multiple measurements for a set of seven gages. Each measurement has its own stream flow value, date and time, and gage ID attributes associated with it.</div>
  <div xmlns="http://www.w3.org/1999/xhtml" xmlns:my="http://schemas.microsoft.com/office/infopath/2003/myXSD/2006-02-10T23:25:53"> </div>
  <div xmlns="http://www.w3.org/1999/xhtml" xmlns:my="http://schemas.microsoft.com/office/infopath/2003/myXSD/2006-02-10T23:25:53">When you click a feature point (gage station) using the Time Series Graph tool, the tool identifies the point and finds the gage ID. All the measurements from this point for this gage ID are used in making a graph based on a graph template. If there is an existing open graph window, the tool creates the graph series in this window. If there is no open graph window, the tool creates the graph series in a new graph window. </div>  


<!-- TODO: Fill this section below with metadata about this sample-->
```
Language:              C#, VB
Subject:               Map
Organization:          Esri, http://www.esri.com
Date:                  11/17/2017
ArcObjects SDK:        10.6
Visual Studio:         2015, 2017
.NET Target Framework: 4.5
```

### Resources

* [ArcObjects .NET API Reference online](http://desktop.arcgis.com/en/arcobjects/latest/net/webframe.htm)  
* [Sample Data Download](../../releases)  
* [What's new](http://desktop.arcgis.com/en/arcobjects/latest/net/webframe.htm#05247c04-bfd9-4e36-ae09-bc6e833c3b14.htm)  
* [Download the ArcObjects SDK for .Net from MyEsri.com](https://my.esri.com/)  

### Usage
1. Open the solution file in Visual Studio and build the project.   
1. Start ArcMap, click the Customize drop-down menu, and click Customize Mode. The Customize dialog box appears.  
1. Click the Commands tab, scroll to Add-in Controls in the categories list, and drag the Time Series Graph tool to a toolbar in ArcMap.   
1. Move the timeseries.tee file from the sample folder to the <your ArcGIS Desktop install location>/GraphTemplates folder.  
1. Add the TimeSerTool.lyr to ArcMap.   
1. Select the Time Series Graph tool and click the point (gage station). A line graph is drawn in a new graph window.   
1. To add lines to the same graph, keep the graph window open, and a new line is added into it. To draw lines on a new graph, close the graph window, and a new line is drawn in a separate graph window.   









---------------------------------

#### Licensing  
| Development licensing | Deployment licensing | 
| ------------- | ------------- | 
| ArcGIS Desktop Basic | ArcGIS Desktop Basic |  
| ArcGIS Desktop Standard | ArcGIS Desktop Standard |  
| ArcGIS Desktop Advanced | ArcGIS Desktop Advanced |  


