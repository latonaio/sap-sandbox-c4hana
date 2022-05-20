<p align="center"> <img src="https://user-images.githubusercontent.com/91356865/144049159-1ebbd095-87d2-4a3c-81cb-277cc1d4c7b7.png" width="300"> </p> <p align="center"> Starting Up the API Environment on a "Full-of-Beans" SandBox </p>

***

# sap-sandbox-c4hana 
sap-sandbox-c4hana は、主にエッジコンピューティング環境において、外部システムをSAP C4HANAと統合することを目的として作成されたリソースをまとめたリポジトリです。  
sap-sandbox の 「sandbox」は、Netflix 韓国ドラマ 「START-UP」 より、すべての開発者のための 地ならし になればという想いから命名されました。  
なお、各リポジトリのリソースは、そのままクラウド環境におけるアプリケーションにも適用可能です。  

## 前提条件  
sap-sandbox-c4hana は、オンプレミス版である（＝クラウド版ではない）SAP C4HANA API の利用を前提としています。  
クラウド版APIを利用する場合は、ご注意ください。  

## Latona における SAP 領域・機能ごと の リソース整備状況    
下の図において、チェックマークが付いているリソースが、Latonaにおいて(少なくとも1次の)整備が行われたものであり、github上に公開されています。  

![リソース整備状況](documents/sap-sandbox-c4hana_20220521.png)

## 各リソースの所在  
各リソースの所在は、次の箇所です。  

### Central Functions
##### READS

* [sap-api-integrations-business-user-reads-c4](https://github.com/latonaio/sap-api-integrations-business-user-reads-c4)
* [sap-api-integrations-business-partner-reads-c4](https://github.com/latonaio/sap-api-integrations-business-partner-reads-c4)

##### SQL

* [sap-business-user-sql-c4](https://github.com/latonaio/sap-business-user-sql-c4)
* [sap-business-partner-sql-c4](https://github.com/latonaio/sap-business-partner-sql-c4)

### Touch Points
##### READS

* [sap-api-integrations-contact-reads](https://github.com/latonaio/sap-api-integrations-contact-reads)
* [sap-api-integrations-campaign-reads](https://github.com/latonaio/sap-api-integrations-campaign-reads)

##### SQL

* [sap-contact-sql](https://github.com/latonaio/sap-contact-sql)
* [sap-campaign-sql](https://github.com/latonaio/sap-campaign-sql)

### Operations
##### READS

* [sap-api-integrations-contract-reads](https://github.com/latonaio/sap-api-integrations-contract-reads)

##### SQL

* [sap-contract-sql](https://github.com/latonaio/sap-contract-sql)

## sap-sandbox-c4hana における SAP領域・機能 の選択基準
sap-sandbox-c4hana におけるSAP領域・機能は、SAP C4HANA のあらゆる領域・機能のうち、世界中の企業で繰り返し利用される、利用頻度の高いものと判断されるものが、選択されています。  

## SQL 作成の基準
sap-sandbox-c4hana において ある機能 に対して SQL を 作成するかどうか は、次の基準に基づいて判断されています。  

* 外部システム側で当該機能の必要十分なデータ量を保持する要求が、平均的にあるかどうか  
* 当該機能の平均的要求に、外部システムから帳票を出力することが含まれるかどうか  

上記基準のいずれかに当てはまれば、sap-sandbox-c4hanaにおいて SQL が作成され、該当するレポジトリが存在します。  
なお、SAP C4HANA API にて READ API が公開されていない機能については、sap-sandbox-c4hana において SQL は作成されません。  
