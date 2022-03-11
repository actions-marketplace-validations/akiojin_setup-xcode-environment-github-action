# setup-xcode-environment-github-action

## Requirement
You will need to install [fastlane][1]

### Installation
```sh
brew install fastlane
```

## Usage

### Simple usage
```yml
- uses: akiojin/setup-xcode-environment-github-action@v1.0
  id: setup-xcode-environment
  with:
    type: 'development'
    app-identifier: com.exmple.App
    team-id: <Team ID>
    git-url: 'https://github.com/certificates'
    git-passphase: ${{ secrets.APPLE_CERTIFICATE_GIT_PASSPHASE }}
    api-key-base64: ${{ secrets.APPLE_API_KEY_JSON_BASE64 }}
    keychain: <Keychain path>
    keychain-password: <Keychain password>
```

## License
Any contributions made under this project will be governed by the [MIT License][3].

[0]: https://github.com/akiojin/xcode-environemt-github-action/actions/workflows/Test.yml/badge.svg
[1]: https://docs.fastlane.tools/
[2]: https://github.com/akiojin/xcode-environemt-github-action/blob/main/action.yml
[3]: https://github.com/akiojin/xcode-environemt-github-action/blob/main/LICENSE