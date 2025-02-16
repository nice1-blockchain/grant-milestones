# Milestone Delivery

**The [invoice form](https://forms.gle/wLuAzXKa9qYrZQob9) has been filled out correctly for this milestone and the delivery is according to the official [milestone delivery guidelines](https://github.com/eosnetworkfoundation/grant-framework/blob/master/docs/milestone-deliverables-guidelines.md).**  

* **Application Document:** https://github.com/eosnetworkfoundation/grant-framework/blob/main/applications/nice1-tools-ecosystem.md
* **Milestone Number:** 1
* **Milestone Payment Amount:** $8,300 USD
* **Contact Name:** Javi Galvez
* **Contact email:** hello@nice1.org

## Context
The Nice1 Plugin for Unity is designed to provide seamless EOS blockchain authentication and integration for Unity developers, enabling secure interactions with blockchain-based applications across multiple platforms. This milestone encompasses critical deliverables that lay the foundation for a cross-platform authentication system leveraging EOS Anchor-Link.

- Core Components: The project includes a well-defined open-source license (Apache 2.0), comprehensive documentation, and unit tests to ensure the plugin’s reliability and ease of adoption.
- Authentication System: The integration of Anchor-Link within a Unity-compatible C# SDK enables a standardized authentication process across Mac, Windows, Linux, iOS, Android, and WebGL.
- Cross-Platform Support: The project initially aimed to develop a Webview plugin for authentication, but after a thorough analysis, we identified a more efficient approach by integrating an existing third-party C# Anchor-Link SDK. This allowed us to optimize development efforts while extending support to additional platforms.

## Deliverables
| Number | Deliverable | Link | Notes |
| ------------- | ------------- | ------------- |------------- |
| 0a. | **License** Apache 2.0 | https://github.com/nice1-blockchain/nice1-plugin/blob/master/LICENSE.txt | ...| 
| 0b.  | **Documentation** Documentation for Unity developers. | https://docs.nice1.dev/nice1-plugin/unity https://docs.nice1.dev/nice1-plugin/frequently-asked-questions | ...| 
| 0c.  | **Unit tests** Unit tests for the plugin | https://github.com/nice1-blockchain/nice1-plugin/tree/master/PluginTest https://github.com/nice1-blockchain/nice1-plugin/tree/master/PluginSource/UnitTest | ...| 
| 1.  | **Webview** Develop a webview plugin to call anchor-link functions. | https://github.com/nice1-blockchain/nice1-plugin/tree/master/UnityProject/Assets/Nice1/Plugins/WebView.bundle | By being able to find a solution based on the integration of C# Anchor-link SDK, we have not had to develop the webview for the Windows, MacOS and Linux platforms. Finally, the iOS, WebGL and Android platforms do work with Webview. | 
| 2.  | **C# Anchor-Link** Analyze the problem to develop a c# Anchor-link SDK. | https://github.com/nice1-blockchain/nice1-plugin/tree/master/UnityProject/Assets/Nice1/Plugins/UniversalAuthenticatorLibrarySharp |  Finally, and after several analyses of possible solutions, we found the library https://github.com/liquiidio/UniversalAuthenticatorLibraryUnity. We held discussions with the developer to adapt this solution to EOS (it was developed for WAX) and so we did. Therefore, we decided to increase the scope and not just stay in an analysis, but in a more advanced development that allows the use of this SDK for Windows, Mac and Linux platforms. | 
| 3.  | **Platform** Mac, Windows, Linux, Android and iOS version. | https://github.com/nice1-blockchain/nice1-plugin/tree/master/PluginSource | As an example of how the plugin works in an application, we have again chosen to use Legendary Legends, in this case for the Android mobile platform. You can watch the video of how it works: https://drive.google.com/file/d/16wPnJHOZlr2ukhVpriXi3xCG0iXaVSXt/view?usp=drive_link  In addition, we distribute the apk (https://drive.google.com/file/d/1wt0pdBKr1Y5sMGcye4yuPt2B57o2JRSa/view?usp=drive_link) so that you can test the execution of the application. Please note that it is prepared for jungle4 and a licensed account is required (request from Nice1)  | 

## Additional Information
There are deviations in number 1 (Webview) and 2 (C# Anchor-Link SDK) compared to the initial plan:
Webview: Initially, the development of a Webview plugin was planned to call Anchor-Link functions across all platforms. However, after analyzing the available options, we found that by integrating the C# Anchor-Link SDK, we could avoid the need to develop a Webview for Windows, MacOS, and Linux. As a result, only iOS, WebGL, and Android utilize Webview, while desktop platforms rely directly on the SDK integration.


C# Anchor-Link SDK: The original scope was to conduct an analysis of how to develop a C# Anchor-Link SDK. However, after exploring potential solutions, we identified an existing library, UniversalAuthenticatorLibraryUnity (initially developed for WAX), and collaborated with its developer to adapt and integrate it into EOS. This extended effort went beyond analysis, resulting in a functional implementation for Windows, MacOS, and Linux platforms, significantly increasing the deliverable's value.


These adjustments allowed us to optimize development efforts while maintaining and even expanding the project's impact across multiple platforms.

### Project Timeline and Justification for Delays

The initial project timeline was exceeded by several months due to the high complexity of developing and maintaining a solution across seven different platforms: iOS, Android, WebGL, Windows, Mac, and Linux. Each platform presented unique challenges in terms of compatibility, API differences, authentication mechanisms, and plugin integration, requiring significant development effort and extensive testing to ensure a consistent and reliable experience.
Moreover, the need to adapt an existing third-party library instead of developing everything from scratch allowed us to expand the project's scope, ultimately delivering a more robust and versatile solution. However, this decision also introduced unexpected technical hurdles that required additional time to resolve, particularly in adapting the authentication system to work seamlessly across all targeted platforms.
Despite these challenges, we have successfully delivered a fully functional, cross-platform solution that exceeds the initial scope in terms of usability and implementation depth.

### Ongoing Development and Adaptation to EOS Changes

Beyond the completion of the planned milestones, we remain actively engaged in continuous development to further improve the plugin, enhance documentation, and ensure long-term maintainability. Given the evolution of EOS over the past years, we are also working on adapting our implementation to align with the latest changes in the ecosystem, ensuring that our solution remains fully compatible and up to date with current and future developments in the EOS blockchain.
This commitment to continuous improvement guarantees that the Nice1 Plugin remains a reliable and scalable tool for developers building on EOS, with a focus on usability, security, and cross-platform performance.
