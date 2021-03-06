Title: Task board | Visual Studio Online
Description: How to work with the Scrum task board when working in Visual Studio Online and team projects connected to Team Foundation Server (TFS)
ms.TocTitle: Task board
ms.ContentId: 278BF8D9-E34F-4D14-BACC-D3BA704C2C47


#Task board
Once you have your [sprint plan](sprint-planning.md) in place, you'll execute that plan for the duration of the sprint. In your daily Scrum meetings, your team can view progress made to backlog items and tasks from the sprint task board.  

Your task board provides a visualization of flow and status of each sprint task. With it, you can focus on the status of backlog items as well as work assigned to each team member. It also summarizes the total amount of remaining work to complete for a task or within a column.  

![Task board, collapsed backlog items](_img/ALM_TB_Intro.png)

<blockquote style="font-size: 13px"><b>Tip:  </b>You can [customize cards](../customize/customize-cards.md) that appear on the task board to show additional fields.  Also, your team can choose to manage bugs similar to product backlog items, as shown in this topic, or manage them similar to tasks. When you track bugs similar to tasks, they’ll show up on your sprint backlogs and task boards at the same level as tasks. [Show bugs on backlogs or boards](../customize/show-bugs-on-backlog.md) provides the details.   </blockquote>  

Your team can use the task board to perform these tasks throughout the sprint:  

