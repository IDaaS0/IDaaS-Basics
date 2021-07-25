## SAMLとは？

SAMLとは、Security Assertion Markup Languageの略称であり、利用者の認証や認可に関する情報を伝達するためのXMLベースのマークアップ言語の一つ。標準化団体のOASISによって2020年に策定され、2005年にはバージョン2.0となっています。

## 利用場面

> 1回認証を通れば許可がされているすべてのサービスが使えるようになる仕組み（シングルサインオン）を実現するときに使われる仕組みのひとつです。

## 属性情報の付与可能

> SAMLはユーザーの属性情報なども付与することができます。単純にユーザーの認証を行うだけでなく、ユーザーがクラウドサービス内のどの機能を許可するなどの認可も行えるプロトコルです。例えば、営業部や情報システム部といった属性情報をユーザー認証に付与することで、この機能は営業部にしか使わせないといったリソースへのアクセス制御が容易にできるようになります。

## IdP

SAMLでは、認証情報を提供する側をIdentity Providerと呼びます。

## SP

SAMLでは、認証情報を利用する側をService Providerと呼びます。

## SAMLの認証フロー

| フロー名 | フローの説明 |
----|---- 
| **IdP-initiated SSO** | ユーザーがIdPへアクセスをしてSAMLの処理を開始した場合のフロー |
| **SP-initiated SSO** | ユーザーがSPへアクセスをしてSAMLの処理を開始した場合のフロー |

### **IdP-initiated SSO**

![](https://i.imgur.com/hrHWa9u.png)

1. ユーザーがIdPの Sign on 画面へアクセスします。
2. IdPからユーザー認証を開始します。
3. ユーザーは認証情報を入力します。
4. IdPで認証後、ユーザーはどのSPへアクセスするか選択をします。
5. IdPは、アサーションを作成しデジタル署名をしてからユーザーのブラウザを介してSPへ送ります。
6. SPは、アサーションを検証し問題がなければユーザーへサインオンを許可します。

### **SP-initiated SSO**

![](https://i.imgur.com/O0QRmAM.png)


1. ユーザーがSPへアクセスします。
2. SPからユーザーのブラウザーを介してIdPへ認証申請が送られます。
3. IdPからユーザー認証を開始します。
4. ユーザーは認証情報を入力します。
5. IdPはユーザー認証を行い、アサーションを作成しでデジタル署名をしてユーザーのブラウザーを介しSPへ送ります
6. SPはアサーションを検証し問題がなければユーザーへサインオンを許可します

## SAML2.0のバインディングについて

- HTTP Redirect Binding　：URLに含めブラウザーを介する
- HTTP POST Binding　　：HTMLに含めブラウザーを介する
- HTTP Artifact Binding　 ：SPとIdPが直接通信する

[IBM SAML 2.0 バインディング](https://www.ibm.com/docs/ja/sva/9.0.7?topic=overview-saml-20-bindings)


## 参考
[SAMLとは - CloudGate](https://cg-support.isr.co.jp/hc/ja/articles/900002918806-SAML%E3%81%A8%E3%81%AF)







