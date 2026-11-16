<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-deepgram 1.3.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-deepgram.git", from: "1.3.0")
```

Products: `SwiftAIDeepgram`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# Deepgram for Swift

`SwiftAIDeepgram` adds Deepgram to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/deepgram` and supports transcription and speech.

Provider guide with models, options, streaming and errors:

- [Deepgram](https://swiftaisdk.github.io/SwiftAISDK/providers/deepgram/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAIDeepgram` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAIDeepgram

let provider = try AIProviders.deepgram(configuration: DeepgramProviderSettings())
```

By default the provider reads `DEEPGRAM_API_KEY` from the environment; values set in `DeepgramProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-deepgram` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