*	Update task status and remaining work  
*	Review progress with the team during the [daily Scrum meetings](#daily-scrum-meetings)  
*	Update items and address uncompleted work at the close of the sprint  

<a id="review-progress">  </a>
##Review progress in daily scrum meetings 
During your daily Scrum, you can filter your task board to help focus on items of interest. 
*	Group by Backlog items or Group by stories to monitor progress of your product backlog items, stories, requirements, or bugs. 
*	Group by People when you want to monitor progress of individual team members.  

Use the Person filter when you want to focus on work assigned to individual team members.

<a id="show-item-progress">  </a>
###Show progress on items
With this view, you can quickly see which items are nearing completion and which have yet to be started. You can expand ![expand icon](../_img/icons/expand_row_icon.png) and collapse ![collapse icon](../_img/icons/collapse_row_icon.png) a row to focus on a particular item and its tasks. 
  
![Group by backlog items, show All team members](_img/ALM_TB_GRP_ItemsAll.png)


<a id="show-individual-progress">  </a>
###Show progress of individuals
With this view, you can focus on the work completed and the work remaining for each individual team member. You can quickly see who may need help to complete their sprint tasks. This view shows items and tasks assigned to the selected team member. 

![Group by Backlog items, show Christie Church team member](_img/ALM_TB_GRP_Items_CC.png)


<a id="group-by-team">  </a>
###Group by team members
With this view, you can quickly see all the tasks associated with each team member. Backlog items don't appear in this view, only the tasks associated with each individual.  

![Group by People, show All team member](_img/ALM_TB_GRP_People_All.png)


<a id="update-tasks">  </a>
##Update tasks during the sprint cycle
The task board makes quick work of updating both task status and remaining work.  

###Update task status
Simply drag tasks to a downstream column to reflect if they are in progress or completed.  

![Task board, update task status](_img/ALM_TB_Move_To_Done.png)  

When you move a task to the Done or Completed column, the system automatically updates the Remaining Work field to 0. If you discover more work is remaining, change the State back to In progress or To do and enter a value for the remaining work. 

###Update remaining work
Updating Remaining Work, preferably prior to the daily Scrum meeting, helps the team stay informed of the progress being made. It also ensures a smoother burndown chart.  

Each team member can review the tasks they've worked on and estimate the work remaining. If they've discovered that it's taking longer than expected to complete, they should increase the remaining work for the task. Remaining work should always reflect exactly how much work the team member estimates is remaining to complete the task. 

![Task board, update task remaining work](_img/ALM_TB_UpdateRWork.png)  


<a id="unparented-tasks">  </a>
###Unparented tasks
Tasks without links to parent backlog items or user stories appear at the top of the task board. You can track unparented tasks in similar ways to other tasks, or drag them to an existing backlog item to parent them. The Unparented card tracks the total of remaining work defined for all unparented tasks, however, it isn’t associated with any work item.

![Unparented tasks](_img/ALM_TB_UnparentedTasks_CO.png)


<a id="close-sprint">  </a>
##Close out a sprint, update your task board
At the end of the sprint, you'll want to perform these final tasks:  
*	Zero out remaining work of all completed tasks
*	Update the status of all completed backlog items
*	Move incomplete tasks or backlog items to the next sprint or back to the product backlog.

Dragging an incomplete item to the product backlog or to a future sprint updates the Iteration Path of all uncompleted child tasks to correspond to the product backlog iteration path or future sprint.   

##Try this next

Work with [sprint burndown](sprint-burndown.md) charts to monitor progress, manage scope creep, and mitigate risks. 


##Related task board notes
As you can see, the task board provides a lot of support for your Scrum activities. For related Scrum topics, see:  
*	[Create your backlog](../backlogs/create-your-backlog.md)
*	[Organize your backlog](../backlogs/organize-backlog.md)
*	[Sprint planning](sprint-planning.md)
*	[Customize cards on the task board](../customize/customize-cards.md#task-board-cards)   

<a id="task-board-controls">  </a>
###Task board controls

| Control                                                                                                                                                | Function                                                                                                                                                                       |
|--------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Backlog                                                                                                                                                | [Switch to sprint backlog view](sprint-planning.md)                                                                                                                                                          |
| Board                                                                                                                                                  | Switch to task board view                                                                             |
| Capacity                                                                                                                                       | [Switch to Capacity planning](sprint-planning.md#set-capacity)   |
| Group by Stories/People                                                                                                                                        | Switch grouping of cards based on backlog items or team members                                                                                                                                                       |
| Person                                                                                                                           | Filter tasks to show items assigned to All or a selected team member                                                                                                          |
| ![Settings icon](../_img/icons/gear_icon.png)                                                                                                                                     | [Open board settings](../customize/customize-cards.md)                                                                                                                                                     |
| ![full screen icon](../_img/icons/fullscreen_icon.png)/![exit full screen icon](../_img/icons/exitfullscreen_icon.png)                                 | Enter or exit full screen mode                                                                                                                                                 |

<a id="reduce-task-board-items">  </a> 
##Reduce the number of items on the task board 

If you exceed the number of items allowed on your task board, you'll receive a message indicating that you need to reduce the number of items or [increase the maximum number of allowed items](https://msdn.microsoft.com/library/hh543813.aspx#count). The maximum number of items includes work item types included in the Requirement and Task categories.

You can reduce the number of items on the task board by moving them to the backlog or another sprint. When you move a parent PBI or user story, all active child tasks (State not equal to Done or Closed) automatically move with the parent item. 

**Visual Studio Online: **

- From the task board, drag the PBI or user story from the first column onto the backlog or future sprint. All child tasks automatically move with the parent item.  
- From the sprint backlog, multi-select the items to move and then click the context menu for an item and select the iteration to move them to.  
	![multi-select items from the sprint backlog](_img/sprint-backlog-multi-select-non-sequential-items.png)  

**On-premises TFS:**   
- From the task board, drag the PBI or user story from the first column onto the backlog or future sprint.  

- From the sprint backlog, drag an item back to the backlog or to another sprint.  
	![Drag items back to product backlog](_img/IC797613.png)  

- If you need to move several items, you can create a query from the sprint backlog and then use the query to [bulk modify the iteration path](https://msdn.microsoft.com/library/hh409280.aspx).  


<a id="scrum-master-role">  </a>
###Role of the Scrum Master  

Scrum Masters help build and maintain healthy teams by employing Scrum processes. They guide, coach, teach, and assist Scrum teams in the proper employment of Scrum methods. Scrum Masters also act as change agents to help teams overcome impediments and to drive the team toward significant productivity increases.   

Core responsibilities of Scrum Masters include: 
*	Support the team to adopt and follow Scrum processes. 
	For example, you should not let the daily Scrum meeting become an open discussion that lasts 45 minutes. 
*	Guard against the product owner or team members from adding work after the sprint begins.  

*	Clear blocking issues that prevent the team from making forward progress. 
	This might require you to perform small tasks, such as approving a purchase order for a new build computer or resolving a conflict within your team.   
*	Help the team work to resolve conflicts and issues that arise and learn from the process.  
*	Ask questions that reveal hidden issues and confirm that what people are communicating is well understood by the entire team.  
*	Identify and safeguard the team from potential issues becoming major issues. Just as it's cheaper to fix a bug soon after it's discovered, it's also easier and less disruptive to fix a team issue when it's small and manageable.  
*	Prevent the team from presenting incomplete user stories during a [sprint review meeting](sprint-burndown.md#sprint-review-meeting).
*	Gather, analyze, and present data to business stakeholders in a way that 
	demonstrates how the team is improving and growing. For example, if your team has significantly increased the amount of value that it has delivered while generating fewer bugs, make the value visible through regular communications to business stakeholders.   

Good Scrum Masters possess or develop excellent communication, negotiation, and conflict resolution skills. They actively listen to not only the words that people say and write but also how they deliver their messages (their body language, facial expressions, vocal pace, and other nonverbal communication). 

Just as it's cheaper to fix a bug soon after it's discovered, it's also easier and less disruptive to fix a team issue when it's small and manageable before it grows into a major issue.  

<a id="daily-scrum-meetings">  </a>
###Daily Scrum meetings
Daily Scrum meetings help keep a team focused on what it needs to do the next day to maximize the team's ability to meet its sprint commitments. Your Scrum Master should enforce the structure of the meeting and ensure that it starts on time and finishes in 15 minutes or less.  

Three aspects of successful Scrum meetings are:


*	Everyone stands up (this helps to keep the meetings focused and short) 
*	They start and end on time and occur at the same time in the same location each day 
*	Everyone participates, each team member answers the three Scrum questions:
	*	*What have I accomplished since the most recent Scrum?*  
	*	*What will I accomplish before the next Scrum?*  
	*	*What blocking issues or impediments might affect my work?*  

Team members should strive to answer their questions quickly and concisely. For example: 

<blockquote style="font-size: 13px">*"Yesterday, I updated the class to reflect the new data element that we pull from the database, and I got it to appear in the interface. This task is complete. Today, I will ensure that the new data element is correctly calculating with the stored procedure and the other data elements in the table. I believe I will accomplish this task today. I will need someone to review my calculations. I have no impediments or blocking issues."*   </blockquote>  

This response conveys what was accomplished, what will be accomplished, and that the team member would like some help looking at the code.

Contrast with this next example:  

<blockquote style="font-size: 13px">*"Yesterday, I worked on the class, and it works. Today, I will work on the interface. No blocking issues."*   </blockquote>  


Here, the team member doesn't provide enough detail about what class they worked on nor which interface components they'll complete. In fact, the word accomplished never came up.

It's important that no one interrupts during report outs. Each person must have sufficient time to answer the three questions. 

More in-depth and follow-up discussions should take place after the meeting, as people return to their desks or, if a significant amount of conversation is necessary, in a follow-up meeting.

Many teams delay discussions by using the "virtual parking lot" method. As topics come up that a team member believes warrants further discussion, they can quietly walk to a whiteboard or flipchart and list the topic in the parking lot. At the end of the meeting, the team determines how they'll handle the listed items. 
 