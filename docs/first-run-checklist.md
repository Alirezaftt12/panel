# PasarGuard first-run checklist
Use this checklist after installing PasarGuard on a new server.
## Secure access
- Configure a domain and SSL certificate before exposing the dashboard publicly.
- For testing without a domain, use SSH port forwarding instead of opening the dashboard to the internet.
- Keep the generated owner setup key private and use it only once.
- Store the dashboard credentials and the `.env` file in a secure location; never commit secrets to Git.
## Verify the installation
- Confirm the service starts successfully and review the application logs.
- Check that data is stored in the expected directory and that backups are available.
- Create one test user, verify its subscription link, expiry, and traffic limit, then remove it if it is no longer needed.
- Document the server address, database choice, backup location, and recovery steps.
## Before production use
- Replace all temporary credentials and revoke unused access.
- Restrict dashboard and API access with firewall rules appropriate for your deployment.
- Test a restore procedure before relying on the installation for production data.
