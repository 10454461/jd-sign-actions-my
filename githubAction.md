

#### 下方提供使用到的 **Secrets全集合**
| Name                    |   值   | 说明                                                         |
| :---------------------: | :----------: | ------------------------------------------------------------ |
| PLANT_BEAN_SHARECODES | `rxggow4kdwppbjuyjdvliwgahkbsbgemalhzlhy@qmnmamd3ukiwrd53w4fjmpmb6c7yyogrbfj2rry` `olmijoxgmjutyskl4hhoeibiavu3pkou3keebla@qmnmamd3ukiwrd53w4fjmpmb6c7yyogrbfj2rry` `olmijoxgmjutyskl4hhoeibiavu3pkou3keebla@rxggow4kdwppbjuyjdvliwgahkbsbgemalhzlhy` | 种豆得豆互助码 |
| JD_BEAN_SIGN_STOP_NOTIFY | false | 京东签到结果通知 |
| JD_BEAN_SIGN_NOTIFY_SIMPLE | false | 京东签到结果简洁版通知 |
| JD_BEAN_STOP | 1 | 京东签到自定义延迟签到 |
| MARKET_COIN_TO_BEANS | 20 | 京小超兑换京豆数量或商品名称 |
| MARKET_REWARD_NOTIFY | false | 京小超兑换奖品静默运行推送开关 |
| DREAMFACTORY_NOTIFY_CONTROL | false | 惊喜工厂静默运行推送开关 |
| FRUIT_BEAN_CARD | true |农场使用水滴换豆卡 |
| FRUIT_NOTIFY_CONTROL | false |东东农场默运行推送开关 |
| FACTORAY_WANTPRODUCT_NAME | '' | 东东工厂心仪商品 |
| JOY_FEED_COUNT | 10 | 宠汪汪喂食数量 |
| JOY_RUN_FLAG | true | 宠汪汪参加双人赛跑 |
| JD_JOY_REWARD_NAME | 20 | 宠汪汪积分兑换多少京豆 |
| JD_JOY_REWARD_NOTIFY | false | 宠汪汪兑换京豆静默运行推送开关 |
| jdJoyStealCoin | true | 宠汪汪偷好友狗粮/积分 |
| JOY_HELP_FEED | true | 宠汪汪帮好友喂食 |
| MONEY_TREE_SELL_FRUIT | true | 摇钱树是否卖出金果 |
| PET_NOTIFY_CONTROL | false | 东东萌宠静默运行推送开关 |
| PURCHASE_SHOPS | true | 东东小窝加购商品 |
| SUPERMARKET_LOTTERY | false | 京小超抽奖 |
| SUPERMARKET_UPGRADE | false | 京小超自动升级 |
| TG_BOT_TOKEN | 1290395423:AAHtbN3JApDKAJCHPIVN7SF1Zkby5cluPk4 | telegram推送 |
| TG_USER_ID | 1049578757 | telegram推送 |

github actions Secrets
github自动化设置

