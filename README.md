# DependabotSample

C#プロジェクト用Dependabotの設定サンプルです。

# 設定手順

1. https://github.com/[user]/[project]/network/updates を開きます
（このプロジェクトの場合 https://github.com/mono-matsu/DependabotSample/network/updates ）
2. `Enable Dependabot` をクリックします <br/><img src="https://user-images.githubusercontent.com/101057471/160287918-5695895e-310f-467c-993a-eb9ed18e4f30.png" width="700px" />
3. `Create config file` をクリックします <br/><img src="https://user-images.githubusercontent.com/101057471/160287921-e6973997-737c-4051-a33d-4d2a98b5184e.png" width="700px" />
4. `package-ecosystem` に `nuget` を設定し、`directory` に csproj のあるディレクトリを設定後、 `Commit new file` をクリックします <br/><img src="https://user-images.githubusercontent.com/101057471/160287924-e1f77589-2a1d-4337-b37d-f7920a533b27.png" width="700px" />

```
# To get started with Dependabot version updates, you'll need to specify which
# package ecosystems to update and where the package manifests are located.
# Please see the documentation for all configuration options:
# https://docs.github.com/github/administering-a-repository/configuration-options-for-dependency-updates

version: 2
updates:
  - package-ecosystem: "nuget" # See documentation for possible values
    directory: "/" # Location of package manifests
    schedule:
      interval: "daily"
```

その他のオプションについては、以下のドキュメントを参照してください。
https://docs.github.com/ja/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file
