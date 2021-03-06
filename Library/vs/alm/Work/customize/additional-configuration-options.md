Title: Additional configuration options | Team Foundation Server
Description: Topic description - Team Foundation Server
ms.TocTitle: Additional configuration options 
ms.ContentId: F89F5890-31E6-47EF-810F-AB75E1AE7E00


*This topic applies only to team projects hosted on an on-premises Team Foundation Server (TFS). Team projects on Visual Studio Online [update automatically with each service upgrade](https://www.visualstudio.com/news/release-archive-vso).  * 


<!---
Supports the following FWLINK: Additional configuration options are available - changes: http://go.microsoft.com/fwlink/?LinkID=242982 - 

-->
#Additional configuration options 

After you update your team project with the Configure Features wizard, you have access to the latest features. However, you may need to make some additional configurations or customizations to support your work tracking needs. Also, you have access to some features based on the source control setting selected when your team project was created.  

<table>
<tbody valign="top">
<tr>
<th width="15%">Feature</th>
<th width="35%">Usage</th>
<th width="50%">Configuration options</th>
</tr>
<tr>
<td>
Code Review
</td>
<td>
Adds the Code Review Request and Code Review Response work item types (WITs). With them, you can [request a code review and track code review responses](https://www.visualstudio.com/get-started/code/get-code-reviewed-vs).  
</td>
<td>
**Required: **[Configure an SMTP server for TFS](https://msdn.microsoft.com/library/ms400808.aspx). <br/>
**Required: **Visual Studio Premium or Visual Studio Ultimate installed.
**Availability: **Only supported when your team project uses Team Foundation version control for source control.
</td></tr>
<tr>
<td>
My Work
</td>
<td>
Adds support for automatic update of bug status when using My Work. Use to automate some activities when [developing code and managing pending changes](https://msdn.microsoft.com/library/ms245462.aspx#my_work).  
</td>
<td>
**Required: **Visual Studio Premium or Visual Studio Ultimate installed.
**Availability: **Only supported when your team project uses Team Foundation version control for source control.
</td>
</tr>
<tr>
<td>
Feedback
</td>
<td>
You can [request feedback](https://msdn.microsoft.com/library/hh301769.aspx) from your stakeholders and capture their comments on your working software. Reviewer feedback--in the form of videos, screenshots, type-written comments, and ratings--is captured into work items that you can review and use to create a bug or suggest a new backlog item. 
</td>
<td>
**Required: **Provide [Advanced access](../connect/change-access-levels.md) to users who'll request feedback.<br/>
**Required: **[Configure an SMTP server for TFS](https://msdn.microsoft.com/library/ms400808.aspx). <br/>
**Required: **[Grant stakeholders permission](https://msdn.microsoft.com/library/hh562968.aspx).

</td>
</tr>
<tr>
<td>
Planning Tools
</td>
<td>
These tools provide access to product and sprint backlogs, the Kanban board and task boards, and the ability to add teams.  
<ul>
<li>[Create-your-backlog](../backlogs/create-your-backlog.md) </li>
<li>[Kanban basics](../kanban/kanban-basics.md) </li>
<li>[Plan a sprint](../scrum/sprint-planning.md)</li>
<li>[Work with the task board](../scrum/task-board.md).</li>
</ul> </td>
<td>
**Required: **To work with sprint backlogs and boards, you must [activate the sprints for each team](../scrum/define-sprints.md). <br/>
Additional options that you can configure:<br/>
<ul>
<li>[Add a team or set up a hierarchy of teams](../scale/multiple-teams.md) </li>
<li>[Set team working days off](../scale/capacity-planning.md#team_settings)</li>
<li>[Define additional sprints or releases](../scrum/define-sprints.md).</li>
</ul> 
In addition, you can customize the following options by modifying the [ProcessConfiguration](https://msdn.microsoft.com/library/hh500408.aspx) definition:<br/>
<ul>
<li>Add fields to the quick add panel of backlogs</li>
<li>Change the color used to display work items</li>
<li>Change the default columns and column sequence of backlogs</li>
<li>Map metastates to customized WIT workflow states</li>
<li>Change the fields used in Agile tools and charts </li>
</ul> 
 
For additional customization options, see [Customize work tracking objects](customize-work.md).<br/>

If you've upgraded your TFS instance from [TFS 2010](#update-from-2010) or [TFS 2012](#update-from-2012), we recommend you update the workflow for select WITs to get the full functionality of your backlogs and boards. 
</td>
</tr>
<tr>
<td>
Storyboarding
</td>
<td>
With this feature, you can [storyboard your ideas using the Storyboarding add-in to PowerPoint](https://msdn.microsoft.com/library/hh409276.aspx).  
</td>
<td>
**Required: **[Office PowerPoint 2007 or later](http://www.microsoftstore.com/store/msstore/pd/PowerPoint-2010/productID.216564300)<br/>
**Required: **Visual Studio Community ([get your free download here](https://www.visualstudio.com/en-us/products/free-developer-offers-vs.aspx)) or other Visual Studio version installed. <br/>
To add and share Storyboard Shapes, go [here](https://msdn.microsoft.com/library/jj920186.aspx).<br/>
To add the Storyboards control to other WITs go [here](https://msdn.microsoft.com/library/hh500409%28v=vs.110%29.aspx#storyboard). 
</td>
</tr>
<tr>
<td>Portfolio Backlogs</td>
<td>With Portfolio Backlogs enabled, you can use the Feature and Epic portfolio backlogs to [organize your backlog](../backlogs/organize-backlog.md) by grouping related items into a hierarchical structure.  
</td>
<td>
Most of your team will be able to view and create Epics and Features once you've enabled the Portfolio Backlogs feature. However, you may need to enable one or more of these backlogs for a team as described in [Organize your backlogs](../backlogs/organize-backlog.md). <br/>

All stakeholders and contributors to your team project can view and add items to a portfolio backlog. However, to reorder, reparent, and exercise other portfolio backlog features, you need to have [Advanced access](../connect/change-access-levels.md).<br/>

<p>Other resources you may find useful to manage your teams and backlogs:</p>
<ul>
<li>[Agile Portfolio Management: Using TFS to support backlogs across multiple teams](https://msdn.microsoft.com/library/dn306083.aspx).</li>
<li>[Scaled Agile Framework: Using TFS to support epics, release trains, and multiple backlogs](https://msdn.microsoft.com/library/dn798712.aspx)</li>
<li>[Set up a hierarchy of teams](http://msdn.microsoft.com/library/hh500414.aspx) </li>
<li>[Add up to 5 levels of portfolio backlogs](add-portfolio-backlogs.md) </li>
</ul> 
</td>
</tr>
<tr>
<td>
Shared Parameters
</td>
<td>
This feature adds the Shared Parameters work item type (WIT). With it [you can repeat a test with different data](https://msdn.microsoft.com/library/dd997832.aspx). 
</td>
<td>
No additional configurations or customizations required. 
</td>
</tr>


<tr>
<td>
Test Plan and Test Suite
</td>
<td>
This feature adds the Test Plan and Test Suite WITs, and converts existing test plans and test suites to work items. With this feature enabled, you can now customize these WITs like other work items, and create queries to find test plans and test suites.  
</td>
<td>
To fully manage web-based test plans, you need to have [Advanced access](../connect/change-access-levels.md).<br/>
You can customize the test plan and test suite WITs in the same way you can customize other WITs. See these topics to learn more: <br/> 
<ul>
<li>[Field customizations](https://msdn.microsoft.com/library/dd695793.aspx): Add a custom field, modify a pick list, or add a field rule.</li>
<li>[Work item form customizations](https://msdn.microsoft.com/library/hh409273.aspx) : Modify the form layout for the bug, test case, test plan, or test suite.</li>
<li>[Workflow customizations](https://msdn.microsoft.com/library/hh409273.aspx) : Modify the workflow definitions for the bug, test case, test plan, or test suite.</li>
<li>[Test failure types](https://msdn.microsoft.com/library/ff398070.aspx): Specifies the reasons why a test run failed. The default configuration includes: Regression, New Issue, Known Issue, and Unknown.</li>
<li>[Test resolution states](https://msdn.microsoft.com/library/ff398070.aspx): Specifies the action to take after a test run failure. The default configuration includes: Needs investigation, Test issue, Product issue, and Configuration issue.</li>
</ul> 
If you add or change the workflow states for the test plan or test suite type definitions, review the [additional configuration requirements when working with  Visual Studio 2013.2 or earlier versions](#test-case-management). 
</td>

</tr>

<tr>
<td>
Bug Behavior
</td>
<td>
This feature allows teams to choose whether to track bugs like requirements or like tasks. 
</td>
<td>
To get started, each team must choose their preference as described in [Show bugs on backlogs and boards feature](show-bugs-on-backlog.md). 
</td>
</tr>
</tbody>
</table>

##Related notes 

If you are the server administrator for TFS and don't actually contribute to a team, then you may want to [remove yourself as a member, and add a project lead as the team administrator](https://msdn.microsoft.com/library/bb558971.aspx). (When you ran the Configure Features wizard, the system automatically added your user account as a team administrator for the team project.)

If you have updated a team project based on v5.0 of MSF for Agile, do the manual updates described in [Update the Workflow for Agile Team Projects](https://msdn.microsoft.com/library/hh500412.aspx).

<a id="test-case-management">   </a> 

###Test case management and custom workflow states 
If you add or change the workflow states for the test plan or test suite type definitions, and you work from a Test Manager client provided with Visual Studio 2013.2 or earlier versions, you must also update the process configuration for the team project as well. Otherwise, you’ll encounter an **Application detected an unexpected fault** error when you connect to your team project. 

![Application fault error message after TFS upgrade](_img/ALM_CF_AppFaultErrMsg.png)  

To resolve this error, see [Import and export process configuration [witadmin]](https://msdn.microsoft.com/library/hh500413.aspx).  

<a id="update-from-2012">   </a> 
###Recommended updates to team projects created from TFS 2012 process templates 

There are no additional required customizations to make after updating from TFS 2012 to TFS 2015. However, there are some recommended updates to make to the workflow of specific WITs.

The updates bring your team project up to date with the workflow settings that are defined in the latest versions of the default process templates. 

You might want to update the workflow of specific WITs to support missing transitions, additional reasons, and field assignments. Making this update revises the workflow for the following WITs to the latest version of their process template workflow: 

* Scrum 2.0 to Scrum 2013: Product Backlog Item and Bug  
* Agile 6.0 to Agile 2013: User Story  
* CMMI 6.0 to CMMI 2013: Requirement  

For details, see [Upgrade your 2012 team project from RTM to Update 2](http://blogs.msdn.com/b/visualstudioalm/archive/2013/04/04/upgrade-your-2012-process-template-from-rtm-to-update-2.aspx). You can learn about additional changes made to enable features from [Changes made to process templates](../guidance/changes-to-process-templates.md).


If you haven’t customized your work item types or process configuration, you can update the items quickly by using **witadmin**. Just [download the latest version of the process template](https://msdn.microsoft.com/library/ff452587.aspx) that is compatible with the one used to create your team project and then [import the updated WITs](https://msdn.microsoft.com/library/dd312129.aspx).

<a id="update-from-2010">   </a> 
###Recommended updates to team projects created from TFS 2010 process templates 

If you’ve updated a team project that was created with an MSF v 5.0 Agile process template, then you’ll also want to [manually update the user story and task workflow assignments](https://msdn.microsoft.com/library/hh500412.aspx). 

If you don't update the workflow, then the task board provides only two states, Active and Closed. This prevents you and your team from distinguishing between tasks that are in progress from those that haven't been started.

Also, you might want to apply the workflow updates to the User Story as described in [Upgrade your 2012 team project from RTM to Update 2](http://blogs.msdn.com/b/visualstudioalm/archive/2013/04/04/upgrade-your-2012-process-template-from-rtm-to-update-2.aspx). 
