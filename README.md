# How to Rotate Data Labels in Syncfusion Blazor Chart

## Overview

This sample demonstrates how to rotate data labels in a Syncfusion [Blazor Charts](https://www.syncfusion.com/blazor-components/blazor-charts) column chart. The implementation binds a collection of weather report data to a column series and displays data labels directly within each column using the built-in chart data label feature.

Rotating data labels can improve visual presentation and readability when labels need to follow a specific orientation or align with custom design requirements. This sample shows how to enable data label rotation, define a rotation angle, customize label appearance, and position labels inside chart columns.

## Key Features

- Uses the `SfChart` component to render a chart.
- Configures a categorical x-axis using `ChartPrimaryXAxis` with `ValueType="ValueType.Category"`.
- Binds data through the `DataSource` property of `ChartSeries`.
- Maps category values with the `XName` property.
- Maps numeric values with the `YName` property.
- Renders a column chart using `Type="ChartSeriesType.Column"`.
- Displays series labels using `ChartDataLabel`.
- Enables label visibility through `Visible="true"`.
- Rotates labels using `EnableRotation="true"`.
- Applies a custom rotation angle through `Angle="45"`.
- Positions labels inside the column using `Position="LabelPosition.Middle"`.
- Customizes label appearance using `ChartDataLabelFont`.
- Uses a strongly typed data model containing `X` and `Y` properties for chart binding.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open the `DataLabelRotation.csproj` project file.
3. Restore all NuGet packages.
4. Build the project.
5. Run the application using `Ctrl+F5`.

**Visual Studio Code**

1. Clone or download this repository.
2. Open the repository folder in Visual Studio Code.
3. Open the integrated terminal.
4. Navigate to the project directory.

```bash
cd DataLabelRotation
```

5. Restore NuGet packages:

```bash
dotnet restore
```

6. Run the application:

```bash
dotnet run
```

7. Open the local URL displayed in the console output.

## Project Structure

`DataLabelRotation/Pages/Index.razor` — Implements the Syncfusion Blazor Chart sample demonstrating rotated data labels using `ChartDataLabel`, `EnableRotation`, and `Angle`.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Refer to the official Syncfusion Blazor Chart data label documentation: https://help.syncfusion.com/chart-sdk/blazor/charts/data-labels

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.