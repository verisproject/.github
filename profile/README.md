# VERIS

**Verified Election via Resilient Immutable System**

Elections are a cornerstone of democratic societies worldwide and confidence in their outcomes is critical to the healthy functioning of democracy. Despite this, suspicions and allegations of manipulation regarding election results are increasing in many countries while centralized election systems used globally lack the tools to definitively refute these allegations. In widely used traditional systems, votes cannot be independently audited, voters cannot verify that their vote has been counted correctly, and the rules governing the process may be changed by centralized authorities during the course of an election. In addition, slow vote-counting processes and high operational costs observed in elections around the world continue to represent structural challenges on a global scale.

VERIS is a blockchain protocol being developed to offer an innovative and viable solution to these common global problems. Through the distributed and immutable nature of blockchain technology, the VERIS Project aims to ensure that election rules cannot be altered by any authority once the electoral process has begun; that votes can be independently audited and counted by anyone; that every voter can verify that their vote has been correctly recorded and counted; and that election costs arising from high labor requirements can be reduced, enabling elections to be conducted in a more sustainable manner. The project also aims to demonstrate the protocol's scalability through a 1:1-scale election simulation.

## Problems Solved

| | |
|---|---|
| **1 · Voters can be sure of their vote** | Every voter can personally verify that their vote was recorded for the party they chose and included in the count. |
| **2 · Safe under coercion** | Even if a voter is forced to reveal their verification information, their real vote is not exposed. |
| **3 · Identity and vote never meet** | Who voted and how they voted are never brought together in any record or by any institution. |
| **4 · Anyone can audit the count** | Any observer can mathematically verify that the national result was computed correctly, without seeing a single vote. |
| **5 · No forged or double votes** | Unauthorised or repeated votes are rejected. Even if the nodes operating the system collude, independent auditing detects it. |
| **6 · Designed for national scale** | With parallel sub-chains, a single computer processed over 2,500 votes per second; a 1:1-scale national election simulation is in preparation. |

> **No other published system provides all three of these properties at the same time:**
> voters verify their vote · resists coercion · national scale.

| System | Voter verifies their vote | Coercion-resistant | National scale | Public audit |
|---|:-:|:-:|:-:|:-:|
| **VERIS** | ✅ | ✅ | ✅ | ✅ |
| Estonia i-Voting | 🟡 verification limited to 15 minutes after voting, on a separate device | ❌ relies only on revoting against coercion | ✅ | 🟡 tally data is not public, only authorised auditors receive it |
| Swiss Post | ✅ | ❌ has no mechanism to protect votes cast at home from coercion | 🟡 the law caps electronic voting at 30% of a canton's and 10% of the national electorate | 🟡 audit data is not public, only authorised auditors receive it |
| Helios | ✅ | ❌ voters can produce a receipt that proves their vote | ❌ depends on one central server; its designers do not recommend it for public elections | ✅ |
| Belenios | ✅ | ❌ voters can produce a receipt that proves their vote | 🟡 credentials are distributed to voters by email; not used in national elections | ✅ |
| Civitas (JCJ) | ✅ | ✅ | ❌ every vote is compared with every other; cost grows quadratically with voters | ✅ |
| Hyperion | ✅ | 🟡 needs a private notification channel to each voter; protects only against a limited coercer | ❌ heavy mixing and decryption: 100k voters ≈ 3.2 hours | ✅ |

✅ provides · 🟡 partially · ❌ does not

<details><summary>Why is revoting not a solution?</summary>

Some systems rely on revoting against coercion: a vote cast under pressure is overridden if the voter later casts a new vote in secret. This approach fails under real coercion:

- The coercer can keep the voter under watch until voting closes, or take their credentials; the voter cannot vote again.
- Voting again in secret carries the fear of being caught. The coercion keeps working through that fear.
- If traces such as the number or timing of votes are visible in the records, the coercer can tell whether the vote was changed.

For this reason, approaches that rely on revoting are not counted as coercion-resistant in the table.

</details>

## Development

The VERIS repositories are private while the protocol is under closed development. Researchers and developers who would like to review the code or take part in development can write to contact@veris.vote. Participation does not come with any obligation to contribute.

---

Seçimler, dünya genelinde demokratik toplumların temel yapı taşıdır ve sonuçlarına duyulan güven, demokrasinin sağlıklı işleyişi için kritik öneme sahiptir. Buna rağmen pek çok ülkede seçim sonuçlarına yönelik şüphe ve manipülasyon iddiaları giderek artmakta; dünya genelinde kullanılan merkezi seçim sistemleri bu iddiaları kesin biçimde çürütecek araçlardan yoksun kalmaktadır. Yaygın olarak kullanılan geleneksel sistemlerde oylar bağımsız olarak denetlenemez, seçmen oyunun doğru sayıldığını doğrulayamaz ve kurallar merkezi otoritelerin kararlarıyla süreç içinde değişebilir. Buna ek olarak dünyanın dört bir yanındaki seçimlerde görülen yavaş sayım süreçleri ve yüksek operasyonel maliyetler de küresel çapta yapısal sorunlar olarak varlığını sürdürmektedir.