JD_COOKIE string #京东cookie,多个账号的cookie使用&隔开或者换行
JD_USER_AGENT string #自定义此库里京东系列脚本的UserAgent，不懂不知不会UserAgent的请不要随意填写内容。
JD_DEBUG true/false #运行脚本时，是否显示log,默认显示。改成false表示不显示，注重隐私的人可以在设置secret -> Name:JD_DEBUG,Value:false
PUSH_KEY string #微信推送 cookie失效推送server酱的微信通知
BARK_PUSH string #BARK推送 cookie失效推送BARK这个APP,填写内容是app提供的设备码，例如：https://api.day.app/123 ，那么此处的设备码就是123
BARK_SOUND string #BARK推送 bark推送声音设置，例如choo,具体值请在bark-推送铃声-查看所有铃声
TG_BOT_TOKEN string #telegram推送 tg推送,填写自己申请@BotFather的Token,如10xxx4:AAFcqxxxxgER5uw
TG_USER_ID int #telegram推送 tg推送,填写@getuseridbot中获取到的纯数字ID
DD_BOT_TOKEN srting #钉钉推送 钉钉推送官方文档 ,只需https://oapi.dingtalk.com/robot/send?access_token=XXX 等于符号后面的XXX， 注：如果钉钉推送只填写DD_BOT_TOKEN，那么安全设置需勾选自定义关键词，内容输入输入账号即可，其他安全设置不要勾选
DD_BOT_SECRET srting #钉钉推送 密钥，机器人安全设置页面，加签一栏下面显示的SEC开头的字符串 , 注:填写了DD_BOT_TOKEN和DD_BOT_SECRET，钉钉机器人安全设置只需勾选加签即可，其他选项不要勾选,再不懂看 https://raw.githubusercontent.com/lxk0301/jd_scripts/master/icon/DD_bot.png
IGOT_PUSH_KEY string #iGot推送 iGot聚合推送，支持多方式推送，确保消息可达。 https://wahao.github.io/Bark-MP-helper

京东签到
JD_BEAN_SIGN_STOP_NOTIFY true/false #jd_bean_sign.js脚本运行后不推送签到结果通知，默认推送，填true表示不发送通知
JD_BEAN_SIGN_NOTIFY_SIMPLE true/false #jd_bean_sign.js脚本运行后推送签到结果简洁版通知，默认推送全部签到结果，填true表示推送简洁通知 https://raw.githubusercontent.com/lxk0301/jd_scripts/master/icon/bean_sign_simple.jpg
JD_BEAN_STOP int #d_bean_sign.js自定义延迟签到,单位毫秒. 默认分批并发无延迟. 延迟作用于每个签到接口, 如填入延迟则切换顺序签到(耗时较长),如需填写建议输入数字1
东东萌宠
PET_NOTIFY_CONTROL true/false #东东萌宠推送开关 控制京东萌宠是否静默运行,false为否(发送推送通知消息),true为是(即：不发送推送通知消息)
东东农场
FRUIT_NOTIFY_CONTROL true/false #东东农场推送开关 控制京东农场是否静默运行,false为否(发送推送通知消息),true为是(即：不发送推送通知消息)
FRUIT_BEAN_CARD true/false #农场使用水滴换豆卡 农场使用水滴换豆卡(如果出现限时活动时100g水换20豆,此时比浇水划算,推荐换豆),true表示换豆(不浇水),false表示不换豆(继续浇水),脚本默认是浇水
京东818互助码
JD_818_SHAREID_NOTIFY true/false #京东818互助码通知开关 控制jd_818.js脚本是否在获取互助码后通知,true为是(发送推送通知消息),false为否(即：不发送推送通知消息)
宠汪汪-jd_joy_feedPets.js
JOY_FEED_COUNT 10/20/40/80 #宠汪汪喂食数量 控制脚本喂食数量 ,可以填的数字10,20,40,80 , 其他数字不可.
JOY_HELP_FEED true/false #宠汪汪帮好友喂食 是否给好友喂食,false为否,true为是(给好友喂食)
JOY_RUN_FLAG true/false #宠汪汪参加双人赛跑 是否参加双人赛跑,false为否,true为是，脚本默认是true
JD_JOY_REWARD_NAME 0/20/500 #宠汪汪积分兑换多少京豆 目前可填值为20或者500,脚本默认20,0表示不兑换京豆
JD_JOY_REWARD_NOTIFY true/false #宠汪汪兑换京豆推送开关 控制jd_joy_reward.js脚本是否静默运行,false为否(发送推送通知消息),true为是(即：不发送推送通知消息)
jdJoyStealCoin true/false #宠汪汪偷好友狗粮/积分 是否偷好友狗粮/积分,false为否,true为是(偷好友狗粮/积分)
京小超
SUPERMARKET_UPGRADE true/false #京小超自动升级 顺序:解锁升级商品、升级货架,true表示自动升级,false表示关闭自动升级
SUPERMARKET_LOTTERY true/false #京小超抽奖 是否用500蓝币去抽奖，true表示开启，false表示关闭。
BUSINESS_CIRCLE_JUMP true/false #京小超自动更换商圈 小于对方300热力值自动更换商圈队伍,true表示运行,false表示禁止
MARKET_COIN_TO_BEANS 20/1000/碧浪洗衣凝珠/... #控制jd_blueCoin.js兑换京豆数量,可输入值为20或者1000的数字或者其他商品的名称,例如碧浪洗衣凝珠
MARKET_REWARD_NOTIFY true/false #京小超兑换奖品推送开关 控制jd_blueCoin.js兑换奖品成功后是否静默运行, false为否(发送推送通知消息),true为是(即：不发送推送通知消息)
摇钱树
MONEY_TREE_SELL_FRUIT true/false #摇钱树是否卖出金果 控制摇钱树脚本是否自动卖出金果兑换成金币，true卖出，false不卖出，默认true
东东工厂
FACTORAY_WANTPRODUCT_NAME tring #东东工厂心仪商品 提供心仪商品名称(请尽量填写完整和别的商品有区分度)，达到条件后兑换，如不提供则会兑换当前所选商品
惊喜工厂
DREAMFACTORY_NOTIFY_CONTROL true/false #惊喜工厂推送开关 控制jd_dreamFactory.js兑换奖品成功后是否静默运行, false为否(发送推送通知消息),true为是(即：不发送推送通知消息)
东东小窝
PURCHASE_SHOPS true/false #东东小窝加购商品 是否一键加购商品到购物车，默认不加购 true表示加购，false表示不加购

