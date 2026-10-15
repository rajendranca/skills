---
name: dotnet
description: Apply dotnet engineering standards to relevant files and reviews.
applyTo: "**/*.{cs,csproj,sln,slnx}"
---
Follow existing target framework and architecture. Prefer clear names, asynchronous IO with cancellation, DI lifetimes, structured logging without sensitive data, input validation, and meaningful tests. Verify rather than assume new runtime APIs.
