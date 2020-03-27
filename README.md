添加-a 参数
# CNVD-2020-10487-Tomcat-Ajp-lfi-POC

拿到POC地址:https://github.com/nibiwodong/CNVD-2020-10487-Tomcat-ajp-POC

发现POC中只能访问ROOT目录 ,不能跨应用

所以改了下POC


CNVD-2020-10487(CVE-2020-1938), tomcat ajp lfi poc

Usage:
pip install -r requirements.txt

python poc.py  -p 8009 -f "/WEB-INF/web.xml" 127.0.0.1 -a applicationName

感谢原作者