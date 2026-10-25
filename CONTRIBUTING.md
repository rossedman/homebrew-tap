# Contributing

Thanks for helping out. This project follows the [Contributor Covenant code of conduct](CODE_OF_CONDUCT.md). By taking part, you agree to uphold it.

## Casks are generated

Every file in `Casks/` is written by [GoReleaser](https://goreleaser.com) when its project cuts a release, and starts with `DO NOT EDIT`. A hand edit is overwritten by the next release, so:

- To change a cask (its description, dependencies, completions, install steps), open an issue or pull request against the `homebrew_casks` section of `.goreleaser.yaml` in that tool's repository. The Packages table in the [README](README.md) links to each one.
- To report a broken install or upgrade, open an [issue here](https://github.com/rossedman/homebrew-tap/issues/new/choose), and it will be fixed upstream.

Pull requests here are welcome for the README, CI and the other repository files.

## Check your work

You need [Homebrew](https://brew.sh) on macOS or Linux. Tap your clone, then run the checks CI runs:

```sh
git clone https://github.com/rossedman/homebrew-tap
cd homebrew-tap
brew tap rossedman/tap "$PWD"
brew style rossedman/tap
brew readall --os=all --arch=all rossedman/tap
```

To try a cask from your clone, `brew install --cask rossedman/tap/<package>`. Run `brew untap rossedman/tap` when you are done, then tap it again from GitHub.

## Pull requests

Write the title as an imperative commit subject that says what the change does, like `Add muscles and sarifix to the Packages table`. Pull requests need the `brew` check to pass and a review from the code owner.

## Questions

Open an [issue](https://github.com/rossedman/homebrew-tap/issues). Report security problems privately, as described in the [security policy](SECURITY.md).
