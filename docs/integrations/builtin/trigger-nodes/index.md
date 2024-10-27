---
#https://www.notion.so/n8n/Frontmatter-432c2b8dff1f43d4b1c8d20075510fe4
contentType: overview
---

# Triggers

Trigger nodes are the starting point of every workflow.  
Unlike other nodes, triggers don't have inputs.

On the canvas, triggers show with a lighting bolt icon and rounded edges on their left.

## Triggering workflows

Most workflows are triggered based on a specific app event or a webhook. You can also schedule workflows to execute at intervals.

While developing, start with the default manual trigger ("Trigger manually") and execute your workflow at once with a single click.
When switching to production, you can remove this trigger or deactivate it.

You can combine one manual trigger and many automated triggers within the same workflow.

For more information about the supported app event triggers, see the Trigger Library in the following sections.

## Trigger types

When [creating a workflow](/workflows/create/), select the trigger among the following types:

- [Trigger manually](/integrations/builtin/core-nodes/n8n-nodes-base.manualworkflowtrigger/): For development and manual executions.
- **On app event**: Execute a workflow when a specific action happens in your third-party systems. Configuration is specific to each system.  
For more information, see the Trigger Library.
- [On a schedule](/integrations/builtin/core-nodes/n8n-nodes-base.scheduletrigger/): Execute a  workflows at intervals.
- [On webook call](/integrations/builtin/core-nodes/n8n-nodes-base.scheduletrigger/): Execute a  workflow when the webhook URL is called.
- [On form submission](/integrations/builtin/core-nodes/n8n-nodes-base.formtrigger/): Execute a workflow when an n8n form is submitted.
- [When called by another workflow](/integrations/builtin/core-nodes/n8n-nodes-base.workflowtrigger/): To set up workflow orchestraion and execute a workflow from within another workflow.
- [On chat message](/integrations/builtin/core-nodes/n8n-nodes-langchain.chattrigger/): Execute workflows in AI scenarios.
- **Other ways...**: Includes [error](/integrations/builtin/core-nodes/n8n-nodes-base.errortrigger/), [emails](/integrations/builtin/core-nodes/n8n-nodes-base.emailimap/), and [server-side events](/integrations/builtin/core-nodes/n8n-nodes-base.ssetrigger/).

## Testing triggers

Testing triggers ensures they are correctly configured.

To view the output for a specific trigger without running the full workflow, hover over the trigger and select the Play icon.

## Going further

- [Monitoring workflow executions](/workflows/executions/single-workflow-executions/)
- [Debugging workflows with Error triggers](/courses/level-two/chapter-4/)
- [Trigger workflows based on other workflows](/flow-logic/subworkflows/)
- [Writing custom triggers](#)