# تشفير المصدر

يوجد المصدر داخل `asma-editor-source.tar.gz.enc` وهو مشفّر باستخدام AES-256-CBC مع PBKDF2.

كلمة المرور محفوظة خارج GitHub لدى مالك المشروع. لا ترفع ملف كلمة المرور إلى المستودع ولا تشاركه علنًا.

للفك محليًا:

```bash
openssl enc -d -aes-256-cbc -pbkdf2 -iter 200000 \\
  -in asma-editor-source.tar.gz.enc \\
  -out asma-editor-source.tar.gz
```
