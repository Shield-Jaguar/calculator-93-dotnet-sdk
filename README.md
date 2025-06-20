
# Getting Started with APIMATIC Calculator

## Introduction

Simple calculator API hosted on APIMATIC

## Install the Package

If you are building with .NET CLI tools then you can also use the following command:

```bash
dotnet add package Calculator93SDK --version 7.8.9
```

You can also view the package at:
https://www.nuget.org/packages/Calculator93SDK/7.8.9

## Test the SDK

The generated SDK also contain one or more Tests, which are contained in the Tests project. In order to invoke these test cases, you will need `NUnit 3.0 Test Adapter Extension` for Visual Studio. Once the SDK is complied, the test cases should appear in the Test Explorer window. Here, you can click `Run All` to execute these test cases.

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Shield-Jaguar/calculator-93-dotnet-sdk/tree/7.8.9/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| Environment | `Environment` | The API environment. <br> **Default: `Environment.Production`** |
| Timeout | `TimeSpan` | Http client timeout.<br>*Default*: `TimeSpan.FromSeconds(100)` |
| HttpClientConfiguration | [`Action<HttpClientConfiguration.Builder>`](https://www.github.com/Shield-Jaguar/calculator-93-dotnet-sdk/tree/7.8.9/doc/http-client-configuration-builder.md) | Action delegate that configures the HTTP client by using the HttpClientConfiguration.Builder for customizing API call settings.<br>*Default*: `new HttpClient()` |

The API client can be initialized as follows:

```csharp
APIMATICCalculatorClient client = new APIMATICCalculatorClient.Builder()
    .Environment(APIMATICCalculator.Standard.Environment.Production)
    .Build();
```

## List of APIs

* [Simple Calculator](https://www.github.com/Shield-Jaguar/calculator-93-dotnet-sdk/tree/7.8.9/doc/controllers/simple-calculator.md)

## SDK Infrastructure

### Configuration

* [HttpClientConfiguration](https://www.github.com/Shield-Jaguar/calculator-93-dotnet-sdk/tree/7.8.9/doc/http-client-configuration.md)
* [HttpClientConfigurationBuilder](https://www.github.com/Shield-Jaguar/calculator-93-dotnet-sdk/tree/7.8.9/doc/http-client-configuration-builder.md)
* [ProxyConfigurationBuilder](https://www.github.com/Shield-Jaguar/calculator-93-dotnet-sdk/tree/7.8.9/doc/proxy-configuration-builder.md)

### HTTP

* [HttpCallback](https://www.github.com/Shield-Jaguar/calculator-93-dotnet-sdk/tree/7.8.9/doc/http-callback.md)
* [HttpContext](https://www.github.com/Shield-Jaguar/calculator-93-dotnet-sdk/tree/7.8.9/doc/http-context.md)
* [HttpRequest](https://www.github.com/Shield-Jaguar/calculator-93-dotnet-sdk/tree/7.8.9/doc/http-request.md)
* [HttpResponse](https://www.github.com/Shield-Jaguar/calculator-93-dotnet-sdk/tree/7.8.9/doc/http-response.md)
* [HttpStringResponse](https://www.github.com/Shield-Jaguar/calculator-93-dotnet-sdk/tree/7.8.9/doc/http-string-response.md)

### Utilities

* [ApiException](https://www.github.com/Shield-Jaguar/calculator-93-dotnet-sdk/tree/7.8.9/doc/api-exception.md)
* [ApiHelper](https://www.github.com/Shield-Jaguar/calculator-93-dotnet-sdk/tree/7.8.9/doc/api-helper.md)

