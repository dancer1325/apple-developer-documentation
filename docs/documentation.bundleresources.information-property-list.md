https://developer.apple.com/documentation/bundleresources/information-property-list

* == 👀resource / contain key-value pairs / configure a bundle 👀
  * uses of these key-value pairs
    * characterize the bundle itself
    * configure the app, framework, or other entity / bundle represents
  * keys -- can be --
    * REQUIRED
    * specific to executable's particular features 
* Bundles / == executables of different kinds
  * -- contain an -- information property list file 
    * == how the system -- should interpret the -- associated bundle
    * if you want to create this file -> see [here](documentation.bundleresources.managing-your-app-s-information-property-list.md)
* "Info.plist"
  * ⚠️Information property list's REQUIRED name ⚠️ / 
    * case-sensitive
    * MUST begin with `I`
    * 's location | bundle -- depends on -- bundle type & platform
      * _Example:_
        * for iOS app bundles -> | bundle’s root directory
        * for macOS app bundles -> | Contents directory
* 👀if you want to access an information property list -> use a Bundle class' instance 👀 
  * Bundle class' instance == bundle | disk
  * ways to access key's value
    * -- via -- bundle instance's properties 
      * _Example:_ `bundleIdentifier` property == `CFBundleIdentifier` key's value 
    * -- via -- `object(forInfoDictionaryKey:)`
