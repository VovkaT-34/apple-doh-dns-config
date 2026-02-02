# apple-doh-dns-config
Коллекция DoH DNS-конфигураций (.mobileconfig) для iOS, iPadOS и macOS. Упор на приватность, анонимность и устойчивость к блокировкам.
# Apple DoH DNS Config

Приватный набор DNS-over-HTTPS конфигураций для устройств Apple.

## Поддерживаемые устройства
- iPhone (iOS)
- iPad (iPadOS)
- MacBook / iMac (macOS)

## Цели
- Повышение конфиденциальности
- Снижение трекинга
- Блокировка рекламы и мусора (где поддерживается)
- Прямая работа с нейросетями, включая ChatGPT, Grok и аналогичные сервисы (после установки подписаны в скобочках как Xbox или GPT)
- Стабильная работа с игровыми платформами и онлайн-играми (подписаны в скобочках как Xbox или GPT)
- Использование официальных и легальных DNS-серверов
- Минимальные задержки при работе с нейросетями и играми
- Простая настройка без дополнительных изменений
- Безопасность и конфиденциальность, без ведения логов активности (подписаны в скобочках (Private))


## Формат
Файлы `.mobileconfig` устанавливаются напрямую в систему Apple.

## Примечание
DNS — не VPN. IP-адрес не меняется.
Некоторые сервера провайдеров могут работать нестабильно из за DDOS атак, либо других неисправностей самих серверов.


## Состав DoH-серверов
🧠 Нейросети / игровые сервисы (после установки подписаны в скобочках как (Xbox или GPT))

1. (GPT, RU) Comss.one (https://dns.comss.one/dns-query) — публичный DoH, оптимизирован для стабильного соединения с AI‑сервисами; проект Comss, РФ
2. (GPT, DE) dns.malw.link (https://dns.malw.link/dns-query) — DoH с фильтрацией мусора, стабильные маршруты к AI‑сервисам; частный проект, Германия
3. (GPT, FL) Cloudflare Gateway (https://5u35p8m9i7.cloudflare-gateway.com/dns-query) — корпоративный DoH Cloudflare для прямого доступа к облачным сервисам; Cloudflare Inc., США
4. (Xbox) Xbox-DNS (https://xbox-dns.ru/dns-query) — DoH для игровых сервисов и платформ; независимый игровой DNS‑проект
5. (Xbox, RU) AstraCat (AI) (https://dns.astracat.ru/dns-query) — DoH для AI‑ и игровых сервисов; AstraCat, РФ

🧠 Нейросети / игровые сервисы, они же — DoT
1. dns.comss.one
2. dns.malw.link
3. 5u35p8m9i7.cloudflare-gateway.com
4. xbox-dns.ru
5. dns.astracat.ru


🔒 Приватные DNS (минимальные логи)  (после установки подписаны в скобочках (Private))

1. Digitale‑Gesellschaft (CH, Private) (https://dns.digitale-gesellschaft.ch/dns-query) — приватный европейский DoH; Digitale Gesellschaft, Швейцария
2. Digitale‑Gesellschaft 2 (CH, Private) (https://dns2.digitale-gesellschaft.ch/dns-query) — резервный приватный DoH; Digitale Gesellschaft, Швейцария
3. LibreDNS (DE, Private) (https://doh.libredns.gr/dns-query) — приватный DNS без цензуры; LibreOps, ЕС
4. UncensoredDNS (DK, Private) (https://anycast.uncensoreddns.org/dns-query) — приватный DNS без фильтрации; UncensoredDNS, Дания
5. Quad9 (SE, EG, Private) (https://dns.quad9.net/dns-query) — приватный DNS с защитой от угроз; Quad9 Foundation, Швейцария
6. RethinkDNS (PL, Private) (https://basic.rethinkdns.com/dns-query) — приватный DNS с блокировкой трекеров; RethinkDNS, ЕС
7. Control D Unfiltered (Private, DE) (https://freedns.controld.com/p0/dns-query) — приватный DNS без фильтрации; Control D / Windscribe, Канада
8. Control D Malware (Private, DE) (https://freedns.controld.com/p2/dns-query) — приватный DNS с защитой; Control D / Windscribe, Канада

🔒 Приватные, они же — DoT
1. dns.digitale-gesellschaft.ch
2. dns2.digitale-gesellschaft.ch
3. dot.libredns.gr
4. unicast.uncensoreddns.org
5. dns.quad9.net
6. basic.rethinkdns.com
7. p0.freedns.controld.com
8. p2.freedns.controld.com


🌍 Публичные и универсальные DoH

1. Google DNS (https://dns.google/dns-query) — публичный высокосовместимый DNS; Google LLC, США
2. OpenDNS (Cisco) (https://doh.opendns.com/dns-query) — коммерческий DNS; Cisco Systems, США
3. NextDNS (https://dns.nextdns.io/dns-query) — настраиваемый DNS с выборочным логированием; NextDNS, ЕС
4. Cloudflare DoH / DoT (https://1dot1dot1dot1.cloudflare-dns.com/dns-query) — быстрый публичный DNS; Cloudflare Inc., США
5. Cloudflare (classic) (https://cloudflare-dns.com/dns-query) — стандартный DoH Cloudflare; Cloudflare Inc., США
6. Cloudflare ODoH (https://odoh.cloudflare-dns.com/dns-query) — обфусцированный DoH; Cloudflare Inc., США
7. Cloudflare Malware Filter (https://security.cloudflare-dns.com/dns-query) — публичный DNS с защитой; Cloudflare Inc., США
8. AdGuard DNS (Filtered) (https://dns.adguard-dns.com/dns-query) — DNS с фильтрацией; AdGuard, Кипр
9. AdGuard DNS (Unfiltered) (https://unfiltered.adguard-dns.com/dns-query) — DNS без фильтрации; AdGuard, Кипр
10. Yandex DNS (Unfiltered) (https://common.dot.dns.yandex.net/dns-query) — базовый DNS; Яндекс, РФ
11. Yandex DNS (Filtered) (https://safe.dot.dns.yandex.net/dns-query) — DNS с фильтрацией; Яндекс, РФ
12. Doh.sb (DE) (https://doh.sb/dns-query) — DNS с защитой от вредоносных доменов; doh.sb project, Германия

🌍 Публичные и универсальные DNS, они же — DoT
1. dns.google
2. doh.opendns.com
3. dns.nextdns.io
4. 1dot1dot1dot1.cloudflare-dns.com
5. cloudflare-dns.com
6. security.cloudflare-dns.com
7. family.cloudflare-dns.com
8. dns.adguard-dns.com
9. unfiltered.adguard-dns.com
10. common.dot.dns.yandex.net
11. safe.dot.dns.yandex.net
12. doh.sb


