https://developer.apple.com/documentation/bundleresources/choosing-the-location-services-authorization-to-request

* app's authorization status
  * == if & when, app -- receives -- location events
  * types
    * "When In Use"
      * if app is in use (foreground OR background / location usage enabled) -> can
        * use ALL location services
        * receive events
      * 👀recommended 👀
      * features
        * Access all available location services while the user is using the app.
          * If the user stops using your app, any outstanding requests suspend until the user resumes using your app.
        * TODO:
    * "Always"
      * ALTHOUGH user NOT aware that your app is running -> app can 
        * use ALL location services
        * receive events  
      * if your app is NOT running -> system 
        * launches your app
        * delivers the event
* TODO: