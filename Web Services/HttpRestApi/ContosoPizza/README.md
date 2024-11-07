# ContosoPizza

> An ASP .Net 8.0 RESTful API

## ASP .NET Core Web API Controllers

### `ControllerBase` Class

A controller is a **public** class with one or more public methods known as *actions*.  
The actions are exposed as HTTP endpoints via routing. So an HTTP `GET` request to `https://localhost/{PORT}/weatherforecast` causes the `Get()` method of the `WeatherForecastController` class to be executed.

> By convention, a controller is placed in the project root's *Controllers/* directory.  

```C#
[ApiController]
[Route("[controller]")]
public class WeatherForecastController : ControllerBase
```

### API controller class attributes  

Two important attributes are applied to `WeatherForecastController`:

- `[ApiController]` enables optionated behaviors (set of default conventions and features provided by the framework). Some behaviors include *parameter source inference*, *attribute routing as requirement*, and *model validation error-handling* enhancements.

- `[Route]` defines the routing pattern `[controller]`. The controller's name (case-insensitive, without the *Controller* suffix) replaces the `[controller]` token. In this case, the controller handles requests to `https://localhost:{PORT}/api/weatherforecast`.
