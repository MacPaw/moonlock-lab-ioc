# macOS Threat Landscape 2026 — Indicators of Compromise

Indicators of compromise (IOCs) accompanying the **Moonlock Threat Report 2026**

**Last updated:** 2026-11-24 · **TLP:** CLEAR

> ⚠️ **Handle with care. Do not open or interact with any IOC without proper security preparation.**

## Commodity & crimeware stealers

### Atomic Stealer (AMOS)

| Type | Indicator | Context |
| :---- | :---- | :---- |
| SHA-256 | `09bfde65a68717ddd65f50dd828dfaf437a292d7439864cbc91d5d9d8ff85a6b` | AMOS dropper payload |
| SHA-256 | `340c48d5a0c32c9295ca5e60e4af9671c2139a2b488994763abe6449ddfc32aa` | AMOS payload |
| SHA-256 | `615ef69e758fd798ebca87ec6d60183f25ff7b2391e8c33ce5d9f3314350855c` | AMOS payload |
| SHA-256 | `7a3d6a1cc9384df6fd31558e16ac356ecbb1960cb78fdbf30a86f9f093c4206b` | AMOS payload |
| SHA-256 | `2bc2b4e876d2fd2ba905b5d82871e09ffb83097d40f9eb1bffc9a8ff1b73ef22` | AMOS `com.apple.SearchKit.agent`, Universal (x86_64 + arm64) |
| Domain | `alragaa[.]com` | AMOS C2 / exfiltration host |
| Domain | `anchorcoral10[.]com` | AMOS delivery infrastructure |
| Domain | `aspen32[.]com` | AMOS fake browser-update lure host |
| Domain | `bridge-schema[.]com` | AMOS staging host |
| Domain | `inktapestry[.]com` | AMOS click metrics / tracking endpoint |
| Domain | `cvols[.]com` | JetBrains lure staging domain |
| Domain | `kayeart[.]com` | Audio-driver fake-update lure host |
| Domain | `szfried[.]com` | Malvertising staging domain |
| Domain | `putuartana[.]com` | "CleanGPT" AI-themed lure host |
| Domain | `ejecen[.]com` | Mac-optimization lure host |

### MacSync Stealer

| Type | Indicator | Context |
| :---- | :---- | :---- |
| SHA-256 | `024044a62ec733a0baac53d555111c796c9bb8b79eb6f39f5a7e58c430cc0954` | MacSync stealer payload |
| SHA-256 | `02ea8e93290607629f567f75458e4d03a2b3f9e047604e24b967dd7d38fe945a` | MacSync Mach-O binary |
| SHA-256 | `04e4bad3a81e9c66d5220459d70f1541ca6b623d92243a633d8733d048bc2330` | MacSync Mach-O binary |
| SHA-256 | `05c556cfb8f531d06e673d4d86b139d7a0b3b02eb3fa001b304ba69870ef8c2b` | MacSync Mach-O binary |
| SHA-256 | `0e01d720a0e545e363736bd9b7fc7df142aadcf7550ffc001f0633f8ac718a8e` | MacSync Mach-O binary |
| SHA-256 | `06c74829d8eee3c47e17d01c41361d314f12277d899cc9dfa789fe767c03693e` | Signed MacSync application bundle |
| SHA-256 | `4ae745bc0e4631f676b3d0a05d5c74e37bdfc8da3076208b24e73e5bbea9178f` | MacSync payload container |
| SHA-256 | `7cfe0b119e616ac81ddb1767a5c7f40bec67d91fdd66e53490c0225789537073` | MacSync payload container |
| SHA-256 | `9990457feac0cd85f450e60c268ddf5789ed4ac81022b0d7c3021d7208ebccd3` | MacSync payload container |
| SHA-256 | `9d43e059111460c4f81351a062fb7eb7dbfd34988a06d756c7206f330c06cb42` | MacSync payload container |
| Domain | `1441bet[.]com` | MacSync distribution & C2 |
| Domain | `3plfast[.]com` | MacSync distribution |
| Domain | `401trading[.]com` | MacSync trading-themed lure |
| Domain | `5x5web[.]com` | MacSync delivery infrastructure |
| Domain | `accesscovidtest[.]com` | MacSync delivery infrastructure |
| Domain | `tryclix[.]com` | MacSync ClickFix payload staging |
| Domain | `realrix[.]com` | MacSync payload hosting |
| Domain | `santaclaracountyproperties[.]com` | Compromised MacSync payload server |
| Domain | `paripassuventures[.]com` | Compromised MacSync payload server |
| Domain | `texastransmissionrepair[.]com` | Compromised MacSync payload server |
| Domain | `gatemaden[.]space` | Gatekeeper-bypass MacSync payload endpoint |
| URL/path | `questlyric8[.]com/api/metrics/run` | ClickFix stager campaign-analytics beacon |
| Path | `/tmp/osalogging.zip` | MacSync staging artifact |

