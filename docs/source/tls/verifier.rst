TLS Verifier
===============

verify host 与 cert中的域名是否匹配。

三种模式：

- allow all：完全不检查, ALLOW_ALL_HOSTNAME_VERIFIER
- strictWithSubDomains: 严格检查，泛域名只能匹配到同级子域名，BROWSER_COMPATIBLE_HOSTNAME_VERIFIER
- not strictWithSubDomains: 泛域名能匹配到所有下级子域名, STRICT_HOSTNAME_VERIFIER


参考资料
--------

- `AbstractVerifier.java <https://android.googlesource.com/platform/frameworks/base.git/+/master/core/java/org/apache/http/conn/ssl/AbstractVerifier.java>`_
