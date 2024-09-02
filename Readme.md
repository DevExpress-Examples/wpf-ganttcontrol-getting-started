<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/190572173/24.2.1%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/T830769)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
[![](https://img.shields.io/badge/💬_Leave_Feedback-feecdd?style=flat-square)](#does-this-example-address-your-development-requirementsobjectives)
<!-- default badges end -->

# WPF Gantt Control - Create and Bind to Data

This example creates a [WPF GanttControl](https://docs.devexpress.com/WPF/400329/controls-and-libraries/gantt-control), adds task columns (*Name*, *StartDate*, *FinishDate*), and binds the Gantt control to a collection of `GanttTask` objects.

![WPF Gantt Control, DevExpress](https://raw.githubusercontent.com/DevExpress-Examples/wpf-ganttcontrol-getting-started/22.2.2%2B/i/wpf-gantt-control-devexpress.png)

```xaml
<dxgn:GanttControl ItemsSource="{Binding Tasks}">
    <dxgn:GanttControl.Columns>
        <dxgn:GanttColumn BindTo="Name" />
        <dxgn:GanttColumn BindTo="StartDate" />
        <dxgn:GanttColumn BindTo="FinishDate" />
    </dxgn:GanttControl.Columns>
    <dxgn:GanttControl.View>
        <dxgn:GanttView
            AutoExpandAllNodes="True"
            AllowEditing="False"
            AllowSorting="False">
        </dxgn:GanttView>
    </dxgn:GanttControl.View>
</dxgn:GanttControl>
```

Please read the following step-by-step tutorial for additional information: [Add GanttControl to a Project](https://docs.devexpress.com/WPF/400331/controls-and-libraries/gantt-control/getting-started/add-ganttcontrol-to-a-project).


## Files to Review

* [MainWindow.xaml](./CS/GanttControlDemoApp/MainWindow.xaml) (VB: [MainWindow.xaml](./VB/GanttControlDemoApp/MainWindow.xaml))
* [ProjectTaskViewModel.cs](./CS/GanttControlDemoApp/ProjectTaskViewModel.cs) (VB: [ProjectTaskViewModel.vb](./VB/GanttControlDemoApp/ProjectTaskViewModel.vb))
<!-- feedback -->
## Does this example address your development requirements/objectives?

[<img src="https://www.devexpress.com/support/examples/i/yes-button.svg"/>](https://www.devexpress.com/support/examples/survey.xml?utm_source=github&utm_campaign=wpf-ganttcontrol-getting-started&~~~was_helpful=yes) [<img src="https://www.devexpress.com/support/examples/i/no-button.svg"/>](https://www.devexpress.com/support/examples/survey.xml?utm_source=github&utm_campaign=wpf-ganttcontrol-getting-started&~~~was_helpful=no)

(you will be redirected to DevExpress.com to submit your response)
<!-- feedback end -->