互助码
FRUITSHARECODES srting #东东农场互助码 填写规则请看 jdFruitShareCodes.js 或见下方互助码的填写规则
PETSHARECODES srting #东东萌宠互助码 填写规则请看 jdPetShareCodes.js 或见下方互助码的填写规则
PLANT_BEAN_SHARECODES srting #种豆得豆互助码 填写规则请看 jdPlantBeanShareCodes.js 或见下方互助码的填写规则
SUPERMARKET_SHARECODES srting #京小超商圈互助码 填写规则请看 jdSuperMarketShareCodes.js 或见下方互助码的填写规则 
DDFACTORY_SHARECODES srting #东东工厂互助码 填写规则请看 jdFactoryShareCodes.js 或见下方互助码的填写规则
DREAM_FACTORY_SHARE_CODES srting #京喜工厂互助码 填写规则请看 jdDreamFactoryShareCodes.js 或见下方互助码的填写规则

TG_PROXY_HOST tring #Telegram代理的IP 代理类型为 http。例子：http代理 http://127.0.0.1:1080 则填写 127.0.0.1
TG_PROXY_PORT int #Telegram 代理的端口 例子：http代理 http://127.0.0.1:1080 则填写 1080

#互助码的填写规则
同一个京东账号的好友互助码用@隔开,不同京东账号互助码用&或者换行隔开,下面给一个文字示例和具体互助码示例说明
京东账号1的shareCode1@京东账号1的shareCode2&京东账号2的shareCode1@京东账号2的shareCode2

关于脚本推送通知
目前默认只有jd_fruit.js,jd_pet.js,jd_bean_sign.js,jd_818.js四个脚本每次运行后都通知
jd_plantBean.js是每周一收集京豆后通知一次，
jd_joy_reward.js是每次兑换到了京豆通知一次，
jd_blueCoin.js是每次兑换到了奖品通知一次，
jd_818.js是每次获取新的互助码会通知一次，以帮助您快速上车，
其余的脚本平常运行都是不通知，只有在京东cookie失效后，才会推送通知

GitHub Actions 手动触发方式进化史 https://p3terx.com/archives/github-actions-manual-trigger.html    
GitHub Actions 入门教程 https://p3terx.com/archives/github-actions-started-tutorial.html