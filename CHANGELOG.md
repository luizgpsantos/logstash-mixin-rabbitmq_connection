## 6.0.0
   - Removed obsolete options `verify_ssl`, `debug`, `tls_certificate_path` and `tls_certificate_password`

## 5.0.2
   - Bug Fix: undefined method `value' for nil:NilClass with SSL enabled, but no certificates provided [#109](https://github.com/logstash-plugins/logstash-input-rabbitmq/issues/109)
## 5.0.1
   - Relax constraint on march hare to allow 3.x [#44](https://github.com/logstash-plugins/logstash-mixin-rabbitmq_connection/issues/44)
   - Validate :ssl_certificate_password as a password [#43](https://github.com/logstash-plugins/logstash-mixin-rabbitmq_connection/issues/43)
## 5.0.0
   - Mark deprecated options `debug`, `tls_certificate_path` and `tls_certificate_password` as obsolete
## 4.3.0
   - Bump march hare to 3.0.0
## 4.2.2
   - Bump march hare to 2.22.0 to properly convert LongString to String
## 4.2.1
   - Bump march_hare version to 2.20.0 to fix reconnection issues
## 4.2.0
   - Include URL of server when logging errors
   - Add warning log when connection is severed
## 4.1.3
   - Bump march_hare version to 2.19.0 to fix reconnection failures with proxies. See [#76](https://github.com/logstash-plugins/logstash-input-rabbitmq/issues/76) for
  more info
## 4.1.2
  - Retry the connection attempt if there is an IO Exception.
## 4.1.1
  - Remove internal Logstash deps that were not necessary
## 4.1.0
  - Fix SSL option to be boolean once again
  - Add separate ssl_version parameter
  - Mark verify_ssl parameter as obsolete since it never worked
  - Better checks for SSL argument consistency
## 2.4.0
  - Add SSL/TLS Support
  - Add support for "x-consistent-hash" and "x-modulus-hash" exchanges
## 2.3.1
  - use logstash-core-plugin-api as dependency instead of logstash-core directly
## 2.3.0
  - Bump march_mare version to 2.15.0 to fix perms issue internal to march hare gem (.jar not installed with o+r perms)
## 2.2.0
  - Rollback the changes in 2.1.0 . prefetch_count only belongs in the input plugin
## 2.1.0
  - Add prefetch_count config option
## 2.0.3
  - Add heartbeat setting
  - Add connect_timeout setting
## 2.0.0
  - Make LS2 compatible
## 1.0.1
  - Initial Release
