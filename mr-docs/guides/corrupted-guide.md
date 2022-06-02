# Fix a corrupted guide in Dynamics 365 Guides

In very rare cases, you may find that a guide has become corrupted. This is most commonly associated with guides that were [shared with authors](admin-share-guide.md) in the time period from September 2021 to December 2021. When sharing a guide with an author, you must select the **Append to** privilege. Otherwise, the author can't save any steps that they add to a guide. For guides shared with an author between September 2021 and December 2021, however, due to a bug in Dynamics 365 Guides, the **Append to** privilege could not be set. If an author added one or more steps to a shared guide, and then saved the guide, the guide would become corrupted. If you open a corrupted guide in the PC app, you'll see the following message. 

![Screenshot of message that appears when a guide is corrupted.](media/corrupted-guide-message.jpg "Screenshot of message that appears when a guide is corrupted")

A guide can also become corrupted if you delete a step [from the model-driven app](open-model-driven-app.md). To delete a step, make sure to use the PC app. 

## Fix a corrupted guide

You can fix a corrupted guide by using a flow in the model-driven app. 
