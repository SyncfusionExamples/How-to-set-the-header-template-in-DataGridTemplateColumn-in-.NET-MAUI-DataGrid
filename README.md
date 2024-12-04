# How to set the header template in DataGridTemplateColumn in .NET MAUI DataGrid?
In this article, we will show you how to set the header template in DataGridTemplateColumn in [.Net Maui DataGrid](https://www.syncfusion.com/maui-controls/maui-datagrid).

## xaml
The code below demonstrates how to set the header template in DataGridTemplateColumn in DataGrid. 
```
 <ContentPage.BindingContext>
     <local:EmployeeViewModel x:Name="viewModel"/>
 </ContentPage.BindingContext>

 <syncfusion:SfDataGrid x:Name="sfGrid" 
                       GridLinesVisibility="Both"
                       AutoGenerateColumnsMode="None"
                       HeaderGridLinesVisibility="Both"
                       ColumnWidthMode="Auto"
                       ItemsSource="{Binding Employees}">

    <syncfusion:SfDataGrid.Columns>
        <syncfusion:DataGridTemplateColumn MappingName="EmployeeID"
                                          Format="#">
            <syncfusion:DataGridTemplateColumn.HeaderTemplate>
                <DataTemplate>
                    <Label Text="Employee ID"
                           FontAttributes="Bold"
                           TextColor="blue"
                           VerticalOptions="Center"
                           HorizontalOptions="Center" />
                </DataTemplate>
            </syncfusion:DataGridTemplateColumn.HeaderTemplate>
            <syncfusion:DataGridTemplateColumn.CellTemplate>
                <DataTemplate>
                    <Label Text="{Binding EmployeeID}"
                           HorizontalOptions="End"
                           VerticalOptions="Center"
                           Padding="14" />
                </DataTemplate>
            </syncfusion:DataGridTemplateColumn.CellTemplate>
        </syncfusion:DataGridTemplateColumn>
        <syncfusion:DataGridTextColumn MappingName="Name"
                                       HeaderText="Employee Name" />
        <syncfusion:DataGridTextColumn MappingName="Title"
                                       HeaderText="Designation" />
        <syncfusion:DataGridDateColumn MappingName="HireDate"
                                       HeaderText="Hire Date" />
    </syncfusion:SfDataGrid.Columns>

</syncfusion:SfDataGrid>
``` 

 ![headerTemplate.png](https://support.syncfusion.com/kb/agent/attachment/inline?token=eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjMzNDM3Iiwib3JnaWQiOiIzIiwiaXNzIjoic3VwcG9ydC5zeW5jZnVzaW9uLmNvbSJ9.Ck4nvfT9Buyj1eQTYIKCjjOdMcAum2iUx77L-kOM51g)

[View sample in GitHub](https://github.com/SyncfusionExamples/How-to-set-the-header-template-in-DataGridTemplateColumn-in-.NET-MAUI-DataGrid)

Take a moment to explore this [documentation](https://help.syncfusion.com/maui/datagrid/overview), where you can find more information about Syncfusion .NET MAUI DataGrid (SfDataGrid) with code examples. Please refer to this [link](https://www.syncfusion.com/maui-controls/maui-datagrid) to learn about the essential features of Syncfusion .NET MAUI DataGrid (SfDataGrid).
 
##### Conclusion
 
I hope you enjoyed learning about how to set the header template in DataGridTemplateColumn in .NET MAUI DataGrid (SfDataGrid).
 
You can refer to our [.NET MAUI DataGrid’s feature tour](https://www.syncfusion.com/maui-controls/maui-datagrid) page to learn about its other groundbreaking feature representations. You can also explore our [.NET MAUI DataGrid Documentation](https://help.syncfusion.com/maui/datagrid/getting-started) to understand how to present and manipulate data. 
For current customers, you can check out our .NET MAUI components on the [License and Downloads](https://www.syncfusion.com/sales/teamlicense) page. If you are new to Syncfusion, you can try our 30-day [free trial](https://www.syncfusion.com/downloads/maui) to explore our .NET MAUI DataGrid and other .NET MAUI components.
 
If you have any queries or require clarifications, please let us know in the comments below. You can also contact us through our [support forums](https://www.syncfusion.com/forums), [Direct-Trac](https://support.syncfusion.com/create) or [feedback portal](https://www.syncfusion.com/feedback/maui?control=sfdatagrid), or the feedback portal. We are always happy to assist you!