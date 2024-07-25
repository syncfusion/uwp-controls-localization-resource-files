# Localization of Syncfusion UWP Controls using .resw files    

This repository contains the default resources file (.resw) of Syncfusion UWP libraries. You can use this resource files to localize the strings for any selected language.

## Localization of Syncfusion UWP controls

Localization is the process of translating the application resources into different language for the specific cultures. You can localize the syncfusion UWP controls by adding resource file for each language.

### Changing application culture

When you are changing the application culture, then you can localize the application based on application culture by creating .resw file.

```
public MainPage()
{
    CultureInfo.CurrentUICulture = new CultureInfo("de");
    this.InitializeComponent();
}
```

### Creating a .resw file

You can create .resw files for any language by following steps,

1) Right click your project and click `New Folder` and set name as `Resources`.

2) Add the default resource file of libraries you are using to the `Resources` folder.

> Consider you are using `SfDataGrid` control in your application. Then you need to copy and include `Syncfusion.SfGrid.UWP.Resources.resw` (since `SfDataGrid` present in `Syncfusion.SfGrid.UWP` library) file in your application under `Resources` folder. So, now you can know the key names and values of default strings used in `Syncfusion.SfGrid.UWP.dll` library. 

![UWP DataGrid Localization](https://help.syncfusion.com/uwp/Localization_images/uwp-default-resw-file.png)

3) Now, right click on `Resources` folder and select `Add` and then `NewItem`. In the `Add New Item` wizard, select `Resources File` option and name the file name as `Syncfusion.SfGrid.UWP.Resources.<culture name>.resw`. For example, you have to give name as `Syncfusion.SfDataGrid.UWP.Resources.de.resw` for `German` culture. In the same way, add new resource files for other libraries used in your application.

![UWP DataGrid Localization](https://help.syncfusion.com/uwp/Localization_images/uwp-adding-resource-file.png)

4) Now, select `Add` and add resource file for german culture in `Resources` folder.

![UWP Localization using .resw file](https://help.syncfusion.com/uwp/Localization_images/uwp-resw-file-to-localize.png)

5) Now, you can copy the key names from default resource files and assign value based on the culture, the resource file targets.

![UWP Localization using key value of .resw file](https://help.syncfusion.com/uwp/Localization_images/uwp-localized-resw-file.png)

> Download demo from [GitHub](https://github.com/SyncfusionExamples/uwp-datagrid-localization)

## Editing default culture settings

You can change the default string of any control by adding the default .resw files ([from GitHub](https://github.com/syncfusion/uwp-controls-localization-resource-files)) to `Resources` folder of your application. Syncfusion UWP controls reads the default string from the .resw files of application if its added. 