### CloudSyncD / Poseidon / Odyssey

| Type | Indicator | Context |
| :---- | :---- | :---- |
| SHA-256 | `06ab1e44941e0ceea9df11729576a091fa8c0388188b599f0ee51c54ee0a3186` | CloudSyncD x86_64 slice from fake Zoom installer |
| SHA-256 | `866c9d7d1e954ff7d1b138c5a53fb37e914a76bcc2e1f8aa194ef8690aeefeca` | CloudSyncD x86_64 backdoor (`com.bravetalk.helper`) |
| SHA-256 | `872a2119432231d7e0281160ccf0033098d0e481ce59b828f671ac525a5200b3` | CloudSyncD arm64 Apple-Silicon native backdoor |
| SHA-256 | `e8b7503f40fbcc41ed6769584b410da29827e505160290335454214074b7a511` | CloudSyncD Universal FAT binary (`main-arm64.out`) |
| Domain | `orchid-led[.]com` | CloudSyncD C2 masquerading as a jQuery script endpoint |
| Domain | `bjzhishang[.]com` | CloudSyncD secondary C2 |
| Domain | `dodiihome[.]com` | CloudSyncD backdoor C2 |
| Domain | `greenactiv[.]com` | Odyssey (fake Codex) staging |
| Domain | `rahtam[.]com` | Odyssey shared traffer staging |
| Domain | `scubin[.]com` | Odyssey shared traffer staging |
| IP | `165[.]245[.]215[.]18` | Odyssey C2 |

### notnullOSX

Returning 2024 actor (0xFFF / alh1mik); net-worth targeting ($10K+ crypto); Go + garble; ClickFix and malicious DMG; modular grabbers; trojanized-wallet swap.

| Type | Indicator | Context |
| :---- | :---- | :---- |
| SHA-256 | `b0cd860f18b0136e063d7ef9a3c84d138a1a21dbea019605ce66a3a1fad91db4` | notnullOSX implant |
| SHA-256 | `636fa90aebab98534dcdbe50508ed8d3607c284c72f831a4503e223540d3f761` | Delivery DMG (Infection Chain B) |
| SHA-256 | `070402c2c531aa3a87b9ccd080532a51d17b01d982b205fc4487246d58de8913` | bash installer script (Infection Chain A) |
| IP/URL | `111[.]90[.]149[.]111:8080/installer` | ClickFix installer host |
| Domain | `mactest-6b2ab-default-rtdb[.]firebaseio[.]com` | C2 (abused Firebase RTDB) |
| Domain | `cdn[.]filestackcontent[.]com` | Module delivery (abused legitimate CDN; `application/x-mach-binary`) |

### DigitStealer

Fake DynamicLake / Webex; Apple-Silicon CPU-feature anti-analysis filter; fileless JXA; Ledger Live `app.asar` swap.

| Type | Indicator | Context |
| :---- | :---- | :---- |
| **SHA-1** | `5c73987e642b8f8067c2f2b92af9fd923c25b2ec` | Unsigned `DynamicLake.dmg` dropper |
| Domain | `dynamiclake[.]org` | Deceptive distribution domain imitating DynamicLake |
| Domain | `diamondpickaxeforge[.]com` | DigitStealer C2 |
| Domain | `ebemvsextiho[.]com` | DigitStealer C2 |
| Domain | `bottleneckid[.]com` | DigitStealer C2 |
| Domain | `booksmagazinetx[.]com` | DigitStealer C2 |
| Domain | `goldenticketsshop[.]com` | DigitStealer C2 |
| Domain | `fixyourallergywithus[.]com` | DigitStealer C2 |
| Domain | `prodbackserv[.]com` | DNS-TXT staging |
| Domain | `*[.]pages[.]dev` | Landing-page hosting (abused) |

