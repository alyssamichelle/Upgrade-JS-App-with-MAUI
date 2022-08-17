# Upgrade-JS-App-with-MAUI

Presented at [DotNetConf](https://github.com/dotnet-presentations/dotNETConf), this repo is still a WIP. This application demonstrates how you can wrap and deploy a JS app using .NET MAUI to ship to mutiple platforms outside of the web.

Inside this repo you will find two innner projects:
- OurWebApp is the Angular Application
  - To serve, run `npm install` in the root and then `ng serve`
- WRAPPERAPP is the .NET MAUI-Blazor Hybrid app that I modified to wrap OurWebApp
  - To run, after installing dotnet and the workloads:
    - Run `dotnet build -t:Run -f net6.0-maccatalyst WRAPPERAPP.csproj` to see it for Mac desktop on Mac
    - or try `dotnet build -t:Run -f net6.0-android WRAPPERAPP.csproj` for Android

![image](https://user-images.githubusercontent.com/1058831/185188315-e2616575-4804-4689-8b95-36979cd243d2.png)
![image](https://user-images.githubusercontent.com/1058831/185188344-00c8ff45-0cab-45c9-9b98-a7b70078b75a.png)
