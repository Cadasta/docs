# Collecting Data with [ODK](#odk-overview) or [GeoODK](#geoodk-overview) Collect (Open Data Kit) 


This chapter is divided into two parts: 

* [ODK Overview](#odk-overview)
* [ODK Initial Setup](#odk-initial-setup)
* [ODK Loading Your Cadasta XLSForm](#odk-loading-your-form)
* [ODK Data Collection](#odk-data-collection)
* [ODK Uploading Data](#odk-uploading-data)
* [ODK Collecting Location Data: GeoTrace, GeoPoint and GeoShape](#odk-geotracing)
* [ODK Editing Data](#odk-editing-data)
* [ODK Deleting Forms](#odk-deleting-questionnaires)
* [ODK Troubleshooting](#odk-troubleshooting)


## ODK Overview {#odk-overview}

Field data collection is an important part of the land and resource rights documentation process. The Cadasta Platform is designed to accommodate a couple of tools for data collection, allowing for ingestion of data. One of those tools is Open Data Kit, or ODK Collect (which we refer to as ODK for short).

ODK is a free, open source mobile data collection application for Android devices \(sorry Apple fans\). To get started, [download ODK Collect from the Google Play Store](https://play.google.com/store/apps/details?id=org.odk.collect.android&hl=en), or wherever you acquire your applications.

This section provides an overview of how ODK and Cadasta work together:

1. First, you'll [set up ODK](#odk-initial-setup) on an Android device.
2. Then you'll [load the Cadasta XLSForm](#odk-loading-your-form) you want to use for data collection.
3. Finally, it's time to [collect your data](#odk-data-collection)! 
4. When you're back to WiFi, [upload your data](#odk-uploading-data) to the Cadasta Platform.

**Important!** Steps 1, 2, and 4 require being near WiFi. You may also want to test step 3 before heading out into the field, just in case you need to [troubleshoot](#odk-troubleshooting) or make any changes. 

For more information and documentation about ODK generally, visit [opendatakit.org](https://opendatakit.org/).

## Initial Setup {#initial-setup}

_**Note:** This step requires being near WiFi!_

To get started, [download ODK from the Google Play Store](https://play.google.com/store/apps/details?id=org.odk.collect.android&hl=en), or wherever you acquire your applications.

If this is the first time you've used ODK with the Cadasta Platform, you'll need to configure ODK for direct syncing. To do this, you'll need to set up your Cadasta account if you haven't already \(see [Getting Started](01-gettingstarted.md)\).

1. Once you've created your account and installed ODK, open the application.

2. From the opening screen (the Main Menu), tap the **three dots**  in the upper right, then select **General Settings**, then **Server**. 

    ![](/assets/new-odk-01.png)

3. On this screen, enter you'll need to change some settings. Change the `Type` field to `Other`. Then you'll need to enter a specific URL: 

    * https://platform.cadasta.org/collect \(if for active projects\); or

    * https://demo.cadasta.org/collect  \(if for testing\)

    ![](/assets/new-odk-02.png)

_**Important!** Notice the `s` at the end of `https` in the URLs above. That's an important part of our URLs! Forgetting it will produce an error. `https` provides authentication of the website and associated web server, meaning that the information being sent and received is more secure than it would be as just `http`. <a href="https://en.wikipedia.org/wiki/HTTPS" target="_blank">Read more.</a> _
Here, you'll also want to enter your Cadasta username and password. This will connect you to your Cadasta account, where you can access your questionnaires for data collection.

Click the back button twice to return to the main menu.

## Loading your Cadasta XLSForms {#odk-loading-your-form}

_**Note:** This step requires being near WiFi!_

Once you've connected ODK with Cadasta, the next thing you need to do is load the forms you're using for your data collection project.

1. From the main menu, select **Get Blank Form**.

    ![](/assets/new-odk-03.png)

2. At this stage, you may be asked to provide your Cadasta username and password. Enter this information and then wait a few moments to be connected to the server.

3. In the page that follows, you'll see a list of questionnaires that have been loaded for your organization's projects. Place a checkmark next to the form you'd like to use and tap **Get Selected**.

Now, ODK is configured to record data using the questions in your form. You can select which form you want to use in a later step.

## Data Collection {#odk-data-collection}

Once you've initialized ODK and loaded your Cadasta XLSForm, now it’s time to collect some data!

For this step, make sure that GPS is enabled on your device and turned on.

1. From the ODK Main Menu select **Fill Blank Form** then the form that you want to use. 

    ![](/assets/new-odk-04.png)

2. Swipe left twice to get started completing the form. 

	![](/assets/new-odk-05.png)

3. Continue answering all the survey questions until you reach the "End of survey" message. During this step, swipe left after you've answered each question. 
    * During this section, you'll likely be asked to GeoTrace your location data, or add a GeoShape or GeoPoint. For more information about how this works, see [Collecting Location Data: GeoTrace, GeoPoint and GeoShape](#geotracing).
4. When all of your questions are completed, select the **Mark Form as finalized** checkbox and **Save Form and Exit**. 

###Collecting Data in Multiple Languages

If you need to collect data in multiple languages, you can set it up in your Cadasta XLSform. _[Learn how.](09-XLSForms.md)_

Once you've chosen your default language and set up your questions in all the languages you need, you'll be able to toggle between the languages during data collection. Select the **More actions** button in the upper right, then **Change Language**, then the language of your choice. 

![](/assets/multi-lang-odk.png)


##Collecting Location Data: GeoTrace, GeoShape, and GeoPoint {#odk-geotracing}

During [data collection](#odk-data-collection), you'll be asked to collect data specifying your location using one of the following options.

![](/assets/new-odk-geoshape-geotrace-geopoint.png)

* **[GeoTrace](#geotrace)** gives you the option of creating polylines or polygons based on your location. In other words, you can use GeoTrace to walk an area, using automatic or manual mode. GeoTrace is the default option provided. _**Important!** If you get to the screen below, be sure to select the Polygon option if you are trying to map an enclosed area._

![](/assets/geo-odk-10-polyline-polygon.png)

* **[GeoShape](#geoshape)** creates polygons (closed shapes). To create a GeoShape, you can use your finger to draw a shape on the map.  

* **[GeoPoint](#geopoint)** creates points (single GPS coordinates) based on your location. 

### GeoTrace {#odk-geotrace}

![](/assets/new-odk-geotrace.png)

When it's time to start your GeoTrace, you'll be prompted to **Start GeoTrace**.

In the next screen, you'll be asked to **Zoom to Current Location**.

![](/assets/odk-geotrace-2.png)

Once your location is identified, you'll be asked to select either Automatic or Manual mode.  

![](/assets/odk-geotrace-3.png)

**Manual mode** allows you to record your geotrace manually. Every time you want to drop a pin, click the **Record Location Point** button at the top of the map. For example, it's common practice to drop pins at each corner of a location. 

![](/assets/odk-geotrace-5.png)

**Automatic mode** records your location at set intervals, for example once every 20 seconds. This mode is helpful if you're recording a large area. 

The amount of time you should set for your interval depends on how you're collecting the data. For example, if you're driving, you may want to set the interval to be once every 5 seconds. If you're walking, you may want to record once every 20-30 seconds. 

If you know you need to record the corners of a large area, then you might want to try manual mode. Or, if you're using automatic mode, pause on the corner long enough for the pin to drop. Alternatively, in automatic mode, you can also use the **Record Location Point** button to manually drop a pin.

For either automatic or manual mode, keep in mind that the more points you record, the bigger your data file will be and the harder it will be to upload when you return to WiFi or you mobile network. Collect all the points you need - and only the points you need!

![](/assets/odk-geotrace-4.png)

When you're done with your GeoTrace, hit the pause button. You'll then be asked to save your information as a polyline or polygon.

If you've recording a point or line, choose polyline. If you've recording an area and created a closed shape, choose polygon.

Finally, you'll be brought to a confirmation screen where you can view your GeoTrace. 

_Note that ODK calls a geotrace a parcel regardless of what kind of location it is._

### GeoShape {#odk-geoshape}

GeoShape is designed for making shapes (or polygons) to represent a specific location. For example, you can use GeoShape to draw a boundary around a building or land area. 

![](/assets/new-odk-geoshape.png)

If you're collecting data using GeoShape, you'll first be asked to zoom to your current location or to a saved feature. 

![](/assets/odk-geoshape-1.png)

In the next screen, you'll be able to start making your shape. Press the screen to place markers around your location, and notice the red lines that are created between each marker. To close your polygon, press on the same point where the polygon began.

![](/assets/odk-geoshape-2.png)

When you're ready to save your GeoShape, hit the **Save** icon on the right. If you wish to discard it, you can also hit the **Trash** button above it.

### GeoPoint {#odk-geopoint}

To collect single GPS coordinates, you can use GeoPoint. GeoPoint only works by tracking your specific location (drawing with your finger is not available).

![](/assets/new-odk-geopoint.png)

When it's time to collect your GeoPoint, it will first load your location. This may take a few minutes. 

![](/assets/odk-geopoint-1.png)

Next it will give you some GPS accuracy information. Here, the accuracy is within a 24-meter radius of where the user is standing. 

![](/assets/odk-geopoint-2.png)

Once the location and accuracy information is loaded, you're ready to save your GeoPoint.

![](/assets/odk-geopoint-3.png)

##Uploading Data {#odk-uploading-data}

When you get back to WiFi or a mobile network, you can upload your completed forms to the Cadasta Platform. 

From the main menu, click **Send Finalized Form** and then check off all the forms that you want to upload (use the **Toggle All** button to select all forms). Then select **Send Selected**.

![](/assets/new-odk-06.png)

Finally, you'll get a confirmation message confirming that the data has been sent. 

It's a good idea to confirm that you see the data on the Cadasta Platform. Then you can [delete any completed XLSForms](#deleting-questionnaires) from your Android device.

## Editing Data {#odk-editing-data}

ODK makes editing your forms relatively easy. From the main menu, select **Edit Data**, then the form you want to edit. When you're done, save your changes.

## Deleting Cadasta XLSForms {#odk-deleting-questionnaires}

You can also delete unwanted forms by selecting **Delete Data** from the main menu. On the page that follows, you can toggle between Saved Forms and Blank Forms to delete either one. 

## ODK Troubleshooting {#odk-troubleshooting}

If you're having trouble using ODK, the answer to your question may be here. If not, please [contact us](http://cadasta.org/contact/) and we'll do our best to help you work through the issue.

### Trouble Loading Your Cadasta XLSForm

##### ISSUE: I can't connect to the Cadasta server because my username and password aren't working. (And yes, I've checked to make sure they're correct!)

The easiest thing to do here is to go to the Cadasta platform and change your password. Then, return to ODK and enter your new password there.  

##### ISSUE: I'm getting a message that says to "Please wait a few moments," but it's been much much longer than that.

If the above screen is taking longer than you think it should, hit Cancel. You may be correctly connected, or you may be asked to enter your username and password again.

##### ISSUE: I'm getting an error that my file is too big. 

ODK cannot upload files that are bigger than 10 MB. Usually, the culprit is a high-resolution photograph. To resolve the issue, find the photograph (or other large file), remove it, and re-attach it with a lower-resolution version. 

### Difficulty Adding Location Data

##### ISSUE: ODK won't let me add any location data. 

![](/assets/odk-trouble-1.png)

If you get the screen like the one above, unfortunately it's a known (and frustrating!) bug. Cadasta is aware that some Android devices simply refuse to log their GPS data with ODK. Our team is working to resolve the issue.

In the meantime, here are some alternatives:

1. Try using another Android device. This mysterious bug does not appear on all of them.
2. Try using GeoODK, which works very similarly to ODK. _[Learn more about how to use GeoODK with Cadasta](06-odkcollect.md)._


# Collecting Data with GeoODK Collect (Geographical Open Data Kit) 

* [GeoODK Overview](#geoodk-overview)
* [GeoODK Initial Setup](#geoodk-initial-setup)
* [GeoODK Loading Your Cadasta XLSForm](#geoodk-loading-your-form)
* [GeoODK Data Collection](#geoodk-data-collection)
* [GeoODK Uploading Data](#geoodk-uploading-data)
* [GeoODK Collecting Location Data: GeoTrace, GeoPoint and GeoShape](#geoodk-geotracing)
* [Editing Data](#geoodk-editing-data)
* [Deleting Forms](#geoodk-deleting-questionnaires)
* [GeoODK Troubleshooting](#geoodk-troubleshooting)

## GeoODK Overview {#geoodk-overview}

Geographical Open Data Kit \(GeoODK Collect\) is a data collection application for Android devices (unfortunately not yet available for Apple devices). Like Open Data Kit (ODK Collect), GeoODK can be used for data collection projects in the Cadasta Platform. 

This section provides an overview of how GeoODK and Cadasta work together:

1. First, you'll [set up GeoODK](#geoodk-initial-setup) on an Android device.
2. Then you'll [load the Cadasta XLSForm](#geoodk-loading-your-form) you want to use for data collection.
3. Finally, it's time to [collect your data](#geoodk-data-collection)! 
4. When you're back to WiFi, [upload your data](#geoodk-uploading-data) to the Cadasta Platform.

**Important!** Steps 1, 2, and 4 require being near WiFi. You may also want to test step 3 before heading out into the field, just in case you need to [troubleshoot](#geoodk-troubleshooting) or make any changes. 

For more information and documentation about GeoODK generally, visit [geoodk.com](http://geoodk.com/).

## Initial Setup {#geoodk-initial-setup}

_**Note:** This step requires being near WiFi!_

To get started, [download GeoODK from the Google Play Store](https://play.google.com/store/apps/details?id=com.geoodk.collect.android), or wherever you acquire your applications.

If this is the first time you've used GeoODK with the Cadasta Platform, you'll need to configure GeoODK for direct syncing. To do this, you'll need to set up your Cadasta account if you haven't already \(see [Getting Started](01-gettingstarted.md)\).

1. Once you've created your account and installed GeoODK, open the application.
2. From the map screen, hit the button with the four squares on the right. Then select **Settings** from the Main Menu, then **General Settings**, then **Configure Platform Settings**. 

    ![](/assets/geo-odk-1-configure-settings.png)

3. On this screen, enter the Platform URL along with your username and password. The username and password do not have to be the same as they are on your Cadasta account, but it may be helpful to keep them consistent. The URL you need should be similar to the one you used when you signed up for your Cadasta account. 
    * https://platform.cadasta.org/collect \(if for active projects\); or
    * https://demo.cadasta.org/collect  \(if for testing\)

    ![](/assets/geo-odk-2-url.png)

You now have a GeoODK account that's synced with the Cadasta Platform.

_**Important!** Notice the `s` at the end of `https` in the URLs above. That's an important part of our URLs! Forgetting it will produce an error. `https` provides authentication of the website and associated web server, meaning that the information being sent and received is more secure than it would be as just `http`. <a href="https://en.wikipedia.org/wiki/HTTPS" target="_blank">Read more.</a> _

Click the back button 3 times to return to the main menu.

## Loading your Cadasta XLSForm {#geoodk-loading-your-form}

_**Note:** This step requires being near WiFi!_

Once you've connected GeoODK with Cadasta, the next thing you need to do is load the form you're using for your data collection project. 

1. From the Main Menu, select **Settings**, then **Form Management**. 

    ![](/assets/geo-odk-3-form-management.png)

2. At this stage, you may be asked to provide your Cadasta username and password. Enter this information and then wait a few moments to be connected to the server. _Having trouble with this step? See [GeoODK Troubleshooting](#geoodk-troubleshooting)._

    ![](/assets/geo-odk-4-user-pass.png)

3. In the page that follows, you'll see a list of Cadasta XLSForms that have been loaded for your organization's projects. Place a checkmark next to the form you'd like to download and tap **Get Selected**.

    ![](/assets/geo-odk-5-questionnaire-list.png)

Now, GeoODK is configured to record data using the questions in your form. 

## Data Collection {#geoodk-data-collection}

Once you've initialized GeoODK and loaded your Cadasta XLSForm, now it’s time to collect some data!

For this step, make sure that GPS is enabled on your device and turned on.

1. From the Main Menu select **Collect Data** then the form that you want to use. 

    ![](/assets/geo-odk-6-collect-data.png)

2. Swipe left twice to get started completing the form.
3. Continue answering all the survey questions until you reach the "End of survey" message. During this step, swipe left after you've answered each question. 
    * During this section, you'll likely be asked to GeoTrace your location data, or add a GeoShape or GeoPoint. For more information about how this works, see [Collecting Location Data: GeoTrace, GeoPoint and GeoShape](#geotracing).
4. When all of your questions are completed, select the **Mark Form as finalized** checkbox and **Save Form and Exit**. 

![](/assets/geo-odk-7-finalized-form.png)

### Collecting Data in Multiple Languages

If you need to collect data in multiple languages, you can set it up in your form. _[Learn how](09-XLSForms.md)_

Once you've chosen your default language and set up your questions in all the languages you need, you'll be able to toggle between the languages during data collection. Select the **More actions** button in the upper right, then **Change Language**, then the language of your choice. 

![](/assets/multi-lang-geoodk.png)


## Collecting Location Data: GeoTrace, GeoShape, and GeoPoint {#geoodk-geotracing}

During [data collection](#geoodk-data-collection), you'll be asked to collect data specifying your location using one of the following options.

* **[GeoTrace](#geotrace)** creates lines  (collections of two or more GPS coordinates) based on your location. In other words, you can use GeoTrace to walk an area, using automatic or manual mode.  GeoTrace is the default option provided. 

* **[GeoShape](#geoshape)** creates polygons (closed shapes). To create a GeoShape, you can use your finger to draw a shape on the map.  

* **[GeoPoint](#geopoint)** creates points (single GPS coordinates) based on your location. 

To learn more about how to configure these options in your form, see the [Cadasta XLSForms & Custom Data Collection](09-XLSForms.md) section.

### GeoTrace {#geoodk-geotrace}

To start geotracing, hit the Play button in the upper left:

![](/assets/geo-odk-geotrace-1-play.png)

From there, you'll be asked to select either Automatic or Manual mode. 

![](/assets/geo-odk-geotrace-2-manual-automatic.png)

**Manual mode** allows you to record your geotrace manually. Every time you want to drop a pin, click the **Record Location Point** button at the top of the map. For example, it's common practice to drop pins at each corner of a location. 

![](/assets/geo-odk-geotrace-3-record-location-point.png)

**Automatic mode** records your location at set intervals, such as once every 20 seconds. This mode is helpful if you're recording a large area. 

The amount of time you should set for your interval depends on how you're collecting the data. For example, if you're driving, you may want to set the interval to be once every 5 seconds. If you're walking, you may want to record once every 20-30 seconds. 

If you know you need to record the corners of a large area, then you might want to try manual mode. Or, if you're using automatic mode, pause on the corner long enough for the pin to drop. Alternatively, in automatic mode, you can also use the **Record Location Point** button to manually drop a pin.

For either automatic or manual mode, keep in mind that the more points you record, the bigger your data file will be and the harder it will be to upload when you return to WiFi or you mobile network. Collect all the points you need - and only the points you need!

When you're done geotracing, hit the pause button. You'll then be asked to save your information as a polyline or polygon.

![](/assets/geo-odk-geotrace-4-save-geotrace.png)

If you've recording a point or line, choose polyline. If you've recording an area and created a closed shape, choose polygon.

**Important!** If you are trying to create a closed area (like, around a property), then choose **Save as Polygon** on this page:

![](/assets/geo-odk-10-polyline-polygon.png)


Finally, you'll be brought to a confirmation screen where you can view your GeoTrace. 

![](/assets/geo-odk-geotrace-5-confirmation.png)

_Note that GeoODK calls a geotrace a parcel regardless of what kind of location it is._

### GeoShape {#geoodk-geoshape}

GeoShape is designed for making shapes (or polygons) to represent a specific location. For example, you can use GeoShape to draw a boundary around a building or land area.  

![](/assets/geo-odk-geoshape-1.png)

To collect location data with GeoShape, you can use your finger to draw a shape on the map. 

To create the shape, press and hold your finger on a point on the map until a marker appears. Then, hold your finger on another point. You'll see a red line appear between the two points. 

Keep placing markers on key points around your polygon. When it's time to complete the polygon, press the **Polygon** button in the upper right. 

![](/assets/geoodk-geoshape-4.png)

This will connect the last and first marker you drew, creating a complete and closed polygon.

When you're done, tap the **Save button** and continue your data collection.

### GeoPoint {#geoodk-geopoint}

To collect single GPS coordinates, you can use GeoPoint. GeoPoint only works by tracking your specific location (drawing with your finger is not available).

First you'll come to a screen asking you to record the location of your parcel. Click **Record Location**. 

![](/assets/geoodk-geopoint-1.png)

In the screen that follows, you'll see a map with your location. To save your pin location, hit the **Save** icon in the upper right. Also note the GPS accuracy logged at the top of the screen. 

![](/assets/geoodk-geopoint-2.png)

When you're done, you'll come to a screen that looks like the one below. You can use this screen to view or edit your recording.

![](/assets/geoodk-geopoint-3.png)

## Uploading Data {#geoodk-uploading-data}

When you get back to WiFi or a mobile network, you can upload your completed forms to the Cadasta Platform. 

From the main menu, click **Send Data** and then check off all the forms that you want to upload (use the **Toggle All** button to select all forms). Then select **Send Selected**.

![](/assets/geo-odk-8-send-data.png)

Next, you'll get a confirmation message confirming that the data has been sent. 

![](/assets/geo-odk-9-confirmation.png)

It's a good idea to confirm that you see the data on the Cadasta Platform. Then you can [delete any completed forms](#deleting-questionnaires) from your Android device.

## Editing Data {#geoodk-editing-data}

ODK makes editing your forms relatively easy. From the main menu, select **Edit Data**, then the form you want to edit. When you're done, save your changes.

## Deleting Forms {#geoodk-deleting-questionnaires}

You can also easily delete unwanted Cadasta XLSForms by selecting **Delete Saved Form** from the main menu. On the page that follows, you can toggle between Saved Forms and Blank Forms to delete either one. 

## GeoODK Troubleshooting {#geoodk-troubleshooting}

If you're having trouble using GeoODK, the answer to your question may be here. If not, please [contact us](http://cadasta.org/contact/) and we'll do our best to help you work through the issue.

### Trouble Loading Your Cadasta XLSForm

##### ISSUE: I can't connect to the Cadasta server because my username and password aren't working. (And yes, I've checked to make sure they're correct!)

The easiest thing to do here is to go to the Cadasta platform and change your password. Then, return to GeoODK and enter your new password there.  

##### ISSUE: I'm getting a message that says to "Please wait a few moments," but it's been much much longer than that.

![](/assets/geo-odk-error-1-wait-a-moment-forever.png)

If the above screen is taking longer than you think it should, hit Cancel. You may be correctly connected, or you may be asked to enter your username and password again. 

### Trouble Uploading Completed Forms

##### ISSUE: I'm getting an error that my file is too big. 

ODK cannot upload files that are bigger than 10 MB. Usually, the culprit is a high-resolution photograph. To resolve the issue, find the photograph (or other large file), remove it, and re-attach it with a lower-resolution version. 

##### ISSUE: I'm getting an error when I upload my completed form.

If you're having trouble uploading your Cadasta XLSForms, the most likely culprit is collecting data using a form that doesn't exactly match the one loaded on the Cadasta Platform. This can happen if you modify your form, load it to Cadasta, and then continue collecting data using an older version. 

Unfortunately, the easiest way to fix this is to uninstall the old form and start over. This is why we recommend that you test GeoODK before heading out into the field. We also recommend refreshing your form before heading out to the field if you think that it might have changed. 

If you've collected too much data to start over, please [contact us](http://cadasta.org/contact/). 