VERIS, dünya genelindeki bu ortak sorunlara yenilikçi ve uygulanabilir bir çözüm sunmak amacıyla geliştirilmekte olan bir blockchain protokolüdür. VERIS Projesi, bu protokol ile blockchain teknolojisinin dağıtık ve değiştirilemez yapısı sayesinde; seçim kurallarının süreç başladıktan sonra hiçbir otorite tarafından değiştirilememesini, oyların herkes tarafından bağımsız şekilde denetlenip sayılabilmesini, her seçmenin kendi oyunun doğru sayıldığından emin olabilmesini, seçimlerin yüksek iş gücü gereksiniminden kaynaklanan maliyetlerinin düşürülmesini ve daha sürdürülebilir bir şekilde seçimlerin yapılabilmesini hedeflemekte ve protokolün ölçeklendirilebilirliğini 1:1 ölçek seçim simülasyonu üzerinden kanıtlamayı hedeflemektedir.

## Çözülen Problemler

| | |
|---|---|
| **1 · Seçmen oyundan emin olur** | Her seçmen, oyunun kendi seçtiği partiye kaydedildiğini ve sayıma girdiğini kendisi doğrulayabilir. |
| **2 · Baskı altında da güvende** | Seçmen zorla doğrulama bilgisini gösterse bile gerçek oyu ortaya çıkmaz. |
| **3 · Kimlik ile oy hiçbir yerde birleşmez** | Kimin oy kullandığı ile hangi oyun verildiği, hiçbir kayıtta ve hiçbir kurumda bir araya gelmez. |
| **4 · Sayım herkes tarafından denetlenir** | Herhangi bir gözlemci, tek bir oyu bile görmeden ulusal sonucun doğru hesaplandığını matematiksel olarak doğrulayabilir. |
| **5 · Sahte ve çift oy giremez** | Yetkisiz ya da ikinci kez verilen oy reddedilir. Sistemi işleten düğümler anlaşsa bile bağımsız denetim bunu yakalar. |
| **6 · Ulusal ölçeğe göre tasarlandı** | Paralel çalışan alt zincirlerle tek bir bilgisayarda saniyede 2.500'ü aşkın oy işlendi; 1:1 ölçek ulusal seçim simülasyonu hazırlanmaktadır. |

> **Yayımlanmış sistemler arasında bu üç özelliği aynı anda sağlayan başka bir sistem bulunmamaktadır:**
> seçmen oyunu doğrular · baskıya dayanır · ulusal ölçekte çalışır.

| Sistem | Seçmen oyunu doğrular | Baskıya dayanıklı | Ulusal ölçek | Herkese açık denetim |
|---|:-:|:-:|:-:|:-:|
| **VERIS** | ✅ | ✅ | ✅ | ✅ |
| Estonya i-Voting | 🟡 doğrulama, oy verdikten sonraki 15 dakikayla ve ayrı bir cihazla sınırlı | ❌ baskıya karşı yalnızca tekrar oya güvenir | ✅ | 🟡 sayım verileri kamuya açık değil, yalnızca yetkili denetçilere verilir |
| İsviçre Post | ✅ | ❌ evden verilen oyu baskıdan koruyacak bir mekanizma içermiyor | 🟡 yasa, elektronik oyu kanton seçmenlerinin %30'u ve ülke genelinin %10'u ile sınırlıyor | 🟡 denetim verileri kamuya açık değil, yalnızca yetkili denetçilere verilir |
| Helios | ✅ | ❌ seçmen, oyunu kanıtlayan bir makbuz üretebiliyor | ❌ tek merkezi sunucuya dayanıyor; tasarımcıları kamu seçimleri için önermiyor | ✅ |
| Belenios | ✅ | ❌ seçmen, oyunu kanıtlayan bir makbuz üretebiliyor | 🟡 kimlik bilgileri seçmenlere e-postayla dağıtılıyor; ulusal seçimde kullanılmadı | ✅ |
| Civitas (JCJ) | ✅ | ✅ | ❌ her oy diğer tüm oylarla karşılaştırılıyor; maliyet seçmen sayısının karesiyle artıyor | ✅ |
| Hyperion | ✅ | 🟡 seçmene gizli bir bildirim kanalı gerektiriyor; yalnızca sınırlı baskıya karşı koruyor | ❌ ağır karıştırma ve şifre çözme işlemleri: 100 bin seçmen ≈ 3,2 saat | ✅ |

✅ sağlar · 🟡 kısmen · ❌ sağlamaz

<details><summary>Tekrar oy neden çözüm değil?</summary>

Bazı sistemler baskıya karşı tekrar oya güvenir: baskı altında verilen oy, seçmen daha sonra gizlice yeniden oy verirse geçersiz sayılır. Bu yaklaşım gerçek baskı koşullarında işe yaramaz:

- Baskı yapan kişi seçmeni oylama süresi bitene kadar gözetim altında tutabilir ya da kimlik bilgisine el koyabilir; seçmen yeniden oy veremez.
- Gizlice yeniden oy vermek yakalanma korkusu yaratır. Baskının etkisi bu korku üzerinden sürer.
- Oy sayısı ya da zamanı gibi izler kayıtlarda görünürse baskı yapan kişi oyun değiştirilip değiştirilmediğini anlayabilir.

Bu nedenle tabloda tekrar oya dayanan yaklaşımlar baskıya dayanıklı sayılmamıştır.

</details>

## Geliştirme

Protokol kapalı geliştirme aşamasında olduğundan VERIS depoları gizli tutulmaktadır. Kodu incelemek veya geliştirmeye katılmak isteyen araştırmacı ve geliştiriciler contact@veris.vote adresine yazabilir. Katılım herhangi bir katkı yükümlülüğü getirmez.

---

https://veris.vote | contact@veris.vote
