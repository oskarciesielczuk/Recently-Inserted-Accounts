# Recently Inserted Accounts

Here is the plan I used to figure out the steps i need to take to construct my Lightning Component:
[Recently Inserted Accounts MVC.pdf](https://github.com/oskarciesielczuk/Recently-Inserted-Accounts/files/8756261/Recently.Inserted.Accounts.MVC.pdf)

In the end, I also decided to add a count of how many records are selected, to have a go at working with 'onclick' events.

# Problems I Ran Into

1. The component was not showing up in Lightning App Builder - fixed by adding Lightning__AppPage as a target in the metadate file.
2. The count stayed at 0 - fixed by using the getSelectedRows() function built in with lightning-datatable to get a list of selected rows.
3. Some columns did not have any data in them - fixed by making sure that the fieldName for each column matched the name of the field returned by the SOQL query.
