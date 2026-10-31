# Apple Keychain and private sign-in

Version: 1.1.0 · 2026-10-31

Use native Apple security and the service's supported authentication. SuperDot does not need
its own password vault. The assistant can keep service names and connection status in the
personal README; secret values stay outside chat, notes and model-visible tools.
Follow the [shared macOS guidance](../references/README.md#macos-and-skill-writing-standard).
Never copy a Linux credential-file recipe into this setup or bypass a macOS access-control prompt.

## Connect a service

Prefer a supported plugin/OAuth connection. Let the person sign in and approve access themselves.
For website access, use the platform's private sign-in or user takeover flow as described in
[OpenAI's computer/app guide](https://learn.chatgpt.com/docs/dots/computers-and-apps).
Website sessions, saved passwords and API credentials are distinct; one does not grant the others.

For local credential storage, the person uses Keychain Access or the appropriate native Passwords
flow for that credential type. Open Keychain Access through Spotlight and use Apple's current
[Keychain guide](https://support.apple.com/en-gb/guide/keychain-access/kyca1085/mac) for item
details/access controls. The assistant must not inspect stored values or request that they be revealed.

## When a tool needs an API key

Use its supported private setup/authentication route. A credential custodian should report only
the service/reference and status; approved tools consume the value without returning it to the
assistant. Never paste values into shell arguments, configuration examples or conversation.

Storing an item in Keychain does not automatically connect a tool or make its use invisible to
the model. A generic hidden API-key field in the Dot composer is not established by these docs.
Until a supported private-entry/use path exists for that tool, leave that connection waiting.
Do not build a secret service or weaken Keychain permissions to complete onboarding.
