# インフラストラクチャのセキュリティ

WordPressのコアを強化する前に、実装者はインスタンスがインストールされるサービスを強化することを検討する必要があります。 インフラストラクチャが実装者の制御下にない場合があります。 インフラストラクチャ側で修正されるべきものを緩和するためにWordPressで強化することができるものがありますが、常に深い防御を考慮する必要があります。 実装者は、インフラストラクチャ管理者に連絡し、その上にインストールされるアプリケーション（この場合はWordPress）をさらに保護するために、具体的な強化を求めることができます。

インフラストラクチャの強化の基盤は、オペレーティングシステムの強化です。 これは幅広いテーマであり、OSに大きく依存しています。特権、アクセス制御、認証、ロギングに関する主な懸案事項があります。 これは、現在のプロジェクトの範囲外のトピックであり、経験豊富なシステム管理者が担当しなければならないものです。

WordPressは多数のプラットフォームにインストールできますが、主な焦点はApacheとMySQLの最も一般的なコンポーネントです。 一般的なルールは、サポートされているすべてのインフラストラクチャコンポーネントに適用されます。

最高のデザインプラクティスに従えば、WordPressインスタンスの層は分離する必要があります。 しかし、WordPressのプレゼンテーション層とアプリケーション層は結合されています。 したがって、データベースとの分離は1つだけ可能です。 小規模なアプリケーションの場合は、一般的な方法ではありませんが、大規模なサイトの場合、これはセキュリティの観点からも必須です。

一般的なセキュリティの場合と同じように、インフラストラクチャを強化するために実行すべきもののリストであり、インフラストラクチャを強化する手段ではありません。

~~~
Infrastructure security

Before hardening the core of WordPress an implementer must consider hardening the services on which the instance will be installed. Sometimes the underlying infrastructure is not under the control of the implementer. While there are things that can be hardened on WordPress to mitigate things that are supposed to be fixed on the infrastructure side, one should always consider defense in depth. The implementer can contact the infrastructure administrator and ask for specific hardening in order to further protect the applications that will be installed on top of that, in this case WordPress.

The foundation of infrastructure hardening is operating system hardening. This is a broad subject and highly dependent on the OS, the main concerns being around privileges, access control, authentication and logging. It’s a topic outside the coverage of the current project and these are things that must be covered by experienced System Administrators.

WordPress can be installed on a multitude of platforms but the main focus below is on the most common components, Apache and MySQL. The general rules though apply to all supported infrastructure components.

Following best design practices, the tiers of the WordPress instance should be separated. However the presentation and application layers of WordPress are bound together. Thus only one separation is possible, the one with the database. For small applications it’s not a common practice, but for larger sites this becomes a must from a security but also a performance perspective.

As was the case with general security, this is just a list of things that should be performed in order to harden the infrastructure and not the means to do it. 
~~~
