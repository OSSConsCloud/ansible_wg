Jenkins playbook

## environment
ansible's version is 1.9.4 or 2.0.0.1

## vars
### /group_vars/all
* user (default "root" user)
    * 実行するユーザ名
*  proxy_env (http_proxy ,https_proxy)
    * 経由するproxyサーバのURL

### /roles/jenkins/vars/main.yml
* openjdk_items
    * yumで取得するopenjdkの名前
* yum_repository_path
    * yumのrepositoryを管理しているpath
* jenkins_key
    * jenkins repository用の鍵があるURL
* jekins_package_url
    * jenkins rpm packageのURL
* jenkins_host_name(default "localhost")
    * jenkinsのホストネーム
* jenkins_port (default "8080")
    * jenkinsのポート番号
* jenkins_updates_json_path
    * jenkinsのpluginを管理しているjsonファイルのpath
* jenkins_cli_url
    * jenkinsのcli用jarを取得できるURL
