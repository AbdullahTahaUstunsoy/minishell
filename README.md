Bu proje, Bash'in (Bourne Again Shell) basitleştirilmiş bir versiyonunu C dilinde yeniden oluşturmayı amaçlayan bir **42 School** projesidir. Süreç yönetimi, dosya tanımlayıcıları (file descriptors) ve sistem çağrıları (system calls) üzerine yoğun bir çalışma içerir.



## Özellikler

Proje, temel bir kabuğun (shell) sahip olması gereken şu ana yeteneklere sahiptir:

- **Komut Yürütme:** `PATH` değişkenini kullanarak veya tam/bağıl yollarla sistemdeki programları çalıştırabilir.
- **Dahili Komutlar (Built-ins):**
  - `echo` (opsiyonel `-n` ile)
  - `cd` (mutlak veya bağıl yollarla)
  - `pwd`, `export`, `unset`, `env`, `exit`
- **Yönlendirmeler (Redirections):** - `<` (input), `>` (output)
  - `<<` (heredoc), `>>` (append mode)
- **Borular (Pipes):** `|` karakteri ile komutlar arası veri akışı sağlanır.
- **Değişken Genişletme:** `$VAR` ve `$?` (son çıkış kodu) desteği.
- **Sinyal Yönetimi:** `Ctrl-C`, `Ctrl-D` ve `Ctrl-\` sinyallerinin Bash ile uyumlu şekilde ele alınması.
- **Geçmiş (History):** `readline` kütüphanesi ile komut geçmişinde gezinebilme.


## Kurulum ve Çalıştırma

Projeyi derlemek için sisteminizde `gcc` ve `make` yüklü olmalıdır.

1. **Depoyu klonlayın:**
   ```bash
   git clone [https://github.com/AbdullahTahaUstunsoy/minishell.git](https://github.com/AbdullahTahaUstunsoy/minishell.git)
   cd minishell
2. Derleme yapın:
   make
3. Shell'i başlatın:
   ./minishell
