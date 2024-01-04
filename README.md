# How-to-rotate-the-data-labels-in-Blazor-chart

This article explains how to rotate the data labels in Blazor Chart Component.

**Rotating data labels in Blazor chart**

[Blazor Chart](https://www.syncfusion.com/blazor-components/blazor-charts) provides the support to rotate data label. Data label can be rotated by setting the  [EnableRotation](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor.Charts.ChartDataLabel.html#Syncfusion_Blazor_Charts_ChartDataLabel_EnableRotation) property to **true** and by setting the angle(in degrees) to the [Angle](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor.Charts.ChartDataLabel.html#Syncfusion_Blazor_Charts_ChartDataLabel_Angle) property of [ChartDataLabel](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor.Charts.ChartDataLabel.html#Syncfusion_Blazor_Charts_ChartDataLabel__ctor).

The following Code example illustrates this.

**Index.razor**

```cshtml 

@using Syncfusion.Blazor.Charts

<SfChart>

    <ChartPrimaryXAxis ValueType="Syncfusion.Blazor.Charts.ValueType.Category" /> 

    <ChartSeriesCollection>
        <ChartSeries DataSource="@WeatherReports" XName="X" YName="Y" Type="ChartSeriesType.Column">
            <ChartMarker>               
                <ChartDataLabel Visible="true" EnableRotation="true" Position="Syncfusion.Blazor.Charts.LabelPosition.Middle" Angle="45">
                    <ChartDataLabelFont Size="20" ></ChartDataLabelFont>                    
                </ChartDataLabel>                
            </ChartMarker>
        </ChartSeries>
    </ChartSeriesCollection>

</SfChart>

@code {

    public class Data
    {
        public string X { get; set; }
        public double Y { get; set; }
    }

    public List<Data> WeatherReports = new List<Data>
    {
        new Data{ X= "Jan", Y= 3 },
        new Data{ X= "Feb", Y= 3.5 },
        new Data{ X= "Mar", Y= 7 },
        new Data{ X= "Apr", Y= 13.5 }
    };     
}

```

The following screenshot illustrates the output of the above code snippet.

**Output:**

![Roatated datalabel](/datalabel-rotation.png)

**Conclusion**

I hope you enjoyed learning how to rotate data label of Blazor Chart Component.

You can refer to our [Blazor Chart feature tour](https://www.syncfusion.com/blazor-components/blazor-charts) page to know about its other groundbreaking feature representations and [documentation](https://blazor.syncfusion.com/documentation/chart/getting-started), and how to quickly get started for configuration specifications. You can also explore our [Blazor Chart example](https://blazor.syncfusion.com/demos/chart/line?theme=bootstrap5) to understand how to create and manipulate data.

For current customers, you can check out our components from the [License and Downloads](https://www.syncfusion.com/sales/teamlicense) page. If you are new to Syncfusion, you can try our 30-day [free trial](https://www.syncfusion.com/downloads/blazor) to check out our other controls.

If you have any queries or require clarifications, please let us know in the comments section below. You can also contact us through our [support forums](https://www.syncfusion.com/forums), [support portal](https://support.syncfusion.com/create), or [feedback portal](https://www.syncfusion.com/feedback/blazor-components?control=charts). We are always happy to assist you!