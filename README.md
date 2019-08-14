# iOS Enterprise Signing&Distribution over Dropbox or Other
Sign your .ipa and distribute ii with Dropbox or other in just 3 steps.


## Work In Progress


## 1. Set entitlements.xml

### Replace : 

- Application identifier => [TEAM\_ID.com.organisation.project] 
- Team identifier => [TEAM\_ID]



## 2. Resign

Within the folder launch the command : [COMMAND]


## 3. Share the app with Dropbox

### On Dropbox :

- Create a folder
- Save the .ipa within
- Make a shared link (we will call it IPA\_SHARED\_LINK) [GIF]

### In manifest.plist replace : 

- Assets url => [IPA\_SHARED\_LINK (it looks like: https://dl.dropbox.com/s/aaaaaaaaa/appResigned.ipa)]
- Bundle identifier => [com.organisation.project]
- Bundle version => [1.0.0]
- Title => [APP\_NAME]

### On Dropbox :

- Save the manifest.plist with the .ipa
- Make a shared link (we will call it MANIFEST\_SHARED\_LINK) [GIF]

### Make the install link

- Create a link itms-services://?action=download-manifest&url=[MANIFEST\_SHARED\_LINK (it look likes https://dl.dropbox.com/s/aaaaaaaaa/manifest.plist)]


## THAT'S ALL 👏👏
### Now you can share the link to install the app on all iOS devices.
