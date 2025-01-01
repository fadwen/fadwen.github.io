- [PowerShell Resources](#powershell-resources)
  - [Practical Hands-on](#practical-hands-on)
  - [Books](#books)
  - [Videos](#videos)
  - [Discords](#discords)
- [Exchange Investigation, DNR, etc.](#exchange-investigation-dnr-etc)
- [VSCode](#vscode)
  - [VSCode Extensions](#vscode-extensions)
  - [More VSCode Goodies](#more-vscode-goodies)
- [Working with PowerShell](#working-with-powershell)
  - [Modules Commonly Used](#modules-commonly-used)
- [Test Lab](#test-lab)
  - [Lab Setup](#lab-setup)

# PowerShell Resources

## Practical Hands-on

- **[PSKoans](https://github.com/vexx32/PSKoans)**

- **[UnderTheWire Wargames](https://underthewire.tech/wargames)**
  - Fun little ssh challenges that require you to fact find on the host to get password to next ssh session . Practical and helps you think critically about solving issues without being spoon-fed.

- **[HacktheBox Academy](https://academy.hackthebox.com/)**
  - The free version can be frustrating due to laggy VPNs and non-responsive VMs. Interestingly, the very first day I made the account I didn't have this issue, it was in subsequent visits that performance degraded.

## Books

- **[Learn PowerShell in a Month of Lunches](https://www.manning.com/books/learn-PowerShell-in-a-month-of-lunches)**
  - I bought the physical copy and went through it. The authors recommend one chapter a day, but if you're not a complete beginner, you can get through chapter 8 before things start getting insightful. They try hard to sell PowerShell as good for Linux and Mac with the 4th edition. Which, if you want to do that then you do you do.

- **[PowerShell Practice and Style](https://poshcode.gitbook.io/PowerShell-practice-and-style)**

- **[Secrets of PowerShell Remoting](https://leanpub.com/secretsofpowershellremoting)**

## Videos

- **[PowerShell Master Class - PowerShell Fundamentals](https://www.youtube.com/watch?v=sQm4zRvvX58&list=PLlVtbbG169nFq_hR7FcMYg32xsSAObuq8)**

- **[Sessions from the PowerShell + DevOps Global Summit 2023](https://www.youtube.com/watch?v=MguCp6jdY20&list=PLfeA8kIs7Cof3Ev-KGonHLdFh8joxDFdW&pp=iAQB)**

- **[Sessions from the PowerShell Conference EU 2023](https://www.youtube.com/watch?v=ce2uZDaM5oE&list=PLDCEho7foSopknKI3VEqjdVpssJa41qs3)**

## Discords

- **[WinAdmins](https://discord.gg/winadmins)**
  - This is a good discord with a lot of MSPs who work with different stacks. It has active Microsoft MVPs and some actual Microsoft employees. Most of the server is active during East Coast business hours.

- **[PowerShell](https://discord.gg/PowerShell)**
  - A bunch of hard-hitting PowerShell nerds here, from people involved with the actual PowerShell GitHub/dev to those who manage aspects of VSCode. Very friendly place as I haven't been shamed for any of the pretty dumb questions I've put to them.

# Exchange Investigation, DNR, etc.

- [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com)
  - Hub for testing issues with Exchange, Teams, DNS. I often forget about it and have come up with some interesting work arounds. Put it here to try to remember. Doesn't work.

# VSCode

## VSCode Extensions

- [PowerShell Extension Pack](https://marketplace.visualstudio.com/items?itemName=justin-grote.PowerShell-extension-pack)
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- [Markdown Preview Enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)

## More VSCode Goodies

- [Viewing Default Settings in VS Code](https://ninmonkeys.com/blog/2022/05/01/viewing-default-settings-in-vs-code/)
- [VS Code Keybindings](https://code.visualstudio.com/docs/getstarted/keybindings#_basic-editing)
  - Good-to-know keybindings. Example: `CTRL + H` for find and replace makes things smoother.
- [Oh My Posh](https://ohmyposh.dev/docs/installation/windows)
  - Different themes for your terminal.  VS Code font types has to be setup through the Integrated Font Family settings.  Current favorites are `night-owl` and `quick-term`

# Working with PowerShell

> There are two versions of PowerShell.  Windows PowerShell `powershell.exe` that comes baked into the OS and PowerShell 7.x.x `pwsh.exe` which has to be downloaded and installed separately.  Install PowerShell 7 and make it your default in everything before you start installing modules as it will just make things easier.  Most modules developed after 2020 are intended for 7, and if you need to run something that errors and requires the 5.x of Windows PowerShell, you can use the `-UseWindowsPowerShell` switch when you import the modules.
>
> Also to note that PowerShell ISE does not support 7 and is not getting any new features.  Learn to use VSCode, install it on your servers, set up an ADMX with Intune to ensure only approved extensions and features are used.

## Modules Commonly Used

- ActiveDirectory
- Az
- ExchangeOnlineManagement
- Microsoft.Graph and Microsoft.Graph.Beta
  - This is an SDK so expect some different powershell inputs, using this you are dev-lite.  Install both, most functionality comes from mgbeta commands which hits the `/beta` api endpoint of graph.  Eventually as you learn graph you'll find that hitting the graph endpoints with `Invoke-WebRequest` direct can provide more functionality than this module.
- [Microsoft.Graph.Entra](https://github.com/microsoftgraph/entra-powershell) and Microsoft.Graph.Entra.Beta
  - This was made for Admins who weren't used to the structuring graph expects, and is a direct replacement for AzureAD module.
- Microsoft.Online.SharePoint.PowerShell
- Microsoft.PowerShell.ConsoleGuiTools
  - `Out-ConsoleGridView` is great for analyzing data within the terminal.
- Microsoft.PowerShell.GraphicalTools
  - `Out-Gridview` is a GUI popout for analyzing data.
- MicrosoftTeams
- PowerShellGet
  - This is only needed if you're running Windows PowerShell.  7.4 and later comes with Microsoft.PowerShell.PSResourceGet preinstalled.
- [PSClippy.FBP.CrossPlatform](https://github.com/HCRitter/PSClippy.FBP.CrossPlatform) 
  - For getting advices to improve cross platform scripts, while scripting.
- [ImportExcel](https://github.com/dfinke/ImportExcel)
  - Despite the module being **import** I most often use in exporting.  Working in a Google Workspace environment made me hate Sheets interactions with csv files so much that I became dependent on this module to export spreadsheets formatted properly.  It can do a ton of the Excel functions like autosize columns, pivot tables, and charts. 

# Test Lab #

## Lab Setup ##

 - [HydrationKit for WS22](https://github.com/DeploymentResearch/HydrationKitWS2022)
   - On-Prem Mockup WS22 AD, SCCM, SQL, and Workstations
 - [Microsoft 365 Test Environment](https://github.com/DevClate/365AutomatedLab)
   - If you don't have a dev tenant before they stopped issuing them.