### PamStealer

Spoofs the Maccy clipboard manager; validates stolen passwords via macOS PAM; later builds add live server-side payload decryption.

| Type | Indicator | Context |
| :---- | :---- | :---- |
| Domain | `maccyapp[.]com` | Spoofed clipboard-app lure domain |

### CrashStealer

Signed & notarized dropper that passes Gatekeeper; poses as Apple Crash Reporter.

| Type | Indicator | Context |
| :---- | :---- | :---- |
| Domain | `endpoint-api-v1[.]com` | CrashStealer payload-staging C2 |

### ClickLock & GhostProfile stagers

ClickFix / curl-based terminal execution stagers feeding in-memory stealers and the GhostProfile hVNC.

| Type | Indicator | Context |
| :---- | :---- | :---- |
| Domain | `pressureulcerlawyer[.]com` | Staging host for curl-based terminal infostealer execution |
| Domain | `apdhlhs3[.]xyz` | Terminal downloader payload domain |
| Domain | `cxciwq3m[.]digeststart[.]us` | Downloader script delivery host |
| Domain | `johncon[.]my` | Compromised staging site |
| Domain | `jse8x92s[.]me` | Downloader script delivery host |
| Domain | `ojo9ip[.]footb[.]xyz` | Terminal update-script delivery host |

### Fake-VC investment-front (ClickFix)

LinkedIn outreach → fake CAPTCHA → clipboard → Terminal; manufactured fund with back-dated site.

| Type | Indicator |
| :---- | :---- |
| Domain | `lumax[.]capital` |
| Domain | `zoom[.]us07-web[.]us` |
| Domain | `hedgeweeks[.]online` |
| SHA-256 | `755cc133ae0519accbcfdd5f8f0d9fe1aa08cbcb306c3e5f29ebcb6ac12d9323` |

### Sonoma / Crazy Evil

Returning 2024 traffer crew; re-skinned Zoom / Brave / StreamYard / Slack; PAM password check; iCloud CalDAV staging.

| Type | Indicator | Context |
| :---- | :---- | :---- |
| Domain | `apple03cloudstore[.]com` | Crazy Evil C2 |
| IP | `109[.]94[.]171[.]225` | Crazy Evil C2 |
| Domain | `waaako[.]proxy08[.]com` | "Waaako" lure C2 (`WaaakoInstaller.dmg`) |
| String/marker | `dm5ne99sw9` | Core payload marker |
| String/marker | `SONOMAC1` / `EVLCFG01` | Config markers |

### Avenger

FUD stealer-to-RAT implant keeping a live operator channel.

| Type | Indicator | Context |
| :---- | :---- | :---- |
| Domain | `api[.]sync-master[.]online` | Avenger C2 |

### Zig C2 implant (VOIDLINK)

Red-team-grade macOS C2 written in Zig; zero detections on VT at first sight; Cobalt-Strike-style beacon, BOF loader, custom "c5" protocol.

| Type | Indicator | Context |
| :---- | :---- | :---- |
| SHA-256 | `05eac3663d47a29da0d32f67e10d161f831138e10958dcd88b9dc97038948f69` | VOIDLINK Zig-compiled modular C2 implant |
| SHA-256 | `0c570d5527e1dd7f516720f7685595d3c569b9a697405b9901bde5da98bda503` | VOIDLINK implant binary |
| SHA-256 | `13025f83ee515b299632d267f94b37c71115b22447a0425ac7baed4bf60b95cd` | VOIDLINK implant binary |
| SHA-256 | `16f255b4ad4de9c70794425ddb4b7ff4b2b89c1fc538fca635f564dbeaf835e8` | VOIDLINK implant binary |
| SHA-256 | `2169023474ce47f890f9637b657375a7ed5ccb9b0e7603815fe8557aacf3ea71` | VOIDLINK implant binary |

