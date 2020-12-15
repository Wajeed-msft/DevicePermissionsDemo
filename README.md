# DevicePermissionsDemo
This is demo app to for device permissions.

## Getting started

1. Install some sort of tunnelling service. These instructions assume you are using ngrok: https://ngrok.com/
1. Begin your tunnelling service to get an https endpoint. For this example ngrok is used. Start an ngrok tunnel with the following command (you'll need the https endpoint for the bot registration):<br>

    ```bash
    ngrok http 3978 --host-header=localhost
    ```

1. Create an app manifest. Navigate to the file, manifest/manifest.json - Change:
    1. <<BASE_URI_DOMAIN>> change to your https endpoint from ngrok excluding the "https://" part
    1. Save the file and zip this file along with both the png icons (located next to it) together to create a manifest.zip file


## See it running

1. Clone the sample and open it in Visual Studio. (Look at [similar steps if you are not sure](https://docs.microsoft.com/microsoftteams/platform/tutorials/get-started-dotnet-app-studio#download-the-sample))
1. [Build and run your sample](https://docs.microsoft.com/microsoftteams/platform/tutorials/get-started-dotnet-app-studio#build-and-run-the-sample)
![Local Running App](Images/Local%20running%20app.png)
1. [Upload an app package](https://docs.microsoft.com/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) (Zip file created in step 3 above) to Microsoft Teams
![Install App](Images/Install%20App.png)
1. Go to Device Permissions Demo Tab.
1. Click on respective button to test the scenario. You will get prompt to accept permission request.
![Accept Permissions](Images/Accept%20Permissions.png)
1. You can also try this on Mobile.
![Mobile Demo](Images/Mobile%20Demo.png)

> [!IMPORTANT]
  > Please take a look at [notes section in Device Permissions](https://docs.microsoft.com/microsoftteams/platform/concepts/device-capabilities/native-device-permissions?tabs=desktop) documentation as not all devices support these permissions.

# Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
