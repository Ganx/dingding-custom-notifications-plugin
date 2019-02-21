# Dingding Notification Plugin 

Dingding notification plugin is a simply config plugin, it can notify to your specified dingding group the build job status including:start build\build success\build failed. 

Chinese Intro: [中文介绍](https://github.com/jenkinsci/dingding-notifications-plugin/blob/master/readme-cn.md)

## Contributing
1. Fork it
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create new Pull Request
6. Dev build
```
mvn package --settings=./settings.xml
```


## Installation
1. create a Dingding robot in Dingding side

Dingding -> ... config -> new robot
![](https://github.com/jenkinsci/dingding-notifications-plugin/blob/master/static/entry.png?raw=true)

choose the 'custom robot' 
![](https://github.com/jenkinsci/dingding-notifications-plugin/blob/master/static/robot.png?raw=true)

config robot
![](https://github.com/jenkinsci/dingding-notifications-plugin/blob/master/static/create_robot.png?raw=true)

save the access token
![](https://github.com/jenkinsci/dingding-notifications-plugin/blob/master/static/token.png?raw=true)
2. Config Jenkins
After you installed the plugin, each job can add a post build step, choose 'dingding notification config'
![](https://github.com/jenkinsci/dingding-notifications-plugin/blob/master/static/config_post_step.png?raw=true)

input the access token in previous step, and please input the Jenkins URL
because plugin don't know where is your jenkins, if you wanna the notification can link directly to your build, please make sure the URL is the Jenkins ROOT url.
![](https://github.com/jenkinsci/dingding-notifications-plugin/blob/master/static/config.png?raw=true)
3. Enjoy!
![](https://github.com/jenkinsci/dingding-notifications-plugin/blob/master/static/result.png?raw=true)

4. Pipeline syntax support(merge from : [pull-request-5](https://github.com/jenkinsci/dingding-notifications-plugin/pull/5) ) 
![](https://user-images.githubusercontent.com/12759495/40215633-1b304956-5a94-11e8-9170-187aa506b583.png)
