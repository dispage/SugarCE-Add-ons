# Installer for Dispage Extension Manager

Dispage Extension Manager ("DEM") is a new SugarCRM tool that allows the
Administrator to manage the Dispage Extensions in a way similar to Mozilla
Firefox. Searches for the available extensions and updates, checks for
compatibility with the SugarCRM versions and logs the related events.
Additionally, it provides a javascript framework integrated to SugarCRM. 


	
## Dispage extension management

After logged in SugarCRM as Admin, DEM connects to the Dispage Resource 
Center (DRC) through the Username and Password of the Dispage portal, then
activates and synchronizes the installed extensions.
If logged as common user, DEM simply activates the installed extensions.

Dispage key features such as the jQuery support are available also in the
Offline Mode, without connecting to the DRC.
Connection to Dispage is still required to install/upgrade packages and to
download the package decryption keys.



## Dispage extension management administration

By clicking on the link "Dispage Extensions", placed at the top SugarCRM bar,
the DEM Administration Tabbed Panel is displayed.


### Tab "Installed Extensions"

Shows all the Dispage Installed Extensions, each followed by the Release, the
Version, the Installed and the Updated dates.
By clicking on one extension, a detail panel containing the "Uninstall" button
appears.
The multiple package uninstallation feature is also available.
All the packages checked can be uninstalled at one time by clicking the
"Uninstall Selected" button at the bottom left of the Panel.

The "Option" button is also present in detail Panels of the Enabled packages.

The new "Repair" button is also available in any extension panel.
It comes in use when an extension (included the Extension Manager itself) is
broken and needs to be restored to its original state.


### Tab " Available Extensions"

Shows all the Dispage extensions available in the DRC, each followed by the
Release, the Version,  the SugarCRM version compatibility list and the supported
languages.
If the extension is compatible with the running SugarCRM version, the "Install"
button appears in the detail panel as one extension is clicked on.

To check the SugarCRM compatibility of the installed extensions, the "Hide
installed Extensions" has to be unchecked.

The multiple packages installation feature is also available.
All the packages checked can be installed at one time by clicking the "Install
Selected" button at the bottom left of the Panel.


### Tab "Event Manager"

Shows the list of events related to the Dispage Extension management.

The grid allows to order the log by date, type and event.
Events can be filtered by:

-- Type (by selecting the event type in the Type header row).

-- Event (by typing a string in the Event header row and then pressing the
Filter icon on the left of the header row).

-- Date (by selecting a date in the Calendar or typing it in the Event header
row and then pressing the Filter icon on the left of the header row).
The Date filter shows all the events before the filter date.

To permanently delete the events from the log, the "Delete" button is available
on the footer menu of the Event Grid.

	
### Tab "Options"

#### Login Options
The Login options are set from this section.

1. The Username and Password of the Dispage portal can be entered from this
area.

2. The Automatic login option can be either activated/deactivated.

3. The "Non-Admin Automatic close" checkbox is available to allow the
Administrator to choose if the Login Popup automatically closes when a non-admin
user logs in.
Non-Admin users connect seamlessly to the (DRC) with the "Non-Admin Automatic
close" option enabled.

4. The "Disable automatic check for updates" option allows to disable the
automatic check for updates at login.

5. Dispage Non-Admin rules can be applied to the Admin users (except the
Administrator itself) specified in the "Apply Non-Admin rules to the Admin
Users" selection field.

#### Connection Options
This section is available to customize the following parameters used for the
Dispage connection:

1. Encode Response: option to receive a base64 encoded response from dispage.
CAUTION: base64 encoded string size is increased by 33% on average.

2. Connection attempts: number of attempts to connect to Dispage.

3. Timeout: timeout of the SOAP request to Dispage.

4. Response Timeout: timeout of the SOAP response from Dispage.

5. (NEW in 1.0.11) Proxy Settings: settings to connect to dipage.com through a
proxy server

#### Themes
Themes for the Dispage widgets can be selected from this section.

If switched to "Auto", Extension Manager automatically switches to the theme
closest to the SugarCRM main one each time the SugarCRM theme is changed.
