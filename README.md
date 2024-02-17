# Kiota-QueryParams-Repro

Maybe this isn't a bug and I'm just new to Kiota. :)

## Issue

For some reason (or at least a reason not known to me), query parameters of the Kiota client aren't included in the API request.

## Repo Overview

This repo has 3 projects:

- WeatherForecast.Client
  - The Kiota client genrated from...

- WeatherForecast.Api
  - Basic `dotnet new webapi`

- Hiker.ConsoleApp
  - Console app that uses the generated Kiota client to hit WeatherForecast.Api

## Running the repro

- Run WeatherForecast.Api, then run Hiker.ConsoleApp. Observe the query parameters aren't sent with the request.
