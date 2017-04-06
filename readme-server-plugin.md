TFS Aggregator is an extension for Team Foundation Server (TFS) and Visual Studio Team Services (VSTS)
that enables running custom scripts when Work Items change, allowing dynamic calculation of field values and more.

It comes in two flavors sharing a common scripting language and configuration.

The [**Server Plugin**](https://github.com/tfsaggregator/tfsaggregator/releases), for TFS 2013 Update 2 up to TFS 2017 Update 1, runs in-process of your on-premise TFS and is the most performing option. TFS takes care of insulating from crashes in the plugin.

Another option is choosing for the [**Web Service**](https://marketplace.visualstudio.com/items?itemName=tfsaggregatorteam.tfs-aggregator-web-service) version, for VSTS or TFS 2015 and later. You have to setup an hosting environment (basically an IIS Web Site) and it runs out-of the TFS process. The Web Service is the only option for Visual Studio Team Services (VSTS).

Go to the project's site <https://tfsaggregator.github.io/> for more information and downloads.

# What's new in v2.2.1

- Fixes bugs.

# What's new in v2.2

- Support for TFS 2017
- Macro snippets and Functions for Rules and make code more modular
- Ability to specify server URL
- Support for multiple workitem Ids in Console application (issue #178)
- Ability to Send email from Rules
- Migrated CI build from AppVeyor to VSTS
- Use of GitVersion to manage Semantic Versioning

# What's new in v2.1.1

- Fixes important bug causing very high CPU usage (see #160).

# What's new in v2.1

- Support for TFS 2015.2 and TFS 2015.2.1
- A 'real' Scripting language (C#, VB, Powershell)
- Scoping allows select which rules apply to which Team Project
- Enhanced filtering to trigger rules when conditions are met
- Console application to quickly test new rules
- Richer logging
- Test harness and modularity to ease adding new features
- Create new Work Items and Links using rules
and more...

# Some uses cases

- Update the state of a Bug, PBI (or any parent) to "In Progress" when a child gets moved to "In Progress"
- Update the state of a Bug, PBI (or any parent) to "Done" when all children get moved to "Done" or "Removed"
- Update the "Work Remaining" on a Bug, PBI, etc with the sum of all the Task's "Work Remaining".
- Update the "Work Remaining" on a Sprint with the sum of all the "Work Remaining" of its grandchildren (i.e. tasks of the PBIs and Bugs in the Sprint).
- Sum up totals on a single work item (i.e. Dev Estimate + Test Estimate = Total Estimate)

