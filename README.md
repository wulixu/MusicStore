# MusicStore application

This project is part of ASP.NET 5.0. You can find samples, documentation and getting started instructions for ASP.NET 5.0 at the [Home](https://github.com/aspnet/home) repo.

## Run the application on Helios:
* If you have Visual Studio 2015
	1. Open MusicStore.sln in Visual Studio 2015 and run the individual applications on `IIS Express`.
* If you don't have Visual Studio 2015
	1. Open a command prompt and cd `\src\MusicStore\`.
	2. Execute `kpm restore`.
	3. Execute `Helios.cmd` to launch the app on IISExpress from command line (Application started at URL **http://localhost:5001/**).
	   NOTE: App and tests require Visual Studio 2015 LocalDB on the machine to run.

## Run on WebListener/Kestrel:
* Open a command prompt and cd `\src\MusicStore\`.
* **[WebListener]:**
	4. Run `k web` (Application started at URL **http://localhost:5002/**).
* **[Kestrel]:**
	5. Run `k kestrel` (Application started at URL **http://localhost:5004/**).
* **[CustomHost]:**
	6. Run `k run` (This hosts the app in a console application - Application started at URL **http://localhost:5003/**).

## To run the sample on Mac/Mono:
* Follow [Home](https://github.com/aspnet/home) instructions to install mono, kvm on Mac.
* Open a command prompt and cd `\src\MusicStore\`.
* Execute `kpm restore`.
* Try `k kestrel` to run the application.
**NOTE: On Mono since SQL client is not available the sample uses an InMemoryStore to run the application. So the changes that you make will not be persisted.

###NTLM authentication
More information at src/MusicStore/StartupNtlmAuthentication.cs.

###OpenIdConnect authentication
More information at src/MusicStore/StartupOpenIdConnect.cs.