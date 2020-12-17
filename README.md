# JSwork
<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>用户登录</title>
<link href="css/index.css" rel="stylesheet" type="text/css" />
<script language="javascript" type="text/javascript">
    var i=800;
    var msg=setInterval(function(){
        document.getElementById("qh1").style.left=i+"px";
        i++;
    }, 100);
    var code ;
    function createCode(){ 
        document.getElementById("qh4").style.display="none";
        code = new Array();
        var codeLength = 4;
        var checkCode = document.getElementById("checkCode");
        checkCode.value = "";
        var selectChar = new Array(2,3,4,5,6,7,8,9,'A','B','C','D','E','F','G','H','J','K','L','M','N','P','Q','R','S','T','U','V','W','X','Y','Z');
        for(var i=0;i<codeLength;i++) {
        var charIndex = Math.floor(Math.random()*32);
        code +=selectChar[charIndex];
        }
        checkCode.value = code;
    }
    function validate () {
        var inputCode = document.getElementById("yzm").value.toUpperCase();
        if(inputCode != code ){
        alert("验证码错误！");
        return false;
        }
        else {
        document.getElementById("qh3").style.display="none";
        document.getElementById("qh1").style.display="none";
        document.getElementById("qh4").style.display="block";
        var mg=setTimeout(function(){
            window.location.href="https://shuidi.cn/company-8a3447f925a737358a0ae31873ee6101.html?from=title&pa_from=1225";
        }, 3000);
        
        return true;
        }
    }
    </script>
<style type="text/css">
    .code{}
    .srk{ float: left;}
    .yzm{ float: right;}
    .bottom{ clear: both;}
 
@charset "utf-8";
input,textarea,select{
    margin:0;padding:0;
    font-size:12px;
    outline:none;
    resize:none;
}
html:root body,html:root input,html:root button,html:root textarea,html:root select{
    font-family:Tahoma,Geneva,'\5fae\8f6f\96c5\9ed1','\5B8B\4F53';
}
form,ul,ol,li,dl,dt,dd,h1,h2,h3,h4,h5,p{
    margin:0;
    padding:0;
    list-style:none;
}
a{
    text-decoration:none;
    color:#224892;
    outline:none;
}
a:hover{
    text-decoration:underline;
}
a img{
    border:none;
}
.button:hover{
    text-decoration:none;
    background-color:#1672e3;
}
.button:active{
    background-color:#3482e1;
}
.button span{
    position:relative;top:11px;
    display:inline-block;
    height:16px;
    line-height:16px;
    vertical-align:top;
    padding-left:8px;
}
.btn-green{
    height:50px;
    line-height:50px;
    background-color:#999;}
.btn-green:hover{
    background-color:#76bf48;
}
.btn-green:active{
    background-color:#51b73d;
}
.reg-slogan{
    height:50px;
    line-height:50px;
    text-align:center;
    font-size:16px;
}
.reg-form{
    width:328px;
    height:280px;
    margin:auto;
}
.reg-form .cell{
    position:relative;
    height:40px;
    margin-bottom:22px;
    zoom:1;}
.reg-form .cell input{position:absolute;
    top:0;left:0;
    width:304px;
    padding:7px 11px;
    font-size:16px;
    background:none;}
.reg-form .bottom{
    height:40px;
}
.reg-form .code{
    position:relative;
    height:40px;
    margin-bottom:22px;
    zoom:1;
}
.reg-form .code input{top:0;
    left:0;width:150px;
    padding:7px 11px;
    font-size:16px;
    background:none;
}
.reg-form .bottom{
    height:40px;
}
.reg-form .bottom .button{
    display:block;
    border-radius:3px;
}
.register-box{
    position: absolute;
    right: 54px;
    width: 396px;
    height: 476px;
    background: white;
    border-radius: 3px;
    top: 39px;
}
.barter_btn{
    border: 0px;
    background: transparent;
    outline: 0px;
}
.button{
    display:inline-block;
    height:40px;
    padding:0 15px;
    line-height:40px;
    text-align:center;
    font-size:18px;
    font-family:'Heiti SC','\5fae\8f6f\96c5\9ed1','\9ed1\4f53';
    color:white;
    border:0 none;
    background-repeat:repeat-x;
    background-position:0 0;
    cursor:pointer;
}
#qh1{
    position: absolute;
    left:800px;
    width: 150px;
    height: 30px;
    background-color:green;
}
#qh4{
    width: 400px;
    height: 300px;
    margin-left:400px;
    margin-top: 200px;
    font-size: 50px;
    color: green;
    background-color:;
}
#checkCode{
    font-size: 15px;
    color: green;
}

</style>
</head>
 
<body background="ztd1.jpg" onload="createCode();" >
<div id="qh1">验证码区分大小写</div>
<div id="qh4">登录成功，三秒后进入公司网页</div>
<div class="wrap" id="qh3">
    <div class="register-box"><br><br>
        <div class="reg-slogan"> 用户登录</div><br>
        <div class="reg-form">
        <form action="" class="login" method="post">
            <div class="cell"> 
           <input type="text" id="name" value="" maxlength="6" οnkeyup="checkName()" placeholder="  请输入用户名（最多6位）"  />
            </div>
            <div class="cell"> 
           <input type="password" name="" id="psd" value=""maxlength="11" placeholder="  请输入密码 （最多11位）" onBlur="javascript:ok_or_errorBylogin(this)" />
            </div>
            
            <div class="code">
            <div class="srk">
            <input type="text" name="code" id="yzm" class="text" maxlength="4"  placeholder="  请输验证码" /> 
            </div>
            <div class="yzm">
            <input type="button" id="checkCode" onclick="createCode()" title="刷新验证码" c >
            </div>
            </div>
               
            <div class="bottom"> <a id="login" onclick="validate()" class="button btn-green"> 登录</a></div>
            </form>
      </div>
            <div class="last">
        <button class="barter_btn" onClick="javascript:barter_btn(this)">没有账号?前往注册</button>  
        <a href="">忘记密码</a>
            </div>
       </div>
  </div>
<input οnclick='window.location="view-source:" + window.location.href' type="button" value="" name="Button7">
</body>
</html>

 
