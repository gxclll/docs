# siteserver_User

用户表，存储用户信息。

字段 | 数据类型 | 数据大小 | 说明
------ | ------ | ------ | ------
Id | Integer | | 自增长主键
UserName | VarChar | 255 | 用户账号
Password | VarChar | 255 | 用户密码
PasswordFormat | VarChar | 50 | 密码加密格式，有`Clear`、`Encrypt`及`Hash`三种，分别代表不加密、可逆加密以及不可逆加密。
PasswordSalt | VarChar | 128 | 密钥，当PasswordFormat为`Encrypt`时使用的加密密钥
CreateDate | DateTime | | 创建时间
LastResetPasswordDate | DateTime | | 最后一次重设密码时间
LastActivityDate | DateTime | | 最后活动时间
CountOfLogin | Integer | | 登录次数
CountOfFailedLogin | Integer | | 连续登录失败次数
CountOfWriting | Integer | | 投稿次数
IsChecked | VarChar | 18 | 是否已审核用户
IsLockedOut | VarChar | 18 | 是否被锁定
DisplayName | VarChar | 255 | 用户姓名
Email | VarChar | 255 | 邮箱
Mobile | VarChar | 20 | 手机号
AvatarUrl | VarChar | 200 | 头像图片路径
Organization | VarChar | 255 | 组织
Department | VarChar | 255 | 部门
Position | VarChar | 255 | 职位
Gender | VarChar | 50 | 性别
Birthday | VarChar | 50 | 出生日期
Education | VarChar | 255 | 毕业院校
Graduation | VarChar | 255 | 学历
Address | VarChar | 255 | 地址
WeiXin | VarChar | 255 | 微信
Qq | VarChar | 50 | QQ
WeiBo | VarChar | 255 | 微博
Interests | VarChar | 255 | 兴趣
Signature | VarChar | 255 | 签名