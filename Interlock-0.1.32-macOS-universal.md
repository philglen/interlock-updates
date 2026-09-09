# Interlock 0.1.32

- Add Touch ID sign-in to the macOS desktop app. After one successful password sign-in, the Cloud credential can be saved in the device-only Keychain and retrieved only after Touch ID.
- Invalidate the saved desktop login when the enrolled fingerprints change, and keep password sign-in as the fallback.
- Add opt-in Face ID, Touch ID and Android biometric login support to the mobile source, using device-only secure storage.

The desktop Touch ID bridge accepts messages only from the main local Interlock login page.
