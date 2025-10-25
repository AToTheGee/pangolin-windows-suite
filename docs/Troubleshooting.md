# Troubleshooting

- **Workflows failing?** Ensure GitHub Actions runners have access to `gitleaks` and `syft`; both are installed during the workflow.
- **Missing binaries?** This scaffold only sets up infrastructure. Check the roadmap in the README for delivery timelines.
- **Credential errors?** Store secrets in Windows Credential Manager or DPAPI—never commit them.
