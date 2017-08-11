# pictureverification
安卓中的图片验证码控件

## 导入方法：
### 1.Gradle：
          compile 'com.againstsky:vcode:1.0.1'
### 2.Maven:
          <dependency>
           <groupId>com.againstsky</groupId>
           <artifactId>vcode</artifactId>
           <version>1.0.1</version>
           <type>pom</type>
          </dependency>

## 使用方法：
### 在layout中加入控件：
           <com.againstsky.verificationcode.VerificationCodeView
        android:id="@+id/code_view"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        app:codeMode="2"
        app:codeQuantity="6"/>
                
  app:codeMode="2"//验证码模式，0纯数字，1纯字母，2字母数字随机混合模式</br>
  app:codeQuantity="6"//验证码数量，支持4，5，6三个模式
  
### 可选的Java中的设置：
- mCodeView.setCodeQuantity(6); //验证码数量
- mCodeView.setCodeMode(2); //验证码模式
- mCodeView.setPointInterfere(true); //是否开启点干扰
- mCodeView.setLineInterfere(true);  //是否开启线干扰
- mCodeView.setLineInterfereQuantity(8); //干扰线的数量
- mCodeView.setPointInterfereQuantity(200); //干扰点的数量
- mCodeView.setMatchCase(true); //是否区分验证码大小写，默认区分。如果设置为不区分大小写，则会返回全小写格式
### Java中获取验证码
  mCodeView.getVerificationCode();
## 效果图：
![image](https://github.com/againstsky/pictureverification/raw/master/show.png)

# 关于作者
### AgainstSky
#### 新手啦，大家一起努力一起加油啦！
### 小控件会继续更新解决其中的bug。欢迎大家加群讨论：188089649（群里有很多安卓java大神哦）

