# Mission Statement

Hello and welcome to the PowerTools github page.  PowerTools is a Dynamics 365 PowerApp that I hope will be embraced by the Dynamics 365 Community as the next big thing to enable high fidelity customizations as it matures.
The pillars of design/architecture are:

- **PowerTools live on the Power Platform** - This means that there is no standalone desktop application and that extensions live within the model driven application as a combination of web resources, flows, actions, entities, attributes, plugin code, azure extensions, etc.
- **PowerTools are modern-looking and fit the design of the new Unified Interface** - Dynamics 365, and most other products in the Microsoft 365 stack, have embraced the latest industry standards by utilizing frameworks such as React and Office-Fabric-UI. The benefits are self-evident after a bit of a learning curve.  PowerTools will follow suit with this initiative so that the customizations are seamless, fast to develop, and fast for the user.
- **PowerTools are readily available and always improving** - By hosting PowerTools in GitHub it is expected and encouraged that customizers fork PowerTools with their own repositories. Their solutions can stand alone on top of the PowerTools framework.  Based on a review process solutions from the community can be added via pull request into the master branch that is made publicly available. Due to all PowerTools being open source, enhancements can also come in via pull requests in addition to new solutions.  Since PowerTools is starting as an idea from Microsoft Employees there is a good chance that upon maturity it will have greater visibility in PowerApps by leveraging relationships within the product group.

## How is this different from XrmToolbox

I'm glad you asked.  XrmToolbox is a legend in the Dynamics 365 Community and contributes heavily to the inspiration of PowerTools.  But it's a desktop application.  And it's my opinion that with that comes challenges that may become unsurmountable as the product continues to advance.

- **Reason #1 - The removal of the Organization Service Endpoint**: As per [docs.microsoft.com](https://docs.microsoft.com/en-us/previous-versions/dynamicscrm-2016/developers-guide/dn281891(v=crm.8)#microsoft-dynamics-crm-2011-endpoint) it is strongly encouraged that developers use WebAPI over the Organization Service because it will eventually be removed.  Without the Organization Service Endpoint, it becomes much harder to have a standalone desktop application that connects to Dynamics because Azure Infrastucture needs to be stood up and tied to it in the form of an [ApplicationID](https://docs.microsoft.com/en-us/azure/active-directory/develop/howto-create-service-principal-portal)
- **Reason #2 - Industry Standards** - At a high level this could be summarized as *JavaScript has taken the world by storm*.  It's now being used as a language to stand up enterprise servers, is the basis for the most popular package manager in npm, and is being used to create modern desktop applications such as Micrsoft Teams and VSCode using electronjs.  By having strong preferences towards ReactJS and Office-Fabric-UI, PowerTools takes a stance as a JavaScript (and TypeScript) first solution.
- **Reason #3 - Branding** - The names speak for themselves.  The product is moving forward with the branding of *PowerApps* instead of *Xrm*.  XrmToolbox doesn't fit that nomenclature as well as PowerTools does.  As much as it shouldn't matter I think it still does.

## Getting Started

Head on over to <https://github.com/power-tools/hub.>  This repository hosts the source code for PowerTools along with an unmanaged solution that should be importable into any Dynamics 365 Environment. It also has a wiki with details on creating your own PowerTools solution.

I am aware that what I am proposing is no small task and would require a lot of rework. I truly think this is necessary though and with the industrious nature of our community and some buy-in could develop into something truly great.  Thanks for your time and if you have any questions feel free to email me at <brendon.colburn@gmail.com>. Or add an issue to the hub if you've found something wrong already :grin:
