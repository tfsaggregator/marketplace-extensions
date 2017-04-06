TFS Aggregator is an extension for Team Foundation Server (TFS) and Visual Studio Team Services (VSTS)
that enables running custom scripts when Work Items change, allowing dynamic calculation of field values and more.

This [**Web Service**](https://github.com/tfsaggregator/tfsaggregator-webhooks) version, for VSTS or TFS 2015 and later. You have to setup an hosting environment (basically an IIS Web Site) and it runs out-of the TFS process. The Web Service is the only option for Visual Studio Team Services (VSTS).

If you have TFS on-premise, you can instead use the [**Server Plugin**](https://marketplace.visualstudio.com/items?itemName=tfsaggregatorteam.tfs-aggregator-server-plugin), for TFS 2013 Update 2 up to TFS 2017 Update 1.

Go to the project's site <https://tfsaggregator.github.io/> for more information and downloads.

# What's new in v2.3 (beta)

- Support for VSTS & TFS 2015+ Web Hooks
- Additional authentication modes
- Filter on change event (New,Change,Delete,Restore)


# Some uses cases

- Update the state of a Bug, PBI (or any parent) to "In Progress" when a child gets moved to "In Progress"
- Update the state of a Bug, PBI (or any parent) to "Done" when all children get moved to "Done" or "Removed"
- Update the "Work Remaining" on a Bug, PBI, etc with the sum of all the Task's "Work Remaining".
- Update the "Work Remaining" on a Sprint with the sum of all the "Work Remaining" of its grandchildren (i.e. tasks of the PBIs and Bugs in the Sprint).
- Sum up totals on a single work item (i.e. Dev Estimate + Test Estimate = Total Estimate)

