# LP AmigoPrev

Landing page estática (HTML/CSS/JS) da AmigoPrev — Assessoria em Seguro e Previdência. Captação de leads de trabalhadores CLT que sofreram acidentes (auxílio-acidente, auxílio-doença, seguros).

- `/` — página principal com formulário final (Nome + Celular)
- `/redirect` — tela de transição que abre o WhatsApp (34) 98422-1619
- `/dashboard` — painel de leads (login via Supabase Auth, usuário `Admin`)

## Dados
Supabase "ADS BR CLIENTES" (`qxhnjzyhtllmtdrcyygi`), tabelas `lp_visits` e `lp_leads` com `site='amigoprev'`.
Acesso ao painel controlado por `lp_acessos` (RLS `pode_ver_site`) — usuário `admin@amigoprev.adsbr.internal`.

## Pendências
- Rodapé: razão social, CNPJ, endereço e link da Política de Privacidade.
- GTM / Pixel: não instalados (o código já dispara `dataLayer`, `fbq` e `gtag` se existirem).
