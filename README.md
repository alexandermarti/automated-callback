#  Automate callbacks using always-running campaigns and data actions

> View the full [Automated Callback Blueprint article](https://developer.mypurecloud.com/blueprints/automated-callback-blueprint/) on the Genesys Cloud Developer Center.

This Genesys Cloud Developer Blueprint explains how to configure automated callbacks by using data actions. The process explained in this blueprint adds calls to a workbin or holding queue. It calculates the estimated wait time (EWT) after which it generates the callback, timing it to match the time the caller would have spent on hold as closely as possible. While a caller's number waits in the holding queue, you can view it and even delete it, if necessary. To initiate the callback after the EWT, a data action adds the number to an agentless always-running outbound dialing campaign on Genesys Cloud. The agentless campaign dials the number and then routes the answered callback into the designated inbound queue. You can choose to have the person receiving the callback confirm that they still need help or send the call directly to an agent. By using a specially-configured holding queue for callback numbers, you can easily filter for these callbacks in reports.

![Automate callbacks using agentless, always-running Campaigns and Data Actions](blueprint/images/bpAutoCallbkOverview.png)
