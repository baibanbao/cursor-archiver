- 详细记录：怎样建立一个Farbox网站
    首先，从hepo那里取得一个邀请码
        - 这次给的邀请码是：邀请码 619d20ca7a4beb4a83126efc
            - 有效期是10年
    然后，登录到farbox.org网站
        - 点击register
        - 输入：invitation code
            - 如图
                - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhaozhongwen%2F7oRLo9oM60.png?alt=media&token=c015acc3-e80c-4892-a38f-f5f2f069d821)
    绑定域名，这一步很关键
        - 点击绑定域名，需要到域名注册商那里修改dns
            - 这里记住host那里要加www
                - 我之前加了@不奏效
            - 1, A record point to **101.33.123.204**
            - 2, The value of TXT record is **927a014c26efbd5323fe51f4bd07f8db5e229fcc**
        - 修改完dns，才能绑定域名
    SSL设定
        - 首先要去https://www.cloudflare.com/ 
            - 使用其免费服务
            - Add a Site
                - 提示修改nameserver
                    - algin.ns.cloudflare.com
                    - nelly.ns.cloudflare.com
            - 然后出现 Quick Start Guide
            - Always Use HTTPS 选择点亮
            - 其余默认
            - 设定好之后，选择上面菜单里的ssl/tls
                - 二级菜单中选择 Client Certificates
                    - Create Certificate
                        - Create
                            - ## Client Certificate and Key Generation
                                - 
                                - Save the certificate and private key below to your client. To save, **Click to copy** and paste the contents into different files on your client, e.g. example.com.pem and example.com.key
                - 把生成的证书和私钥拷贝到farbox设定界面中去
                    - Install ssl 即可
    选择模板
        - Chose Builtin Theme:
    设定网站信息
    Done
- 元中文读书会
    - 定价策略
        - debts
            - loan 361006.18
                - jb
                    - 163400 
                        - in 17892.30
                - zlhqd
                    - 150589.65
                        - in  19237.82
                - lightning
                    - 5382.42
                    - 4503.99
                - sum=361006.18
            - 3680/50 weeks
                - each week 73.6
                    - 4 cups of coffee
            - 100 students
                - 
    - 