### EvilOSX

Python-based macOS post-exploitation RAT.

| Type | Indicator | Context |
| :---- | :---- | :---- |
| SHA-256 | `49a6fd89c084f2580615f388edc53ef44b3fe725001d6967a6ac12ec3fdfa2f2` | EvilOSX RAT payload |
| SHA-256 | `5c9ea2fa246607b7147c77767fcac74feb19989d3e9b7d3941c6b30a0c3f1fc6` | EvilOSX RAT payload |
| SHA-256 | `7f9cd1eedf0a9088fc3e07a275d04dceadcf0a5cd425a17e9666b63685d3a37e` | EvilOSX RAT payload |
| SHA-256 | `972a4e5ddbb99ff0e03898d8279a42d962e36aa3392e234a94cc0138c4411374` | EvilOSX RAT payload |

---

## DPRK / state-aligned clusters

### NUKESPED

| Type | Indicator | Context |
| :---- | :---- | :---- |
| SHA-256 | `0c7ea5fbe533a3df3c63e78376137f79dd668ba9f7895a9b1d110c301a5bfe36` | NUKESPED macOS backdoor |
| SHA-256 | `6f7a5f1d52d3bfc6f175bf2bbb665e4bd99b0453e2d2e27712fe9b71c55962dc` | NUKESPED `.FlashUpdateCheck` backdoor payload |
| SHA-256 | `735365ef9aa6cca946cfef9a4b85f68e7f9f03011da0cf5f5ab517a381e40d02` | NUKESPED trojanized Flash Player bundle |
| SHA-256 | `761bcff9401bed2ace80b85c43b230294f41fc4d1c0dd1ff454650b624cf239d` | NUKESPED backdoor binary |
| SHA-256 | `8f714548d7502863a89b2fe1e95420e542e439c1f38ee8727ff8a15b2826adb4` | NUKESPED backdoor binary |
| SHA-256 | `d91c233b2f1177357387c29d92bd3f29fab7b90760e59a893a0f447ef2cb4715` | NUKESPED `Album.app` binary |
| SHA-256 | `60b3cfe2ec3100caf4afde734cfd5147f78acf58ab17d4480196831db4aa5f18` | NUKESPED `DAFOM-1.0.0.dmg` installer |
| SHA-256 | `5b40b73934c1583144f41d8463e227529fa7157e26e6012babd062e3fd7e0b03` | NUKESPED `TokenAIS.app.zip` archive |
| SHA-256 | `f0e8c29e3349d030a97f4a8673387c2e21858cccd1fb9ebbf9009b27743b2e5b` | NUKESPED `CryptAIS.dmg` installer |
| SHA-256 | `9ba02f8a985ec1a99ab7b78fa678f26c0273d91ae7cbe45b814e6775ec477598` | NUKESPED `Esilet.dmg` trojanized app |
| SHA-256 | `89b5e248c222ebf2cb3b525d3650259e01cf7d8fff5e4aa15ccd7512b1e63957` | NUKESPED `darwin64.bin` core Mach-O |
| SHA-256 | `00fc41d6fbab80e2b5e60c5965ff34d8a7225896a4f87d390b1b801bda6fc9d7` | NUKESPED arm64 downloader |
| SHA-256 | `04566b6181a801c2b045ba5bc8e69827a10a2510847ff6fb658552cba63ccd20` | NUKESPED downloader binary |
| SHA-256 | `2b8424b587723329e8fea54382239efd6acb6cb78712b39c9970b14e6629694c` | NUKESPED downloader binary |
| SHA-256 | `2ba31472d6cc4959a8a7c5c05a923fc2974f2a4c911d74076a8697de8820bb62` | NUKESPED downloader binary |
| SHA-256 | `315503862cb7ebb0a731483827016015e355bad51f872db5c650a822de744937` | NUKESPED downloader binary |
| Domain | `baseballcharlemagnelegardeur[.]com` | Compromised C2 |
| Domain | `tangowithcolette[.]com` | Compromised C2 |
| Domain | `towingoperations[.]com` | Compromised C2 |
| Domain | `nzssdm[.]com` | Payload download host (`/assets/mt.dat`) |
| Domain | `concrecapital[.]com` | NUKESPED C2 |
| Domain | `onlinestockwatch[.]net` | NUKESPED C2 |

