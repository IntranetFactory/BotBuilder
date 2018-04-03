This project is used just to build Microsoft.Bot.Connector.dll.
There are small adaptations of code according our needs, and:
- for project Microsoft.Bot.Connector.NetFramework target framework is changed from 4.6. to 4.5.2
- references to some dlls are updated to lower version, according framework 4.5.2, for what we have \lib folder:
	- System.Net.Http.dll
	- System.Net.Http.Formatting.dll
	- System.Web.Http.dll
- for now we have changed:
	\BotBuilder\CSharp\Library\Microsoft.Bot.Connector.Shared\MicrosoftAppCredentials.cs

It is needed just to rebuild Microsoft.Bot.Connector.NetFramework project with next steps
- open bin/debug folder below Microsoft.Bot.Connector.NetFramework project and delete all Microsoft.Bot.Connector.* files
- be sure that all packages are downloaded, and that dlls are in \packages subfolder
- right click on project Microsoft.Bot.Connector.NetFramework project in Solution explorer, and click on Rebuild.
- in bin/debug folder there are new builded Microsoft.Bot.Connector.* files.

That is all









