# BingImage
 
There are several ways to get BING images.  
This library uses the following URL. just change the format parameter in the URL .  
http://www.bing.com/HPImageArchive.aspx?format=rss&idx=0&n=1&mkt=en-US  

USE:  
BingImage bingImage = new BingImage();  
var bingUnit = await bingImage.GetTodayBingUnit(BingImageResolution.LARGE);
if (bingUnit != null)
{  
    imgPreview.Source = new BitmapImage(new Uri(bingUnit.Path));
}  
