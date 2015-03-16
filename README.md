# SymbolSource

-	Install the windbg sdk https://www.microsoft.com/click/services/Redirect2.ashx?CR_EAC=300135395. 
-	Create a new website in IIS for SymbolSource (using a subfolder of the NuGetGallery did not work for me because of inherited web.config that breaks SymbolSource server. I had to use a completely new site listening on another port)
- Publish the site from Visual Studio to IIS
-	Grant write permission on the App_Data, Data & Index folders to whatever user the SymbolServer application pool is running under
