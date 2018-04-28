BootstrapChart - How to bind to filtered or sorted ASPxGridView data on the server side at runtime
This example demonstrates how to show filtered or sorted ASPxGridView data in BootstrapChart on a callback at runtime by using server side data binding.

In page markup, enable ASPxGridView’s ShowFilterRow property to show FilterRow in it. Handle the DataBound event on the first page load to bind BootstrapChart data to ASPxGridView data. Use the VisibleRowCount property to determine what ASPxGridView data is not filtered. Set the ValueType property of the ValueAxisCollection.BootstrapChartValueAxis settings to enable sorting of against BootstrapChart's ValueAxis values.

Handle the ASPxClientGridView.BeginCallback event to save the callback command name in the javascript variable. Then handle ASPxClientGridView's EndCallback to check the callback command name and perform a callback if the condition is satisfied (the command name is "APPLYCOLUMNFILTER" or "SORT").

Put the BootstrapChart to ASPxCallbackPanel to update its data source on the server side after a callback. Then, handle ASPxCallbackPanel's Callback event to get the filtered or sorted ASPxGridView data, convert it to BootstrapChart's data format and bind to BootstrapChart on the server side on a callback.



SOURCE:https://github.com/DevExpress-Examples/bootstrapchart-how-to-bind-to-filtered-or-sorted-aspxgridview-data-on-the-server-side-at-r-t556711
