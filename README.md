#Scrypt.NETCore

[![NuGet](https://img.shields.io/nuget/v/Scrypt.NETCore.svg?maxAge=2592000)](https://www.nuget.org/packages/Scrypt.NETCore/)

scrypt is a password hash algorithm created by [Tarsnap](http://www.tarsnap.com/scrypt.html) in 2012 that allow us to protect passwords stored on databases against brute force attacks.

This is netstandard1.3 port of https://github.com/viniciuschiele/Scrypt (with minor changes)
##Examples
Generating a new hash for a password:
```csharp

ScryptEncoder encoder = new ScryptEncoder();

string hashsedPassword = encoder.Encode("mypassword");
```

Comparing a password against a hashed password:
```csharp
ScryptEncoder encoder = new ScryptEncoder();

bool areEquals = encoder.Compare("mypassword", hashedPassword);
```

##Install
Install via NuGet: Install-Package Scrypt.NETCore

##Feedback
Please use the [Issues](https://github.com/prajaybasu/scrypt/issues) for feature requests and troubleshooting usage.
