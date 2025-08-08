# 💥 PHP Disable_Functions Exploit Collection

Kumpulan eksploitasi bypass `disable_functions` di PHP, yang bekerja pada berbagai versi (7.0–8.1). Cocok untuk analisis keamanan, riset exploitasi, dan pembelajaran teknik bypass pada environment terbatas.

> ⚠️ For **educational** and **ethical research** only.

---

## 📂 Daftar Exploit

### 🔹 [php-concat-bypass](php-concat-bypass)
Bypass `disable_functions` menggunakan **bug [#81705](https://bugs.php.net/bug.php?id=81705)**.  
✅ Support: PHP 7.3 – 8.1  
📌 Teknik: Manipulasi zval dengan teknik concatenation array & bucket override.  
🛠️ PoC recoded by: `ZeroHitman` (original: [mm0r1](https://github.com/mm0r1))

---

### 🔹 [php-filter-bypass](php-filter-bypass)
Bypass menggunakan **bug [#54350](https://bugs.php.net/bug.php?id=54350)**.  
✅ Support: PHP 7.0 – 8.0  
📌 Teknik: Abuse fitur `php://filter` stream wrapper untuk eksekusi tak langsung.

---

### 🔹 [php7-backtrace-bypass](php7-backtrace-bypass)
Bypass dengan **bug [#76047](https://bugs.php.net/bug.php?id=76047)**.  
✅ Support: PHP 7.0 – 7.4  
📌 Teknik: Abuse dari `debug_backtrace()` untuk manipulasi internal call stack.

---

### 🔹 [php7-gc-bypass](php7-gc-bypass)
Bypass `disable_functions` memanfaatkan **bug [#72530](https://bugs.php.net/bug.php?id=72530)**.  
✅ Support: PHP 7.0 – 7.3  
⛔ Bug ini telah di-*patch* pada PHP 7.4  
📌 Teknik: Abuse garbage collector dan use-after-free.

---

### 🔹 [php-json-bypass](php-json-bypass)
Bypass menggunakan **bug [#77843](https://bugs.php.net/bug.php?id=77843)**.  
✅ Support: PHP 7.1 – 7.3 *(rilis sebelum 30 Mei 2019)*  
📌 Teknik: Ekploitasi internal JSON parser.

---

## ✒️ Credits

- 💡 Original PoCs by [mm0r1](https://github.com/mm0r1)
- 🔧 Recode, UI & structure improvements by `ZeroHitman`
- 📚 Bug references from [bugs.php.net](https://bugs.php.net)

---

## 📜 License

MIT / Research Purpose Only – Please use responsibly.
