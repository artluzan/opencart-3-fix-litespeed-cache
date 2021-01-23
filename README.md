# opencart-3-fix-litespeed-cache
1. Add header to .htaccess:

```sh
<FilesMatch "\.php$">
Header set Cache-Control: no-store, no-cache, must-revalidate
Header set Expires: Thu, 19 Nov 1981 08:52:00 GMT
Header set Pragma: no-cache
</FilesMatch>
```

2. Disable LiteSpeed ESI Feature in module setting
