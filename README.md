# sap-sandbox-c4hana 
sap-sandbox-c4hana は、主にエッジコンピューティング環境において、外部システムをSAP C4HANAと統合することを目的として作成されたリソースをまとめたリポジトリです。  
sap-sandbox の 「sandbox」は、Netflix 韓国ドラマ 「START-UP」 より、すべての開発者のための 地ならし になればという想いから命名されました。  
なお、各リポジトリのリソースは、そのままクラウド環境におけるアプリケーションにも適用可能です。  

## 前提条件  
sap-sandbox-c4hana は、オンプレミス版である（＝クラウド版ではない）SAP C4HANA API の利用を前提としています。  
クラウド版APIを利用する場合は、ご注意ください。  

## Latona における SAP 領域・機能ごと の リソース整備状況    
下の図において、チェックマークが付いているリソースが、Latonaにおいて(少なくとも1次の)整備が行われたものであり、github上に公開されています。  

![リソース整備状況](documents/sap-sandbox-c4hana-20220812.drawio.png)

## 各リソースの所在  
各リソースの所在は、次の箇所です。  

### Central Functions
##### READS

* [sap-api-integrations-business-user-reads-c4](https://github.com/latonaio/sap-api-integrations-business-user-reads-c4)
* [sap-api-integrations-business-partner-reads-c4](https://github.com/latonaio/sap-api-integrations-business-partner-reads-c4)
* [sap-api-integrations-business-partner-relationship-reads](https://github.com/latonaio/sap-api-integrations-business-partner-relationship-reads)
* [sap-api-integrations-competitor-reads-c4](https://github.com/latonaio/sap-api-integrations-competitor-reads-c4)
* [sap-api-integrations-product-reads-c4](https://github.com/latonaio/sap-api-integrations-product-reads-c4)
* [sap-api-integrations-competitor-product-reads-c4](https://github.com/latonaio/sap-api-integrations-competitor-product-reads-c4)

##### SQL

* [sap-account-and-individual-customer-master-sql](https://github.com/latonaio/sap-account-and-individual-customer-master-sql)
* [sap-business-user-sql-c4](https://github.com/latonaio/sap-business-user-sql-c4)
* [sap-business-partner-sql-c4](https://github.com/latonaio/sap-business-partner-sql-c4)
* [sap-api-integrations-business-partner-relationship-reads ](https://github.com/latonaio/sap-api-integrations-business-partner-relationship-reads )
* [sap-competitor-sql](https://github.com/latonaio/sap-competitor-sql)
* [sap-product-sql-c4](https://github.com/latonaio/sap-product-sql-c4)
* [sap-competitor-product-sql](https://github.com/latonaio/sap-competitor-product-sql)


### Touch Points
##### READS

* [sap-api-integrations-contact-reads](https://github.com/latonaio/sap-api-integrations-contact-reads)
* [sap-api-integrations-activity-reads](https://github.com/latonaio/sap-api-integrations-activity-reads)
* [sap-api-integrations-chat-activity-reads](https://github.com/latonaio/sap-api-integrations-chat-activity-reads)
* [sap-api-integrations-campaign-reads](https://github.com/latonaio/sap-api-integrations-campaign-reads)
* [sap-api-integrations-promotion-reads](https://github.com/latonaio/sap-api-integrations-promotion-reads)

##### SQL

* [sap-contact-sql](https://github.com/latonaio/sap-contact-sql)
* [sap-activity-sql](https://github.com/latonaio/sap-activity-sql)
* [sap-chat-activity-sql](https://github.com/latonaio/sap-chat-activity-sql)
* [sap-campaign-sql](https://github.com/latonaio/sap-campaign-sql)
* [sap-promotion-sql](https://github.com/latonaio/sap-promotion-sql)

### Operations
##### READS

* [sap-api-integrations-contract-reads](https://github.com/latonaio/sap-api-integrations-contract-reads)
* [sap-api-integrations-sales-orders-reads-c4](https://github.com/latonaio/sap-api-integrations-sales-orders-reads-c4)
* [sap-api-integrations-sales-points-of-delivery-reads-c4](https://github.com/latonaio/sap-api-integrations-sales-points-of-delivery-reads-c4)
* [sap-api-integrations-sales-price-and-discount-list-reads](https://github.com/latonaio/sap-api-integrations-sales-price-and-discount-list-reads)
* [sap-api-integrations-payments-reads-c4](https://github.com/latonaio/sap-api-integrations-payments-reads-c4)

##### SQL

* [sap-contract-sql](https://github.com/latonaio/sap-contract-sql)
* [sap-sales-orders-sql](https://github.com/latonaio/sap-sales-orders-sql)
* [sap-sales-points-of-delivery-sql](https://github.com/latonaio/sap-sales-points-of-delivery-sql)
* [sap-sales-price-and-discount-list-sql](https://github.com/latonaio/sap-sales-price-and-discount-list-sql)
* [sap-payments-sql](https://github.com/latonaio/sap-payments-sql)

### Employee
##### READS
* [sap-api-integrations-job-definition-reads](https://github.com/latonaio/sap-api-integrations-job-definition-reads)
* [sap-api-integrations-time-entry-reads](https://github.com/latonaio/sap-api-integrations-time-entry-reads)

##### SQL
* [sap-employee-basic-data-sql](https://github.com/latonaio/sap-employee-basic-data-sql)
* [sap-job-definition-sql](https://github.com/latonaio/sap-job-definition-sql)
* [sap-time-entry-sql](https://github.com/latonaio/sap-time-entry-sql)


### Authentication
##### READS
* [sap-api-integrations-identity-reads](https://github.com/latonaio/sap-api-integrations-identity-reads)

##### SQL
* [sap-identity-sql](https://github.com/latonaio/sap-identity-sql)

### Marketing
##### READS
* [sap-api-integrations-survey-reads](https://github.com/latonaio/sap-api-integrations-survey-reads)
* [sap-api-integrations-survey-response-reads](https://github.com/latonaio/sap-api-integrations-survey-response-reads)

##### SQL
* [sap-survey-sql](https://github.com/latonaio/sap-survey-sql)
* [sap-survey-response-sql](https://github.com/latonaio/sap-survey-response-sql)



## sap-sandbox-c4hana における SAP領域・機能 の選択基準
sap-sandbox-c4hana におけるSAP領域・機能は、SAP C4HANA のあらゆる領域・機能のうち、世界中の企業で繰り返し利用される、利用頻度の高いものと判断されるものが、選択されています。  

## SQL 作成の基準
sap-sandbox-c4hana において ある機能 に対して SQL を 作成するかどうか は、次の基準に基づいて判断されています。  

* 外部システム側で当該機能の必要十分なデータ量を保持する要求が、平均的にあるかどうか  
* 当該機能の平均的要求に、外部システムから帳票を出力することが含まれるかどうか  

上記基準のいずれかに当てはまれば、sap-sandbox-c4hanaにおいて SQL が作成され、該当するレポジトリが存在します。  
なお、SAP C4HANA API にて READ API が公開されていない機能については、sap-sandbox-c4hana において SQL は作成されません。
