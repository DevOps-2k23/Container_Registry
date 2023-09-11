# Use the official Microsoft ASP.NET Framework image as a base image
FROM mcr.microsoft.com/dotnet/aspnet:6.0

# Create a directory to copy your application files into
WORKDIR /app

# Copy the contents of your ASP.NET application into the container
COPY . .

# Expose the default HTTP port (80) that IIS uses
EXPOSE 80

# Start IIS when the container starts
CMD ["C:\\ServiceMonitor.exe", "w3svc"]

# Set the entry point for the container
ENTRYPOINT ["dotnet", "webapp100.dll"]
