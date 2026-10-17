# lmdlaw-sketch

I build software around voice interaction, local data and document workflows. My public work includes small, independently runnable components in **Kotlin, Java and Python**, published for focused review and testing.

## Public components

[**yoni-open-components**](https://github.com/lmdlaw-sketch/yoni-open-components) brings together five standalone components:

[![Component tests](https://github.com/lmdlaw-sketch/yoni-open-components/actions/workflows/component-tests.yml/badge.svg?branch=main&event=push)](https://github.com/lmdlaw-sketch/yoni-open-components/actions/workflows/component-tests.yml)

| Component | Language | Focus |
| --- | --- | --- |
| [Voice history](https://github.com/lmdlaw-sketch/yoni-open-components/tree/main/voice-history) | Kotlin | Bounded conversation history, interruption boundaries and explicit omission behavior. |
| [Encrypted rolling buffer](https://github.com/lmdlaw-sketch/yoni-open-components/tree/main/rolling-buffer) | Java | Encrypted local segments, bounded retention, durable state and recovery scenarios. |
| [Visible-send observation](https://github.com/lmdlaw-sketch/yoni-open-components/tree/main/visible-send) | Java | Tracking observed send evidence and handling ambiguity in event sequences. |
| [Transcript coverage](https://github.com/lmdlaw-sketch/yoni-open-components/tree/main/transcript-coverage) | Python | Comparing supplied source and reader text, with explicit coverage and omission results. |
| [Duplicate selection](https://github.com/lmdlaw-sketch/yoni-open-components/tree/main/duplicate-selection) | Kotlin | Keeping unselected paths across overlapping duplicate groups. |

The repository includes standalone test scripts, examples and a validation record. CI runs the existing suites and examples. Component tests document their scope; they do not establish device, live-provider or complete-application acceptance.

## How I approach the work

- Keep state transitions, failure paths and uncertain outcomes explicit.
- Preserve source identities and reproducible validation evidence.
- Give each component a clear scope and document the remaining limits.
