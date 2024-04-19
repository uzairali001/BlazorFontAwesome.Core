## FontAwesomeIcon - A Razor Class Library for Simplified Icon Integration

This NuGet package provides a convenient `FontAwesomeIcon` Razor component to streamline the integration of FontAwesome icons into your Blazor or ASP.NET Core Razor applications.

### Key Features:

- **Simplified Icon Usage:** Encapsulates the icon markup with customizable styling options, reducing repetitive code.
- **Customizable Appearance:** Easily control size, color, stroke, and secondary color/opacity.
- **Declarative Syntax:** Integrates seamlessly into your Razor views using parameters.

### Installation:

1. Search for `"UzairAli/BlazorFontAwesome.Core"` in the NuGet Package Manager within your project.
2. Install the package.

### Usage:

1. Add the `@using UzairAli.BlazorFontAwesome.Core` directive to your Razor view.
2. Use the `FontAwesomeIcon` component with desired parameters:

```razor
@using FontAwesomeIcon

<FontAwesomeIcon Size="32" Color="blue" Stroke="2" StrokeColor="white">
  ...
</FontAwesomeIcon>
```

### Parameters:

- `Size` (int): Sets the width and height of the icon wrapper (default: 20px).
- `Color` (string): Defines the primary fill color of the icon (default: "black").
- `Stroke` (int): Controls the thickness of the icon stroke (default: 0px).
- `StrokeColor` (string): Specifies the color of the stroke (default: "black").
- `SecondaryColor` (string): Sets the fill color for the secondary icon state (default: "black").
- `SecondaryOpacity` (string): Adjusts the opacity of the secondary icon state (default: "40%").
- `ChildContent` (RenderFragment): The FontAwesome icon class (e.g., fas fa-star).

### Example (Secondary Icon State):

```razor
<FontAwesomeIcon Size="40" Color="red" SecondaryColor="white" SecondaryOpacity="80%">
  ...
</FontAwesomeIcon>
```