# simplehook-juicessh-crack

### 方法
- 在 `resources.arsc` 找 `Unlock Pro Features`, 找到 `com.sonelli.juicessh/string/unlock_pro_version_capitals` 然後 copy id
- 在 `com.sonelli.juicessh.activities` 的 `MainActivity` 中 找到 `const v1,0x7f1103eb`
- 在 `classes.dex` 找 哪個東西 用了 `com.sonelli.juicessh.activities` 的 `MainActivity`
- 找到後把返回結果強制改成 `true`
