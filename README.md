 <div align="center"> 

<p>This page is used to keep track of resources used in my professional development, or things I have found afterward that I wish I had known.</p>

<p>
<a href="https://hits.seeyoufarm.com">
    <img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Ffadwen.github.io&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false" alt="hits">
</a>
<a href="https://www.linkedin.com/in/jeffrey-stuhr-034214aa/">
    <img src="https://img.shields.io/badge/LinkedIn-blue?style=flat-square&logo=linkedin" alt="LinkedIn">
</a>
<a href="https://bsky.app/profile/techbyjeff.net">
    <img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fpublic.api.bsky.app%2Fxrpc%2Fapp.bsky.actor.getProfile%2F%3Factor%3Dtechbyjeff.net&query=%24.followersCount&style=social&logo=bluesky&label=Follow%20on%20BSky" alt="BlueSky">
</a>
<a href="https://techbyjeff.net">
    <img src="https://img.shields.io/badge/Read%20My%20Blog-grey?style=flat-square&logo=ghost" alt="Blog">
</a>
</p>

</div>

## Table of Contents <!-- omit in toc -->

- [PowerShell Resources](#powershell-resources)
  - [Books](#books)
  - [Browser Extensions](#browser-extensions)
  - [Discords](#discords)
  - [Practical Hands-on](#practical-hands-on)
  - [Videos](#videos)
  - [Websites](#websites)
- [VSCode](#vscode)
  - [VSCode Extensions](#vscode-extensions)
  - [More VSCode Goodies](#more-vscode-goodies)
- [Working with PowerShell](#working-with-powershell)
  - [Modules Commonly Used](#modules-commonly-used)
    - [Microsoft Modules](#microsoft-modules)
    - [3rd Party Modules](#3rd-party-modules)
- [MgGraph bits](#mggraph-bits)
- [Useful non-portal MS websites](#useful-non-portal-ms-websites)
  - [365 Configuration Tool](#365-configuration-tool)
  - [Graph Explorer](#graph-explorer)
  - [Microsoft Remote Connectivity Analyzer](#microsoft-remote-connectivity-analyzer)
- [Test Lab](#test-lab)
  - [Lab Setup](#lab-setup)
- [Certifications](#certifications)
  - [~~Axelos~~ PeopleCert](#axelos-peoplecert)
    - [ITIL 4 Foundation](#itil-4-foundation)
  - [BetterCloud](#bettercloud)
    - [BetterCloud Certified Administrator](#bettercloud-certified-administrator)
  - [CompTIA](#comptia)
    - [A+](#a)
    - [Network+](#network)
    - [Security+](#security)
    - [Linux+](#linux)
  - [Microsoft](#microsoft)
    - [-900s/foundations exams](#-900sfoundations-exams)
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

## Books ##

- **[Learn PowerShell in a Month of Lunches](https://www.manning.com/books/learn-powershell-in-a-month-of-lunches)**
  - The authors recommend one chapter a day, but if you're not a complete beginner, you can get through chapter 8 before things start getting insightful. Really informative book that I wish I'd been recommended instead of stumbling through trial and error.

- **[Learn PowerShell Scripting in a Month of Lunches](https://www.manning.com/books/learn-powershell-scripting-in-a-month-of-lunches-second-edition)**
  - This goes above and beyond the aforementioned book, assuming your familiarity and that you are now writing your own modules/functions.  Has some things on pestering as well.
  - [Companion Github](https://github.com/psjamesp/MOL-Scripting/tree/main)

- **[Secrets of PowerShell Remoting](https://leanpub.com/secretsofpowershellremoting)**
  - Honestly any of the [DevOps Collective](https://leanpub.com/u/devopscollective) books are recommended.

[🔝 Back to Top](#toc)

## Browser Extensions ##

- [Centro 365](https://seanosullivan.co.uk/projects/centro365/welcome)
  - With every MS product having a portal and no connecting links, saves so much time flipping through tabs/bookmarks.
  
- [Graph X-Ray](https://graphxray.merill.net/)
  - Great way to see what GUI actions use Graph behind the scenes as well as translating to powershell for your own scripts.

- [Postman Interceptor](https://www.postman.com/product/postman-interceptor/)
  - For when you want to see or replay the api query on something Graph X-ray/browser dev tools doesn't capture.

[🔝 Back to Top](#toc)

## Discords ##

- **[PowerShell](https://discord.gg/PowerShell)**
  - A bunch of hard-hitting PowerShell nerds here, from people involved with the actual PowerShell GitHub/dev to those who manage aspects of VSCode. Very friendly place as I haven't been shamed for any of the pretty dumb questions I've put to them.

- **[WinAdmins](https://discord.gg/winadmins)**
  - This is a good discord with a lot of MSPs who work with different stacks. It has active Microsoft MVPs and some actual Microsoft employees. Most of the server is active during East Coast business hours.

[🔝 Back to Top](#toc)

## Practical Hands-on ##

- **[HacktheBox Academy](https://academy.hackthebox.com/)**
  - The free version can be frustrating due to laggy VPNs and non-responsive VMs. Interestingly, the very first day I made the account I didn't have this issue, it was in subsequent visits that performance degraded.

- **[PSKoans](https://github.com/vexx32/PSKoans)**

- **[UnderTheWire Wargames](https://underthewire.tech/wargames)**
  - Fun little ssh challenges that require you to fact find on the host to get password to next ssh session . Practical and helps you think critically about solving issues without being spoon-fed.

[🔝 Back to Top](#toc)

## Videos ##

- **[PowerShell Master Class - PowerShell Fundamentals](https://www.youtube.com/watch?v=sQm4zRvvX58&list=PLlVtbbG169nFq_hR7FcMYg32xsSAObuq8)**

- **[PowerShell + DevOps Global Summits](https://www.youtube.com/@PowershellOrg/playlists)**

- **[PowerShell Conferences EU](https://www.youtube.com/@PowerShellConferenceEU/playlists)**

- **[Getting Started with Graph](https://www.youtube.com/playlist?list=PLKROqDcmQsFls8cPHk3HFz2mUURHx46_O)**

[🔝 Back to Top](#toc)

## Websites ##

- **[Deep Dives on MSLearn](https://learn.microsoft.com/en-us/powershell/scripting/learn/deep-dives/overview?view=powershell-7.4&viewFallbackFrom=powershell-7.3)**

- **[PowerShell Practice and Style](https://poshcode.gitbook.io/PowerShell-practice-and-style)**

- **[RegExLibrary](https://regexlib.com/)**
  - While not PowerShell specific, useful for regex examples. [RegEx Tester](https://www.regextester.com/) can be used to validate.

- **[Sample Code](https://powershell.one/code)**

[🔝 Back to Top](#toc)

# VSCode

> Note that PowerShell ISE does not support version 7+ and is not getting any new features.  Learn to use VSCode, install it on your servers that used ISE, set up an ADMX with Intune to ensure only approved extensions and features are used.
> 
> Tunnels are a great remoting feature if you secure them properly.
>
> If VSCode is too dev-y and you really liked ISE [Powershell Studio](https://www.sapien.com/software/powershell_studio) is a solid replacement.  If you can get the approval to shell out for the $550 license.

## VSCode Extensions

- [PowerShell Extension Pack](https://marketplace.visualstudio.com/items?itemName=justin-grote.PowerShell-extension-pack)
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- [Markdown Preview Enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)

[🔝 Back to Top](#toc)

## More VSCode Goodies

- [Viewing Default Settings in VS Code](https://ninmonkeys.com/blog/2022/05/01/viewing-default-settings-in-vs-code/)
- [VS Code Keybindings](https://code.visualstudio.com/docs/getstarted/keybindings#_basic-editing)
  - Good-to-know keybindings. Example: `CTRL + H` for find and replace makes things smoother.
- [Oh My Posh](https://ohmyposh.dev/docs/installation/windows)
  - Different themes for your terminal.  VS Code font types has to be setup through the Integrated Font Family settings.  `$PROFILE` for VSCode is separate from your non-vscode pwsh. Current favorites are `night-owl` and `quick-term`.

[🔝 Back to Top](#toc)

# Working with PowerShell

> There are two versions of PowerShell.  Windows PowerShell `powershell.exe` that comes baked into the OS and PowerShell 7.x.x `pwsh.exe` which has to be downloaded and installed separately.  Install PowerShell 7 and make it your default in everything before you start installing modules as it will just make things easier.  Most modules developed after 2020 are intended for 7, and if you need to run something that errors and requires the 5.x of Windows PowerShell, you can use the `-UseWindowsPowerShell` switch when you import the modules.

## Modules Commonly Used

### Microsoft Modules ###

- ActiveDirectory
- Az
- ExchangeOnlineManagement
- Microsoft.Graph and Microsoft.Graph.Beta 
  - This is an SDK so expect some different powershell inputs, using this you are dev-lite.  Install both, most functionality comes from mgbeta commands which hits the `/beta` api endpoint of graph.  Eventually as you learn graph you'll find that hitting the graph endpoints with `Invoke-WebRequest`or `Invoke-RestMethod` direct can provide more functionality than this module.  The Microsoft.Graph.PlusPlus module below helps if you really hate the structure.
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

[🔝 Back to Top](#toc)

### 3rd Party Modules ###
**Always make sure to assess and evaluate before implementing in production.**
- [Graph EasyPIM](https://github.com/rakheshster/PowerShell-GraphEasyPIM) ![PowerShell Gallery Downloads](https://img.shields.io/powershellgallery/dt/Graph.EasyPIM)
  - Activating PIM roles via CLI rather than GUI blades.
- [ImportExcel](https://github.com/dfinke/ImportExcel) ![PowerShell Gallery Downloads](https://img.shields.io/powershellgallery/dt/ImportExcel)
  - Despite the module being **import** I most often use in exporting.  Working in a Google Workspace environment made me hate Sheets interactions with csv files so much that I became dependent on this module to export spreadsheets formatted properly.  It can do a ton of the Excel functions like autosize columns, pivot tables, and charts. 
- [Microsoft.Graph.PlusPlus](https://github.com/jhoneill/MsftGraph) ![PowerShell Gallery Downloads](https://img.shields.io/powershellgallery/dt/Microsoft.Graph.PlusPlus)

  - Extends Microsoft.Graph SDK to be more PowerShell like.
- [platyPS](https://github.com/PowerShell/platyPS) ![PowerShell Gallery Downloads](https://img.shields.io/powershellgallery/dt/platyPS)
  - Great for building out documentation for modules you make once you get used to the schema it needs.
- [PSClippy.FBP.CrossPlatform](https://github.com/HCRitter/PSClippy.FBP.CrossPlatform) 
  - For getting advices to improve cross platform scripts, while scripting.
- [psframework](https://github.com/PowershellFrameworkCollective/psframework) ![PowerShell Gallery Downloads](https://img.shields.io/powershellgallery/dt/psframework)

  - A great logging module that I wish I had found years ago, saves so much time.  Found more use cases than logging, makes some Param functions simpler.

[🔝 Back to Top](#toc)

# MgGraph bits #

  - [Find-MgGraphCommand](https://learn.microsoft.com/en-us/powershell/microsoftgraph/find-mg-graph-command?view=graph-powershell-1.0) 
    - To see what perms are needed, as well as URI it is hitting.
  - [Find-MgGraphPermission](https://learn.microsoft.com/en-us/powershell/microsoftgraph/find-mg-graph-permission?view=graph-powershell-1.0) 
    - To look up details on the permission that a script/app has.
  - [Invoke-MgGraphRequest](https://learn.microsoft.com/en-us/powershell/module/microsoft.graph.authentication/invoke-mggraphrequest?view=graph-powershell-1.0)
    - Cleaner Graph specific invoke that can be used rather than `Invoke-WebRequest` or `Invoke-RestMethod` if the API endpoint does not have a cmdlet built out with all options yet.

[🔝 Back to Top](#toc)

# Useful non-portal MS websites #

## [365 Configuration Tool](https://config.office.com/deploymentsettings)
 - I often see people deploying scripts or remediations for Office configs when this tool should be used instead.

## [Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer)
  - Useful to explore Graph's URI structure, needed permissions, and responses.

## [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com) ##
  - Hub for testing issues with Exchange, Teams, DNS. I often forget about it and have come up with some interesting work arounds. Put it here to try to remember. Doesn't work.

[🔝 Back to Top](#toc)

# Test Lab #

## Lab Setup ##

 - [HydrationKit for WS22](https://github.com/DeploymentResearch/HydrationKitWS2022)
   - On-Prem Mockup WS22 AD, SCCM, SQL, and Workstations
 - [Microsoft 365 Test Environment](https://github.com/DevClate/365AutomatedLab)
   - If you don't have a dev tenant before they stopped issuing them.
 - [Cybersecurity Lab](https://benheater.com/proxmox-laptop-cybersecurity-lab/)  
   - Focuses on Proxmox as the hypervisor, Wazuh SIEM, and various pentesting VMs.
 - [Ludus](https://docs.ludus.cloud/docs/category/quick-start)
   - Another Debian/Proxmox specific, but completely takes over so if you need the host for other things be warned.

[🔝 Back to Top](#toc)

# Certifications #

Personal thoughts on industry certification usefulness, all opinions my own.

## ~~Axelos~~ PeopleCert ##

Whether it was due to acquisition by PeopleCert or their own fault, this company is everything bad with the certification industry.  They make you pay a subscription in order to keep your digital badge up to date, they introduced renewals on their certs despite adding no new knowledge.  That being said they are firmly entrenched in the industry now, with Agile, ITIL, Prince2, PMP, etc.  We just have to suck it up and deal with their demands.

[🔝 Back to Top](#toc)

### [ITIL 4 Foundation](https://www.axelos.com/certifications/itil-service-management/itil-4-foundation) ###

- This establishes a framework that modern enterprises follow.  Change management, Issue vs Incident vs Problem, and a ton of other ITIL specific vocabulary that requires rote memorization.  This is a general purpose certification that adds value to a resume, whether you are technically inclined, sales, or management.  This used to be a lifetime certification, but now renews on a 3 year cycle, despite there being no revisions to the learning material.

[🔝 Back to Top](#toc)

## BetterCloud ##

The product itself is not complex, competing with other lifecycle management tools: Entra, Okta, etc.  It seems to have emphasis/more functionality on working with Google Workspace and Slack functionality over Microsoft offerings.  The plus side is their [Flight School website](https://www.bettercloud.com/training/) gives you a free code to take their exams, on top of swag mailed to you on completion.

[🔝 Back to Top](#toc)

### [BetterCloud Certified Administrator](https://learn.bettercloud.com/path/certification) ###

 - This exam tests for competency in the product as an administrator: connecting to HRIS, connecting to IDP,  DLP options, etc. With a spoon fed free learning webinar that will walk you through what the exam tests on, if you fail it I assume you have never been in the admin portal at all.  Anecdotally I've never met another person who's worked in the product, and a recruiter has never reached out to me for it.

[🔝 Back to Top](#toc)

## CompTIA ##

These are great as they are vendor agnostic. The CompTIA certs are slightly costly, especially at the beginning of your career, ranging in the $300-400 price range per certification.  They last three years from earning if you don't get one that renews "[downstream](https://www.comptia.org/continuing-education/learn/renewing-multiple-certifications)".  They also renew/stay current if you get other vendor's certifications - my Microsoft ones renew everything I've earned.

There are plenty of learning sources out there, but I can't recommend [ProfessorMesser](https://www.professormesser.com/) enough for the "CompTIA Trifecta" (A/Net/Sec).  His Youtube playlists are updated to the latest versions, comprehensive, and always free.

[🔝 Back to Top](#toc)

### [A+](https://www.comptia.org/certifications/a) ###
- The industry standard certification for IT professionals starting their careers. It's a mile wide and an inch deep.  It's there to introduce you to the basics of everything.  This one takes two tests to pass, you are not A+ certified until you pass both.  By itself, holds no weight on the resume, but will get you to the interview for entry level jobs.

[🔝 Back to Top](#toc)

### [Network+](https://www.comptia.org/certifications/network) ###
- This focuses on wired and wireless networks with emphasis on subnetting without a calculator like a monster.  It will give foundational network familiarity that goes beyond what the A+ does.  If I had to do-over I would get a CCNA instead as it holds more weight and goes slightly beyond with ios commands.

[🔝 Back to Top](#toc)

### [Security+](https://www.comptia.org/certifications/security) ###
- It covers key topics like network security, risk management, cryptography, and threat mitigation. This one is the one you'll get the most mileage out of on your resume.  Virtually any professional IT-adjacent would benefit from the concepts in this, you don't have to be shooting for a InfoSec or Pentest position.

[🔝 Back to Top](#toc)

### [Linux+](https://www.comptia.org/certifications/linux) ###
- Honestly I bought the voucher to Linux+ with the above CompTIA vouchers to get the most discount of my CompTIA Store subscription.  I took it a week before the voucher expired with 0 prep and passed.  TLDR: it teaches a surface level of Linux that anyone slightly familiar could pass, LPIC or RHEL certs would get more mileage.

[🔝 Back to Top](#toc)

## Microsoft ##

This mainly goes into the certifications as those add value to the resume/employers, but Microsoft does have something relatively new called [Applied Skills](https://learn.microsoft.com/en-us/credentials/browse/?credential_types=applied%20skills) which are free to take and showcase your proficiency in a specific task.  I'm not sure if they are prestigious enough to add to a resume, but it can certainly validate a role-based skill if you're looking to make an internal move.

[🔝 Back to Top](#toc)

### [-900s/foundations exams](https://learn.microsoft.com/en-us/credentials/browse/?credential_types=certification&levels=beginner) ###
- These last a lifetime and provide a very general overview of what that category/service entails.  They won’t add value to a resume or validate skills but it’s good to dip your feet in.  I picture these as existing for recruiters, non-technical managers to get an overall understanding, or a way to see if it’s something you’re interested in.
  - **Note:**	Never pay for these as you can get for free via a [virtual training day](https://events.microsoft.com/en-us/mvtd?startTime=08:00&endTime=17:00) event.  Sign up for any event, join the day of, and earn a free voucher that’s applicable to any -900 not just the one you attended.  These happen at least twice a month in English, sign up for one and your inbox will forever be spammed on new ones.

All other MS exam vouchers cost $165 each and if passed the certification is valid for a year.  The option to renew being free and a self paced quiz via your Microsoft account that will also have some Learn pages with anything new compared to when you last took it.

An overall view of existing certifications and their prerequisites can be found at [Become Microsoft Certified](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE2PjDI) with click throughs to the specific exam(s) and the associated Learn pages.
Speaking of, the Learn pages are excellent study materials for the exams and completely free.  I would recommend the Learn pages over the Linkedin Learning videos on the same topic, as they are often out-of-date and incorrect from the few I’ve audited.  Familiarizing yourself with the content in Learn is great since you can now access Learn pages during the exam.

It’s tough to practice some of these outside of a production environment as things become more cloud based and the average subscriptions aren’t feasible for a personal user.

You can setup a free trial via [Azure Free Trial](https://azure.microsoft.com/en-us/pricing/offers/ms-azr-0044p/) and then further activate free trial licenses for various plans you are testing.  Be cautious when going this route as generally you have to put a card on file and if you’re not careful you may blow past the $200/mo free cap pretty easily.  Also check out the [Lab Setup](#lab-setup) section to create your own, keeping in mind for some cloud features you may be charged if you go on past trial dates.

[🔝 Back to Top](#toc)

### [MD-102 – Endpoint Administrator](https://learn.microsoft.com/en-us/credentials/certifications/modern-desktop/?practice-assessment-type=certification&WT.mc_id=certposter_poster-wwl) ###
- A lot of people I’ve talked to think this is Microsoft’s equivalent of the A+ because it used to be called Managing Modern Desktops, but it provides a lot more value if you are working with the Windows stack.  This describes everything from the different versions of Windows (10/11, Home, Professional, Enterprise, etc), Windows Server, registry, active directory, as well as going in depth on prem/cloud solutions like GPO’s/OMA-URI’s, MDT/Autopilot, SCCM/Intune, WSUS/WufB.  I would really recommend this as the first Microsoft cert to get if you are dealing with workstations on a regular basis.  Also if you’re discussing with someone and they mention the old MCSA, this is the one that translates most to it.

[🔝 Back to Top](#toc)

### [SC-300 – Identity and Access Administrator](https://learn.microsoft.com/en-us/credentials/certifications/identity-and-access-administrator/?practice-assessment-type=certification&WT.mc_id=certposter_poster-wwl) ###
- This is a great foundation for understanding the Entra tenant.  Users, groups, roles, application registrations, SSO, etc.  If you deal or are looking to deal with IAM, this would be a great validation/intro.

[🔝 Back to Top](#toc)

### [MS-102 – Enterprise Administrator](https://learn.microsoft.com/en-us/credentials/certifications/m365-administrator-expert/?WT.mc_id=certposter_poster-wwl) ###
- This is an Expert certification that builds on the knowledge from MD-102 and SC-300 as well as some voip/teams.  This has emphasis on building out a tenant, IAM polices like Conditional Access, how to configure Defender, and managing retention/compliance policies with Purview.  This is the nearest equivalent of the older MCSE.

[🔝 Back to Top](#toc)

### [AZ-104 – Azure Administrator](https://learn.microsoft.com/en-us/credentials/certifications/azure-administrator/?practice-assessment-type=certification&WT.mc_id=certposter_poster-wwl) ###
- This is great for showing you have the technical skills for Azure with an emphasis on DevOps.  Managing VMs, Networks, Subscriptions, Kubernetes clusters, and Storage solutions with Powershell, Az CLI, or ARM templates to implement them to describe a few.

[🔝 Back to Top](#toc)

### [AZ-305 – Azure Solutions Architect](https://learn.microsoft.com/en-us/credentials/certifications/azure-solutions-architect/?WT.mc_id=certposter_poster-wwl) ###
- This is an Expert level certification with AZ-104 as a pre-requisite.  While AZ-104 focuses on the technical aspects and how to implement, this focuses on the why.  Emphasis on VM change control, network peering/failover, disaster recovery solutions, choosing different SQL implementations, requirements to shift from on-prem to cloud, and auditing role assignments between subscriptions as some examples.

[🔝 Back to Top](#toc)

### [AZ-800/801 – Windows Server Hybrid Administrator](https://learn.microsoft.com/en-us/credentials/certifications/windows-server-hybrid-administrator/?WT.mc_id=certposter_poster-wwl) ###
- Unlike the MD/MS-102 Microsoft hasn’t combined both into a single exam yet and there is some overlap.  In most companies you’ll have a hybrid tenant at some level not pure cloud (unless you get lucky) and the Learn pages will provide a great benefit in the configuration needed to implement it.  This is also really the only path currently available for Windows Server skill validation.

[🔝 Back to Top](#toc)

### [Specialty: Azure Virtual Desktop](https://learn.microsoft.com/en-us/credentials/certifications/azure-virtual-desktop-specialty/?practice-assessment-type=certification&WT.mc_id=certposter_poster-wwl) ### 
- AVD is currently hands down the best-in-class solution for VDI’s from both a cost and feature perspective.  If you are familiar with Citrix or VMware’s Horizon this is Microsoft’s implementation.  More and more companies use VDI’s to cut down on costs associated with hardware/power/licensing.  This will show/validate what skills are needed to implement and administrate it.

[🔝 Back to Top](#toc)

## Okta ##

Okta tests are interesting in that you cannot go back and review your answers/change them.  The format I've had is that each question is weighted and you have to choose the best answer, not necessarily the only right answer.

[🔝 Back to Top](#toc)

### [Okta Certified Professional](https://certification.okta.com/okta-certified-professional-hands-on-configuration-exam-for-oie) ###

- This is a bit more intensive than a -900 from Microsoft but still geared to Sales, Managers, or entry level administrators.  You'll know the capabilities of the product and a base level of things to do with it.  I earned mine while having basic help desk permissions within the product, and renewed it successfully on my first try after not touching it for two years and no studying.  I'm not sure if this adds anything of value to your resume for job seekers, more of a progression internally if you are in a company with the product.

[🔝 Back to Top](#toc)