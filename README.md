# Proton VPN Free-Server Selectors

**Custom Windows and Android clients with explicit selection from the available free-server catalogue.**

## The problem

I wanted to choose a country or server on my free plan. The client kept choosing randomly.

"Connect somewhere" and "connect where I selected" are two rather different features. So I inspected the selection flow and built custom clients that expose the choice within the available free-server catalogue.

## The solution

Source-based Windows and Android customizations that add country/server selection while preserving free-tier filtering, cooldown behavior, and backend authorization.

## What it does

- Explicit free-country and individual-server selection.
- Windows selector integration, including a pre-connection selection path.
- A separately identified and signed Android build.
- Upstream-version matching for the customized code.
- Reversible Windows installation/backup tooling.
- Preserved service-side account and plan checks.

## Engineering highlights

Traced the upstream selection flow and integrated explicit country/server choices into version-matched Windows and Android clients. The customizations preserve free-catalogue filtering and account authorization, with a separate Android identity and reversible Windows installation tooling.

## Technology

C#/.NET Windows client, Kotlin/Android client, upstream Proton VPN source, platform build and test tooling.

## Source code

This showcase documents customizations built on the open-source Proton VPN clients: [ProtonVPN/win-app](https://github.com/ProtonVPN/win-app) and [ProtonVPN/android-app](https://github.com/ProtonVPN/android-app), under their respective licenses. The customized working code and builds are maintained separately. Credit for the underlying VPN clients belongs to Proton and its contributors.
