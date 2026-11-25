# EcommerceSystem

Full-stack e-commerce web application built with ASP.NET Core MVC, Entity Framework Core and SQL Server.

## Features

- Product catalog with categories, brands, product colors and sub-images
- Shopping cart and checkout with Stripe payments
- Admin area for managing products, brands, categories and users
- ASP.NET Core Identity with confirmed-email sign-in and OTP verification
- Email sending for account confirmation and notifications
- Generic repository pattern with dependency injection
- Object mapping with Mapster
- Custom validation attributes

## Tech stack

- .NET 10, ASP.NET Core MVC
- Entity Framework Core (code-first migrations)
- Microsoft SQL Server
- ASP.NET Core Identity
- Stripe.net
- Mapster

## Getting started

1. Install the .NET 10 SDK.
2. Set `ConnectionStrings:DefaultConnection` in `Ecommerce535/appsettings.json` to your SQL Server instance.
3. Apply the database migrations:

   ```powershell
   dotnet ef database update
   ```

4. Run the project:

   ```powershell
   dotnet run --project Ecommerce535
   ```

5. For Stripe checkout, set your test keys with User Secrets:

   ```powershell
   dotnet user-secrets set "Stripe:SecretKey" "sk_test_..."
   ```
