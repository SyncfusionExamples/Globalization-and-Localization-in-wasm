# Globalization and Localization in Blazor WebAssembly

## Overview

This sample demonstrates how globalization and localization can be implemented in a Syncfusion Blazor WebAssembly application. The project shows how a Blazor WebAssembly application can be configured to support multiple cultures, localized resources, and culture-specific formatting behavior so that users can interact with the application in their preferred language and regional format.

The solution is organized as a hosted Blazor WebAssembly application containing Client, Server, and Shared projects. It illustrates the foundational setup required for localization in Blazor WebAssembly applications and how Syncfusion components participate in the localization workflow. The sample is useful for developers who need to build multilingual applications while ensuring that dates, numbers, currencies, and user interface text are displayed according to the active culture settings.

## Key Features

- Uses the Syncfusion [Blazor DataGrid](https://www.syncfusion.com/blazor-components/blazor-datagrid) component to display and manage order data.
- Binds a collection of `Order` objects to the grid using the `DataSource` property.
- Enables built-in filtering functionality through `AllowFiltering="true"`.
- Configures menu-based filtering using the `GridFilterSettings` component with `Type="Syncfusion.Blazor.Grids.FilterType.Menu"`.
- Enables paging support using `AllowPaging="true"` for efficient navigation through large datasets.
- Sets a fixed grid viewport using the `Height="315"` property.
- Defines strongly typed grid columns using the `Field="@nameof(...)"` pattern.
- Displays localized date values using the `Format="d"` property on the `OrderDate` column.
- Displays localized currency values using the `Format="C2"` property on the `Freight` column.
- Configures the `OrderDate` column as a date field using `Type="ColumnType.Date"`.
- Applies right alignment to numeric and date columns using the `TextAlign="TextAlign.Right"` property.
- Demonstrates culture-aware formatting behavior where date and currency values automatically adapt to the currently selected application culture.
- Generates and binds a collection of 75 sample order records during component initialization through the `OnInitialized()` lifecycle method.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone the repository to your local machine.
2. Open the solution file:

   `GlobalizationAndLocalization.sln`

3. Restore NuGet packages by building the solution.
4. Set the appropriate startup project if required.
5. Build the solution.
6. Run the application using **Ctrl+F5**.
7. Open the generated application URL displayed by Visual Studio.

**Visual Studio Code**

1. Clone the repository.
2. Open the repository folder in Visual Studio Code.
3. Open a terminal and navigate to the project directory.

```bash
dotnet restore
dotnet run
```

4. Open the URL displayed in the terminal after the application starts.

## Project Structure

`Client/Pages/Index.razor` - Main sample page that demonstrates globalization and localization behavior using a Syncfusion Blazor DataGrid with paging, menu filtering, localized date formatting (`Format="d"`), and localized currency formatting (`Format="C2"`). The page generates sample `Order` data in the `OnInitialized()` method and binds it to the grid through the `DataSource` property.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Official documentation: https://blazor.syncfusion.com/documentation/getting-started/blazor-webassembly-app

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.