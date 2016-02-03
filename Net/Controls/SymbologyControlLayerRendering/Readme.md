##Change layer rendering using the SymbologyControl

###Purpose  
This sample demonstrates using the SymbologyControl to display marker, line, and fill symbols, which update the symbol used by the renderer of a feature layer. The sample uses the SymbologyControl in conjunction with the PageLayoutControl, TOCControl, ToolbarControl, and the controls commands.  


###Usage
1. Load a map document into the PageLayoutControl.    
1. Right-click a feature layer to change its symbology.   





####Additional information  
<div xmlns="http://www.w3.org/1999/xhtml" xmlns:my="http://schemas.microsoft.com/office/infopath/2003/myXSD/2006-02-10T23:25:53">The ITOCControl.HitTest method is used in the OnMouseDown event of the TOCControl to determine whether the type of item clicked implements IGeoFeatureLayer. If the IFeatureClass.ShapeType returns points, lines, or polygons, the IGeoFeatureLayer.Renderer is updated with the symbol selected in the SymbologyControl.</div>  
<div xmlns="http://www.w3.org/1999/xhtml" xmlns:my="http://schemas.microsoft.com/office/infopath/2003/myXSD/2006-02-10T23:25:53"> </div>  
<div xmlns="http://www.w3.org/1999/xhtml" xmlns:my="http://schemas.microsoft.com/office/infopath/2003/myXSD/2006-02-10T23:25:53">In the Form_Load event of the SymbolForm, the LoadStyleFile method is used to add the contents of the ESRI.ServerStyle into the SymbologyControl, and the StyleClass property is used to display MarkerSymbols, LineSymbols, or FillSymbols. The ISymbologyStyleClass.AddItem method is used to add a ServerStyleGalleryItem to the SymbologyControl with its item set to the symbol currently used by IGeoFeatureLayer.Renderer.</div>  
<div xmlns="http://www.w3.org/1999/xhtml" xmlns:my="http://schemas.microsoft.com/office/infopath/2003/myXSD/2006-02-10T23:25:53"> </div>  
<div xmlns="http://www.w3.org/1999/xhtml" xmlns:my="http://schemas.microsoft.com/office/infopath/2003/myXSD/2006-02-10T23:25:53">Clicking an item displayed in the SymbologyControl passes the selected item to the OnItemSelected event, and the ISymbologyStyleClass.PreviewItem method is used to preview the item in a PictureBox.</div>  


####See Also  
[SymbologyControl class](http://desktop.arcgis.com/search/?q=SymbologyControl%20class&p=0&language=en&product=arcobjects-sdk-dotnet&version=&n=15&collection=help)  
[ISymbologyControl interface](http://desktop.arcgis.com/search/?q=ISymbologyControl%20interface&p=0&language=en&product=arcobjects-sdk-dotnet&version=&n=15&collection=help)  
[ISymbologyStyleClass interface](http://desktop.arcgis.com/search/?q=ISymbologyStyleClass%20interface&p=0&language=en&product=arcobjects-sdk-dotnet&version=&n=15&collection=help)  


---------------------------------

####Licensing  
| Development licensing | Deployment licensing | 
| :------------- | :------------- | 
| Engine Developer Kit | Engine |  
|  | ArcGIS for Desktop Basic |  
|  | ArcGIS for Desktop Standard |  
|  | ArcGIS for Desktop Advanced |  

