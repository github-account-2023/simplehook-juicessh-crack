# simplehook-juicessh-crack

### 方法
- 在 `resources.arsc` 找 `Unlock Pro Features`, 找到 `com.sonelli.juicessh/string/unlock_pro_version_capitals` 然後 copy id
- 在 `com.sonelli.juicessh.activities` 的 `MainActivity` 中 找到 `const v1,0x7f1103eb`
- 在 `classes.dex` 找 哪個東西 用了 `com.sonelli.juicessh.activities` 的 `MainActivity`
- 找到後把返回結果強制改成 `true`

### 結果
- 由以上方法得出在 class `com.sonelli.oi0` 中的 `d(Ljava.lang.Object;)` 來知道是不是 Pro
- 因為要谷歌登入, 所以不直接改smali
- 利用 `simplehook` 把 `com.sonelli.oi0` 的 method `d` 和 param `java.lang.Object` 的返回 改成 `true`

### 使用
- 下載 [simplehook](https://github.com/littleWhiteDuck/SimpleHook)
- 點 右下方加號 把 `hook.json` 的內容 import 進去
- 登入
- 完成
