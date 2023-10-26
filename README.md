Sure, here's a README for your `whisperd` HTTP server:

```markdown
# whisperd 🎙️

[![Crates.io](https://img.shields.io/crates/v/whisperd)](https://crates.io/crates/whisperd)
[![Documentation](https://docs.rs/whisperd/badge.svg)](https://docs.rs/whisperd)
[![License](https://img.shields.io/crates/l/whisperd)](LICENSE)

A simple HTTP server written in Rust for the OpenAI Whisper speech-to-text model.

## Features ✨

- 🎧 Transcribe audio files 
- 🔄 OpenAI API compatibility  
- 🌈 Models 
  - `tiny.en`
  - `tiny`
  - `base.en`
  - `base`
  - `small.en`
  - `small`
  - `medium.en`
  - `medium`
  - `large`
  - `large-v1`
- 🌎 Languages
  - 🇬🇧 English (en)
  - 🇨🇳 Chinese (zh)
  - 🇩🇪 German (de)
  - 🇪🇸 Spanish (es)
  - 🇷🇺 Russian (ru)



## Quickstart 🚀

1. Clone this repository:

```bash
git clone https://github.com/tiero/whisperd.git
```

2. Navigate to the repository and build:

```bash
cd whisperd
cargo build --release
```

3. Run the server:

```bash
./target/release/whisperd serve --model_path path_to_whisper_model
```

Now, the server is running at `http://localhost:8000` and ready to transcribe!

## Usage 🛠️

### CLI Commands

- Start the transcription server:

```bash
whisperd serve --port 5000 --model_path <path_to_model> 
```

- Transcribe a given audio file (this downloads the model automatically from HuggingFace):

```bash
whisperd transcribe --audio <path_to_audio>
```

For more advanced options, use:

```bash
whisperd --help
```

## Contribution 🤝

Pull requests and issues are welcome!

## License 📜

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```