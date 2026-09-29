# How to Group and Filter the Blazor MultiSelect Dropdown Items

## Overview

This sample demonstrates how to use the Syncfusion [Blazor MultiSelect Dropdown](https://www.syncfusion.com/blazor-components/blazor-multiselect-dropdown) to organize items into groups and enable filtering within a single lication allows users to browse categorized data and quickly locate records through built-in search functionality. Combining grouping and filtering improves navigation and usability when working with larger datasets. The sample provides a practical reference for implementing an efficient multi-selection experience in a Blazor WebAssembly application.

## Key Features

- Uses the Syncfusion `SfMultiSelect` component to enable multiple item selection.
- Binds a local `List<MultiSelectDropdownDataModel>` collection to the `DataSource` property.
- Groups dropdown items by category using the `MultiSelectFieldSettings.GroupBy` property.
- Maps item values and display text through `MultiSelectFieldSettings.Value` and `MultiSelectFieldSettings.Text`.
- Enables built-in search functionality using the `AllowFiltering="true"` property.
- Configures case-sensitive filtering behavior with `IgnoreCase="false"`.
- Uses `FilterType="Contains"` to match search text against any part of the item text.
- Displays vegetables grouped under categories such as **Beans**, **Bulb and Stem**, and **Leafy and Salad**.
- Configures custom popup dimensions through the `PopupHeight` and `PopupWidth` properties.
- Demonstrates a client-side implementation without requiring a remote data source or API integration for the MultiSelect component.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open `GroupAndFilter.sln`.
3. Restore all NuGet packages.
4. If prompted, select the hosted Blazor application startup project.
5. Build the solution.
6. Run the application using `Ctrl+F5`.

**Visual Studio Code**

1. Open the repository folder in Visual Studio Code.
2. Open a terminal and navigate to the repository root directory.

```bash
dotnet restore
```

3. Run the application.

```bash
dotnet run
```

4. Open the local application URL displayed in the terminal after the application starts.

## Project Structure

`GroupAndFilter.sln` - Solution file containing the Blazor WebAssembly hosted application.

`Client/Pages/Index.razor` - Main sample page that demonstrates the Syncfusion MultiSelect component with grouping and filtering capabilities.

`Client/Pages/FetchData.razor` - Default Blazor sample page that retrieves weather forecast data from the server and is not directly related to the MultiSelect implementation.

`Server/Controllers/WeatherForecastController.cs` - ASP.NET Core API controller that supplies sample weather forecast data for the FetchData page.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Documentation: https://blazor.syncfusion.com/documentation/multiselect-dropdown/grouping

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.