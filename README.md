## IDaaSとは？

IDaaS(Identity as a Service)とは、ID管理を行うクラウドサービスで、一回ログインすれば、事前に登録・連携している複数のクラウドサービスが使えるようになる。

## IDaasの機能要件

|  項目  |  内容  |
| ---- | ---- |
|  認証・シングルサインオン  |  ユーザーの認証、多要素認証、複数のクラウドサービスへのシングルサインオン(SSO)など  |
|  ID管理  |  IDaaS自体と登録・連携したクラウドサービスそれぞれのID管理機能を提供する |
|  ID連携  |  IDaaSと各クラウドサービスとのID連携および、オンプレミスの社内システムとのID連携機能を提供  |
|  認可  |  認可機能には、クラウドサービスへの適切なアクセス権の付与、条件によるクラウドサービスへのアクセスコントロールが含まれる  |
|  監査  |  IDaaSおよびクラウドサービスに対する認証や、管理者作業のログを取得する機能のこと。  |  

```
***IDフェデレーションとIDプロビジョニング***

・IDフェデレーションとは
独自のID管理システムを持つ複数のサービスで、それぞれのユーザーIDをリンクさせる。IDフェデレーションにより、一度認証されていれば再び認証画面を表示せずとも連携されアクセスが可能となる。

・IDプロビジョニングとは
複数サービスでIDの整合性を取るなど、自動的に管理する機能だ。IDプロビジョニングにより、あるIDを追加したら他の連携サービスでも自動的にIDが追加される。IDを削除すると、自動的に他の連携サービスでもIDが削除され、ID管理の手間が大幅に削減される。
```

## IDaaSの主要プレイヤーとサービス解説

|  国内の主要プレーヤー  |  サービス名  |
| ---- | ---- |
|  Microsoft  |  Azure AD  |
|  Okta  |  Okta Identity Cloud  |
|  OneLogin  |  OneLogin  |
|  Google  |  Google Cloud Identity  |
|  Henge  |  Henge One  |
|  GMO Global Sign  |  Trust Login  |
|  ISR  |  Cloud Gate  |
|  Oracle  |  Oracle Identity Cloud Service  |
|  SAP  |  SAP Identity and Access Management  |
|  Secioss  |  Secioss Link  |
| Auth0  |  Auth0  |
|  Firebase(Google)  |  Firebase Auth  |
|  Amazon  |  Cognito User Pools  |

## メリット・デメリット

### 1. 作業の効率化

IDaaSを導入することでIDやパスワードの管理作業が簡単になり、管理者の負担を軽減できます。　また、同じパスワードを使いまわさなくなるため、セキュリティも向上します。

### 2. セキュリティ面の向上

IDやパスワードだけでなく、多要素認証でのログインを導入しているシステムが多いため、セキュリティ面を向上させられます。そのため、時間や場所を問うことなく、安心してシステムをりようできるようになります。

## 参考記事

- [IDaaSについて詳しく解説｜IDaaSのメリットやサービスも紹介](https://www.fenet.jp/infla/column/technology/202/#IDaaS%E3%81%AB%E3%82%88%E3%81%A3%E3%81%A6%E3%82%82%E3%81%9F%E3%82%89%E3%81%95%E3%82%8C%E3%82%8B%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0%E3%81%AE%E5%8A%B9%E7%8E%87%E5%8C%96)

- [【2021年版】初心者向け！おすすめのIDaaS6選を徹底比較](https://kigyolog.com/service.php?id=179#5-0)