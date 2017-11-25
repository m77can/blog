#### 设置多个ssh-key
1. `ssh-keygen -t rsa -C "your@mail.com"`     
在 ~/.ssh/生成 id_rsa 、id_rsa.pub 文件.     
类似的可以生成 id_rsa_a,id_rsa_b.
2. ~/.ssh/ 下添加config文件,如下配置     
默认使用 id_rsa文件
````
Host github.com
    HostName github.com
    User git
    IdentityFile ~/.ssh/id_rsa_a

Host gitlab.com
    HostName gitlab.com
    User git
    IdentityFile ~/.ssh/id_rsa_b

````




