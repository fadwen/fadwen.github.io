- [PowerShell Resources](#powershell-resources)
  - [Practical Hands-on](#practical-hands-on)
  - [Books](#books)
  - [Videos](#videos)
  - [Discords](#discords)
  - [Browser Extensions](#browser-extensions)
- [Exchange Investigation, DNR, etc.](#exchange-investigation-dnr-etc)
- [VSCode](#vscode)
  - [VSCode Extensions](#vscode-extensions)
  - [More VSCode Goodies](#more-vscode-goodies)
- [Working with PowerShell](#working-with-powershell)
  - [Modules Commonly Used](#modules-commonly-used)
- [Test Lab](#test-lab)
  - [Lab Setup](#lab-setup)
- [Certifications](#certifications)
  - [Axelos](#axelos)
    - [ITIL 4 Foundation](#itil-4-foundation)
  - [BetterCloud](#bettercloud)
    - [BetterCloud Certified Administrator](#bettercloud-certified-administrator)
  - [CompTIA](#comptia)
    - [A+](#a)
    - [Network+](#network)
    - [Security+](#security)
    - [Linux+](#linux)
  - [Microsoft](#microsoft)
    - [900s/foundations exams](#900sfoundations-exams)
    - [MD-102 – Endpoint Administrator](#md-102--endpoint-administrator)
    - [SC-300 – Identity and Access Administrator](#sc-300--identity-and-access-administrator)
    - [MS-102 – Enterprise Administrator](#ms-102--enterprise-administrator)
    - [AZ-104 – Azure Administrator](#az-104--azure-administrator)
    - [AZ-305 – Azure Solutions Architect](#az-305--azure-solutions-architect)
    - [AZ-800/801 – Windows Server Hybrid Administrator](#az-800801--windows-server-hybrid-administrator)
    - [Specialty: Azure Virtual Desktop](#specialty-azure-virtual-desktop)
  - [Okta](#okta)
    - [Okta Certified Professional](#okta-certified-professional)

# PowerShell Resources #

## Practical Hands-on ##

- **[PSKoans](https://github.com/vexx32/PSKoans)**

- **[UnderTheWire Wargames](https://underthewire.tech/wargames)**
  - Fun little ssh challenges that require you to fact find on the host to get password to next ssh session . Practical and helps you think critically about solving issues without being spoon-fed.

- **[HacktheBox Academy](https://academy.hackthebox.com/)**
  - The free version can be frustrating due to laggy VPNs and non-responsive VMs. Interestingly, the very first day I made the account I didn't have this issue, it was in subsequent visits that performance degraded.

## Books ##

- **[Learn PowerShell in a Month of Lunches](https://www.manning.com/books/learn-PowerShell-in-a-month-of-lunches)**
  - I bought the physical copy and went through it. The authors recommend one chapter a day, but if you're not a complete beginner, you can get through chapter 8 before things start getting insightful. They try hard to sell PowerShell as good for Linux and Mac with the 4th edition. Which, if you want to do that then you do you do.

- **[PowerShell Practice and Style](https://poshcode.gitbook.io/PowerShell-practice-and-style)**

- **[Secrets of PowerShell Remoting](https://leanpub.com/secretsofpowershellremoting)**

## Videos ##

- **[PowerShell Master Class - PowerShell Fundamentals](https://www.youtube.com/watch?v=sQm4zRvvX58&list=PLlVtbbG169nFq_hR7FcMYg32xsSAObuq8)**

- **[PowerShell + DevOps Global Summits](https://www.youtube.com/@PowershellOrg/playlists)**

- **[PowerShell Conferences EU](https://www.youtube.com/@PowerShellConferenceEU/playlists)**

- **[Getting Started with Graph](https://www.youtube.com/playlist?list=PLKROqDcmQsFls8cPHk3HFz2mUURHx46_O)**

## Discords ##

- **[WinAdmins](https://discord.gg/winadmins)**
  - This is a good discord with a lot of MSPs who work with different stacks. It has active Microsoft MVPs and some actual Microsoft employees. Most of the server is active during East Coast business hours.

- **[PowerShell](https://discord.gg/PowerShell)**
  - A bunch of hard-hitting PowerShell nerds here, from people involved with the actual PowerShell GitHub/dev to those who manage aspects of VSCode. Very friendly place as I haven't been shamed for any of the pretty dumb questions I've put to them.

## Browser Extensions ##

- [Centro 365](https://seanosullivan.co.uk/projects/centro365/welcome)
  - With every MS product having a portal and no connecting links, saves so much time flipping through tabs/bookmarks.
  
- [Graph X-Ray](https://graphxray.merill.net/)
  - Great way to see what GUI actions use Graph behind the scenes as well as translating to powershell for your own scripts.

- [Postman Interceptor](https://www.postman.com/product/postman-interceptor/)
  - For when you want to see the api query on something Graph X-ray/browser dev tools doesn't capture.


# Exchange Investigation, DNR, etc. #

- [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com)
  - Hub for testing issues with Exchange, Teams, DNS. I often forget about it and have come up with some interesting work arounds. Put it here to try to remember. Doesn't work.

# VSCode

> Note that PowerShell ISE does not support version 7+ and is not getting any new features.  Learn to use VSCode, install it on your servers, set up an ADMX with Intune to ensure only approved extensions and features are used.
>
> If VSCode is too dev-y and you really liked ISE [Powershell Studio](https://www.sapien.com/software/powershell_studio) is a solid replacement.  If you can get the approval to shell out for the $550 license.

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

# Certifications #

Personal thoughts on industry certification usefulness, all opinions my own.

## Axelos ##

Whether it was due to acquisition by PeopleCert or their own fault, this company is everything bad with the certification industry.  They make you pay a subscription in order to keep your digital badge up to date, they introduced renewals on their certs despite adding no new knowledge.  That being said they are firmly entrenched in the industry now, with Agile, ITIL, Prince2, PMP, etc.  We just have to suck it up and deal with their demands.

### ITIL 4 Foundation ###

- This establishes a framework that modern enterprises follow.  Change management, Issue vs Incident vs Problem, and a ton of other ITIL specific vocabulary that requires rote memorization.  This is a general purpose certification that adds value to a resume, whether you are technically inclined, sales, or management.  This used to be a lifetime certification, but now renews on a 3 year cycle, despite there being no revisions to the learning material.

## BetterCloud ##

The product itself is not complex, competing with other lifecycle management tools: Entra, Okta, etc.  It seems to have emphasis/more functionality on working with Google Workspace and Slack functionality over Microsoft offerings.  The plus side is their learning website gives you a free code to take their exams, on top of swag mailed to you on completion.

### BetterCloud Certified Administrator ###

 - This exam tests for competency in the product as an administrator: connecting to HRIS, connecting to IDP,  DLP options, etc. With a spoon fed free learning webinar that will walk you through what the exam tests on, if you fail it I assume you have never been in the admin portal at all.  Anecdotally I've never met another person who's worked in the product, and a recruiter has never reached out to me for it.

## CompTIA ##

These are great as they are vendor agnostic. The CompTIA certs are slightly costly, especially at the beginning of your career, ranging in the $300-400 price range per certification.  They last three years from earning if you don't get one that renews "[downstream](https://www.comptia.org/continuing-education/learn/renewing-multiple-certifications)".  They also renew/stay current if you get other vendor's certifications - my Microsoft ones renew everything I've earned.

### A+ ###
- The industry standard certification for IT professionals starting their careers. It's a mile wide and an inch deep.  It's there to introduce you to the basics of everything.  This one takes two tests to pass, you are not A+ certified until you pass both.  By itself, holds no weight on the resume, but will get you to the interview for entry level jobs.

### Network+ ###
- This focuses on wired and wireless networks with emphasis on subnetting without a calculator like a monster.  It will give foundational network familiarity that goes beyond what the A+ does.  If I had to do-over I would get a CCNA instead as it holds more weight and goes slightly beyond with ios commands.

### Security+ ###
- It covers key topics like network security, risk management, cryptography, and threat mitigation. This one is the one you'll get the most mileage out of on your resume.  Virtually any professional IT-adjacent would benefit from the concepts in this, you don't have to be shooting for a InfoSec or Pentest position.

### Linux+ ###
- Honestly I bought the voucher to Linux+ with the above CompTIA vouchers to get the most discount of my CompTIA Store subscription.  I took it a week before the voucher expired with 0 prep and passed.  TLDR: it teaches a surface level of Linux that anyone slightly familiar could pass, LPIC or RHEL certs would get more mileage.


## Microsoft ##

### 900s/foundations exams ###
- These last a lifetime and provide a very general overview of what that category/service entails.  They won’t add value to a resume or validate skills but it’s good to dip your feet in.  I picture these as existing for recruiters, non-technical managers to get an overall understanding, or a way to see if it’s something you’re interested in.
  **Note:**	Never pay for these as you can get for free via a [virtual training day](https://events.microsoft.com/en-us/mvtd?startTime=08:00&endTime=17:00) event.  Sign up for any event, join the day of, and earn a free voucher that’s applicable to any -900 not just the one you attended.  These happen at least twice a month in English, sign up for one and your inbox will forever be spammed on new ones.

All other MS exam vouchers cost $165 each and if passed the certification is valid for a year.  The option to renew being free and a self paced quiz via your Microsoft account that will also have some Learn pages with anything new compared to when you last took it.

An overall view of existing certifications and their prerequisites can be found at [Become Microsoft Certified](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE2PjDI) with click throughs to the specific exam(s) and the associated Learn pages.
Speaking of, the Learn pages are excellent study materials for the exams and completely free.  I would recommend the Learn pages over the Linkedin Learning videos on the same topic, as they are often out-of-date and incorrect from the few I’ve audited.

It’s tough to practice some of these outside of a production environment as things become more cloud based and the average subscriptions aren’t feasible for a personal user.  

You can setup a free trial via [Azure Free Trial | Microsoft Azure](https://azure.microsoft.com/en-us/pricing/offers/ms-azr-0044p/) and then further activate free trial licenses for various plans you are testing.  Be cautious when going this route as generally you have to put a card on file and if you’re not careful you may blow past the $200/mo free cap pretty easily.

### MD-102 – Endpoint Administrator ###
- A lot of people I’ve talked to think this is Microsoft’s equivalent of the A+ because it used to be called Managing Modern Desktops, but it provides a lot more value if you are working with the Windows stack.  This describes everything from the different versions of Windows (10/11, Home, Professional, Enterprise, etc), Windows Server, registry, active directory, as well as going in depth on prem/cloud solutions like GPO’s/OMA-URI’s, MDT/Autopilot, SCCM/Intune, WSUS/WufB.  I would really recommend this as the first Microsoft cert to get if you are dealing with workstations on a regular basis.  Also if you’re discussing with someone and they mention the old MCSA, this is the one that translates most to it.

### SC-300 – Identity and Access Administrator ###
- This is a great foundation for understanding the Entra tenant.  Users, groups, roles, application registrations, SSO, etc.  If you deal or are looking to deal with IAM, this would be a great validation/intro.

### MS-102 – Enterprise Administrator ###
- This is an Expert certification that builds on the knowledge from MD-102 and SC-300 as well as some voip/teams.  This has emphasis on building out a tenant, IAM, how to configure Defender, and managing retention/compliance policies with Purview.  This is the nearest equivalent of the older MCSE.

### AZ-104 – Azure Administrator ###
- This is great for showing you have the technical skills for Azure with an emphasis on DevOps.  Managing VMs, Networks, Subscriptions, Kubernetes clusters, and Storage solutions with Powershell, Az CLI, or ARM templates to implement them to describe a few.

### AZ-305 – Azure Solutions Architect ###
- This is an Expert level certification with AZ-104 as a pre-requisite.  While AZ-104 focuses on the technical aspects and how to implement, this focuses on the why.  Emphasis on VM change control, network peering/failover, disaster recovery solutions, choosing different SQL implementations, requirements to shift from on-prem to cloud, and auditing role assignments between subscriptions as some examples.

### AZ-800/801 – Windows Server Hybrid Administrator ###
- Unlike the MD/MS-102 Microsoft hasn’t combined both into a single exam yet and there is some overlap.  In most companies you’ll have a hybrid tenant at some level not pure cloud (unless you get lucky) and the Learn pages will provide a great benefit in the configuration needed to implement it.  This is also really the only path currently available for Windows Server skill validation.

### Specialty: Azure Virtual Desktop ### 
- AVD is currently hands down the best-in-class solution for VDI’s from both a cost and feature perspective.  If you are familiar with Citrix or VMware’s Horizon this is Microsoft’s implementation and they did it surprisingly well.  More and more companies use VDI’s to cut down on costs associated with hardware/power/licensing.  This will show/validate what skills are needed to run and administrate it.

## Okta ##

Okta tests are interesting in that you cannot go back and review your answers/change them.  The format I've had is that each question is weighted and you have to choose the best answer, not necessarily the right answer.

### Okta Certified Professional ###

- This is a bit more intensive than a -900 from Microsoft but still geared to Sales, Managers, or entry level administrators.  You'll know the capabilities of the product and a base level of things to do with it.  I earned mine while having basic help desk permissions within the product, and renewed it successfully on my first try after not touching it for two years and no studying.  I'm not sure if this adds anything of value to your resume for job seekers.