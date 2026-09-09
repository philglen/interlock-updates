# Interlock 0.1.36

- Preserve the last verified Cloud account topology while the desktop service restarts, so Cloud broker accounts are not incorrectly presented as new Local execution accounts.
- Restore the Cloud session from macOS Keychain automatically after app updates and service restarts.
- Let a verified Cloud identity attach to the desktop user that is already signed in, without requesting the local desktop password again.
- Keep Cloud account data visible while automatic session restoration retries instead of clearing it on a transient authentication response.
