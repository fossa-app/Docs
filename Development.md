# Development

This section documents the development scripts and environment setup.

## Scriptures

Located in the `scripts` directory.

| Script | Description | Details |
| --- | --- | --- |
| `Setup.ps1` | Sets up the development environment. | Installs `Microsoft.PowerShell.SecretManagement` and `Keybase` modules. Registers `FossaApp` secret vault. |
| `Start.ps1` | Starts the application services. | Uses `Invoke-Build` to start services defined in `docker-compose.yml`. Supports `-Pull` to pull images and `-Services` to start specific services. |
| `Stop.ps1` | Stops the application services. | Uses `Invoke-Build` to stop services. |
| `Set-ConnectionString.ps1` | Configures database connection strings. | Helper to set up local dev connection strings. |
| `gat.ps1` | git all tags | Utility to fetch all tags. |
| `gig.ps1` | git ignore generator | Utility to generate `.gitignore`. |

## Environment

The local development environment uses Docker Compose to run services.
- **Orchestration**: `Invoke-Build` module is used for task automation.
- **Secrets**: Managed via PowerShell SecretStore and Keybase.

