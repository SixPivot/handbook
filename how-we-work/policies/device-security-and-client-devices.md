# Device Security and Client Devices

## Purpose

As consultants, our devices regularly have access to SixPivot systems, client environments, source code and other sensitive information.

Most of the time we work from our own laptop under the [SixPivot laptop scheme](https://handbook.sixpivot.com.au/perks-and-benefits/laptop-allowance). Sometimes a client requires us to use a device they provide and manage instead.

These are two different trust boundaries.

> **Your SixPivot work device is your responsibility to keep secure. A client device belongs inside the client's environment and should be treated as separate from ours.**

This policy describes how we work across those boundaries.

It should be read alongside our [Cybersecurity Policy](https://handbook.sixpivot.com.au/how-we-work/policies/cybersecurity-policy) and any security requirements imposed by the client.

## Your SixPivot work device

Under our [laptop scheme](https://handbook.sixpivot.com.au/perks-and-benefits/laptop-allowance), Pivots choose and ultimately own their laptops. While you're using one for SixPivot work, we expect it to be maintained as a secure work device.

Whether you use Windows, macOS or Linux, it should:

* run a supported operating system and receive security updates;
* use full-disk encryption;
* have appropriate anti-malware or endpoint protection running;
* have its firewall enabled;
* require authentication and automatically lock when unattended;
* use MFA for SixPivot and client accounts where available; and
* not be shared with other people while it contains or provides access to SixPivot or client information.

Our [Cybersecurity Policy](https://handbook.sixpivot.com.au/how-we-work/policies/cybersecurity-policy) contains the broader security requirements and guidance for protecting your device.

We don't prescribe a particular operating system or security stack. We do expect everyone to maintain a reasonable security posture appropriate to the device they're using.

## Engagement Lifecycle

### Before an Engagement

Before starting with a client, take a moment to understand how they expect you to work and what access you'll be given.

This doesn't need to be complicated, but you should know:

* whether you'll use your SixPivot work device, a client-provided device or both;
* the client's relevant security and acceptable-use policies;
* how you'll access client systems, such as VPN, VDI or a client-managed device;
* which accounts and identities you'll be expected to use;
* where source code, documents and other client information should be stored;
* whether there are restrictions on local development, downloading data or using external services;
* whether there are specific requirements around AI or development tools, source code assistants or sharing information with third-party services; and
* who to contact if you need access or aren't sure whether something is permitted.

If you're using your SixPivot work device, make sure it continues to meet the requirements in our [Cybersecurity Policy](https://handbook.sixpivot.com.au/how-we-work/policies/cybersecurity-policy) before connecting it to client systems.

If the client provides a device, understand how they expect it to be used before you start moving work onto it. Keep it separate from your SixPivot and personal environments from the beginning rather than trying to untangle them later.

When something isn't clear, ask your PC or team mates. It's much easier to establish the right boundaries at the start of an engagement than fix them afterwards.

### During an engagement

Client information should only be kept locally where there's a reason for it to be there and prior approval by the client.

Where practical, keep source code, documents and other project artefacts in the systems provided for the engagement rather than accumulating permanent local copies.

Credentials should be kept in an appropriate credential manager (our standard being [1Password](https://1password.com/)) and production or sensitive client data should not be copied locally unless the engagement requires it.

Client security requirements may be stronger than ours. When working in their environment, find out their policies and follow those requirements.

### When an engagement ends

When you finish working with a client, clean up after the engagement.

That generally means removing things you no longer need, including:

* local source repositories;
* downloaded documents, exports and client data;
* temporary files and database backups;
* client credentials, certificates and SSH keys;
* disconnect Github or other provider accounts, remove PATS or tokens;
* VPN profiles and client-specific software where no longer required;
* Chrome/Browser Profiles or custom software installed for client use, licenses associated and
* virtual machines, containers or development environments containing client information.

Have a quick look through places like Downloads, Desktop and temporary working directories too. It's surprisingly easy for client information to end up there during an engagement.

There may be legitimate reasons for SixPivot to retain information for ongoing support or other agreed purposes. Those cases should follow the relevant project arrangements and our [Cybersecurity Policy](https://handbook.sixpivot.com.au/how-we-work/policies/cybersecurity-policy).

The goal isn't to forget everything you learnt. Reusable knowledge and patterns are valuable. Client confidential information, credentials, data and intellectual property we aren't entitled to retain are not.

## When a client gives you a device

Some clients require us to work from a laptop, virtual desktop or other device that they provide and manage.

Treat that device as part of **their environment**, not ours.

The client may manage or monitor the device using endpoint security, device management, network controls or other tools. That's normal for a client-managed device and one reason we keep the environments separate.

Use the device for the engagement it was provided for.

Unless there's a specific business requirement, don't sign into unrelated SixPivot or personal services from it.

This includes things like:

* SixPivot Slack or Teams;
* personal email or Microsoft/Google accounts;
* personal GitHub accounts;
* personal password managers or cloud storage;
* personal banking, financial or other personal accounts;
* other clients' systems, cloud services or other third-party providers; and
* unrelated SixPivot systems.

Where the client provides their own Microsoft 365, Teams, GitHub or other services, use the identity and environment they've provided.

This avoids unnecessarily creating connections between the client, SixPivot and your personal accounts.

## Client Device Isolation

<figure><img src="../../.gitbook/assets/image (30).png" alt=""><figcaption><p><strong>One Internet connection, two trust zones.</strong> Client-provided devices should have direct Internet access without access to devices on your trusted network.</p></figcaption></figure>

### Keep client devices off your trusted network

A client-provided device should be treated as untrusted from the perspective of your home or SixPivot network.

Where possible, connect it through an isolated network such as:

* guest Wi-Fi; or
* a dedicated VLAN with appropriate firewall rules.

The device should be able to reach the Internet but should **not be able to initiate connections to trusted devices on your local network**.

This isn't about bypassing the client's security controls. Client VPNs, proxies, endpoint protection, DNS policies and other controls should continue to work normally.

We're simply keeping their environment separate from ours.

If you can't provide network isolation or aren't sure how to configure it safely, ask for help.

### Don't bridge the environments

Avoid moving information directly between a client device and your SixPivot work device.

Don't use USB drives, personal cloud storage, Slack/Teams, personal email or similar tools as an informal bridge between them. Eg. Sending a message from customer Teams to your SixPivot Teams account.

If information legitimately needs to move between a client environment and SixPivot, use an approved repository, document store, collaboration platform or another mechanism agreed for the engagement.

Likewise, don't disable or work around security controls on a client device. If something prevents you from doing your job, raise it with the client or project team rather than circumventing it.

## Returning a client device

When the device is no longer required, follow the client's return process.

Remove SixPivot information or sessions where appropriate, but don't factory-reset, uninstall client security software or otherwise attempt to clean the device on the client's behalf unless they've asked you to.

The device belongs to their environment and should be returned in the state they expect.

## If something goes wrong

If a device is lost, stolen, compromised or you suspect something isn't right, follow our [Cybersecurity Policy](https://handbook.sixpivot.com.au/how-we-work/policies/cybersecurity-policy) and the client's incident process where applicable.

The same applies if you accidentally cross one of these boundaries, for example by copying client information somewhere it shouldn't be or signing into an account from the wrong device.

Raise it early so we can work out whether there's actually a risk and deal with it appropriately.

## In short

**Your SixPivot work device**

Keep it secure, encrypted, patched and protected. Look after client information while you're working with it and clean up when the engagement ends.

**A client-provided device**

Treat it as part of the client's environment. Don't use it as a personal or general SixPivot device and keep it isolated from trusted networks.

**Between the two**

Keep the environments separate and only move information between them through mechanisms appropriate for the engagement.