### FlexibleFerret (UNC5975 / DPRK)

Contagious-Interview Go backdoor via fake assessment/interview portals.

| Type | Indicator | Context |
| :---- | :---- | :---- |
| SHA-256 | `0267702a659b7e6b8ae0ce994ad3e6d426747f1a1c199a89398622d0189b56d0` | FlexibleFerret Go backdoor payload |
| SHA-256 | `14a56d6381c1ee8e0561da1fbdb895e6ba70578245fc43177f0b4635a155ee84` | FlexibleFerret backdoor payload |
| SHA-256 | `7c1e5f1fadd194555a77f13105b988c0f2994b741e932837228fe47bc30d8dcf` | FlexibleFerret backdoor payload |
| SHA-256 | `8cacecc1d0da29a5928f73d5b1c1301c6e78300cc6b78db787acdb19f1eaaec3` | FlexibleFerret backdoor payload |
| SHA-256 | `d9ee3e3af1c57022ba1e843d78ec2b4fb6cb8a65b7eecab9b94c5f4b34338e8d` | FlexibleFerret backdoor payload |
| Domain | `api[.]jz-aws[.]info` | FlexibleFerret staging host |
| Domain | `app[.]compassidea[.]org` | Interview-assessment lure domain |
| Domain | `app[.]evaluino[.]com` | Assessment lure domain |
| Domain | `app[.]evaluza[.]com` | Assessment lure domain |
| Domain | `app[.]proficiencycert[.]com` | Certificate lure domain |
| Domain | `app[.]zynoracreative[.]com` | C2 payload delivery host |

### FlutterShell (CL-CRI-1089)

Flutter-framework backdoor delivered via malvertising.

| Type | Indicator | Context |
| :---- | :---- | :---- |
| Domain | `mbupdate[.]linkpc[.]net` | FlutterShell C2 callback domain |

### BeaverTail / Contagious Interview

Trojanized interview repos; git `post-checkout` hook dropper → BeaverTail / OtterCookie / InvisibleFerret.

| Type | Indicator | Context |
| :---- | :---- | :---- |
| URL/path | `vercel[.]app/api/{m,l,w}` | OS-branched staging (abused Vercel) |
| IP | `45[.]154[.]98[.]86:15152` | C2 |
| Path | `~/Library/tokenlinux.sh` | Dropped artifact |

### TraderTraitor

DPRK Lazarus subgroup (UNC4899 / Jade Sleet).

| Type | Indicator | Context |
| :---- | :---- | :---- |
| Domain | `registry[.]hashicorp-aws[.]com` | Typosquatted Terraform provider registry in weaponized `.terraform.lock.hcl` |
| Filename | `SystemUpdate` | macOS.Gaslight implant on disk |
| Filename | `iSync` / `loginwindow` | ROOFDECK implant on disk (renamed Apr 20, 2026) |
| Technique | Nostr relay dead-drop → `/app_version` command polling | ROOFDECK C2 resolution |

### Macma

Modular macOS backdoor (historically PRC-aligned tooling).

| Type | Indicator | Context |
| :---- | :---- | :---- |
| SHA-256 | `003764fd74bf13cff9bf1ddd870cbf593b23e2b584ba4465114023870ea6fbef` | Macma modular backdoor payload |
| SHA-256 | `0cabb6780b804d4ee285b0ddb00b02468f91b218bd2db2e2310c90471f7f8e74` | Macma modular backdoor binary |
| SHA-256 | `1f5e4d2f71478518fe76b0efbb75609d3fb6cab06d1b021d6aa30db424f84a5e` | Macma modular backdoor binary |
| SHA-256 | `3894a8b82338791764524fddac786a2c5025cad37175877959a06c372b96ef05` | Macma modular backdoor binary |
| SHA-256 | `3a6605266184d967ab4643af2c73dafb8b7724d21c7aa69e58d78b84ebc06612` | Macma modular backdoor binary |

---

