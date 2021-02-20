# GitHub Sponsorsの確定申告手順

日本におけるGitHub Sponsorsに関する収入を確定申告に関するドキュメントです。

:warning: 確定申告の内容は人によって異なるため、詳細は税理士や所轄税務署で確認してください :warning:

:warning: このドキュメントは専門家のレビューを受けていないので、間違っている可能性があります :warning:

- [Issue作成はこちらから](https://github.com/azu/github-sponsors-tax/issues/new)

## 前提条件

- GitHub Sponsors登録時に[W-8BEN](https://www.irs.gov/pub/irs-pdf/iw8ben.pdf)をサブミットしている
- GitHub Sponsorsとは別に給与収入がある
- 日本に在住していて日本で確定申告する

Github Sponsporsの設定方法は次を参照してください。

- [ユーザアカウントに GitHub スポンサーを設定する - GitHub Docs](https://docs.github.com/ja/github/supporting-the-open-source-community-with-github-sponsors/setting-up-github-sponsors-for-your-user-account)

## 所得区分

GitHub Sponsorsで得た収入は、一般的には次のどちらかに分類するのが妥当だと考えられます。

- 開業届を出していない場合: [雑所得](https://www.nta.go.jp/taxes/shiraberu/taxanswer/shotoku/1500.htm)
- 開業届を出している場合: [事業所得](https://www.nta.go.jp/taxes/shiraberu/taxanswer/shotoku/1350.htm)

参考:

- [FANBOXの支援金はどの所得区分に該当しますか？また、課税対象ですか？ – pixivFANBOX](https://fanbox.pixiv.help/hc/ja/articles/900004208286-FANBOX%E3%81%AE%E6%94%AF%E6%8F%B4%E9%87%91%E3%81%AF%E3%81%A9%E3%81%AE%E6%89%80%E5%BE%97%E5%8C%BA%E5%88%86%E3%81%AB%E8%A9%B2%E5%BD%93%E3%81%97%E3%81%BE%E3%81%99%E3%81%8B-%E3%81%BE%E3%81%9F-%E8%AA%B2%E7%A8%8E%E5%AF%BE%E8%B1%A1%E3%81%A7%E3%81%99%E3%81%8B-)
- [税理士ドットコム - \[白色申告\]パトロンサイトなどの支援金の確定申告について](https://www.zeiri4.com/c_5/c_1059/q_58145/)

## 雑（その他）所得の入力

[国税庁 確定申告書等作成コーナー](https://www.keisan.nta.go.jp/kyoutu/ky/sm/top)を使った入力例です。

### 種目

提供しているコンテンツに依存します。
Sponsors登録の見返りに広告を出しているなら、`その他: 広告収入`など

- 参考: [FANBOXの支援金は税務上の「種目」だと何になりますか？ – pixivFANBOX](https://fanbox.pixiv.help/hc/ja/articles/900004208266-FANBOX%E3%81%AE%E6%94%AF%E6%8F%B4%E9%87%91%E3%81%AF%E7%A8%8E%E5%8B%99%E4%B8%8A%E3%81%AE-%E7%A8%AE%E7%9B%AE-%E3%81%A0%E3%81%A8%E4%BD%95%E3%81%AB%E3%81%AA%E3%82%8A%E3%81%BE%E3%81%99%E3%81%8B-)

### 業務に該当しますか

人によって異なるため、[こちらを参照](https://www.keisan.nta.go.jp/r2yokuaru/ocat2/ocat22/cid557.html)

> 業務に係るものとは、副業に係る収入のうち営利を目的とした継続的なものをいいます。  
> -- [No.1500 雑所得｜国税庁](https://www.nta.go.jp/taxes/shiraberu/taxanswer/shotoku/1500.htm)

### 収入金額

> GitHub Sponsorsの年間の収入

`https://github.com/sponsors/{user}/dashboard/payouts` から "View all payouts" でStripeの口座が確認できます。
Stripe Connectの口座で確認できる `20XX年` の合計金額が `収入金額` の値になります。

### 必要経費

人によって異なります。

### 源泉徴収税額

> `0`円

W-8BENをサブミットしている場合、GitHub Sposorsの支払いは源泉徴収されません。
そのため、源泉徴収税額は0円です

> GitHub は、GitHub Sponsors の支払いについて源泉徴収しません。 スポンサード開発者は、自らの税金を算出して支払う責任を負います。  
> [GitHub スポンサーの納税情報 - GitHub Docs](https://docs.github.com/ja/github/supporting-the-open-source-community-with-github-sponsors/tax-information-for-github-sponsors)

### 所得の生ずる場所（全角28文字以内）（ビル名等省略可）

`88 Colin P. Kelly Jr. Street, San Francisco, CA 94107 United States`が正式な場所ですが、
確定申告コーナーでは最大28文字のみしか入力できません。

最も確実な方法は、印刷して手書きで補完する方法です。

> 印刷して提出する方は、先頭から入力できるだけ入力し、印刷後に入力できなかった文字を、手書きで補完してください。
> e-Taxへ直接送信する方は、手書きで補完できないことから、できるだけ省略して入力してください
> [【確定申告書等作成コーナー】-入力内容が文字数制限を超えるときはどうしたらいいですか?](https://www.keisan.nta.go.jp/r1yokuaru/cat1/cat13/cat131/cid094.html)

- [ ] 無理やり28文字にしたバージョン: `88 Colin,SanFran,CA 94107,US`

申請が通るのかは未確認です

住所は変更されることがあるので次を参照してください。

- 参考: [GitHub Privacy Statement - GitHub Docs](https://docs.github.com/en/github/site-policy/github-privacy-statement#githubs-global-privacy-practices)

### 報酬などの支払者の氏名・名称（全角28文字以内）

> `GitHub, Inc.`

- 参考: [GitHub Privacy Statement - GitHub Docs](https://docs.github.com/en/github/site-policy/github-privacy-statement#githubs-global-privacy-practices)

---

## 事業所得の入力

- [ ] Welcome to Pull Request!

## License

CC0 1.0 Universal