# Readme
本リポでは、様々な環境におけるDatadogモニターリング用のAgentのコンフィグファイルのテンプレートをご用意します。
迅速にAgentのセットアップができるよう、以下詳細なステップをご確認お願い致します。

また、もし設定上より詳細な内容やAgentのコマンドをご確認されたい場合は以下のオフィシャルドキュメントにてご参照お願いします。  
&nbsp;&nbsp;&nbsp;Agentの使い方：<[https://docs.datadoghq.com/ja/agent/](https://docs.datadoghq.com/ja/agent/basic_agent_usage/?tab=Linux)>

**Windows**  
※注意点として、DatadogのコンフィグファイルはすべてエンコードがUTF-8であり、エンドーどutf-8を指定した上で編集するようお願いします。  
Step1.  
Step2.  
Step3.  
Step4.  

**Linux**  
Step1. LinuxサーバにAgentをインストール後、datadog/Host Based/Linux配下すべてのファイルをDatadogフォルダ(/etc/datadog-agent/)にコピーし上書き保存  
Step2. /etc/datadog-agent/datadog.yaml を編集し、<API_KEY>のところにDatadogのAPI keyで入れ替えて保存    
Step3. 以下コマンドでAgentを再起動      
&nbsp;&nbsp;&nbsp;Centos/Redhat/Amazon linxu: `sudo systemctl restart datadog-agent`  
&nbsp;&nbsp;&nbsp;Ubuntu/Debian: `sudo service datadog-agent restart`  
Step4. 以下コマンドでAgentのステータスを確認し、エラーがなかれば設定完了  
&nbsp;&nbsp;&nbsp;`sudo datadog-agent status`  
