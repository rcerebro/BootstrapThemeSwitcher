Bootstrap Controls - How to implement Theme Switcher
This example demonstrates the way of creating a Bootstrap Theme Switcher User Control as in Devexpress Bootstrap demos (all themes are taken from the Bootswatch web site).
The selected theme name is stored in cookies.
HOW TO APPLY:
1. Add all three files in App_Code directory: BootstrapThemeModel.cs, BundleConfig.cs, ThemeModelBase.cs;
2. Add User Control BootstrapThemeSwitcher and register and add it on the page. In this example, it's registered and added on the Master Page Site.master; 
3. Add the SwitcherResources folder. It contains the Content and Scripts folders, the client resources for Theme Switcher User Control and Themes.xml file which contains the list of Bootstrap Themes.
After performing all actions above, you will have an attractive Theme Switcher like in our demos.
Description
BootstrapThemeSwitcher User Control contains an attribute ThemeLinkID and requires the value of the link's element id which is responsible for representing the current theme.
ThemeLinkID is connected with BootstrapThemeSwitcher's ASPxHiddenField and this value is used for changing the theme on the client side.


Credits: Team DevExpress
Source: https://github.com/DevExpress-Examples/bootstrap-controls-how-to-implement-theme-switcher-t547560