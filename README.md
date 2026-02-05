#  ⚜️ CERBERUS-AGI 2026 ⚜️

iOS On-Device AI Interaction Runtime (Research Project)

A long-running iOS interaction framework designed for persistent UI automation, testing, and research on jailbroken devices.

This project focuses on stability, low resource usage, and reliable on-device execution without requiring a permanent connection to a computer.

A demo video is available in VIDEO.mp4.

⸻

Overview

Most iOS automation approaches rely on external control (computer connection, simulators, WebDriver, etc.) or become unstable during long runtimes.

This project explores a different approach:

Running a standalone interaction engine directly on the device, capable of operating for extended periods while remaining lightweight and resilient.

The system is packaged as a TrollStore IPA supported by a small background helper component to improve reliability during long sessions.

⸻

Design Goals
	•	Extremely lightweight footprint (~20MB)
	•	Designed for long runtimes (days/weeks)
	•	Standalone operation directly on the device
	•	Simple scripting model
	•	Low CPU and battery impact
	•	Resolution-agnostic interaction using OCR
	•	Integration with the native iOS Shortcuts app
	•	File-based IPC for stability

⸻

Core Capabilities
	•	Launch applications
	•	Read screen content using OCR
	•	Perform taps, swipes, and gestures
	•	Execute iOS Shortcuts
	•	Background execution designed for long sessions
	•	Script-driven interaction model
	•	Optional integration with external AI systems for decision making (when configured by the user)

⸻

Automation Modes

Script Mode
Uses a simple proprietary line-based script format designed for reliability and ease of generation.

AI-Assisted Mode (Optional)
External AI systems can be connected to interpret screen state and decide next actions. This is optional and fully user-configured.

⸻

Architecture
	•	TrollStore application
	•	Lightweight background helper for stability
	•	File-based communication between components
	•	Designed to remain operational across common interruption scenarios
	•	Compatible with rootless jailbreak environments

⸻

Compatibility
	•	TrollStore
	•	Dopamine / Palera1n (rootless / roothide)
	•	iOS 15 / 16 / 17
	•	iPhone and iPad

⸻

Scripting Engine

The project uses a very simple custom scripting format where each line represents an action. This avoids complex languages and improves reliability for long runs.

An example script is included in the repository.

⸻

Resource Efficiency
	•	Near-zero CPU usage when idle
	•	Automatic memory recycling
	•	Designed for minimal battery impact

⸻

Disclaimer

This is an independent research project exploring persistent on-device UI interaction on jailbroken iOS devices.
It is not affiliated with Apple Inc.

Users are responsible for ensuring their usage complies with local laws and the terms of service of the applications they interact with.

⸻

Contact

If you are interested in the research, collaboration, or technical discussion, you can contact:

albertosendr@gmail.com

⸻

<img width="1620" height="2160" alt="image" src="https://github.com/user-attachments/assets/304c4306-6a8b-442a-a56e-fac5b392e268" />

![unnamed](https://github.com/user-attachments/assets/a8f6b42e-8f09-45db-8369-86dbd7a838fe)

